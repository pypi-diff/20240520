# Comparing `tmp/apysc-4.3.0.tar.gz` & `tmp/apysc-4.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apysc-4.3.0.tar", last modified: Thu May 16 12:54:53 2024, max compression
+gzip compressed data, was "apysc-4.3.2.tar", last modified: Sun May 19 13:25:59 2024, max compression
```

## Comparing `apysc-4.3.0.tar` & `apysc-4.3.2.tar`

### file list

```diff
@@ -1,763 +1,1909 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:53.309003 apysc-4.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-16 12:54:36.000000 apysc-4.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 12:54:36.000000 apysc-4.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-16 12:54:53.309003 apysc-4.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-05-16 12:54:36.000000 apysc-4.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:53.225003 apysc-4.3.0/apysc/
--rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:53.233003 apysc-4.3.0/apysc/_animation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10351 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_cx.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_cx_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_cy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_cy_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_fill_alpha.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_fill_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_fill_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_fill_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_finish_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_height.py
--rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_height_for_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_height_for_ellipse_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_height_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_line_alpha.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_line_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_line_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_line_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_line_thickness.py
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_line_thickness_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_move.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_move_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    10250 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_parallel_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_pause_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_play_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_radius.py
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_radius_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_reset_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_reverse_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_rotation_around_center.py
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_rotation_around_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_rotation_around_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_rotation_around_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_scale_x_from_center.py
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_scale_x_from_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_scale_x_from_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_scale_x_from_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_scale_y_from_center.py
--rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_scale_y_from_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6921 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_scale_y_from_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_scale_y_from_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_time_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_width.py
--rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_width_for_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_width_for_ellipse_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_x.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_y.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/animation_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_animation/easing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:53.233003 apysc-4.3.0/apysc/_auto_reloading/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_auto_reloading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_auto_reloading/auto_reloading_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:53.233003 apysc-4.3.0/apysc/_branch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_branch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_branch/_elif.py
--rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_branch/_else.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_branch/_if.py
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_branch/if_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:53.233003 apysc-4.3.0/apysc/_callable/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_callable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_callable/callable_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:53.237003 apysc-4.3.0/apysc/_chart/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/add_background_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/add_border_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/axis_label_bold_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/axis_label_fill_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/axis_label_fill_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/axis_label_font_family_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/axis_label_font_size_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/axis_label_italic_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/axis_line_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/axis_line_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/axis_line_thickness_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/background_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/border_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/chart_const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/chart_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    22705 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/create_single_column_y_axis_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/initialize_each_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/is_display_axis_label_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/overall_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/set_initial_background_fill_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/set_initial_background_fill_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/set_initial_border_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/set_initial_border_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/set_initial_border_thickness_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/set_initial_height_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/set_initial_horizontal_padding_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/set_initial_matrix_data_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/set_initial_overall_container_coordinates_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/set_initial_vertical_padding_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/set_initial_width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/set_initial_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/set_initial_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/tick_max_num_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/tick_text_bold_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/tick_text_fill_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/tick_text_fill_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/tick_text_font_family_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/tick_text_font_size_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/tick_text_italic_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/tick_text_max_num_of_decimal_places_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     9647 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/vertical_bar_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/x_axis_column_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/x_axis_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/x_axis_label_position.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/x_axis_label_position_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    11482 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/x_axis_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/y_axis_column_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/y_axis_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/y_axis_label_position.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/y_axis_label_position_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/y_axis_single_column_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/y_max_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_chart/y_min_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:53.241003 apysc-4.3.0/apysc/_color/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_color/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_color/blue_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_color/color.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_color/color_copy_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7843 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_color/color_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_color/colorless.py
--rw-r--r--   0 runner    (1001) docker     (127)    84071 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_color/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_color/copy_color_if_default_value_specified_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_color/from_rgb_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_color/get_colors_members_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_color/green_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_color/red_color_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:53.241003 apysc-4.3.0/apysc/_console/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_console/_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)    32116 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_console/assertion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_console/loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:53.241003 apysc-4.3.0/apysc/_converter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_converter/cast.py
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_converter/to_apysc_val_from_builtin.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_converter/to_builtin_val_from_apysc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:53.257003 apysc-4.3.0/apysc/_display/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/add_foreign_object_child_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/add_to_parent_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/any_display_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/append_fill_alpha_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/append_fill_color_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/append_foreign_object_constructor_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/append_line_alpha_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/append_line_cap_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/append_line_color_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/append_line_joints_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/append_line_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/append_line_thickness_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/append_x_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/append_y_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/begin_fill_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    15676 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/child_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    17462 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/circle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/css_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/css_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/css_text_align.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/css_text_align_last.py
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/cx_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/cy_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/display_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    17384 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/ellipse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5438 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/ellipse_height_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/ellipse_width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/fill_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/fill_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/flip_interface_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/flip_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/flip_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/get_bounds_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    49066 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/graphics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/graphics_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/graphics_clear_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/graphics_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/height_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    15906 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/line.py
--rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/line_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/line_cap_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/line_caps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/line_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/line_dash_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/line_dash_dot_setting_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/line_dash_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/line_dash_setting_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/line_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/line_dot_setting_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/line_joints.py
--rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/line_joints_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/line_round_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/line_round_dot_setting_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    26709 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/line_style_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/line_thickness_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    12333 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/multi_line_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/opacity_css_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/parent_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    18730 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/points_2d_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/points_var_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    15565 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/polygon_append_constructor_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/polygon_apply_current_points_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/polygon_x1_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/polygon_x2_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/polygon_x3_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/polygon_y1_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/polygon_y2_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/polygon_y3_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    17466 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/polyline.py
--rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/radius_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    19494 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/rectangle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/rotation_around_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     9157 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/rotation_around_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/rotation_interface_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/scale_interface_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/scale_x_from_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/scale_x_from_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/scale_y_from_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/scale_y_from_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/set_lower_scale_limit_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/set_overflow_visible_setting_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/set_x_and_y_with_minimum_point_interface_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/skew_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/skew_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7453 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/sprite.py
--rw-r--r--   0 runner    (1001) docker     (127)    12655 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/svg_foreign_object_child.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/svg_foreign_object_child_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/svg_foreign_object_initialize_width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/svg_foreign_object_text_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/svg_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)    23384 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/svg_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/svg_text_align_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/svg_text_bold_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/svg_text_delta_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/svg_text_delta_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/svg_text_font_family_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/svg_text_font_size_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/svg_text_italic_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/svg_text_leading_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/svg_text_set_align_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/svg_text_set_bold_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/svg_text_set_delta_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/svg_text_set_delta_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/svg_text_set_font_family_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/svg_text_set_font_size_value_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/svg_text_set_italic_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/svg_text_set_leading_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/svg_text_set_text_value_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/svg_text_singleton_for_text_span.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/svg_text_skip_fill_alpha_exp_appending_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/svg_text_skip_fill_color_exp_appending_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/svg_text_skip_line_alpha_exp_appending_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/svg_text_skip_line_color_exp_appending_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/svg_text_skip_line_thickness_exp_appending_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    16986 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/svg_text_span.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/svg_text_text_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/text_align_css_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/text_align_last_css_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/text_bold_css_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/text_decoration_underline_css_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/text_fill_color_css_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/text_font_size_css_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/text_italic_css_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/text_line_height_css_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    17673 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/triangle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/visible_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/width_and_height_mixin_for_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/x_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/y_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_display/y_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:53.261003 apysc-4.3.0/apysc/_event/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_event/animation_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_event/click_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    14746 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_event/custom_event_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_event/custom_event_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_event/document_mouse_wheel_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_event/double_click_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_event/enter_frame_event.py
--rw-r--r--   0 runner    (1001) docker     (127)    15687 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_event/enter_frame_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_event/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_event/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9989 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_event/handler_circular_calling_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_event/mouse_down_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_event/mouse_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_event/mouse_event_binding_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_event/mouse_event_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_event/mouse_event_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_event/mouse_event_unbinding_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_event/mouse_move_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6824 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_event/mouse_out_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_event/mouse_over_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_event/mouse_up_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_event/prevent_default_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_event/set_handler_data_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_event/stop_propagation_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_event/timer_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_event/wheel_event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:53.261003 apysc-4.3.0/apysc/_expression/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_expression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_expression/event_handler_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    17851 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_expression/expression_data_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_expression/expression_variables_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_expression/get_last_scope_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_expression/indent_num.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_expression/js_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_expression/last_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_expression/var_names.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:53.261003 apysc-4.3.0/apysc/_file/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_file/file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_file/module_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:53.265003 apysc-4.3.0/apysc/_geom/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_geom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10201 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_geom/path_bezier_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     7960 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_geom/path_bezier_2d_continual.py
--rw-r--r--   0 runner    (1001) docker     (127)    13379 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_geom/path_bezier_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11011 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_geom/path_bezier_3d_continual.py
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_geom/path_close.py
--rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_geom/path_control_x1_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_geom/path_control_x2_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_geom/path_control_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_geom/path_control_y1_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_geom/path_control_y2_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_geom/path_control_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_geom/path_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_geom/path_data_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_geom/path_data_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_geom/path_dest_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_geom/path_dest_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6540 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_geom/path_horizontal.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_geom/path_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_geom/path_line_to.py
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_geom/path_move_to.py
--rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_geom/path_vertical.py
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_geom/path_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_geom/path_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    12328 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_geom/point2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_geom/rectangle_geom.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_geom/rectangle_geom_bottom_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_geom/rectangle_geom_center_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_geom/rectangle_geom_center_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_geom/rectangle_geom_height_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_geom/rectangle_geom_left_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_geom/rectangle_geom_right_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_geom/rectangle_geom_top_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_geom/rectangle_geom_width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_geom/relative_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:53.265003 apysc-4.3.0/apysc/_html/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14617 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_html/debug_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)    20660 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_html/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_html/html_const.py
--rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_html/html_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:53.265003 apysc-4.3.0/apysc/_jslib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_jslib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    70264 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_jslib/jquery-3.7.1.slim.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_jslib/jquery.mousewheel-3.1.13.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_jslib/jslib_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    78572 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_jslib/svg-3.1.2.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    19431 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_jslib/underscore-1.12.0.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:53.265003 apysc-4.3.0/apysc/_jupyter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_jupyter/jupyter_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:53.269003 apysc-4.3.0/apysc/_lint_and_doc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_lint_and_doc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17625 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_lint_and_doc/add_doc_translation_mapping_blank_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_lint_and_doc/conf_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    10316 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_lint_and_doc/docs_keyword_link_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_lint_and_doc/docs_lang.py
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_lint_and_doc/docs_toctree_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    17282 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_lint_and_doc/docs_translation_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13722 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_lint_and_doc/docstring_to_markdown_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    51969 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_lint_and_doc/docstring_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     7636 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_lint_and_doc/document_text_split_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_lint_and_doc/document_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:53.269003 apysc-4.3.0/apysc/_lint_and_doc/fixed_translation_mapping/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_lint_and_doc/fixed_translation_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_lint_and_doc/fixed_translation_mapping/data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)   245896 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_lint_and_doc/fixed_translation_mapping/jp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_lint_and_doc/lint_and_doc_hash_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    11174 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_lint_and_doc/translation_mapping_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:53.269003 apysc-4.3.0/apysc/_loop/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_loop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_loop/_continue.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_loop/_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_loop/for_array_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_loop/for_array_indices_and_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_loop/for_array_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_loop/for_dict_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     7806 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_loop/for_dict_keys_and_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_loop/for_dict_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_loop/for_loop_exit_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_loop/initialize_with_base_value_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_loop/loop_count.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:53.269003 apysc-4.3.0/apysc/_material_design/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_material_design/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:53.269003 apysc-4.3.0/apysc/_material_design/icon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_material_design/icon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:53.269003 apysc-4.3.0/apysc/_math/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_math/math.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_math/max_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_math/min_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_math/trunc_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:53.269003 apysc-4.3.0/apysc/_string/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_string/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_string/indent_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_string/string_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:53.269003 apysc-4.3.0/apysc/_testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9001 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_testing/e2e_testing_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_testing/testing_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:53.273003 apysc-4.3.0/apysc/_time/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10971 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_time/datetime_.py
--rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_time/day_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_time/days_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_time/fps.py
--rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_time/hour_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_time/left_and_right_datetimes_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_time/millisecond_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_time/minute_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_time/month_end_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_time/month_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_time/now_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_time/second_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_time/timedelta_.py
--rw-r--r--   0 runner    (1001) docker     (127)    22600 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_time/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_time/total_seconds_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_time/weekday_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_time/year_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:53.273003 apysc-4.3.0/apysc/_translation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:53.301003 apysc-4.3.0/apysc/_translation/jp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/about_handler_options_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    15423 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/add_child_and_remove_child.py
--rw-r--r--   0 runner    (1001) docker     (127)     7811 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/add_debug_info_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/animation_base_start.py
--rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/animation_base_target.py
--rw-r--r--   0 runner    (1001) docker     (127)    15505 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/animation_complete.py
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/animation_delay.py
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/animation_duration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14477 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/animation_event.py
--rw-r--r--   0 runner    (1001) docker     (127)    11101 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/animation_fill_alpha.py
--rw-r--r--   0 runner    (1001) docker     (127)    11517 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/animation_fill_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     8179 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/animation_finish.py
--rw-r--r--   0 runner    (1001) docker     (127)   146934 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/animation_interfaces_abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    11565 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/animation_line_alpha.py
--rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/animation_line_color.py
--rw-r--r--   0 runner    (1001) docker     (127)    11623 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/animation_line_thickness.py
--rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/animation_method_chaining.py
--rw-r--r--   0 runner    (1001) docker     (127)    11788 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/animation_move.py
--rw-r--r--   0 runner    (1001) docker     (127)    13907 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/animation_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/animation_pause_and_play.py
--rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/animation_radius.py
--rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/animation_reset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/animation_return_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    11504 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/animation_reverse.py
--rw-r--r--   0 runner    (1001) docker     (127)    12174 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/animation_rotation_around_center.py
--rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/animation_rotation_around_point.py
--rw-r--r--   0 runner    (1001) docker     (127)    22680 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/animation_scale_x_and_y_from_center.py
--rw-r--r--   0 runner    (1001) docker     (127)    10757 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/animation_scale_x_and_y_from_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/animation_time.py
--rw-r--r--   0 runner    (1001) docker     (127)    24451 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/animation_width_and_height.py
--rw-r--r--   0 runner    (1001) docker     (127)    13114 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/animation_x.py
--rw-r--r--   0 runner    (1001) docker     (127)    13134 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/animation_y.py
--rw-r--r--   0 runner    (1001) docker     (127)     6068 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/append_js_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)    16245 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/array_append_and_push.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/array_clear.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/array_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/array_extend_and_concat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/array_index_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/array_insert_and_insert_at.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/array_join.py
--rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/array_last_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/array_length.py
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/array_pop.py
--rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/array_remove_and_remove_at.py
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/array_reverse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/array_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/array_sort.py
--rw-r--r--   0 runner    (1001) docker     (127)    16324 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/assert_arrays_equal_and_arrays_not_equal.py
--rw-r--r--   0 runner    (1001) docker     (127)    11225 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/assert_defined_and_undefined.py
--rw-r--r--   0 runner    (1001) docker     (127)    16840 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/assert_dicts_equal_and_dicts_not_equal.py
--rw-r--r--   0 runner    (1001) docker     (127)    11685 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/assert_equal_and_not_equal.py
--rw-r--r--   0 runner    (1001) docker     (127)    11047 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/assert_greater_and_greater_equal.py
--rw-r--r--   0 runner    (1001) docker     (127)    10860 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/assert_less_and_less_equal.py
--rw-r--r--   0 runner    (1001) docker     (127)    15946 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/assert_true_and_false.py
--rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/assertion_basic_behavior.py
--rw-r--r--   0 runner    (1001) docker     (127)    25610 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/bind_and_trigger_custom_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/blue_color.py
--rw-r--r--   0 runner    (1001) docker     (127)    15004 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/branch_instruction_variables_reverting_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)    49953 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/circle.py
--rw-r--r--   0 runner    (1001) docker     (127)    18952 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/click.py
--rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/color.py
--rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/color_from_rgb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/colorless.py
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/contains.py
--rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/continue.py
--rw-r--r--   0 runner    (1001) docker     (127)    14030 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/datetime_day.py
--rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/datetime_hour.py
--rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/datetime_millisecond.py
--rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/datetime_minute.py
--rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/datetime_month.py
--rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/datetime_now.py
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/datetime_second.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/datetime_set_month_end.py
--rw-r--r--   0 runner    (1001) docker     (127)     9065 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/datetime_weekday_js_and_weekday_py.py
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/datetime_year.py
--rw-r--r--   0 runner    (1001) docker     (127)    16601 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/dblclick.py
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/dictionary_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/dictionary_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/dictionary_length.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/display_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    23405 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/display_object_and_graphics_base_prop_abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     9723 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/display_object_get_and_set_css.py
--rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/display_object_mouse_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     9021 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/display_object_parent.py
--rw-r--r--   0 runner    (1001) docker     (127)     8567 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/display_object_visible.py
--rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/display_object_x_and_y.py
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/display_on_colaboratory.py
--rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/display_on_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12092 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/draw_interfaces_abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    85549 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/easing_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    12136 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/elif.py
--rw-r--r--   0 runner    (1001) docker     (127)    51515 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/ellipse.py
--rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/else.py
--rw-r--r--   0 runner    (1001) docker     (127)     9718 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/enter_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)    12970 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/event_prevent_default_and_stop_propagation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10715 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/for_array_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/for_array_indices_and_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     9557 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/for_array_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     9783 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/for_dict_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    11463 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/for_dict_keys_and_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     8642 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/for_dict_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/fps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/fundamental_data_classes_value_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     6667 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/get_bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/get_child_at.py
--rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/graphics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/graphics_base_fill_alpha.py
--rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/graphics_base_fill_color.py
--rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/graphics_base_flip_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/graphics_base_line_alpha.py
--rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/graphics_base_line_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     9355 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/graphics_base_line_dash_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     8863 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/graphics_base_line_dash_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     9053 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/graphics_base_line_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     9250 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/graphics_base_line_round_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/graphics_base_line_thickness.py
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/graphics_base_rotation_around_center.py
--rw-r--r--   0 runner    (1001) docker     (127)    11688 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/graphics_base_rotation_around_point.py
--rw-r--r--   0 runner    (1001) docker     (127)    16144 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/graphics_base_scale_from_center.py
--rw-r--r--   0 runner    (1001) docker     (127)    24463 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/graphics_base_scale_from_point.py
--rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/graphics_base_skew.py
--rw-r--r--   0 runner    (1001) docker     (127)    19456 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/graphics_begin_fill.py
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/graphics_clear.py
--rw-r--r--   0 runner    (1001) docker     (127)     8915 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/graphics_draw_circle.py
--rw-r--r--   0 runner    (1001) docker     (127)     9154 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/graphics_draw_dash_dotted_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     8546 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/graphics_draw_dashed_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     8098 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/graphics_draw_dotted_line.py
--rw-r--r--   0 runner    (1001) docker     (127)    10266 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/graphics_draw_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (127)    11252 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/graphics_draw_line.py
--rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/graphics_draw_path.py
--rw-r--r--   0 runner    (1001) docker     (127)    15102 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/graphics_draw_polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)    10632 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/graphics_draw_rect.py
--rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/graphics_draw_round_dotted_line.py
--rw-r--r--   0 runner    (1001) docker     (127)    10286 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/graphics_draw_round_rect.py
--rw-r--r--   0 runner    (1001) docker     (127)    10974 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/graphics_draw_triangle.py
--rw-r--r--   0 runner    (1001) docker     (127)    64374 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/graphics_line_style.py
--rw-r--r--   0 runner    (1001) docker     (127)    18270 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/graphics_move_to_and_line_to.py
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/green_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/if.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/import_conventions.py
--rw-r--r--   0 runner    (1001) docker     (127)    20761 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/index.py
--rw-r--r--   0 runner    (1001) docker     (127)    18347 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/int_and_number.py
--rw-r--r--   0 runner    (1001) docker     (127)    11684 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/int_and_number_arithmetic_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/int_and_number_comparison_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/int_and_number_to_fixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/int_and_number_to_hex.py
--rw-r--r--   0 runner    (1001) docker     (127)    48186 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/line.py
--rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/material_design_colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/math_max.py
--rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/math_min.py
--rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/math_trunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/mouse_event_abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    38153 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/mouse_event_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    27701 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/mousedown_and_mouseup.py
--rw-r--r--   0 runner    (1001) docker     (127)    17541 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/mousemove.py
--rw-r--r--   0 runner    (1001) docker     (127)    28272 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/mouseover_and_mouseout.py
--rw-r--r--   0 runner    (1001) docker     (127)    12910 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/multi_line_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/num_children.py
--rw-r--r--   0 runner    (1001) docker     (127)    62153 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/path.py
--rw-r--r--   0 runner    (1001) docker     (127)    13516 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/path_bezier_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11122 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/path_bezier_2d_continual.py
--rw-r--r--   0 runner    (1001) docker     (127)    16364 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/path_bezier_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    16314 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/path_bezier_3d_continual.py
--rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/path_close.py
--rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/path_horizontal.py
--rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/path_line_to.py
--rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/path_move_to.py
--rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/path_vertical.py
--rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/point2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    50966 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)    53243 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/polyline.py
--rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/quick_start.py
--rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/range.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/recommended_type_checker_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    54921 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/rectangle.py
--rw-r--r--   0 runner    (1001) docker     (127)    25542 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/rectangle_geom.py
--rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/red_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/remove_children.py
--rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/return.py
--rw-r--r--   0 runner    (1001) docker     (127)    17504 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/save_overall_html.py
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/sequential_animation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10214 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/set_debug_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/sprite.py
--rw-r--r--   0 runner    (1001) docker     (127)    31274 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/string_addition_and_multiplication.py
--rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/string_apply_max_num_of_decimal_places.py
--rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/string_comparison_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/string_length.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/string_lower.py
--rw-r--r--   0 runner    (1001) docker     (127)     7143 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/string_lstrip.py
--rw-r--r--   0 runner    (1001) docker     (127)     7074 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/string_rstrip.py
--rw-r--r--   0 runner    (1001) docker     (127)     8198 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/string_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/string_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/string_strip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/string_upper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/string_zfill.py
--rw-r--r--   0 runner    (1001) docker     (127)    50075 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/svg_text.py
--rw-r--r--   0 runner    (1001) docker     (127)    46028 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/svg_text_span.py
--rw-r--r--   0 runner    (1001) docker     (127)    11135 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/text_align.py
--rw-r--r--   0 runner    (1001) docker     (127)    14274 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/text_align_last.py
--rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/text_bold.py
--rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/text_fill_alpha.py
--rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/text_fill_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/text_font_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/text_italic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/text_line_height.py
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/text_underline.py
--rw-r--r--   0 runner    (1001) docker     (127)     8047 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/timedelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/timedelta_days.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/timedelta_total_seconds.py
--rw-r--r--   0 runner    (1001) docker     (127)    12931 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/timer_complete.py
--rw-r--r--   0 runner    (1001) docker     (127)    17339 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/timer_delay.py
--rw-r--r--   0 runner    (1001) docker     (127)    13318 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/timer_event.py
--rw-r--r--   0 runner    (1001) docker     (127)    13574 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/timer_repeat_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     9013 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/timer_reset.py
--rw-r--r--   0 runner    (1001) docker     (127)     9087 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/timer_start_and_stop.py
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/to_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/trace.py
--rw-r--r--   0 runner    (1001) docker     (127)    66343 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/triangle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/true_and_false.py
--rw-r--r--   0 runner    (1001) docker     (127)    14525 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/unbind_enter_frame_and_unbind_enter_frame_all.py
--rw-r--r--   0 runner    (1001) docker     (127)    10005 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/unset_debug_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/variable_name_suffix.py
--rw-r--r--   0 runner    (1001) docker     (127)    19570 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/what_apysc_can_do.py
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_translation/jp/why_apysc_doesnt_use_python_builtin_data_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:53.309003 apysc-4.3.0/apysc/_type/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/_return.py
--rw-r--r--   0 runner    (1001) docker     (127)    17556 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/any_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    50943 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/attr_linking_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/attr_to_apysc_val_from_builtin_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/blank_object_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/bool_const_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    17955 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/copy_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/copy_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/deleted_object_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    24160 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/dictionary_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/expression_string.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/false.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/hashable_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/initial_substitution_exp_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/initialize_locals_and_globals_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/int.py
--rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/number.py
--rw-r--r--   0 runner    (1001) docker     (127)    35138 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/number_value_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/py_builtin_iter_disabling_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/repr_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/revert_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    10223 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/revert_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    28760 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/string_apply_max_num_of_decimal_places_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/string_length_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/string_lower_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/string_lstrip_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6652 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/string_rstrip_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/string_slice_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/string_split_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6806 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/string_strip_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/string_upper_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/string_zfill_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/to_fixed_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/to_hex_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/to_number_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/to_string_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/true.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/type_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/type_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/value_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/variable_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/variable_name_suffix_attr_or_var_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/variable_name_suffix_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_type/variable_name_suffix_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:53.309003 apysc-4.3.0/apysc/_validation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   119148 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_validation/arg_validation_decos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_validation/bool_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_validation/color_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10661 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_validation/display_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_validation/event_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_validation/geom_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_validation/handler_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_validation/matrix_data_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8629 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_validation/number_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_validation/parent_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_validation/path_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_validation/string_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_validation/validation_common_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-16 12:54:36.000000 apysc-4.3.0/apysc/_validation/variable_name_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:53.225003 apysc-4.3.0/apysc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-16 12:54:53.000000 apysc-4.3.0/apysc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    28657 2024-05-16 12:54:53.000000 apysc-4.3.0/apysc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 12:54:53.000000 apysc-4.3.0/apysc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-16 12:54:53.000000 apysc-4.3.0/apysc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 12:54:53.000000 apysc-4.3.0/apysc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 12:54:53.309003 apysc-4.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:59.776471 apysc-4.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-19 13:25:32.000000 apysc-4.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-19 13:25:32.000000 apysc-4.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-19 13:25:59.776471 apysc-4.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-05-19 13:25:32.000000 apysc-4.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:59.536472 apysc-4.3.2/apysc/
+-rw-r--r--   0 runner    (1001) docker     (127)   120458 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:59.544472 apysc-4.3.2/apysc/_animation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10351 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_cx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_cx_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_cy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_cy_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_fill_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_fill_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_fill_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_fill_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_finish_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_height.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_height_for_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_height_for_ellipse_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_height_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_line_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_line_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_line_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_line_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_line_thickness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_line_thickness_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_move.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_move_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10250 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_parallel_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_pause_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_play_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_radius.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_radius_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_reset_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_reverse_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_rotation_around_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_rotation_around_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_rotation_around_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_rotation_around_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_scale_x_from_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_scale_x_from_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_scale_x_from_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_scale_x_from_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_scale_y_from_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_scale_y_from_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6921 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_scale_y_from_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_scale_y_from_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_time_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_width.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_width_for_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_width_for_ellipse_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_x.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_y.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/animation_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_animation/easing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:59.544472 apysc-4.3.2/apysc/_auto_reloading/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_auto_reloading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_auto_reloading/auto_reloading_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:59.544472 apysc-4.3.2/apysc/_branch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_branch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_branch/_elif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_branch/_else.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_branch/_if.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_branch/if_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:59.544472 apysc-4.3.2/apysc/_callable/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_callable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_callable/callable_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:59.552472 apysc-4.3.2/apysc/_chart/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/add_background_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/add_border_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/axis_label_bold_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/axis_label_fill_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/axis_label_fill_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/axis_label_font_family_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/axis_label_font_size_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/axis_label_italic_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/axis_line_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/axis_line_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/axis_line_thickness_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/background_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/border_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/chart_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/chart_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22705 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/create_single_column_y_axis_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/initialize_each_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/is_display_axis_label_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/overall_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/set_initial_background_fill_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/set_initial_background_fill_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/set_initial_border_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/set_initial_border_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/set_initial_border_thickness_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/set_initial_height_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/set_initial_horizontal_padding_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/set_initial_matrix_data_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/set_initial_overall_container_coordinates_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/set_initial_vertical_padding_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/set_initial_width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/set_initial_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/set_initial_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/tick_max_num_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/tick_text_bold_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/tick_text_fill_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/tick_text_fill_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/tick_text_font_family_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/tick_text_font_size_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/tick_text_italic_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/tick_text_max_num_of_decimal_places_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9647 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/vertical_bar_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/x_axis_column_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/x_axis_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/x_axis_label_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/x_axis_label_position_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11482 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/x_axis_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/y_axis_column_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/y_axis_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/y_axis_label_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/y_axis_label_position_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/y_axis_single_column_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/y_max_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_chart/y_min_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:59.552472 apysc-4.3.2/apysc/_color/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_color/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_color/blue_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_color/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_color/color_copy_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7843 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_color/color_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_color/colorless.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84071 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_color/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_color/copy_color_if_default_value_specified_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_color/from_rgb_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_color/get_colors_members_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_color/green_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_color/red_color_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:59.552472 apysc-4.3.2/apysc/_console/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_console/_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32116 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_console/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_console/loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:59.556472 apysc-4.3.2/apysc/_converter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_converter/cast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_converter/to_apysc_val_from_builtin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_converter/to_builtin_val_from_apysc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:59.572472 apysc-4.3.2/apysc/_display/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/add_foreign_object_child_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/add_to_parent_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/any_display_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/append_fill_alpha_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/append_fill_color_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/append_foreign_object_constructor_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/append_line_alpha_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/append_line_cap_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/append_line_color_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/append_line_joints_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/append_line_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/append_line_thickness_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/append_x_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/append_y_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/begin_fill_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15676 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/child_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17462 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/circle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/css_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/css_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/css_text_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/css_text_align_last.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/cx_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/cy_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/display_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17384 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5438 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/ellipse_height_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/ellipse_width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/fill_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/fill_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/fixed_html_svg_icon_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/flip_interface_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/flip_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/flip_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/get_bounds_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49066 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/graphics_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/graphics_clear_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/graphics_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/height_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15906 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/line_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/line_cap_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/line_caps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/line_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/line_dash_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/line_dash_dot_setting_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/line_dash_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/line_dash_setting_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/line_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/line_dot_setting_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/line_joints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/line_joints_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/line_round_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/line_round_dot_setting_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26709 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/line_style_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/line_thickness_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12333 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/multi_line_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/opacity_css_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/parent_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18730 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/points_2d_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/points_var_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15565 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/polygon_append_constructor_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/polygon_apply_current_points_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/polygon_x1_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/polygon_x2_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/polygon_x3_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/polygon_y1_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/polygon_y2_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/polygon_y3_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17466 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/polyline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/radius_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19494 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/rotation_around_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9157 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/rotation_around_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/rotation_interface_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/scale_interface_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/scale_x_from_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/scale_x_from_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/scale_y_from_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/scale_y_from_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/set_lower_scale_limit_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/set_overflow_visible_setting_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/set_x_and_y_with_minimum_point_interface_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/skew_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/skew_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7453 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/sprite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12655 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/svg_foreign_object_child.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/svg_foreign_object_child_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/svg_foreign_object_initialize_width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/svg_foreign_object_text_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/svg_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23384 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/svg_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/svg_text_align_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/svg_text_bold_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/svg_text_delta_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/svg_text_delta_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/svg_text_font_family_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/svg_text_font_size_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/svg_text_italic_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/svg_text_leading_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/svg_text_set_align_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/svg_text_set_bold_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/svg_text_set_delta_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/svg_text_set_delta_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/svg_text_set_font_family_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/svg_text_set_font_size_value_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/svg_text_set_italic_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/svg_text_set_leading_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/svg_text_set_text_value_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/svg_text_singleton_for_text_span.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/svg_text_skip_fill_alpha_exp_appending_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/svg_text_skip_fill_color_exp_appending_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/svg_text_skip_line_alpha_exp_appending_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/svg_text_skip_line_color_exp_appending_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/svg_text_skip_line_thickness_exp_appending_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16986 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/svg_text_span.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/svg_text_text_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/text_align_css_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/text_align_last_css_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/text_bold_css_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/text_decoration_underline_css_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/text_fill_color_css_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/text_font_size_css_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/text_italic_css_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/text_line_height_css_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17673 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/triangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/visible_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/width_and_height_mixin_for_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/x_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/y_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_display/y_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:59.576472 apysc-4.3.2/apysc/_event/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_event/animation_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_event/click_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14746 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_event/custom_event_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_event/custom_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_event/document_mouse_wheel_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_event/double_click_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_event/enter_frame_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15687 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_event/enter_frame_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_event/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_event/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9989 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_event/handler_circular_calling_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_event/mouse_down_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_event/mouse_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_event/mouse_event_binding_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_event/mouse_event_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_event/mouse_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_event/mouse_event_unbinding_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_event/mouse_move_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6824 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_event/mouse_out_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_event/mouse_over_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_event/mouse_up_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_event/prevent_default_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_event/set_handler_data_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_event/stop_propagation_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_event/timer_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_event/wheel_event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:59.576472 apysc-4.3.2/apysc/_expression/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_expression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_expression/event_handler_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17851 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_expression/expression_data_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_expression/expression_variables_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_expression/get_last_scope_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_expression/indent_num.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_expression/js_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_expression/last_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_expression/var_names.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:59.576472 apysc-4.3.2/apysc/_file/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_file/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_file/module_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:59.584472 apysc-4.3.2/apysc/_geom/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_geom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10201 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_geom/path_bezier_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7960 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_geom/path_bezier_2d_continual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13379 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_geom/path_bezier_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11011 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_geom/path_bezier_3d_continual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_geom/path_close.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_geom/path_control_x1_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_geom/path_control_x2_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_geom/path_control_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_geom/path_control_y1_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_geom/path_control_y2_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_geom/path_control_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_geom/path_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_geom/path_data_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_geom/path_data_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_geom/path_dest_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_geom/path_dest_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6540 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_geom/path_horizontal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_geom/path_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_geom/path_line_to.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_geom/path_move_to.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_geom/path_vertical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_geom/path_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_geom/path_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12328 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_geom/point2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_geom/rectangle_geom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_geom/rectangle_geom_bottom_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_geom/rectangle_geom_center_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_geom/rectangle_geom_center_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_geom/rectangle_geom_height_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_geom/rectangle_geom_left_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_geom/rectangle_geom_right_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_geom/rectangle_geom_top_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_geom/rectangle_geom_width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_geom/relative_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:59.584472 apysc-4.3.2/apysc/_html/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14617 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_html/debug_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20660 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_html/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_html/html_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_html/html_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:59.584472 apysc-4.3.2/apysc/_jslib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_jslib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70264 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_jslib/jquery-3.7.1.slim.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_jslib/jquery.mousewheel-3.1.13.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_jslib/jslib_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78572 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_jslib/svg-3.1.2.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19431 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_jslib/underscore-1.12.0.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:59.584472 apysc-4.3.2/apysc/_jupyter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_jupyter/jupyter_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:59.584472 apysc-4.3.2/apysc/_lint_and_doc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_lint_and_doc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17625 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_lint_and_doc/add_doc_translation_mapping_blank_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_lint_and_doc/conf_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10316 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_lint_and_doc/docs_keyword_link_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_lint_and_doc/docs_lang.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_lint_and_doc/docs_toctree_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17282 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_lint_and_doc/docs_translation_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13722 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_lint_and_doc/docstring_to_markdown_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51969 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_lint_and_doc/docstring_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7636 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_lint_and_doc/document_text_split_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_lint_and_doc/document_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:59.588472 apysc-4.3.2/apysc/_lint_and_doc/fixed_translation_mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_lint_and_doc/fixed_translation_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_lint_and_doc/fixed_translation_mapping/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)   245896 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_lint_and_doc/fixed_translation_mapping/jp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_lint_and_doc/lint_and_doc_hash_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11174 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_lint_and_doc/translation_mapping_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:59.588472 apysc-4.3.2/apysc/_loop/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_loop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_loop/_continue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_loop/_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_loop/for_array_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_loop/for_array_indices_and_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_loop/for_array_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_loop/for_dict_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7806 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_loop/for_dict_keys_and_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_loop/for_dict_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_loop/for_loop_exit_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_loop/initialize_with_base_value_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_loop/loop_count.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:59.588472 apysc-4.3.2/apysc/_material_design/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:59.736471 apysc-4.3.2/apysc/_material_design/icon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_10k_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_1k_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_1k_plus_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_2k_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_2k_plus_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_3d_rotation_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_3d_rotation_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_3k_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_3k_plus_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_4k_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_4k_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_4k_plus_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_5g_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_5g_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_5k_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_5k_plus_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_6k_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_6k_plus_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_7k_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_7k_plus_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_8k_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_8k_plus_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_9k_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_9k_plus_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_accessibility_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_accessibility_new_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_accessibility_new_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_accessibility_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_accessible_forward_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_accessible_forward_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_accessible_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_accessible_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_account_balance_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_account_balance_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_account_balance_wallet_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_account_balance_wallet_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_account_box_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_account_box_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_account_circle_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_account_circle_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_add_alert_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_add_alert_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_add_box_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_add_box_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_add_circle_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_add_circle_outline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_add_circle_outline_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_add_circle_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_add_ic_call_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_add_ic_call_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_add_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_add_link_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_add_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_add_shopping_cart_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_add_shopping_cart_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_add_task_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_add_task_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_add_to_drive_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_add_to_queue_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_add_to_queue_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_addchart_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_addchart_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_admin_panel_settings_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_admin_panel_settings_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_airplay_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_airplay_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_alarm_add_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_alarm_add_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_alarm_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_alarm_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_alarm_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_alarm_on_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_alarm_on_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_alarm_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_album_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_album_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_all_inbox_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_all_inbox_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_all_out_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_all_out_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_alternate_email_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_alternate_email_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_amp_stories_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_amp_stories_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_analytics_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_analytics_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_anchor_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_anchor_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_android_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_android_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_announcement_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_announcement_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_api_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_api_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_app_blocking_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_app_blocking_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_app_registration_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_archive_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_archive_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_arrow_circle_down_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_arrow_circle_down_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_arrow_circle_up_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_arrow_circle_up_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_arrow_right_alt_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_arrow_right_alt_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_art_track_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_art_track_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_article_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_article_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_aspect_ratio_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_aspect_ratio_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_assessment_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_assessment_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_assignment_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_assignment_ind_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_assignment_ind_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_assignment_late_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_assignment_late_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_assignment_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_assignment_return_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_assignment_return_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_assignment_returned_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_assignment_returned_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_assignment_turned_in_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_assignment_turned_in_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_attribution_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_auto_delete_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_auto_delete_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_autorenew_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_autorenew_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_av_timer_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_av_timer_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_backspace_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_backspace_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_backup_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_backup_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_backup_table_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_backup_table_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_ballot_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_ballot_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_batch_prediction_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_batch_prediction_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_biotech_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_biotech_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_block_flipped_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_block_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_block_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_bolt_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_book_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_book_online_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_book_online_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_book_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_bookmark_border_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_bookmark_border_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_bookmark_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_bookmark_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_bookmarks_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_bookmarks_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_branding_watermark_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_branding_watermark_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_bug_report_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_bug_report_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_build_circle_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_build_circle_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_build_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_build_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_business_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_business_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_cached_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_cached_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_calculate_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_calculate_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_calendar_today_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_calendar_today_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_calendar_view_day_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_calendar_view_day_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_call_end_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_call_end_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_call_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_call_made_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_call_made_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_call_merge_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_call_merge_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_call_missed_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_call_missed_outgoing_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_call_missed_outgoing_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_call_missed_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_call_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_call_received_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_call_received_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_call_split_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_call_split_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_call_to_action_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_call_to_action_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_camera_enhance_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_camera_enhance_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_cancel_presentation_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_cancel_presentation_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_cancel_schedule_send_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_cancel_schedule_send_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_card_giftcard_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_card_giftcard_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_card_membership_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_card_membership_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_card_travel_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_card_travel_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_cell_wifi_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_change_history_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_change_history_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_chat_bubble_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_chat_bubble_outline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_chat_bubble_outline_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_chat_bubble_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_chat_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_chat_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_check_circle_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_check_circle_outline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_check_circle_outline_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_check_circle_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_chrome_reader_mode_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_chrome_reader_mode_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_circle_notifications_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_class_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_class_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_clear_all_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_clear_all_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_clear_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_clear_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_close_fullscreen_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_close_fullscreen_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_closed_caption_disabled_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_closed_caption_disabled_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_closed_caption_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_closed_caption_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_closed_caption_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_code_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_code_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_comment_bank_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_comment_bank_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_comment_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_comment_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_commute_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_commute_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_compare_arrows_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_compare_arrows_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_compress_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_contact_mail_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_contact_mail_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_contact_page_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_contact_page_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_contact_phone_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_contact_phone_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_contact_support_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_contact_support_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_contactless_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_contactless_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_contacts_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_contacts_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_content_copy_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_content_copy_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_content_cut_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_content_cut_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_content_paste_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_content_paste_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_control_camera_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_control_camera_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_copyright_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_copyright_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_create_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_create_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_credit_card_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_credit_card_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_dangerous_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_dashboard_customize_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_dashboard_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_dashboard_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_date_range_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_date_range_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_delete_forever_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_delete_forever_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_delete_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_delete_outline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_delete_outline_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_delete_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_delete_sweep_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_delete_sweep_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_description_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_description_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_desktop_access_disabled_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_desktop_access_disabled_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_dialer_sip_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_dialer_sip_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_dialpad_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_dialpad_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_disabled_by_default_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_disabled_by_default_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_dns_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_dns_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_domain_disabled_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_domain_disabled_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_domain_verification_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_domain_verification_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_done_all_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_done_all_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_done_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_done_outline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_done_outline_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_done_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_donut_large_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_donut_large_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_donut_small_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_donut_small_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_drafts_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_drafts_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_drag_indicator_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_drag_indicator_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_duo_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_duo_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_dynamic_feed_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_dynamic_feed_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_dynamic_form_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_dynamic_form_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_eco_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_eco_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_edit_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_eject_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_eject_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_email_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_email_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_equalizer_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_equalizer_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_error_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_error_outline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_error_outline_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_error_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_euro_symbol_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_euro_symbol_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_event_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_event_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_event_seat_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_event_seat_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_exit_to_app_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_exit_to_app_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_expand_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_explicit_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_explicit_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_explore_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_explore_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_explore_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_explore_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_extension_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_extension_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_face_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_face_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_face_unlock_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_fact_check_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_fact_check_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_fast_forward_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_fast_forward_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_fast_rewind_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_fast_rewind_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_favorite_border_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_favorite_border_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_favorite_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_favorite_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_featured_play_list_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_featured_play_list_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_featured_video_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_featured_video_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_feedback_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_feedback_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_fiber_dvr_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_fiber_dvr_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_fiber_manual_record_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_fiber_manual_record_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_fiber_new_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_fiber_new_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_fiber_pin_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_fiber_pin_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_fiber_smart_record_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_fiber_smart_record_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_file_copy_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_file_copy_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_file_present_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_filter_alt_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_filter_alt_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_filter_list_alt_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_filter_list_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_filter_list_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_find_in_page_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_find_in_page_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_find_replace_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_find_replace_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_fingerprint_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_fingerprint_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_fit_screen_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_flag_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_flag_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_flaky_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_flaky_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_flight_land_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_flight_land_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_flight_takeoff_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_flight_takeoff_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_flip_to_back_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_flip_to_back_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_flip_to_front_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_flip_to_front_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_font_download_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_font_download_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_forum_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_forum_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_forward_10_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_forward_10_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_forward_30_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_forward_30_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_forward_5_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_forward_5_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_forward_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_forward_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_forward_to_inbox_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_forward_to_inbox_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_g_translate_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_g_translate_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_games_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_games_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_gavel_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_gavel_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_gesture_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_gesture_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_get_app_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_get_app_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_gif_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_gif_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_grade_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_grade_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_grading_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_grading_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_group_work_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_group_work_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_hd_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_hd_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_hearing_disabled_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_hearing_disabled_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_hearing_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_hearing_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_help_center_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_help_center_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_help_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_help_outline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_help_outline_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_help_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_high_quality_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_high_quality_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_highlight_alt_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_highlight_alt_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_highlight_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_highlight_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_history_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_history_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_history_toggle_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_history_toggle_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_home_filled_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_home_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_home_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_horizontal_split_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_horizontal_split_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_hourglass_bottom_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_hourglass_bottom_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_hourglass_disabled_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_hourglass_disabled_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_hourglass_empty_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_hourglass_empty_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_hourglass_full_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_hourglass_full_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_hourglass_top_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_hourglass_top_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_how_to_reg_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_how_to_reg_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_how_to_vote_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_how_to_vote_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_http_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_http_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_https_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_https_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_import_contacts_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_import_contacts_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_import_export_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_import_export_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_important_devices_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_important_devices_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_inbox_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_inbox_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_info_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_info_outline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_info_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_input_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_input_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_insights_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_insights_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_integration_instructions_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_integration_instructions_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_inventory_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_invert_colors_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_invert_colors_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_invert_colors_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_invert_colors_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_label_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_label_important_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_label_important_outline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_label_important_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_label_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_label_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_label_outline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_label_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_language_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_language_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_launch_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_launch_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_leaderboard_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_leaderboard_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_library_add_check_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_library_add_check_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_library_add_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_library_add_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_library_books_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_library_books_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_library_music_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_library_music_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_lightbulb_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_lightbulb_outline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_lightbulb_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_line_style_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_line_style_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_line_weight_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_line_weight_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_link_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_link_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_link_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_link_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_list_alt_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_list_alt_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_list_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_list_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_live_help_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_live_help_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_location_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_location_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_location_on_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_location_on_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_lock_clock_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_lock_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_lock_open_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_lock_open_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_lock_outline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_lock_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_login_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_login_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_logout_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_loop_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_loop_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_low_priority_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_low_priority_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_loyalty_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_loyalty_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_mail_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_mail_outline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_mail_outline_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_mail_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_mark_as_unread_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_mark_chat_read_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_mark_chat_read_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_mark_chat_unread_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_mark_chat_unread_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_mark_email_read_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_mark_email_read_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_mark_email_unread_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_mark_email_unread_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_markunread_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_markunread_mailbox_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_markunread_mailbox_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_markunread_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_maximize_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_maximize_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_mediation_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_mediation_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_message_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_message_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_mic_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_mic_none_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_mic_none_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_mic_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_mic_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_mic_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_minimize_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_minimize_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_missed_video_call_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_missed_video_call_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_mobile_screen_share_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_mobile_screen_share_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_model_training_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_model_training_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_more_time_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_more_time_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_move_to_inbox_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_move_to_inbox_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_movie_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_movie_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_music_video_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_music_video_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_nat_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_nat_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_new_releases_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_new_releases_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_next_plan_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_next_plan_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_next_week_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_next_week_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_nightlight_round_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_no_sim_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_no_sim_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_not_accessible_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_not_accessible_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_not_interested_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_not_interested_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_not_started_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_not_started_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_note_add_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_note_add_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_note_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_note_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_notification_important_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_notification_important_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_offline_bolt_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_offline_bolt_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_offline_pin_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_offline_pin_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_online_prediction_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_online_prediction_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_opacity_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_opacity_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_open_in_browser_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_open_in_browser_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_open_in_full_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_open_in_full_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_open_in_new_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_open_in_new_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_open_with_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_open_with_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_outbond_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_outbond_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_outbox_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_outgoing_mail_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_outlet_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_outlet_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_outlined_flag_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_outlined_flag_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_pageview_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_pageview_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_pan_tool_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_pan_tool_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_pause_circle_filled_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_pause_circle_filled_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_pause_circle_outline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_pause_circle_outline_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_pause_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_pause_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_pause_presentation_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_pause_presentation_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_payment_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_payment_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_pending_actions_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_pending_actions_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_pending_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_pending_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_perm_camera_mic_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_perm_camera_mic_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_perm_contact_calendar_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_perm_contact_calendar_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_perm_data_setting_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_perm_data_setting_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_perm_device_information_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_perm_device_information_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_perm_identity_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_perm_identity_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_perm_media_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_perm_media_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_perm_phone_msg_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_perm_phone_msg_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_perm_scan_wifi_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_perm_scan_wifi_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_person_add_disabled_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_person_add_disabled_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_person_search_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_person_search_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_pets_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_pets_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_phone_disabled_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_phone_disabled_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_phone_enabled_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_phone_enabled_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_phone_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_phone_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_phonelink_erase_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_phonelink_erase_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_phonelink_lock_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_phonelink_lock_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_phonelink_ring_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_phonelink_ring_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_phonelink_setup_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_phonelink_setup_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_picture_in_picture_alt_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_picture_in_picture_alt_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_picture_in_picture_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_picture_in_picture_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_plagiarism_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_plagiarism_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_play_arrow_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_play_arrow_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_play_circle_filled_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_play_circle_filled_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_play_circle_outline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_play_circle_outline_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_play_disabled_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_play_for_work_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_play_for_work_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_playlist_add_check_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_playlist_add_check_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_playlist_add_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_playlist_add_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_playlist_play_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_playlist_play_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_policy_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_policy_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_polymer_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_polymer_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_portable_wifi_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_portable_wifi_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_power_settings_new_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_power_settings_new_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_pregnant_woman_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_pregnant_woman_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_present_to_all_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_present_to_all_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_preview_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_preview_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_print_disabled_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_print_disabled_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_print_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_print_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_privacy_tip_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_privacy_tip_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_published_with_changes_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_published_with_changes_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_push_pin_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_push_pin_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_qr_code_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_qr_code_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_qr_code_scanner_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_qr_code_scanner_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_query_builder_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_query_builder_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_question_answer_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_question_answer_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_queue_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_queue_music_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_queue_music_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_queue_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_queue_play_next_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_queue_play_next_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_quickreply_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_quickreply_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_radio_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_radio_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_read_more_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_read_more_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_receipt_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_receipt_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_recent_actors_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_recent_actors_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_record_voice_over_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_record_voice_over_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_redeem_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_redeem_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_redo_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_redo_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_remove_circle_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_remove_circle_outline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_remove_circle_outline_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_remove_circle_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_remove_done_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_remove_from_queue_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_remove_from_queue_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_remove_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_remove_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_remove_shopping_cart_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_remove_shopping_cart_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_reorder_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_reorder_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_repeat_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_repeat_on_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_repeat_one_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_repeat_one_on_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_repeat_one_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_repeat_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_replay_10_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_replay_10_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_replay_30_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_replay_30_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_replay_5_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_replay_5_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_replay_circle_filled_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_replay_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_replay_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_reply_all_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_reply_all_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_reply_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_reply_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_report_gmailerrorred_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_report_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_report_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_report_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_report_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_report_problem_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_report_problem_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_request_page_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_request_page_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_restore_from_trash_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_restore_from_trash_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_restore_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_restore_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_restore_page_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_restore_page_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_ring_volume_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_ring_volume_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_room_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_room_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_rounded_corner_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_rounded_corner_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_rowing_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_rowing_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_rss_feed_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_rss_feed_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_rtt_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_rule_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_rule_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_save_alt_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_save_alt_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_save_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_save_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_saved_search_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_schedule_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_schedule_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_schedule_send_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_screen_share_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_screen_share_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_sd_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_search_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_search_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_search_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_search_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_segment_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_select_all_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_select_all_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_send_and_archive_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_send_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_send_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_sentiment_satisfied_alt_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_sentiment_satisfied_alt_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_settings_applications_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_settings_applications_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_settings_backup_restore_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_settings_backup_restore_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_settings_bluetooth_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_settings_bluetooth_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_settings_brightness_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_settings_brightness_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_settings_cell_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_settings_cell_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_settings_ethernet_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_settings_ethernet_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_settings_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_settings_input_antenna_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_settings_input_antenna_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_settings_input_component_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_settings_input_component_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_settings_input_composite_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_settings_input_composite_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_settings_input_hdmi_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_settings_input_hdmi_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_settings_input_svideo_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_settings_input_svideo_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_settings_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_settings_overscan_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_settings_overscan_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_settings_phone_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_settings_phone_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_settings_power_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_settings_power_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_settings_remote_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_settings_remote_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_settings_voice_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_settings_voice_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_shop_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_shop_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_shop_two_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_shop_two_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_shopping_bag_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_shopping_bag_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_shopping_basket_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_shopping_basket_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_shopping_cart_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_shopping_cart_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_shuffle_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_shuffle_on_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_shuffle_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_skip_next_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_skip_next_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_skip_previous_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_skip_previous_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_slow_motion_video_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_slow_motion_video_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_smart_button_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_smart_button_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_snooze_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_snooze_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_sort_by_alpha_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_sort_by_alpha_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_source_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_source_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_speaker_notes_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_speaker_notes_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_speaker_notes_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_speaker_notes_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_speaker_phone_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_speaker_phone_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_speed_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_speed_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_spellcheck_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_spellcheck_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_star_rate_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_star_rate_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_stars_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_stars_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_stay_current_landscape_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_stay_current_landscape_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_stay_current_portrait_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_stay_current_portrait_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_stay_primary_landscape_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_stay_primary_landscape_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_stay_primary_portrait_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_stay_primary_portrait_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_sticky_note_2_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_sticky_note_2_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_stop_circle_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_stop_circle_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_stop_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_stop_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_stop_screen_share_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_stop_screen_share_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_store_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_store_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_subject_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_subject_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_subscriptions_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_subscriptions_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_subtitles_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_subtitles_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_subtitles_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_subtitles_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_supervised_user_circle_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_supervised_user_circle_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_supervisor_account_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_supervisor_account_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_support_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_support_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_surround_sound_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_surround_sound_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_swap_calls_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_swap_calls_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_swap_horiz_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_swap_horiz_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_swap_horizontal_circle_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_swap_horizontal_circle_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_swap_vert_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_swap_vert_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_swap_vertical_circle_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_swap_vertical_circle_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_swipe_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_sync_alt_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_sync_alt_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_system_update_alt_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_system_update_alt_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_tab_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_tab_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_tab_unselected_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_tab_unselected_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_table_view_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_table_view_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_text_rotate_up_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_text_rotate_up_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_text_rotate_vertical_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_text_rotate_vertical_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_text_rotation_angledown_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_text_rotation_angledown_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_text_rotation_angleup_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_text_rotation_angleup_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_text_rotation_down_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_text_rotation_down_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_text_rotation_none_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_text_rotation_none_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_textsms_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_textsms_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_theaters_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_theaters_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_thumb_down_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_thumb_down_off_alt_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_thumb_down_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_thumb_up_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_thumb_up_off_alt_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_thumb_up_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_thumbs_up_down_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_thumbs_up_down_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_timeline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_timeline_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_toc_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_toc_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_today_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_today_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_toll_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_toll_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_touch_app_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_touch_app_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_tour_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_tour_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_track_changes_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_track_changes_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_translate_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_translate_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_trending_down_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_trending_down_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_trending_flat_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_trending_flat_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_trending_up_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_trending_up_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_turned_in_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_turned_in_not_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_turned_in_not_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_turned_in_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_unpublished_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_unpublished_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_unsubscribe_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_unsubscribe_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_update_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_update_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_upgrade_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_upgrade_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_verified_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_verified_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_verified_user_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_verified_user_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_vertical_split_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_vertical_split_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_video_call_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_video_call_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_video_label_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_video_label_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_video_library_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_video_library_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_video_settings_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_video_settings_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_videocam_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_videocam_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_videocam_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_videocam_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_view_agenda_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_view_agenda_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_view_array_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_view_array_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_view_carousel_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_view_carousel_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_view_column_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_view_column_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_view_day_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_view_day_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_view_headline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_view_headline_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_view_in_ar_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_view_list_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_view_list_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_view_module_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_view_module_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_view_quilt_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_view_quilt_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_view_sidebar_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_view_sidebar_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_view_stream_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_view_stream_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_view_week_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_view_week_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_visibility_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_visibility_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_visibility_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_visibility_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_voice_over_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_voice_over_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_voicemail_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_voicemail_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_volume_down_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_volume_down_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_volume_mute_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_volume_mute_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_volume_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_volume_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_volume_up_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_volume_up_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_vpn_key_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_vpn_key_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_warning_amber_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_warning_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_warning_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_watch_later_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_watch_later_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_web_asset_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_web_asset_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_web_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_web_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_wifi_calling_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_wifi_calling_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_wifi_protected_setup_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_wifi_protected_setup_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_work_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_work_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_work_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_work_outline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_work_outline_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_work_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_wysiwyg_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_wysiwyg_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_youtube_searched_for_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_youtube_searched_for_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_zoom_in_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_zoom_in_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_zoom_out_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_material_design/icon/material_zoom_out_outlined_icon.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:59.736471 apysc-4.3.2/apysc/_math/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_math/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_math/max_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_math/min_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_math/trunc_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:59.736471 apysc-4.3.2/apysc/_string/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_string/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_string/indent_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_string/string_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:59.736471 apysc-4.3.2/apysc/_testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9001 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_testing/e2e_testing_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_testing/testing_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:59.740471 apysc-4.3.2/apysc/_time/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10971 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_time/datetime_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_time/day_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_time/days_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_time/fps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_time/hour_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_time/left_and_right_datetimes_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_time/millisecond_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_time/minute_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_time/month_end_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_time/month_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_time/now_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_time/second_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_time/timedelta_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22600 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_time/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_time/total_seconds_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_time/weekday_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_time/year_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:59.740471 apysc-4.3.2/apysc/_translation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:59.768471 apysc-4.3.2/apysc/_translation/jp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/about_handler_options_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15423 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/add_child_and_remove_child.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7811 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/add_debug_info_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/animation_base_start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/animation_base_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15505 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/animation_complete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/animation_delay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/animation_duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14477 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/animation_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11101 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/animation_fill_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11517 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/animation_fill_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8179 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/animation_finish.py
+-rw-r--r--   0 runner    (1001) docker     (127)   146934 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/animation_interfaces_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11565 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/animation_line_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/animation_line_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11623 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/animation_line_thickness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/animation_method_chaining.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11788 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/animation_move.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13907 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/animation_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/animation_pause_and_play.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/animation_radius.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/animation_reset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/animation_return_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11504 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/animation_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12174 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/animation_rotation_around_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/animation_rotation_around_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22680 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/animation_scale_x_and_y_from_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10757 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/animation_scale_x_and_y_from_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/animation_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24451 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/animation_width_and_height.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13114 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/animation_x.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13134 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/animation_y.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6068 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/append_js_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16245 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/array_append_and_push.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/array_clear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/array_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/array_extend_and_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/array_index_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/array_insert_and_insert_at.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/array_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/array_last_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/array_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/array_pop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/array_remove_and_remove_at.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/array_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/array_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/array_sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16324 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/assert_arrays_equal_and_arrays_not_equal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11225 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/assert_defined_and_undefined.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16840 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/assert_dicts_equal_and_dicts_not_equal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11685 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/assert_equal_and_not_equal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11047 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/assert_greater_and_greater_equal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10860 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/assert_less_and_less_equal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15946 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/assert_true_and_false.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/assertion_basic_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25610 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/bind_and_trigger_custom_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/blue_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15004 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/branch_instruction_variables_reverting_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49953 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/circle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18952 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/color_from_rgb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/colorless.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/contains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/continue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14030 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/datetime_day.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/datetime_hour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/datetime_millisecond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/datetime_minute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/datetime_month.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/datetime_now.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/datetime_second.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/datetime_set_month_end.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9065 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/datetime_weekday_js_and_weekday_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/datetime_year.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16601 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/dblclick.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/dictionary_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/dictionary_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/dictionary_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/display_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23405 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/display_object_and_graphics_base_prop_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9723 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/display_object_get_and_set_css.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/display_object_mouse_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9021 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/display_object_parent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8567 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/display_object_visible.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/display_object_x_and_y.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/display_on_colaboratory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/display_on_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12092 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/draw_interfaces_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85549 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/easing_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12136 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/elif.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51515 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/else.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9718 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/enter_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12970 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/event_prevent_default_and_stop_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10715 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/for_array_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/for_array_indices_and_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9557 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/for_array_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9783 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/for_dict_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11463 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/for_dict_keys_and_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8642 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/for_dict_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/fps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/fundamental_data_classes_value_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6667 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/get_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/get_child_at.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/graphics_base_fill_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/graphics_base_fill_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/graphics_base_flip_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/graphics_base_line_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/graphics_base_line_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9355 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/graphics_base_line_dash_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8863 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/graphics_base_line_dash_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9053 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/graphics_base_line_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9250 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/graphics_base_line_round_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/graphics_base_line_thickness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/graphics_base_rotation_around_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11688 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/graphics_base_rotation_around_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16144 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/graphics_base_scale_from_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24463 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/graphics_base_scale_from_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/graphics_base_skew.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19456 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/graphics_begin_fill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/graphics_clear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8915 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/graphics_draw_circle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9154 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/graphics_draw_dash_dotted_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8546 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/graphics_draw_dashed_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8098 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/graphics_draw_dotted_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10266 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/graphics_draw_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11252 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/graphics_draw_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/graphics_draw_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15102 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/graphics_draw_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10632 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/graphics_draw_rect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/graphics_draw_round_dotted_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10286 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/graphics_draw_round_rect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10974 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/graphics_draw_triangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64374 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/graphics_line_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18270 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/graphics_move_to_and_line_to.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/green_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/if.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/import_conventions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20761 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18347 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/int_and_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11684 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/int_and_number_arithmetic_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/int_and_number_comparison_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/int_and_number_to_fixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/int_and_number_to_hex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48186 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/material_design_colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/math_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/math_min.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/math_trunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/mouse_event_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38153 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/mouse_event_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27701 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/mousedown_and_mouseup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17541 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/mousemove.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28272 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/mouseover_and_mouseout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12910 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/multi_line_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/num_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62153 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13516 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/path_bezier_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11122 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/path_bezier_2d_continual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16364 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/path_bezier_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16314 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/path_bezier_3d_continual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/path_close.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/path_horizontal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/path_line_to.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/path_move_to.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/path_vertical.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/point2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50966 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53243 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/polyline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/quick_start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/recommended_type_checker_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54921 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25542 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/rectangle_geom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/red_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/remove_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/return.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17504 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/save_overall_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/sequential_animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10214 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/set_debug_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/sprite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31274 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/string_addition_and_multiplication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/string_apply_max_num_of_decimal_places.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/string_comparison_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/string_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/string_lower.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7143 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/string_lstrip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7074 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/string_rstrip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8198 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/string_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/string_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/string_strip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/string_upper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/string_zfill.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49436 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/svg_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45588 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/svg_text_span.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11135 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/text_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14274 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/text_align_last.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/text_bold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/text_fill_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/text_fill_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/text_font_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/text_italic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/text_line_height.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/text_underline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8047 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/timedelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/timedelta_days.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/timedelta_total_seconds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12931 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/timer_complete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17339 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/timer_delay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13318 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/timer_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13574 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/timer_repeat_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9013 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/timer_reset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9087 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/timer_start_and_stop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/to_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66343 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/triangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/true_and_false.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14525 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/unbind_enter_frame_and_unbind_enter_frame_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10005 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/unset_debug_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/variable_name_suffix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19570 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/what_apysc_can_do.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_translation/jp/why_apysc_doesnt_use_python_builtin_data_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:59.776471 apysc-4.3.2/apysc/_type/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/_return.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17556 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/any_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50943 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/attr_linking_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/attr_to_apysc_val_from_builtin_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/blank_object_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/bool_const_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17955 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/copy_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/copy_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/deleted_object_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24160 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/dictionary_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/expression_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/false.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/hashable_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/initial_substitution_exp_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/initialize_locals_and_globals_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/int.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35138 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/number_value_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/py_builtin_iter_disabling_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/repr_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/revert_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10223 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/revert_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28760 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/string_apply_max_num_of_decimal_places_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/string_length_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/string_lower_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/string_lstrip_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6652 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/string_rstrip_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/string_slice_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/string_split_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6806 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/string_strip_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/string_upper_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/string_zfill_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/to_fixed_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/to_hex_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/to_number_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/to_string_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/true.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/type_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/type_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/value_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/variable_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/variable_name_suffix_attr_or_var_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/variable_name_suffix_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_type/variable_name_suffix_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:59.776471 apysc-4.3.2/apysc/_validation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119148 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_validation/arg_validation_decos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_validation/bool_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_validation/color_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10661 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_validation/display_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_validation/event_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_validation/geom_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_validation/handler_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_validation/matrix_data_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8629 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_validation/number_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_validation/parent_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_validation/path_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_validation/string_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_validation/validation_common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-19 13:25:32.000000 apysc-4.3.2/apysc/_validation/variable_name_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:59.536472 apysc-4.3.2/apysc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-19 13:25:59.000000 apysc-4.3.2/apysc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    98991 2024-05-19 13:25:59.000000 apysc-4.3.2/apysc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 13:25:59.000000 apysc-4.3.2/apysc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-19 13:25:59.000000 apysc-4.3.2/apysc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-19 13:25:59.000000 apysc-4.3.2/apysc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 13:25:59.776471 apysc-4.3.2/setup.cfg
```

### Comparing `apysc-4.3.0/LICENSE` & `apysc-4.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/PKG-INFO` & `apysc-4.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apysc
-Version: 4.3.0
+Version: 4.3.2
 Summary: apysc is the Python's frontend library to create html and js file, that has the ActionScript 3 (as3)-like interface.
 Home-page: https://github.com/simon-ritchie/apysc
 Maintainer: simon-ritchie
 Maintainer-email: 
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `apysc-4.3.0/README.md` & `apysc-4.3.2/README.md`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_base.py` & `apysc-4.3.2/apysc/_animation/animation_base.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_cx.py` & `apysc-4.3.2/apysc/_animation/animation_cx.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_cx_mixin.py` & `apysc-4.3.2/apysc/_animation/animation_cx_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_cy.py` & `apysc-4.3.2/apysc/_animation/animation_cy.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_cy_mixin.py` & `apysc-4.3.2/apysc/_animation/animation_cy_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_fill_alpha.py` & `apysc-4.3.2/apysc/_animation/animation_fill_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_fill_alpha_mixin.py` & `apysc-4.3.2/apysc/_animation/animation_fill_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_fill_color.py` & `apysc-4.3.2/apysc/_animation/animation_fill_color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_fill_color_mixin.py` & `apysc-4.3.2/apysc/_animation/animation_fill_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_finish_mixin.py` & `apysc-4.3.2/apysc/_animation/animation_finish_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_height.py` & `apysc-4.3.2/apysc/_animation/animation_height.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_height_for_ellipse.py` & `apysc-4.3.2/apysc/_animation/animation_height_for_ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_height_for_ellipse_mixin.py` & `apysc-4.3.2/apysc/_animation/animation_height_for_ellipse_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_height_mixin.py` & `apysc-4.3.2/apysc/_animation/animation_height_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_line_alpha.py` & `apysc-4.3.2/apysc/_animation/animation_line_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_line_alpha_mixin.py` & `apysc-4.3.2/apysc/_animation/animation_line_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_line_color.py` & `apysc-4.3.2/apysc/_animation/animation_line_color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_line_color_mixin.py` & `apysc-4.3.2/apysc/_animation/animation_line_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_line_thickness.py` & `apysc-4.3.2/apysc/_animation/animation_line_thickness.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_line_thickness_mixin.py` & `apysc-4.3.2/apysc/_animation/animation_line_thickness_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_mixins.py` & `apysc-4.3.2/apysc/_animation/animation_mixins.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_move.py` & `apysc-4.3.2/apysc/_animation/animation_move.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_move_mixin.py` & `apysc-4.3.2/apysc/_animation/animation_move_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_parallel.py` & `apysc-4.3.2/apysc/_animation/animation_parallel.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_parallel_mixin.py` & `apysc-4.3.2/apysc/_animation/animation_parallel_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_pause_mixin.py` & `apysc-4.3.2/apysc/_animation/animation_pause_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_play_mixin.py` & `apysc-4.3.2/apysc/_animation/animation_play_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_radius.py` & `apysc-4.3.2/apysc/_animation/animation_radius.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_radius_mixin.py` & `apysc-4.3.2/apysc/_animation/animation_radius_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_reset_mixin.py` & `apysc-4.3.2/apysc/_animation/animation_reset_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_reverse_mixin.py` & `apysc-4.3.2/apysc/_animation/animation_reverse_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_rotation_around_center.py` & `apysc-4.3.2/apysc/_animation/animation_rotation_around_center.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_rotation_around_center_mixin.py` & `apysc-4.3.2/apysc/_animation/animation_rotation_around_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_rotation_around_point.py` & `apysc-4.3.2/apysc/_animation/animation_rotation_around_point.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_rotation_around_point_mixin.py` & `apysc-4.3.2/apysc/_animation/animation_rotation_around_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_scale_x_from_center.py` & `apysc-4.3.2/apysc/_animation/animation_scale_x_from_center.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_scale_x_from_center_mixin.py` & `apysc-4.3.2/apysc/_animation/animation_scale_x_from_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_scale_x_from_point.py` & `apysc-4.3.2/apysc/_animation/animation_scale_x_from_point.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_scale_x_from_point_mixin.py` & `apysc-4.3.2/apysc/_animation/animation_scale_x_from_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_scale_y_from_center.py` & `apysc-4.3.2/apysc/_animation/animation_scale_y_from_center.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_scale_y_from_center_mixin.py` & `apysc-4.3.2/apysc/_animation/animation_scale_y_from_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_scale_y_from_point.py` & `apysc-4.3.2/apysc/_animation/animation_scale_y_from_point.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_scale_y_from_point_mixin.py` & `apysc-4.3.2/apysc/_animation/animation_scale_y_from_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_time_mixin.py` & `apysc-4.3.2/apysc/_animation/animation_time_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_width.py` & `apysc-4.3.2/apysc/_animation/animation_width.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_width_for_ellipse.py` & `apysc-4.3.2/apysc/_animation/animation_width_for_ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_width_for_ellipse_mixin.py` & `apysc-4.3.2/apysc/_animation/animation_width_for_ellipse_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_width_mixin.py` & `apysc-4.3.2/apysc/_animation/animation_width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_x.py` & `apysc-4.3.2/apysc/_animation/animation_x.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_x_mixin.py` & `apysc-4.3.2/apysc/_animation/animation_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_y.py` & `apysc-4.3.2/apysc/_animation/animation_y.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/animation_y_mixin.py` & `apysc-4.3.2/apysc/_animation/animation_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_animation/easing.py` & `apysc-4.3.2/apysc/_animation/easing.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_auto_reloading/auto_reloading_decorator.py` & `apysc-4.3.2/apysc/_auto_reloading/auto_reloading_decorator.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_branch/_elif.py` & `apysc-4.3.2/apysc/_branch/_elif.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_branch/_else.py` & `apysc-4.3.2/apysc/_branch/_else.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_branch/_if.py` & `apysc-4.3.2/apysc/_branch/_if.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_branch/if_base.py` & `apysc-4.3.2/apysc/_branch/if_base.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_callable/callable_util.py` & `apysc-4.3.2/apysc/_callable/callable_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/add_background_mixin.py` & `apysc-4.3.2/apysc/_chart/add_background_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/add_border_mixin.py` & `apysc-4.3.2/apysc/_chart/add_border_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/axis_label_bold_mixin.py` & `apysc-4.3.2/apysc/_chart/axis_label_bold_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/axis_label_fill_alpha_mixin.py` & `apysc-4.3.2/apysc/_chart/axis_label_fill_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/axis_label_fill_color_mixin.py` & `apysc-4.3.2/apysc/_chart/axis_label_fill_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/axis_label_font_family_mixin.py` & `apysc-4.3.2/apysc/_chart/axis_label_font_family_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/axis_label_font_size_mixin.py` & `apysc-4.3.2/apysc/_chart/axis_label_font_size_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/axis_label_italic_mixin.py` & `apysc-4.3.2/apysc/_chart/axis_label_italic_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/axis_line_alpha_mixin.py` & `apysc-4.3.2/apysc/_chart/axis_line_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/axis_line_color_mixin.py` & `apysc-4.3.2/apysc/_chart/axis_line_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/axis_line_thickness_mixin.py` & `apysc-4.3.2/apysc/_chart/axis_line_thickness_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/background_container_mixin.py` & `apysc-4.3.2/apysc/_chart/background_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/border_container_mixin.py` & `apysc-4.3.2/apysc/_chart/border_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/chart_container_mixin.py` & `apysc-4.3.2/apysc/_chart/chart_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/create_single_column_y_axis_mixin.py` & `apysc-4.3.2/apysc/_chart/create_single_column_y_axis_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/initialize_each_container_mixin.py` & `apysc-4.3.2/apysc/_chart/initialize_each_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/is_display_axis_label_mixin.py` & `apysc-4.3.2/apysc/_chart/is_display_axis_label_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/overall_container_mixin.py` & `apysc-4.3.2/apysc/_chart/overall_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/set_initial_background_fill_alpha_mixin.py` & `apysc-4.3.2/apysc/_chart/set_initial_background_fill_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/set_initial_background_fill_color_mixin.py` & `apysc-4.3.2/apysc/_chart/set_initial_background_fill_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/set_initial_border_alpha_mixin.py` & `apysc-4.3.2/apysc/_chart/set_initial_border_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/set_initial_border_color_mixin.py` & `apysc-4.3.2/apysc/_chart/set_initial_border_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/set_initial_border_thickness_mixin.py` & `apysc-4.3.2/apysc/_chart/set_initial_border_thickness_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/set_initial_height_mixin.py` & `apysc-4.3.2/apysc/_chart/set_initial_height_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/set_initial_horizontal_padding_mixin.py` & `apysc-4.3.2/apysc/_chart/set_initial_horizontal_padding_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/set_initial_matrix_data_mixin.py` & `apysc-4.3.2/apysc/_chart/set_initial_matrix_data_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/set_initial_overall_container_coordinates_mixin.py` & `apysc-4.3.2/apysc/_chart/set_initial_overall_container_coordinates_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/set_initial_vertical_padding_mixin.py` & `apysc-4.3.2/apysc/_chart/set_initial_vertical_padding_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/set_initial_width_mixin.py` & `apysc-4.3.2/apysc/_chart/set_initial_width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/set_initial_x_mixin.py` & `apysc-4.3.2/apysc/_chart/set_initial_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/set_initial_y_mixin.py` & `apysc-4.3.2/apysc/_chart/set_initial_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/tick_max_num_mixin.py` & `apysc-4.3.2/apysc/_chart/tick_max_num_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/tick_text_bold_mixin.py` & `apysc-4.3.2/apysc/_chart/tick_text_bold_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/tick_text_fill_alpha_mixin.py` & `apysc-4.3.2/apysc/_chart/tick_text_fill_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/tick_text_fill_color_mixin.py` & `apysc-4.3.2/apysc/_chart/tick_text_fill_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/tick_text_font_family_mixin.py` & `apysc-4.3.2/apysc/_chart/tick_text_font_family_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/tick_text_font_size_mixin.py` & `apysc-4.3.2/apysc/_chart/tick_text_font_size_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/tick_text_italic_mixin.py` & `apysc-4.3.2/apysc/_chart/tick_text_italic_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/tick_text_max_num_of_decimal_places_mixin.py` & `apysc-4.3.2/apysc/_chart/tick_text_max_num_of_decimal_places_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/vertical_bar_chart.py` & `apysc-4.3.2/apysc/_chart/vertical_bar_chart.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/x_axis_column_name_mixin.py` & `apysc-4.3.2/apysc/_chart/x_axis_column_name_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/x_axis_container_mixin.py` & `apysc-4.3.2/apysc/_chart/x_axis_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/x_axis_label_position_mixin.py` & `apysc-4.3.2/apysc/_chart/x_axis_label_position_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/x_axis_settings.py` & `apysc-4.3.2/apysc/_chart/x_axis_settings.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/y_axis_column_name_mixin.py` & `apysc-4.3.2/apysc/_chart/y_axis_column_name_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/y_axis_container_mixin.py` & `apysc-4.3.2/apysc/_chart/y_axis_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/y_axis_label_position_mixin.py` & `apysc-4.3.2/apysc/_chart/y_axis_label_position_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/y_axis_single_column_settings.py` & `apysc-4.3.2/apysc/_chart/y_axis_single_column_settings.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/y_max_mixin.py` & `apysc-4.3.2/apysc/_chart/y_max_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_chart/y_min_mixin.py` & `apysc-4.3.2/apysc/_chart/y_min_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_color/blue_color_mixin.py` & `apysc-4.3.2/apysc/_color/blue_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_color/color.py` & `apysc-4.3.2/apysc/_color/color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_color/color_copy_mixin.py` & `apysc-4.3.2/apysc/_color/color_copy_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_color/color_util.py` & `apysc-4.3.2/apysc/_color/color_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_color/colors.py` & `apysc-4.3.2/apysc/_color/colors.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_color/copy_color_if_default_value_specified_mixin.py` & `apysc-4.3.2/apysc/_color/copy_color_if_default_value_specified_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_color/from_rgb_mixin.py` & `apysc-4.3.2/apysc/_color/from_rgb_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_color/get_colors_members_mixin.py` & `apysc-4.3.2/apysc/_color/get_colors_members_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_color/green_color_mixin.py` & `apysc-4.3.2/apysc/_color/green_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_color/red_color_mixin.py` & `apysc-4.3.2/apysc/_color/red_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_console/_trace.py` & `apysc-4.3.2/apysc/_console/_trace.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_console/assertion.py` & `apysc-4.3.2/apysc/_console/assertion.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_console/loggers.py` & `apysc-4.3.2/apysc/_console/loggers.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_converter/cast.py` & `apysc-4.3.2/apysc/_converter/cast.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_converter/to_apysc_val_from_builtin.py` & `apysc-4.3.2/apysc/_converter/to_apysc_val_from_builtin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_converter/to_builtin_val_from_apysc.py` & `apysc-4.3.2/apysc/_converter/to_builtin_val_from_apysc.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/_document.py` & `apysc-4.3.2/apysc/_display/_document.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/add_foreign_object_child_mixin.py` & `apysc-4.3.2/apysc/_display/add_foreign_object_child_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/add_to_parent_mixin.py` & `apysc-4.3.2/apysc/_display/add_to_parent_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/any_display_object.py` & `apysc-4.3.2/apysc/_display/any_display_object.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/append_fill_alpha_attr_expression_mixin.py` & `apysc-4.3.2/apysc/_display/append_fill_alpha_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/append_fill_color_expression_mixin.py` & `apysc-4.3.2/apysc/_display/append_fill_color_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/append_foreign_object_constructor_expression_mixin.py` & `apysc-4.3.2/apysc/_display/append_foreign_object_constructor_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/append_line_alpha_attr_expression_mixin.py` & `apysc-4.3.2/apysc/_display/append_line_alpha_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/append_line_cap_attr_expression_mixin.py` & `apysc-4.3.2/apysc/_display/append_line_cap_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/append_line_color_attr_expression_mixin.py` & `apysc-4.3.2/apysc/_display/append_line_color_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/append_line_joints_attr_expression_mixin.py` & `apysc-4.3.2/apysc/_display/append_line_joints_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/append_line_point_mixin.py` & `apysc-4.3.2/apysc/_display/append_line_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/append_line_thickness_attr_expression_mixin.py` & `apysc-4.3.2/apysc/_display/append_line_thickness_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/append_x_attr_expression_mixin.py` & `apysc-4.3.2/apysc/_display/append_x_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/append_y_attr_expression_mixin.py` & `apysc-4.3.2/apysc/_display/append_y_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/begin_fill_mixin.py` & `apysc-4.3.2/apysc/_display/begin_fill_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/child_mixin.py` & `apysc-4.3.2/apysc/_display/child_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/circle.py` & `apysc-4.3.2/apysc/_display/circle.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/css_interface.py` & `apysc-4.3.2/apysc/_display/css_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/css_mixin.py` & `apysc-4.3.2/apysc/_display/css_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/cx_mixin.py` & `apysc-4.3.2/apysc/_display/cx_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/cy_mixin.py` & `apysc-4.3.2/apysc/_display/cy_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/display_object.py` & `apysc-4.3.2/apysc/_display/display_object.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/ellipse.py` & `apysc-4.3.2/apysc/_display/ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/ellipse_height_mixin.py` & `apysc-4.3.2/apysc/_display/ellipse_height_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/ellipse_width_mixin.py` & `apysc-4.3.2/apysc/_display/ellipse_width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/fill_alpha_mixin.py` & `apysc-4.3.2/apysc/_display/fill_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/fill_color_mixin.py` & `apysc-4.3.2/apysc/_display/fill_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/flip_interface_helper.py` & `apysc-4.3.2/apysc/_display/flip_interface_helper.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/flip_x_mixin.py` & `apysc-4.3.2/apysc/_display/flip_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/flip_y_mixin.py` & `apysc-4.3.2/apysc/_display/flip_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/get_bounds_mixin.py` & `apysc-4.3.2/apysc/_display/get_bounds_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/graphics.py` & `apysc-4.3.2/apysc/_display/graphics.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/graphics_base.py` & `apysc-4.3.2/apysc/_display/graphics_base.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/graphics_clear_mixin.py` & `apysc-4.3.2/apysc/_display/graphics_clear_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/graphics_expression.py` & `apysc-4.3.2/apysc/_display/graphics_expression.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/height_mixin.py` & `apysc-4.3.2/apysc/_display/height_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/line.py` & `apysc-4.3.2/apysc/_display/line.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/line_alpha_mixin.py` & `apysc-4.3.2/apysc/_display/line_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/line_cap_mixin.py` & `apysc-4.3.2/apysc/_display/line_cap_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/line_caps.py` & `apysc-4.3.2/apysc/_display/line_caps.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/line_color_mixin.py` & `apysc-4.3.2/apysc/_display/line_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/line_dash_dot_setting.py` & `apysc-4.3.2/apysc/_display/line_dash_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/line_dash_dot_setting_mixin.py` & `apysc-4.3.2/apysc/_display/line_dash_dot_setting_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/line_dash_setting.py` & `apysc-4.3.2/apysc/_display/line_dash_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/line_dash_setting_mixin.py` & `apysc-4.3.2/apysc/_display/line_dash_setting_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/line_dot_setting.py` & `apysc-4.3.2/apysc/_display/line_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/line_dot_setting_mixin.py` & `apysc-4.3.2/apysc/_display/line_dot_setting_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/line_joints.py` & `apysc-4.3.2/apysc/_display/line_joints.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/line_joints_mixin.py` & `apysc-4.3.2/apysc/_display/line_joints_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/line_round_dot_setting.py` & `apysc-4.3.2/apysc/_display/line_round_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/line_round_dot_setting_mixin.py` & `apysc-4.3.2/apysc/_display/line_round_dot_setting_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/line_style_mixin.py` & `apysc-4.3.2/apysc/_display/line_style_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/line_thickness_mixin.py` & `apysc-4.3.2/apysc/_display/line_thickness_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/multi_line_text.py` & `apysc-4.3.2/apysc/_display/multi_line_text.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/opacity_css_mixin.py` & `apysc-4.3.2/apysc/_display/opacity_css_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/parent_mixin.py` & `apysc-4.3.2/apysc/_display/parent_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/path.py` & `apysc-4.3.2/apysc/_display/path.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/points_2d_mixin.py` & `apysc-4.3.2/apysc/_display/points_2d_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/polygon.py` & `apysc-4.3.2/apysc/_display/polygon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/polygon_append_constructor_expression_mixin.py` & `apysc-4.3.2/apysc/_display/polygon_append_constructor_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/polygon_apply_current_points_mixin.py` & `apysc-4.3.2/apysc/_display/polygon_apply_current_points_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/polygon_x1_mixin.py` & `apysc-4.3.2/apysc/_display/polygon_x1_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/polygon_x2_mixin.py` & `apysc-4.3.2/apysc/_display/polygon_x2_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/polygon_x3_mixin.py` & `apysc-4.3.2/apysc/_display/polygon_x3_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/polygon_y1_mixin.py` & `apysc-4.3.2/apysc/_display/polygon_y1_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/polygon_y2_mixin.py` & `apysc-4.3.2/apysc/_display/polygon_y2_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/polygon_y3_mixin.py` & `apysc-4.3.2/apysc/_display/polygon_y3_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/polyline.py` & `apysc-4.3.2/apysc/_display/polyline.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/radius_mixin.py` & `apysc-4.3.2/apysc/_display/radius_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/rectangle.py` & `apysc-4.3.2/apysc/_display/rectangle.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/rotation_around_center_mixin.py` & `apysc-4.3.2/apysc/_display/rotation_around_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/rotation_around_point_mixin.py` & `apysc-4.3.2/apysc/_display/rotation_around_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/rotation_interface_helper.py` & `apysc-4.3.2/apysc/_display/rotation_interface_helper.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/scale_interface_helper.py` & `apysc-4.3.2/apysc/_display/scale_interface_helper.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/scale_x_from_center_mixin.py` & `apysc-4.3.2/apysc/_display/scale_x_from_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/scale_x_from_point_mixin.py` & `apysc-4.3.2/apysc/_display/scale_x_from_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/scale_y_from_center_mixin.py` & `apysc-4.3.2/apysc/_display/scale_y_from_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/scale_y_from_point_mixin.py` & `apysc-4.3.2/apysc/_display/scale_y_from_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/set_lower_scale_limit_mixin.py` & `apysc-4.3.2/apysc/_display/set_lower_scale_limit_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/set_overflow_visible_setting_mixin.py` & `apysc-4.3.2/apysc/_display/set_overflow_visible_setting_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/skew_x_mixin.py` & `apysc-4.3.2/apysc/_display/skew_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/skew_y_mixin.py` & `apysc-4.3.2/apysc/_display/skew_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/sprite.py` & `apysc-4.3.2/apysc/_display/sprite.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/stage.py` & `apysc-4.3.2/apysc/_display/stage.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/svg_foreign_object_child.py` & `apysc-4.3.2/apysc/_display/svg_foreign_object_child.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/svg_foreign_object_child_mixin.py` & `apysc-4.3.2/apysc/_display/svg_foreign_object_child_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/svg_foreign_object_initialize_width_mixin.py` & `apysc-4.3.2/apysc/_display/svg_foreign_object_initialize_width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/svg_foreign_object_text_mixin.py` & `apysc-4.3.2/apysc/_display/svg_foreign_object_text_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/svg_icon.py` & `apysc-4.3.2/apysc/_display/svg_icon.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 """
 
 from typing import Optional
 from typing import Union
 
 from apysc._color.color import Color
 from apysc._color.colors import Colors
+from apysc._converter.to_apysc_val_from_builtin import get_copied_int_from_builtin_val
 from apysc._display.add_to_parent_mixin import AddToParentMixIn
 from apysc._display.append_fill_alpha_attr_expression_mixin import (
     AppendFillAlphaAttrExpressionMixIn,
 )
 from apysc._display.append_fill_color_expression_mixin import (
     AppendFillColorAttrExpressionMixIn,
 )
@@ -17,51 +18,72 @@
 from apysc._display.append_y_attr_expression_mixin import AppendYAttrExpressionMixIn
 from apysc._display.child_mixin import ChildMixIn
 from apysc._display.css_mixin import CssMixIn
 from apysc._display.display_object import DisplayObject
 from apysc._display.fill_alpha_mixin import FillAlphaMixIn
 from apysc._display.fill_color_mixin import FillColorMixIn
 from apysc._display.get_bounds_mixin import GetBoundsMixIn
-from apysc._display.scale_x_from_center_mixin import ScaleXFromCenterMixIn
-from apysc._display.scale_y_from_center_mixin import ScaleYFromCenterMixIn
+from apysc._display.height_mixin import HeightMixIn
 from apysc._display.set_overflow_visible_setting_mixin import (
     SetOverflowVisibleSettingMixIn,
 )
+from apysc._display.width_mixin import WidthMixIn
 from apysc._display.x_mixin import XMixIn
 from apysc._display.y_mixin import YMixIn
+from apysc._type.int import Int
 from apysc._type.number import Number
 from apysc._type.variable_name_suffix_mixin import VariableNameSuffixMixIn
+from apysc._validation import arg_validation_decos
 
 
 class SvgIcon(
     XMixIn,
     AppendXAttrExpressionMixIn,
     YMixIn,
     AppendYAttrExpressionMixIn,
-    ScaleXFromCenterMixIn,
-    ScaleYFromCenterMixIn,
     FillColorMixIn,
     AppendFillColorAttrExpressionMixIn,
     FillAlphaMixIn,
     AppendFillAlphaAttrExpressionMixIn,
+    WidthMixIn,
+    HeightMixIn,
     CssMixIn,
     DisplayObject,
     AddToParentMixIn,
     SetOverflowVisibleSettingMixIn,
     GetBoundsMixIn,
     VariableNameSuffixMixIn,
 ):
     _svg_icon_html: str
 
+    # svg_icon_html
+    @arg_validation_decos.is_builtin_string(arg_position_index=1, optional=False)
+    # x
+    @arg_validation_decos.is_num(arg_position_index=2, optional=False)
+    # y
+    @arg_validation_decos.is_num(arg_position_index=3, optional=False)
+    # size
+    @arg_validation_decos.is_integer(arg_position_index=4, optional=False)
+    # fill_color
+    @arg_validation_decos.is_color(arg_position_index=5, optional=False)
+    # fill_alpha
+    @arg_validation_decos.num_is_0_to_1_range(arg_position_index=6, optional=False)
+    # parent
+    @arg_validation_decos.is_display_object_container(
+        arg_position_index=7, optional=True
+    )
+    # variable_name_suffix
+    @arg_validation_decos.is_builtin_string(arg_position_index=8, optional=False)
     def __init__(
         self,
         *,
         svg_icon_html: str,
         x: Union[float, Number] = 0.0,
         y: Union[float, Number] = 0.0,
+        size: Union[int, Int] = 24,
         fill_color: Color = Colors.GRAY_666666,
         fill_alpha: Union[float, Number] = 1.0,
         parent: Optional[ChildMixIn] = None,
         variable_name_suffix: str = "",
     ) -> None:
         """
         The SVG icon class implementation.
@@ -71,14 +93,16 @@
         svg_icon_html : str
             An SVG icon html string.
             For example, "<svg xmlns="http://www.w3.org/2000/svg" ...>...</svg>"
         x : float or Number, optional
             X-coordinate of the icon.
         y : float or Number, optional
             Y-coordinate of the icon.
+        size : int or Int, default 24
+            Size of the icon.
         fill_color : Color, default Colors.GRAY_666666
             Fill-color of the icon.
         fill_alpha : float or Number, default 1.0
             Fill-alpha of the icon.
         parent : ChildMixIn or None, default None
             A parent instance to add this instance.
             If the specified value is None, this interface uses
@@ -94,19 +118,22 @@
         from apysc._expression import var_names
 
         self._variable_name_suffix = variable_name_suffix
         variable_name: str = expression_variables_util.get_next_variable_name(
             type_name=var_names.SVG_ICON
         )
         self.variable_name = variable_name
-        self._svg_icon_html = svg_icon_html
+        self._svg_icon_html = svg_icon_html.replace("'", '"')
         self._append_constructor_expression()
         super(SvgIcon, self).__init__(variable_name=variable_name)
         self.x = get_copied_number_from_builtin_val(float_or_num=x)
         self.y = get_copied_number_from_builtin_val(float_or_num=y)
+        size_: Int = get_copied_int_from_builtin_val(integer=size)
+        self.width = size_
+        self.height = size_
         self.fill_color = fill_color
         self.fill_alpha = get_copied_number_from_builtin_val(float_or_num=fill_alpha)
         self._set_overflow_visible_setting()
         self._add_to_parent(parent=parent)
 
     def _append_constructor_expression(self) -> None:
         """
```

### Comparing `apysc-4.3.0/apysc/_display/svg_text.py` & `apysc-4.3.2/apysc/_display/svg_text.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/svg_text_align_mixin.py` & `apysc-4.3.2/apysc/_display/svg_text_align_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/svg_text_bold_mixin.py` & `apysc-4.3.2/apysc/_display/svg_text_bold_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/svg_text_delta_x_mixin.py` & `apysc-4.3.2/apysc/_display/svg_text_delta_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/svg_text_delta_y_mixin.py` & `apysc-4.3.2/apysc/_display/svg_text_delta_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/svg_text_font_family_mixin.py` & `apysc-4.3.2/apysc/_display/svg_text_font_family_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/svg_text_font_size_mixin.py` & `apysc-4.3.2/apysc/_display/svg_text_font_size_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/svg_text_italic_mixin.py` & `apysc-4.3.2/apysc/_display/svg_text_italic_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/svg_text_leading_mixin.py` & `apysc-4.3.2/apysc/_display/svg_text_leading_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/svg_text_set_align_mixin.py` & `apysc-4.3.2/apysc/_display/svg_text_set_align_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/svg_text_set_bold_mixin.py` & `apysc-4.3.2/apysc/_display/svg_text_set_bold_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/svg_text_set_delta_x_mixin.py` & `apysc-4.3.2/apysc/_display/svg_text_set_delta_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/svg_text_set_delta_y_mixin.py` & `apysc-4.3.2/apysc/_display/svg_text_set_delta_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/svg_text_set_font_family_mixin.py` & `apysc-4.3.2/apysc/_display/svg_text_set_font_family_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/svg_text_set_font_size_value_mixin.py` & `apysc-4.3.2/apysc/_display/svg_text_set_font_size_value_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/svg_text_set_italic_mixin.py` & `apysc-4.3.2/apysc/_display/svg_text_set_italic_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/svg_text_set_leading_mixin.py` & `apysc-4.3.2/apysc/_display/svg_text_set_leading_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/svg_text_set_text_value_mixin.py` & `apysc-4.3.2/apysc/_display/svg_text_set_text_value_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/svg_text_singleton_for_text_span.py` & `apysc-4.3.2/apysc/_display/svg_text_singleton_for_text_span.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/svg_text_skip_fill_alpha_exp_appending_mixin.py` & `apysc-4.3.2/apysc/_display/svg_text_skip_fill_alpha_exp_appending_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/svg_text_skip_fill_color_exp_appending_mixin.py` & `apysc-4.3.2/apysc/_display/svg_text_skip_fill_color_exp_appending_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/svg_text_skip_line_alpha_exp_appending_mixin.py` & `apysc-4.3.2/apysc/_display/svg_text_skip_line_alpha_exp_appending_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/svg_text_skip_line_color_exp_appending_mixin.py` & `apysc-4.3.2/apysc/_display/svg_text_skip_line_color_exp_appending_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/svg_text_skip_line_thickness_exp_appending_mixin.py` & `apysc-4.3.2/apysc/_display/svg_text_skip_line_thickness_exp_appending_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/svg_text_span.py` & `apysc-4.3.2/apysc/_display/svg_text_span.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/svg_text_text_mixin.py` & `apysc-4.3.2/apysc/_display/svg_text_text_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/text_align_css_mixin.py` & `apysc-4.3.2/apysc/_display/text_align_css_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/text_align_last_css_mixin.py` & `apysc-4.3.2/apysc/_display/text_align_last_css_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/text_bold_css_mixin.py` & `apysc-4.3.2/apysc/_display/text_bold_css_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/text_decoration_underline_css_mixin.py` & `apysc-4.3.2/apysc/_display/text_decoration_underline_css_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/text_fill_color_css_mixin.py` & `apysc-4.3.2/apysc/_display/text_fill_color_css_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/text_font_size_css_mixin.py` & `apysc-4.3.2/apysc/_display/text_font_size_css_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/text_italic_css_mixin.py` & `apysc-4.3.2/apysc/_display/text_italic_css_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/text_line_height_css_mixin.py` & `apysc-4.3.2/apysc/_display/text_line_height_css_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/triangle.py` & `apysc-4.3.2/apysc/_display/triangle.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/visible_mixin.py` & `apysc-4.3.2/apysc/_display/visible_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/width_and_height_mixin_for_ellipse.py` & `apysc-4.3.2/apysc/_display/width_and_height_mixin_for_ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/width_mixin.py` & `apysc-4.3.2/apysc/_display/width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/x_interface.py` & `apysc-4.3.2/apysc/_display/x_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/x_mixin.py` & `apysc-4.3.2/apysc/_display/x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/y_interface.py` & `apysc-4.3.2/apysc/_display/y_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_display/y_mixin.py` & `apysc-4.3.2/apysc/_display/y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_event/animation_event.py` & `apysc-4.3.2/apysc/_event/animation_event.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_event/click_mixin.py` & `apysc-4.3.2/apysc/_event/click_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_event/custom_event_mixin.py` & `apysc-4.3.2/apysc/_event/custom_event_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_event/document_mouse_wheel_func.py` & `apysc-4.3.2/apysc/_event/document_mouse_wheel_func.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_event/double_click_mixin.py` & `apysc-4.3.2/apysc/_event/double_click_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_event/enter_frame_event.py` & `apysc-4.3.2/apysc/_event/enter_frame_event.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_event/enter_frame_mixin.py` & `apysc-4.3.2/apysc/_event/enter_frame_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_event/event.py` & `apysc-4.3.2/apysc/_event/event.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_event/handler.py` & `apysc-4.3.2/apysc/_event/handler.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_event/handler_circular_calling_util.py` & `apysc-4.3.2/apysc/_event/handler_circular_calling_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_event/mouse_down_mixin.py` & `apysc-4.3.2/apysc/_event/mouse_down_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_event/mouse_event.py` & `apysc-4.3.2/apysc/_event/mouse_event.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_event/mouse_event_binding_expression_mixin.py` & `apysc-4.3.2/apysc/_event/mouse_event_binding_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_event/mouse_event_mixins.py` & `apysc-4.3.2/apysc/_event/mouse_event_mixins.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_event/mouse_event_unbinding_mixin.py` & `apysc-4.3.2/apysc/_event/mouse_event_unbinding_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_event/mouse_move_mixin.py` & `apysc-4.3.2/apysc/_event/mouse_move_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_event/mouse_out_mixin.py` & `apysc-4.3.2/apysc/_event/mouse_out_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_event/mouse_over_mixin.py` & `apysc-4.3.2/apysc/_event/mouse_over_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_event/mouse_up_mixin.py` & `apysc-4.3.2/apysc/_event/mouse_up_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_event/prevent_default_mixin.py` & `apysc-4.3.2/apysc/_event/prevent_default_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_event/set_handler_data_mixin.py` & `apysc-4.3.2/apysc/_event/set_handler_data_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_event/stop_propagation_mixin.py` & `apysc-4.3.2/apysc/_event/stop_propagation_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_event/timer_event.py` & `apysc-4.3.2/apysc/_event/timer_event.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_event/wheel_event.py` & `apysc-4.3.2/apysc/_event/wheel_event.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_expression/event_handler_scope.py` & `apysc-4.3.2/apysc/_expression/event_handler_scope.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_expression/expression_data_util.py` & `apysc-4.3.2/apysc/_expression/expression_data_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_expression/expression_variables_util.py` & `apysc-4.3.2/apysc/_expression/expression_variables_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_expression/indent_num.py` & `apysc-4.3.2/apysc/_expression/indent_num.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_expression/js_functions.py` & `apysc-4.3.2/apysc/_expression/js_functions.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_expression/last_scope.py` & `apysc-4.3.2/apysc/_expression/last_scope.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_expression/var_names.py` & `apysc-4.3.2/apysc/_expression/var_names.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_file/file_util.py` & `apysc-4.3.2/apysc/_file/file_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_file/module_util.py` & `apysc-4.3.2/apysc/_file/module_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_geom/path_bezier_2d.py` & `apysc-4.3.2/apysc/_geom/path_bezier_2d.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_geom/path_bezier_2d_continual.py` & `apysc-4.3.2/apysc/_geom/path_bezier_2d_continual.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_geom/path_bezier_3d.py` & `apysc-4.3.2/apysc/_geom/path_bezier_3d.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_geom/path_bezier_3d_continual.py` & `apysc-4.3.2/apysc/_geom/path_bezier_3d_continual.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_geom/path_close.py` & `apysc-4.3.2/apysc/_geom/path_close.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_geom/path_control_x1_mixin.py` & `apysc-4.3.2/apysc/_geom/path_control_x1_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_geom/path_control_x2_mixin.py` & `apysc-4.3.2/apysc/_geom/path_control_x2_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_geom/path_control_x_mixin.py` & `apysc-4.3.2/apysc/_geom/path_control_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_geom/path_control_y1_mixin.py` & `apysc-4.3.2/apysc/_geom/path_control_y1_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_geom/path_control_y2_mixin.py` & `apysc-4.3.2/apysc/_geom/path_control_y2_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_geom/path_control_y_mixin.py` & `apysc-4.3.2/apysc/_geom/path_control_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_geom/path_data.py` & `apysc-4.3.2/apysc/_geom/path_data.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_geom/path_data_base.py` & `apysc-4.3.2/apysc/_geom/path_data_base.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_geom/path_data_util.py` & `apysc-4.3.2/apysc/_geom/path_data_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_geom/path_dest_x_mixin.py` & `apysc-4.3.2/apysc/_geom/path_dest_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_geom/path_dest_y_mixin.py` & `apysc-4.3.2/apysc/_geom/path_dest_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_geom/path_horizontal.py` & `apysc-4.3.2/apysc/_geom/path_horizontal.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_geom/path_line_to.py` & `apysc-4.3.2/apysc/_geom/path_line_to.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_geom/path_move_to.py` & `apysc-4.3.2/apysc/_geom/path_move_to.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_geom/path_vertical.py` & `apysc-4.3.2/apysc/_geom/path_vertical.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_geom/path_x_mixin.py` & `apysc-4.3.2/apysc/_geom/path_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_geom/path_y_mixin.py` & `apysc-4.3.2/apysc/_geom/path_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_geom/point2d.py` & `apysc-4.3.2/apysc/_geom/point2d.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_geom/rectangle_geom.py` & `apysc-4.3.2/apysc/_geom/rectangle_geom.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_geom/rectangle_geom_bottom_y_mixin.py` & `apysc-4.3.2/apysc/_geom/rectangle_geom_bottom_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_geom/rectangle_geom_center_x_mixin.py` & `apysc-4.3.2/apysc/_geom/rectangle_geom_center_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_geom/rectangle_geom_center_y_mixin.py` & `apysc-4.3.2/apysc/_geom/rectangle_geom_center_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_geom/rectangle_geom_height_mixin.py` & `apysc-4.3.2/apysc/_geom/rectangle_geom_height_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_geom/rectangle_geom_left_x_mixin.py` & `apysc-4.3.2/apysc/_geom/rectangle_geom_left_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_geom/rectangle_geom_right_x_mixin.py` & `apysc-4.3.2/apysc/_geom/rectangle_geom_right_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_geom/rectangle_geom_top_y_mixin.py` & `apysc-4.3.2/apysc/_geom/rectangle_geom_top_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_geom/rectangle_geom_width_mixin.py` & `apysc-4.3.2/apysc/_geom/rectangle_geom_width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_geom/relative_mixin.py` & `apysc-4.3.2/apysc/_geom/relative_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_html/debug_mode.py` & `apysc-4.3.2/apysc/_html/debug_mode.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_html/exporter.py` & `apysc-4.3.2/apysc/_html/exporter.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_html/html_util.py` & `apysc-4.3.2/apysc/_html/html_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_jslib/jquery-3.7.1.slim.min.js` & `apysc-4.3.2/apysc/_jslib/jquery-3.7.1.slim.min.js`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_jslib/jquery.mousewheel-3.1.13.min.js` & `apysc-4.3.2/apysc/_jslib/jquery.mousewheel-3.1.13.min.js`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_jslib/jslib_util.py` & `apysc-4.3.2/apysc/_jslib/jslib_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_jslib/svg-3.1.2.min.js` & `apysc-4.3.2/apysc/_jslib/svg-3.1.2.min.js`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_jslib/underscore-1.12.0.min.js` & `apysc-4.3.2/apysc/_jslib/underscore-1.12.0.min.js`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_jupyter/jupyter_util.py` & `apysc-4.3.2/apysc/_jupyter/jupyter_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_lint_and_doc/add_doc_translation_mapping_blank_data.py` & `apysc-4.3.2/apysc/_lint_and_doc/add_doc_translation_mapping_blank_data.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_lint_and_doc/conf_common.py` & `apysc-4.3.2/apysc/_lint_and_doc/conf_common.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_lint_and_doc/docs_keyword_link_mapping.py` & `apysc-4.3.2/apysc/_lint_and_doc/docs_keyword_link_mapping.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_lint_and_doc/docs_lang.py` & `apysc-4.3.2/apysc/_lint_and_doc/docs_lang.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_lint_and_doc/docs_toctree_util.py` & `apysc-4.3.2/apysc/_lint_and_doc/docs_toctree_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_lint_and_doc/docs_translation_converter.py` & `apysc-4.3.2/apysc/_lint_and_doc/docs_translation_converter.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_lint_and_doc/docstring_to_markdown_converter.py` & `apysc-4.3.2/apysc/_lint_and_doc/docstring_to_markdown_converter.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_lint_and_doc/docstring_util.py` & `apysc-4.3.2/apysc/_lint_and_doc/docstring_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_lint_and_doc/document_text_split_util.py` & `apysc-4.3.2/apysc/_lint_and_doc/document_text_split_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_lint_and_doc/document_util.py` & `apysc-4.3.2/apysc/_lint_and_doc/document_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_lint_and_doc/fixed_translation_mapping/data_model.py` & `apysc-4.3.2/apysc/_lint_and_doc/fixed_translation_mapping/data_model.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_lint_and_doc/fixed_translation_mapping/jp.py` & `apysc-4.3.2/apysc/_lint_and_doc/fixed_translation_mapping/jp.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_lint_and_doc/lint_and_doc_hash_util.py` & `apysc-4.3.2/apysc/_lint_and_doc/lint_and_doc_hash_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_lint_and_doc/translation_mapping_utils.py` & `apysc-4.3.2/apysc/_lint_and_doc/translation_mapping_utils.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_loop/_continue.py` & `apysc-4.3.2/apysc/_loop/_continue.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_loop/_range.py` & `apysc-4.3.2/apysc/_loop/_range.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_loop/for_array_indices.py` & `apysc-4.3.2/apysc/_loop/for_array_indices.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_loop/for_array_indices_and_values.py` & `apysc-4.3.2/apysc/_loop/for_array_indices_and_values.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_loop/for_array_values.py` & `apysc-4.3.2/apysc/_loop/for_array_values.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_loop/for_dict_keys.py` & `apysc-4.3.2/apysc/_loop/for_dict_keys.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_loop/for_dict_keys_and_values.py` & `apysc-4.3.2/apysc/_loop/for_dict_keys_and_values.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_loop/for_dict_values.py` & `apysc-4.3.2/apysc/_loop/for_dict_values.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_loop/for_loop_exit_mixin.py` & `apysc-4.3.2/apysc/_loop/for_loop_exit_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_loop/loop_count.py` & `apysc-4.3.2/apysc/_loop/loop_count.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_math/max_mixin.py` & `apysc-4.3.2/apysc/_math/max_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_math/min_mixin.py` & `apysc-4.3.2/apysc/_math/min_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_math/trunc_mixin.py` & `apysc-4.3.2/apysc/_math/trunc_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_string/indent_util.py` & `apysc-4.3.2/apysc/_string/indent_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_string/string_util.py` & `apysc-4.3.2/apysc/_string/string_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_testing/e2e_testing_helper.py` & `apysc-4.3.2/apysc/_testing/e2e_testing_helper.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_testing/testing_helper.py` & `apysc-4.3.2/apysc/_testing/testing_helper.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_time/datetime_.py` & `apysc-4.3.2/apysc/_time/datetime_.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_time/day_mixin.py` & `apysc-4.3.2/apysc/_time/day_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_time/days_mixin.py` & `apysc-4.3.2/apysc/_time/days_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_time/fps.py` & `apysc-4.3.2/apysc/_time/fps.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_time/hour_mixin.py` & `apysc-4.3.2/apysc/_time/hour_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_time/left_and_right_datetimes_mixin.py` & `apysc-4.3.2/apysc/_time/left_and_right_datetimes_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_time/millisecond_mixin.py` & `apysc-4.3.2/apysc/_time/millisecond_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_time/minute_mixin.py` & `apysc-4.3.2/apysc/_time/minute_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_time/month_end_mixin.py` & `apysc-4.3.2/apysc/_time/month_end_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_time/month_mixin.py` & `apysc-4.3.2/apysc/_time/month_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_time/now_mixin.py` & `apysc-4.3.2/apysc/_time/now_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_time/second_mixin.py` & `apysc-4.3.2/apysc/_time/second_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_time/timedelta_.py` & `apysc-4.3.2/apysc/_time/timedelta_.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_time/timer.py` & `apysc-4.3.2/apysc/_time/timer.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_time/total_seconds_mixin.py` & `apysc-4.3.2/apysc/_time/total_seconds_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_time/weekday_mixin.py` & `apysc-4.3.2/apysc/_time/weekday_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_time/year_mixin.py` & `apysc-4.3.2/apysc/_time/year_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/about_handler_options_type.py` & `apysc-4.3.2/apysc/_translation/jp/about_handler_options_type.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/add_child_and_remove_child.py` & `apysc-4.3.2/apysc/_translation/jp/add_child_and_remove_child.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/add_debug_info_setting.py` & `apysc-4.3.2/apysc/_translation/jp/add_debug_info_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/animation_base_start.py` & `apysc-4.3.2/apysc/_translation/jp/animation_base_start.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/animation_base_target.py` & `apysc-4.3.2/apysc/_translation/jp/animation_base_target.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/animation_complete.py` & `apysc-4.3.2/apysc/_translation/jp/animation_complete.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/animation_delay.py` & `apysc-4.3.2/apysc/_translation/jp/animation_delay.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/animation_duration.py` & `apysc-4.3.2/apysc/_translation/jp/animation_duration.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/animation_event.py` & `apysc-4.3.2/apysc/_translation/jp/animation_event.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/animation_fill_alpha.py` & `apysc-4.3.2/apysc/_translation/jp/animation_fill_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/animation_fill_color.py` & `apysc-4.3.2/apysc/_translation/jp/animation_fill_color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/animation_finish.py` & `apysc-4.3.2/apysc/_translation/jp/animation_finish.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/animation_interfaces_abstract.py` & `apysc-4.3.2/apysc/_translation/jp/animation_interfaces_abstract.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/animation_line_alpha.py` & `apysc-4.3.2/apysc/_translation/jp/animation_line_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/animation_line_color.py` & `apysc-4.3.2/apysc/_translation/jp/animation_line_color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/animation_line_thickness.py` & `apysc-4.3.2/apysc/_translation/jp/animation_line_thickness.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/animation_method_chaining.py` & `apysc-4.3.2/apysc/_translation/jp/animation_method_chaining.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/animation_move.py` & `apysc-4.3.2/apysc/_translation/jp/animation_move.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/animation_parallel.py` & `apysc-4.3.2/apysc/_translation/jp/animation_parallel.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/animation_pause_and_play.py` & `apysc-4.3.2/apysc/_translation/jp/animation_pause_and_play.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/animation_radius.py` & `apysc-4.3.2/apysc/_translation/jp/animation_radius.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/animation_reset.py` & `apysc-4.3.2/apysc/_translation/jp/animation_reset.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/animation_return_value.py` & `apysc-4.3.2/apysc/_translation/jp/animation_return_value.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/animation_reverse.py` & `apysc-4.3.2/apysc/_translation/jp/animation_reverse.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/animation_rotation_around_center.py` & `apysc-4.3.2/apysc/_translation/jp/animation_rotation_around_center.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/animation_rotation_around_point.py` & `apysc-4.3.2/apysc/_translation/jp/animation_rotation_around_point.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/animation_scale_x_and_y_from_center.py` & `apysc-4.3.2/apysc/_translation/jp/animation_scale_x_and_y_from_center.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/animation_scale_x_and_y_from_point.py` & `apysc-4.3.2/apysc/_translation/jp/animation_scale_x_and_y_from_point.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/animation_time.py` & `apysc-4.3.2/apysc/_translation/jp/animation_time.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/animation_width_and_height.py` & `apysc-4.3.2/apysc/_translation/jp/animation_width_and_height.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/animation_x.py` & `apysc-4.3.2/apysc/_translation/jp/animation_x.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/animation_y.py` & `apysc-4.3.2/apysc/_translation/jp/animation_y.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/append_js_expression.py` & `apysc-4.3.2/apysc/_translation/jp/append_js_expression.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/array.py` & `apysc-4.3.2/apysc/_translation/jp/array.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/array_append_and_push.py` & `apysc-4.3.2/apysc/_translation/jp/array_append_and_push.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/array_clear.py` & `apysc-4.3.2/apysc/_translation/jp/array_clear.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/array_comparison.py` & `apysc-4.3.2/apysc/_translation/jp/array_comparison.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/array_extend_and_concat.py` & `apysc-4.3.2/apysc/_translation/jp/array_extend_and_concat.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/array_index_of.py` & `apysc-4.3.2/apysc/_translation/jp/array_index_of.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/array_insert_and_insert_at.py` & `apysc-4.3.2/apysc/_translation/jp/array_insert_and_insert_at.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/array_join.py` & `apysc-4.3.2/apysc/_translation/jp/array_join.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/array_last_value.py` & `apysc-4.3.2/apysc/_translation/jp/array_last_value.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/array_length.py` & `apysc-4.3.2/apysc/_translation/jp/array_length.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/array_pop.py` & `apysc-4.3.2/apysc/_translation/jp/array_pop.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/array_remove_and_remove_at.py` & `apysc-4.3.2/apysc/_translation/jp/array_remove_and_remove_at.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/array_reverse.py` & `apysc-4.3.2/apysc/_translation/jp/array_reverse.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/array_slice.py` & `apysc-4.3.2/apysc/_translation/jp/array_slice.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/array_sort.py` & `apysc-4.3.2/apysc/_translation/jp/array_sort.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/assert_arrays_equal_and_arrays_not_equal.py` & `apysc-4.3.2/apysc/_translation/jp/assert_arrays_equal_and_arrays_not_equal.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/assert_defined_and_undefined.py` & `apysc-4.3.2/apysc/_translation/jp/assert_defined_and_undefined.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/assert_dicts_equal_and_dicts_not_equal.py` & `apysc-4.3.2/apysc/_translation/jp/assert_dicts_equal_and_dicts_not_equal.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/assert_equal_and_not_equal.py` & `apysc-4.3.2/apysc/_translation/jp/assert_equal_and_not_equal.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/assert_greater_and_greater_equal.py` & `apysc-4.3.2/apysc/_translation/jp/assert_greater_and_greater_equal.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/assert_less_and_less_equal.py` & `apysc-4.3.2/apysc/_translation/jp/assert_less_and_less_equal.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/assert_true_and_false.py` & `apysc-4.3.2/apysc/_translation/jp/assert_true_and_false.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/assertion_basic_behavior.py` & `apysc-4.3.2/apysc/_translation/jp/assertion_basic_behavior.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/bind_and_trigger_custom_event.py` & `apysc-4.3.2/apysc/_translation/jp/bind_and_trigger_custom_event.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/blue_color.py` & `apysc-4.3.2/apysc/_translation/jp/blue_color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/boolean.py` & `apysc-4.3.2/apysc/_translation/jp/boolean.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/branch_instruction_variables_reverting_setting.py` & `apysc-4.3.2/apysc/_translation/jp/branch_instruction_variables_reverting_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/circle.py` & `apysc-4.3.2/apysc/_translation/jp/circle.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/click.py` & `apysc-4.3.2/apysc/_translation/jp/click.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/color.py` & `apysc-4.3.2/apysc/_translation/jp/color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/color_from_rgb.py` & `apysc-4.3.2/apysc/_translation/jp/color_from_rgb.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/colorless.py` & `apysc-4.3.2/apysc/_translation/jp/colorless.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/colors.py` & `apysc-4.3.2/apysc/_translation/jp/colors.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/contains.py` & `apysc-4.3.2/apysc/_translation/jp/contains.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/continue.py` & `apysc-4.3.2/apysc/_translation/jp/continue.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/datetime.py` & `apysc-4.3.2/apysc/_translation/jp/datetime.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/datetime_day.py` & `apysc-4.3.2/apysc/_translation/jp/datetime_day.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/datetime_hour.py` & `apysc-4.3.2/apysc/_translation/jp/datetime_hour.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/datetime_millisecond.py` & `apysc-4.3.2/apysc/_translation/jp/datetime_millisecond.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/datetime_minute.py` & `apysc-4.3.2/apysc/_translation/jp/datetime_minute.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/datetime_month.py` & `apysc-4.3.2/apysc/_translation/jp/datetime_month.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/datetime_now.py` & `apysc-4.3.2/apysc/_translation/jp/datetime_now.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/datetime_second.py` & `apysc-4.3.2/apysc/_translation/jp/datetime_second.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/datetime_set_month_end.py` & `apysc-4.3.2/apysc/_translation/jp/datetime_set_month_end.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/datetime_weekday_js_and_weekday_py.py` & `apysc-4.3.2/apysc/_translation/jp/datetime_weekday_js_and_weekday_py.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/datetime_year.py` & `apysc-4.3.2/apysc/_translation/jp/datetime_year.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/dblclick.py` & `apysc-4.3.2/apysc/_translation/jp/dblclick.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/delete.py` & `apysc-4.3.2/apysc/_translation/jp/delete.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/dictionary.py` & `apysc-4.3.2/apysc/_translation/jp/dictionary.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/dictionary_generic.py` & `apysc-4.3.2/apysc/_translation/jp/dictionary_generic.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/dictionary_get.py` & `apysc-4.3.2/apysc/_translation/jp/dictionary_get.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/dictionary_length.py` & `apysc-4.3.2/apysc/_translation/jp/dictionary_length.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/display_object.py` & `apysc-4.3.2/apysc/_translation/jp/display_object.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/display_object_and_graphics_base_prop_abstract.py` & `apysc-4.3.2/apysc/_translation/jp/display_object_and_graphics_base_prop_abstract.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/display_object_get_and_set_css.py` & `apysc-4.3.2/apysc/_translation/jp/display_object_get_and_set_css.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/display_object_mouse_event.py` & `apysc-4.3.2/apysc/_translation/jp/display_object_mouse_event.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/display_object_parent.py` & `apysc-4.3.2/apysc/_translation/jp/display_object_parent.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/display_object_visible.py` & `apysc-4.3.2/apysc/_translation/jp/display_object_visible.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/display_object_x_and_y.py` & `apysc-4.3.2/apysc/_translation/jp/display_object_x_and_y.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/display_on_colaboratory.py` & `apysc-4.3.2/apysc/_translation/jp/display_on_colaboratory.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/display_on_jupyter.py` & `apysc-4.3.2/apysc/_translation/jp/display_on_jupyter.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/draw_interfaces_abstract.py` & `apysc-4.3.2/apysc/_translation/jp/draw_interfaces_abstract.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/easing_enum.py` & `apysc-4.3.2/apysc/_translation/jp/easing_enum.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/elif.py` & `apysc-4.3.2/apysc/_translation/jp/elif.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/ellipse.py` & `apysc-4.3.2/apysc/_translation/jp/ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/else.py` & `apysc-4.3.2/apysc/_translation/jp/else.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/enter_frame.py` & `apysc-4.3.2/apysc/_translation/jp/enter_frame.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/event_prevent_default_and_stop_propagation.py` & `apysc-4.3.2/apysc/_translation/jp/event_prevent_default_and_stop_propagation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/for_array_indices.py` & `apysc-4.3.2/apysc/_translation/jp/for_array_indices.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/for_array_indices_and_values.py` & `apysc-4.3.2/apysc/_translation/jp/for_array_indices_and_values.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/for_array_values.py` & `apysc-4.3.2/apysc/_translation/jp/for_array_values.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/for_dict_keys.py` & `apysc-4.3.2/apysc/_translation/jp/for_dict_keys.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/for_dict_keys_and_values.py` & `apysc-4.3.2/apysc/_translation/jp/for_dict_keys_and_values.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/for_dict_values.py` & `apysc-4.3.2/apysc/_translation/jp/for_dict_values.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/fps.py` & `apysc-4.3.2/apysc/_translation/jp/fps.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/fundamental_data_classes_value_interface.py` & `apysc-4.3.2/apysc/_translation/jp/fundamental_data_classes_value_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/get_bounds.py` & `apysc-4.3.2/apysc/_translation/jp/get_bounds.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/get_child_at.py` & `apysc-4.3.2/apysc/_translation/jp/get_child_at.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/graphics.py` & `apysc-4.3.2/apysc/_translation/jp/graphics.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/graphics_base_fill_alpha.py` & `apysc-4.3.2/apysc/_translation/jp/graphics_base_fill_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/graphics_base_fill_color.py` & `apysc-4.3.2/apysc/_translation/jp/graphics_base_fill_color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/graphics_base_flip_interfaces.py` & `apysc-4.3.2/apysc/_translation/jp/graphics_base_flip_interfaces.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/graphics_base_line_alpha.py` & `apysc-4.3.2/apysc/_translation/jp/graphics_base_line_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/graphics_base_line_color.py` & `apysc-4.3.2/apysc/_translation/jp/graphics_base_line_color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/graphics_base_line_dash_dot_setting.py` & `apysc-4.3.2/apysc/_translation/jp/graphics_base_line_dash_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/graphics_base_line_dash_setting.py` & `apysc-4.3.2/apysc/_translation/jp/graphics_base_line_dash_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/graphics_base_line_dot_setting.py` & `apysc-4.3.2/apysc/_translation/jp/graphics_base_line_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/graphics_base_line_round_dot_setting.py` & `apysc-4.3.2/apysc/_translation/jp/graphics_base_line_round_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/graphics_base_line_thickness.py` & `apysc-4.3.2/apysc/_translation/jp/graphics_base_line_thickness.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/graphics_base_rotation_around_center.py` & `apysc-4.3.2/apysc/_translation/jp/graphics_base_rotation_around_center.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/graphics_base_rotation_around_point.py` & `apysc-4.3.2/apysc/_translation/jp/graphics_base_rotation_around_point.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/graphics_base_scale_from_center.py` & `apysc-4.3.2/apysc/_translation/jp/graphics_base_scale_from_center.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/graphics_base_scale_from_point.py` & `apysc-4.3.2/apysc/_translation/jp/graphics_base_scale_from_point.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/graphics_base_skew.py` & `apysc-4.3.2/apysc/_translation/jp/graphics_base_skew.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/graphics_begin_fill.py` & `apysc-4.3.2/apysc/_translation/jp/graphics_begin_fill.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/graphics_clear.py` & `apysc-4.3.2/apysc/_translation/jp/graphics_clear.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/graphics_draw_circle.py` & `apysc-4.3.2/apysc/_translation/jp/graphics_draw_circle.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/graphics_draw_dash_dotted_line.py` & `apysc-4.3.2/apysc/_translation/jp/graphics_draw_dash_dotted_line.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/graphics_draw_dashed_line.py` & `apysc-4.3.2/apysc/_translation/jp/graphics_draw_dashed_line.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/graphics_draw_dotted_line.py` & `apysc-4.3.2/apysc/_translation/jp/graphics_draw_dotted_line.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/graphics_draw_ellipse.py` & `apysc-4.3.2/apysc/_translation/jp/graphics_draw_ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/graphics_draw_line.py` & `apysc-4.3.2/apysc/_translation/jp/graphics_draw_line.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/graphics_draw_path.py` & `apysc-4.3.2/apysc/_translation/jp/graphics_draw_path.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/graphics_draw_polygon.py` & `apysc-4.3.2/apysc/_translation/jp/graphics_draw_polygon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/graphics_draw_rect.py` & `apysc-4.3.2/apysc/_translation/jp/graphics_draw_rect.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/graphics_draw_round_dotted_line.py` & `apysc-4.3.2/apysc/_translation/jp/graphics_draw_round_dotted_line.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/graphics_draw_round_rect.py` & `apysc-4.3.2/apysc/_translation/jp/graphics_draw_round_rect.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/graphics_draw_triangle.py` & `apysc-4.3.2/apysc/_translation/jp/graphics_draw_triangle.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/graphics_line_style.py` & `apysc-4.3.2/apysc/_translation/jp/graphics_line_style.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/graphics_move_to_and_line_to.py` & `apysc-4.3.2/apysc/_translation/jp/graphics_move_to_and_line_to.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/green_color.py` & `apysc-4.3.2/apysc/_translation/jp/green_color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/if.py` & `apysc-4.3.2/apysc/_translation/jp/if.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/import_conventions.py` & `apysc-4.3.2/apysc/_translation/jp/import_conventions.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/index.py` & `apysc-4.3.2/apysc/_translation/jp/index.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/int_and_number.py` & `apysc-4.3.2/apysc/_translation/jp/int_and_number.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/int_and_number_arithmetic_operations.py` & `apysc-4.3.2/apysc/_translation/jp/int_and_number_arithmetic_operations.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/int_and_number_comparison_operations.py` & `apysc-4.3.2/apysc/_translation/jp/int_and_number_comparison_operations.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/int_and_number_to_fixed.py` & `apysc-4.3.2/apysc/_translation/jp/int_and_number_to_fixed.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/int_and_number_to_hex.py` & `apysc-4.3.2/apysc/_translation/jp/int_and_number_to_hex.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/line.py` & `apysc-4.3.2/apysc/_translation/jp/line.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/material_design_colors.py` & `apysc-4.3.2/apysc/_translation/jp/material_design_colors.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/math_max.py` & `apysc-4.3.2/apysc/_translation/jp/math_max.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/math_min.py` & `apysc-4.3.2/apysc/_translation/jp/math_min.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/math_trunc.py` & `apysc-4.3.2/apysc/_translation/jp/math_trunc.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/mouse_event_abstract.py` & `apysc-4.3.2/apysc/_translation/jp/mouse_event_abstract.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/mouse_event_basic.py` & `apysc-4.3.2/apysc/_translation/jp/mouse_event_basic.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/mousedown_and_mouseup.py` & `apysc-4.3.2/apysc/_translation/jp/mousedown_and_mouseup.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/mousemove.py` & `apysc-4.3.2/apysc/_translation/jp/mousemove.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/mouseover_and_mouseout.py` & `apysc-4.3.2/apysc/_translation/jp/mouseover_and_mouseout.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/multi_line_text.py` & `apysc-4.3.2/apysc/_translation/jp/multi_line_text.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/num_children.py` & `apysc-4.3.2/apysc/_translation/jp/num_children.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/path.py` & `apysc-4.3.2/apysc/_translation/jp/path.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/path_bezier_2d.py` & `apysc-4.3.2/apysc/_translation/jp/path_bezier_2d.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/path_bezier_2d_continual.py` & `apysc-4.3.2/apysc/_translation/jp/path_bezier_2d_continual.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/path_bezier_3d.py` & `apysc-4.3.2/apysc/_translation/jp/path_bezier_3d.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/path_bezier_3d_continual.py` & `apysc-4.3.2/apysc/_translation/jp/path_bezier_3d_continual.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/path_close.py` & `apysc-4.3.2/apysc/_translation/jp/path_close.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/path_horizontal.py` & `apysc-4.3.2/apysc/_translation/jp/path_horizontal.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/path_line_to.py` & `apysc-4.3.2/apysc/_translation/jp/path_line_to.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/path_move_to.py` & `apysc-4.3.2/apysc/_translation/jp/path_move_to.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/path_vertical.py` & `apysc-4.3.2/apysc/_translation/jp/path_vertical.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/point2d.py` & `apysc-4.3.2/apysc/_translation/jp/point2d.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/polygon.py` & `apysc-4.3.2/apysc/_translation/jp/polygon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/polyline.py` & `apysc-4.3.2/apysc/_translation/jp/polyline.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/quick_start.py` & `apysc-4.3.2/apysc/_translation/jp/quick_start.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/range.py` & `apysc-4.3.2/apysc/_translation/jp/range.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/recommended_type_checker_settings.py` & `apysc-4.3.2/apysc/_translation/jp/recommended_type_checker_settings.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/rectangle.py` & `apysc-4.3.2/apysc/_translation/jp/rectangle.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/rectangle_geom.py` & `apysc-4.3.2/apysc/_translation/jp/rectangle_geom.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/red_color.py` & `apysc-4.3.2/apysc/_translation/jp/red_color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/remove_children.py` & `apysc-4.3.2/apysc/_translation/jp/remove_children.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/return.py` & `apysc-4.3.2/apysc/_translation/jp/return.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/save_overall_html.py` & `apysc-4.3.2/apysc/_translation/jp/save_overall_html.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/sequential_animation.py` & `apysc-4.3.2/apysc/_translation/jp/sequential_animation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/set_debug_mode.py` & `apysc-4.3.2/apysc/_translation/jp/set_debug_mode.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/sprite.py` & `apysc-4.3.2/apysc/_translation/jp/sprite.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/stage.py` & `apysc-4.3.2/apysc/_translation/jp/stage.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/string.py` & `apysc-4.3.2/apysc/_translation/jp/string.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/string_addition_and_multiplication.py` & `apysc-4.3.2/apysc/_translation/jp/string_addition_and_multiplication.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/string_apply_max_num_of_decimal_places.py` & `apysc-4.3.2/apysc/_translation/jp/string_apply_max_num_of_decimal_places.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/string_comparison_operations.py` & `apysc-4.3.2/apysc/_translation/jp/string_comparison_operations.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/string_length.py` & `apysc-4.3.2/apysc/_translation/jp/string_length.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/string_lower.py` & `apysc-4.3.2/apysc/_translation/jp/string_lower.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/string_lstrip.py` & `apysc-4.3.2/apysc/_translation/jp/string_lstrip.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/string_rstrip.py` & `apysc-4.3.2/apysc/_translation/jp/string_rstrip.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/string_slice.py` & `apysc-4.3.2/apysc/_translation/jp/string_slice.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/string_split.py` & `apysc-4.3.2/apysc/_translation/jp/string_split.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/string_strip.py` & `apysc-4.3.2/apysc/_translation/jp/string_strip.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/string_upper.py` & `apysc-4.3.2/apysc/_translation/jp/string_upper.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/string_zfill.py` & `apysc-4.3.2/apysc/_translation/jp/string_zfill.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/svg_text.py` & `apysc-4.3.2/apysc/_translation/jp/svg_text.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,169 +17,169 @@
     ##################################################
     "The `SvgText` class creates an SVG text object.": "`SvgText`クラスはSVGテキストのオブジェクトを生成します。",  # noqa
     ##################################################
     "## Basic usage": "## 基本的な使い方",
     ##################################################
     "The `SvgText` class constructor requires the `text` argument.": "`SvgText`クラスのコンストラクタは`text`引数の指定を必要とします。",  # noqa
     ##################################################
-    "The constructor also accepts each font\'s and style\'s argument, such as the `font_size`, `font_family`, `fill_color`, and `bold`.": "コンストラクタでは`font_size`や`font_family`、`fill_color`、`bold`などのフォントやスタイルなどの引数を指定することもできます。",  # noqa
+    "The constructor also accepts each font's and style's argument, such as the `font_size`, `font_family`, `fill_color`, and `bold`.": "コンストラクタでは`font_size`や`font_family`、`fill_color`、`bold`などのフォントやスタイルなどの引数を指定することもできます。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\nap.save_overall_html(dest_dir_path=\"svg_text_basic_usage/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\nap.save_overall_html(dest_dir_path=\"svg_text_basic_usage/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\nap.save_overall_html(dest_dir_path="svg_text_basic_usage/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\nap.save_overall_html(dest_dir_path="svg_text_basic_usage/")\n```',  # noqa
     ##################################################
-    "## Note on the baseline of a text\'s y-coordinate": "## テキストのY座標の基準点に対する特記事項",
+    "## Note on the baseline of a text's y-coordinate": "## テキストのY座標の基準点に対する特記事項",
     ##################################################
-    "The baseline of a text\'s y-coordinate is the text\'s bottom position (this is the specification of the SVG text).": "テキストのY座標の基準点はテキストの下部付近の位置となります（これはSVGテキストの仕様となります）。",  # noqa
+    "The baseline of a text's y-coordinate is the text's bottom position (this is the specification of the SVG text).": "テキストのY座標の基準点はテキストの下部付近の位置となります（これはSVGテキストの仕様となります）。",  # noqa
     ##################################################
-    "So if you specify `y=0` as the coordinate, you can see almost nothing of a text\'s content (barely see the bottom of the comma in the following example).": "そのためもしもY座標に`y=0`を指定した場合、テキストのコンテンツがほとんど見えなくなります（以下の例では辛うじてコンマの一部が確認できます）。",  # noqa
+    "So if you specify `y=0` as the coordinate, you can see almost nothing of a text's content (barely see the bottom of the comma in the following example).": "そのためもしもY座標に`y=0`を指定した場合、テキストのコンテンツがほとんど見えなくなります（以下の例では辛うじてコンマの一部が確認できます）。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    x=20,\n    y=0,\n    fill_color=ap.Color(\"#aaa\"),\n)\nap.save_overall_html(dest_dir_path=\"svg_text_note_on_the_y_baseline/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    x=20,\n    y=0,\n    fill_color=ap.Color(\"#aaa\"),\n)\nap.save_overall_html(dest_dir_path=\"svg_text_note_on_the_y_baseline/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    x=20,\n    y=0,\n    fill_color=ap.Color("#aaa"),\n)\nap.save_overall_html(dest_dir_path="svg_text_note_on_the_y_baseline/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    x=20,\n    y=0,\n    fill_color=ap.Color("#aaa"),\n)\nap.save_overall_html(dest_dir_path="svg_text_note_on_the_y_baseline/")\n```',  # noqa
     ##################################################
     "## text property interface example": "## text 属性のインターフェイス例",
     ##################################################
-    "The `text` property updates or gets the instance\'s text.": "`text`属性ではインスタンスのテキストの更新もしくは取得を行えます。",  # noqa
+    "The `text` property updates or gets the instance's text.": "`text`属性ではインスタンスのテキストの更新もしくは取得を行えます。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\nsvg_text.text = ap.String(\"Lorem ipsum\")\nap.save_overall_html(dest_dir_path=\"svg_text_text/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\nsvg_text.text = ap.String(\"Lorem ipsum\")\nap.save_overall_html(dest_dir_path=\"svg_text_text/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\nsvg_text.text = ap.String("Lorem ipsum")\nap.save_overall_html(dest_dir_path="svg_text_text/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\nsvg_text.text = ap.String("Lorem ipsum")\nap.save_overall_html(dest_dir_path="svg_text_text/")\n```',  # noqa
     ##################################################
     "## font_size property interface example": "## font_size 属性のインターフェイス例",
     ##################################################
-    "The `font_size` property updates or gets the instance\'s font size.": "`font_size`属性ではインスタンスのフォントサイズの更新もしくは取得を行えます。",  # noqa
+    "The `font_size` property updates or gets the instance's font size.": "`font_size`属性ではインスタンスのフォントサイズの更新もしくは取得を行えます。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    x=20,\n    y=34,\n    fill_color=ap.Color(\"#aaa\"),\n)\nsvg_text.font_size = ap.Int(24)\nap.save_overall_html(dest_dir_path=\"svg_text_font_size/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    x=20,\n    y=34,\n    fill_color=ap.Color(\"#aaa\"),\n)\nsvg_text.font_size = ap.Int(24)\nap.save_overall_html(dest_dir_path=\"svg_text_font_size/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    x=20,\n    y=34,\n    fill_color=ap.Color("#aaa"),\n)\nsvg_text.font_size = ap.Int(24)\nap.save_overall_html(dest_dir_path="svg_text_font_size/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    x=20,\n    y=34,\n    fill_color=ap.Color("#aaa"),\n)\nsvg_text.font_size = ap.Int(24)\nap.save_overall_html(dest_dir_path="svg_text_font_size/")\n```',  # noqa
     ##################################################
     "## font_family property interface example": "## font_family 属性のインターフェイス例",
     ##################################################
-    "The `font_family` property updates or gets the instance\'s font family.": "`font_family`属性ではインスタンスのフォントファミリー（フォントの指定）の更新もしくは取得を行えます。",  # noqa
+    "The `font_family` property updates or gets the instance's font family.": "`font_family`属性ではインスタンスのフォントファミリー（フォントの指定）の更新もしくは取得を行えます。",  # noqa
     ##################################################
     "This property requires an `Array` of each font name `String`.": "この属性は各フォント名の`String`型の文字列を格納した`Array`型の配列を必要とします。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\nsvg_text.font_family = ap.Array([ap.String(\"Impact\"), ap.String(\"Times New Roman\")])\nap.save_overall_html(dest_dir_path=\"svg_text_font_family/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\nsvg_text.font_family = ap.Array([ap.String(\"Impact\"), ap.String(\"Times New Roman\")])\nap.save_overall_html(dest_dir_path=\"svg_text_font_family/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\nsvg_text.font_family = ap.Array([ap.String("Impact"), ap.String("Times New Roman")])\nap.save_overall_html(dest_dir_path="svg_text_font_family/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\nsvg_text.font_family = ap.Array([ap.String("Impact"), ap.String("Times New Roman")])\nap.save_overall_html(dest_dir_path="svg_text_font_family/")\n```',  # noqa
     ##################################################
     "## x property interface example": "## x属性のインターフェイス例",
     ##################################################
-    "The `x` property updates or gets the instance\'s x-coordinate:": "`x`属性ではX座標の値の更新もしくは取得を行えます:",  # noqa
+    "The `x` property updates or gets the instance's x-coordinate:": "`x`属性ではX座標の値の更新もしくは取得を行えます:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\nsvg_text.x = ap.Number(50)\nap.save_overall_html(dest_dir_path=\"svg_text_x/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\nsvg_text.x = ap.Number(50)\nap.save_overall_html(dest_dir_path=\"svg_text_x/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\nsvg_text.x = ap.Number(50)\nap.save_overall_html(dest_dir_path="svg_text_x/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\nsvg_text.x = ap.Number(50)\nap.save_overall_html(dest_dir_path="svg_text_x/")\n```',  # noqa
     ##################################################
     "## y property interface example": "## y属性のインターフェイス例",
     ##################################################
-    "The `y` property updates or gets the instance\'s y-coordinate:": "`y`属性ではY座標の値の更新もしくは取得を行えます:",  # noqa
+    "The `y` property updates or gets the instance's y-coordinate:": "`y`属性ではY座標の値の更新もしくは取得を行えます:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=70,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\nsvg_text.y = ap.Number(45)\nap.save_overall_html(dest_dir_path=\"svg_text_y/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=70,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\nsvg_text.y = ap.Number(45)\nap.save_overall_html(dest_dir_path=\"svg_text_y/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=70,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\nsvg_text.y = ap.Number(45)\nap.save_overall_html(dest_dir_path="svg_text_y/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=70,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\nsvg_text.y = ap.Number(45)\nap.save_overall_html(dest_dir_path="svg_text_y/")\n```',  # noqa
     ##################################################
     "## fill_color property interface example": "## fill_color属性のインターフェイス例",
     ##################################################
-    "The `fill_color` property updates or gets the instance\'s fill color:": "`fill_color`属性は塗りの色の値の更新もしくは取得を行えます:",  # noqa
+    "The `fill_color` property updates or gets the instance's fill color:": "`fill_color`属性は塗りの色の値の更新もしくは取得を行えます:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n)\nsvg_text.fill_color = ap.Color(\"#0af\")\nap.save_overall_html(dest_dir_path=\"svg_text_fill_color/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n)\nsvg_text.fill_color = ap.Color(\"#0af\")\nap.save_overall_html(dest_dir_path=\"svg_text_fill_color/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n)\nsvg_text.fill_color = ap.Color("#0af")\nap.save_overall_html(dest_dir_path="svg_text_fill_color/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n)\nsvg_text.fill_color = ap.Color("#0af")\nap.save_overall_html(dest_dir_path="svg_text_fill_color/")\n```',  # noqa
     ##################################################
     "## fill_alpha property interface example": "## fill_alpha属性のインターフェイス例",
     ##################################################
-    "The `fill_alpha` property updates or gets the instance\'s fill alpha (opacity):": "`fill_alpha`属性は塗りの透明度の値の更新もしくは取得を行えます:",  # noqa
+    "The `fill_alpha` property updates or gets the instance's fill alpha (opacity):": "`fill_alpha`属性は塗りの透明度の値の更新もしくは取得を行えます:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\nsvg_text.fill_alpha = ap.Number(0.3)\nap.save_overall_html(dest_dir_path=\"svg_text_fill_alpha/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\nsvg_text.fill_alpha = ap.Number(0.3)\nap.save_overall_html(dest_dir_path=\"svg_text_fill_alpha/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\nsvg_text.fill_alpha = ap.Number(0.3)\nap.save_overall_html(dest_dir_path="svg_text_fill_alpha/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\nsvg_text.fill_alpha = ap.Number(0.3)\nap.save_overall_html(dest_dir_path="svg_text_fill_alpha/")\n```',  # noqa
     ##################################################
     "## line_color property interface example": "## line_color属性のインターフェイス例",
     ##################################################
-    "The `line_color` property updates or gets the instance\'s line color:": "`line_color`属性では線の色の値の更新もしくは取得を行えます:",  # noqa
+    "The `line_color` property updates or gets the instance's line color:": "`line_color`属性では線の色の値の更新もしくは取得を行えます:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    x=20,\n    y=34,\n    font_size=24,\n    bold=True,\n    fill_color=ap.COLORLESS,\n    line_thickness=1,\n)\nsvg_text.line_color = ap.Color(\"#0af\")\nap.save_overall_html(dest_dir_path=\"svg_text_line_color/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    x=20,\n    y=34,\n    font_size=24,\n    bold=True,\n    fill_color=ap.COLORLESS,\n    line_thickness=1,\n)\nsvg_text.line_color = ap.Color(\"#0af\")\nap.save_overall_html(dest_dir_path=\"svg_text_line_color/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    x=20,\n    y=34,\n    font_size=24,\n    bold=True,\n    fill_color=ap.COLORLESS,\n    line_thickness=1,\n)\nsvg_text.line_color = ap.Color("#0af")\nap.save_overall_html(dest_dir_path="svg_text_line_color/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    x=20,\n    y=34,\n    font_size=24,\n    bold=True,\n    fill_color=ap.COLORLESS,\n    line_thickness=1,\n)\nsvg_text.line_color = ap.Color("#0af")\nap.save_overall_html(dest_dir_path="svg_text_line_color/")\n```',  # noqa
     ##################################################
     "## line_alpha property interface example": "## line_alpha属性のインターフェイス例",
     ##################################################
-    "The `line_alpha` property updates or gets the instance\'s line alpha (opacity):": "`line_alpha`属性では線の透明度の値の更新もしくは取得を行えます:",  # noqa
+    "The `line_alpha` property updates or gets the instance's line alpha (opacity):": "`line_alpha`属性では線の透明度の値の更新もしくは取得を行えます:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    x=20,\n    y=34,\n    font_size=24,\n    bold=True,\n    fill_color=ap.COLORLESS,\n    line_color=ap.Color(\"#0af\"),\n    line_thickness=1,\n)\nsvg_text.line_alpha = ap.Number(0.3)\nap.save_overall_html(dest_dir_path=\"svg_text_line_alpha/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    x=20,\n    y=34,\n    font_size=24,\n    bold=True,\n    fill_color=ap.COLORLESS,\n    line_color=ap.Color(\"#0af\"),\n    line_thickness=1,\n)\nsvg_text.line_alpha = ap.Number(0.3)\nap.save_overall_html(dest_dir_path=\"svg_text_line_alpha/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    x=20,\n    y=34,\n    font_size=24,\n    bold=True,\n    fill_color=ap.COLORLESS,\n    line_color=ap.Color("#0af"),\n    line_thickness=1,\n)\nsvg_text.line_alpha = ap.Number(0.3)\nap.save_overall_html(dest_dir_path="svg_text_line_alpha/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    x=20,\n    y=34,\n    font_size=24,\n    bold=True,\n    fill_color=ap.COLORLESS,\n    line_color=ap.Color("#0af"),\n    line_thickness=1,\n)\nsvg_text.line_alpha = ap.Number(0.3)\nap.save_overall_html(dest_dir_path="svg_text_line_alpha/")\n```',  # noqa
     ##################################################
     "## line_thickness property interface example": "## line_thickness属性のインターフェイス例",
     ##################################################
-    "The `line_thickness` property updates or gets the instance\'s line thickness (line width):": "`line_thickness`属性では線の幅の更新もしくは取得を行えます:",  # noqa
+    "The `line_thickness` property updates or gets the instance's line thickness (line width):": "`line_thickness`属性では線の幅の更新もしくは取得を行えます:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    x=20,\n    y=34,\n    font_size=24,\n    bold=True,\n    fill_color=ap.COLORLESS,\n    line_color=ap.Color(\"#0af\"),\n)\nsvg_text.line_thickness = ap.Int(3)\nap.save_overall_html(dest_dir_path=\"svg_text_line_thickness/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    x=20,\n    y=34,\n    font_size=24,\n    bold=True,\n    fill_color=ap.COLORLESS,\n    line_color=ap.Color(\"#0af\"),\n)\nsvg_text.line_thickness = ap.Int(3)\nap.save_overall_html(dest_dir_path=\"svg_text_line_thickness/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    x=20,\n    y=34,\n    font_size=24,\n    bold=True,\n    fill_color=ap.COLORLESS,\n    line_color=ap.Color("#0af"),\n)\nsvg_text.line_thickness = ap.Int(3)\nap.save_overall_html(dest_dir_path="svg_text_line_thickness/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    x=20,\n    y=34,\n    font_size=24,\n    bold=True,\n    fill_color=ap.COLORLESS,\n    line_color=ap.Color("#0af"),\n)\nsvg_text.line_thickness = ap.Int(3)\nap.save_overall_html(dest_dir_path="svg_text_line_thickness/")\n```',  # noqa
     ##################################################
     "## leading property interface example": "## leading 属性のインターフェイス例",
     ##################################################
-    "The `leading` property updates or gets the instance\'s text leading (line height).": "`leading`属性ではインスタンスの行間の更新もしくは取得を行えます。",  # noqa
+    "The `leading` property updates or gets the instance's text leading (line height).": "`leading`属性ではインスタンスの行間の更新もしくは取得を行えます。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=500,\n    stage_height=120,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Lorem ipsum dolor sit amet,\nconsectetur adipiscing elit,\n\"\n    \"sed do eiusmod tempor incididunt\",\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\nsvg_text.leading = ap.Number(2.0)\n\nap.save_overall_html(dest_dir_path=\"svg_text_leading/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=500,\n    stage_height=120,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Lorem ipsum dolor sit amet,\nconsectetur adipiscing elit,\n\"\n    \"sed do eiusmod tempor incididunt\",\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\nsvg_text.leading = ap.Number(2.0)\n\nap.save_overall_html(dest_dir_path=\"svg_text_leading/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=500,\n    stage_height=120,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Lorem ipsum dolor sit amet,\nconsectetur adipiscing elit,\n"\n    "sed do eiusmod tempor incididunt",\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\nsvg_text.leading = ap.Number(2.0)\n\nap.save_overall_html(dest_dir_path="svg_text_leading/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=500,\n    stage_height=120,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Lorem ipsum dolor sit amet,\nconsectetur adipiscing elit,\n"\n    "sed do eiusmod tempor incididunt",\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\nsvg_text.leading = ap.Number(2.0)\n\nap.save_overall_html(dest_dir_path="svg_text_leading/")\n```',  # noqa
     ##################################################
     "## align property interface example": "## align 属性のインターフェイス例",
     ##################################################
-    "The `align` property updates or gets the instance\'s horizontal text alignment (left, center, or right).": "`align`属性ではインスタンスの水平方向の行揃えの設定（左端、中央、右端）の更新もしくは取得を行えます。",  # noqa
+    "The `align` property updates or gets the instance's horizontal text alignment (left, center, or right).": "`align`属性ではインスタンスの水平方向の行揃えの設定（左端、中央、右端）の更新もしくは取得を行えます。",  # noqa
     ##################################################
     "This property requires the `SvgTextAlign` enum.": "この属性は`SvgTextAlign`のenumの値を必要とします。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=500,\n    stage_height=100,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Lorem ipsum dolor sit amet,\nconsectetur adipiscing elit,\n\"\n    \"sed do eiusmod tempor incididunt\",\n    x=250,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\nsvg_text.align = ap.SvgTextAlign.CENTER\n\nap.save_overall_html(dest_dir_path=\"svg_text_align/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=500,\n    stage_height=100,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Lorem ipsum dolor sit amet,\nconsectetur adipiscing elit,\n\"\n    \"sed do eiusmod tempor incididunt\",\n    x=250,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\nsvg_text.align = ap.SvgTextAlign.CENTER\n\nap.save_overall_html(dest_dir_path=\"svg_text_align/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=500,\n    stage_height=100,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Lorem ipsum dolor sit amet,\nconsectetur adipiscing elit,\n"\n    "sed do eiusmod tempor incididunt",\n    x=250,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\nsvg_text.align = ap.SvgTextAlign.CENTER\n\nap.save_overall_html(dest_dir_path="svg_text_align/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=500,\n    stage_height=100,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Lorem ipsum dolor sit amet,\nconsectetur adipiscing elit,\n"\n    "sed do eiusmod tempor incididunt",\n    x=250,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\nsvg_text.align = ap.SvgTextAlign.CENTER\n\nap.save_overall_html(dest_dir_path="svg_text_align/")\n```',  # noqa
     ##################################################
     "Note: This property setting changes x coordinate baseline (position of `x=0`), as follows:": "特記事項: この属性はX座標の基準位置（`x=0`の位置）を以下のように変更します:",  # noqa
     ##################################################
-    "- SvgTextAlign.CENTER: X coordinate baseline becomes the text\'s center position.": "- SvgTextAlign.CENTER: X座標の基準位置はテキストの中央位置になります。",  # noqa
+    "- SvgTextAlign.CENTER: X coordinate baseline becomes the text's center position.": "- SvgTextAlign.CENTER: X座標の基準位置はテキストの中央位置になります。",  # noqa
     ##################################################
-    "- SvgTextAlign.RIGHT: X coordinate baseline becomes the text\'s right position.": "- SvgTextAlign.RIGHT: X座標の基準位置はテキストの右端の位置になります。",  # noqa
+    "- SvgTextAlign.RIGHT: X coordinate baseline becomes the text's right position.": "- SvgTextAlign.RIGHT: X座標の基準位置はテキストの右端の位置になります。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nSTAGE_WIDTH: int = 500\nSTAGE_HEIGHT: int = 120\nap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=STAGE_WIDTH,\n    stage_height=STAGE_HEIGHT,\n    stage_elem_id=\"stage\",\n)\ncontainer_sprite: ap.Sprite = ap.Sprite()\ncontainer_sprite.x = ap.Number(STAGE_WIDTH / 2)\n\nvertical_x0_line: ap.Line = ap.Line(\n    start_point=ap.Point2D(0, 0),\n    end_point=ap.Point2D(0, STAGE_HEIGHT),\n    line_color=ap.Color(\"#666\"),\n    parent=container_sprite,\n)\nx0_text: ap.SvgText = ap.SvgText(\n    text=\"Text\'s x=0 position\",\n    fill_color=ap.Color(\"#666\"),\n    x=5,\n    y=20,\n    parent=container_sprite,\n)\n\nleft_align_sample_text: ap.SvgText = ap.SvgText(\n    text=\"Left align sample (default)\",\n    x=0,\n    y=52,\n    fill_color=ap.Color(\"#aaa\"),\n    parent=container_sprite,\n)\n\ncenter_align_sample_text: ap.SvgText = ap.SvgText(\n    text=\"Center align sample\",\n    x=0,\n    y=72,\n    fill_color=ap.Color(\"#aaa\"),\n    parent=container_sprite,\n)\ncenter_align_sample_text.align = ap.SvgTextAlign.CENTER\n\nright_align_sample_text: ap.SvgText = ap.SvgText(\n    text=\"Right align sample\",\n    x=0,\n    y=92,\n    fill_color=ap.Color(\"#aaa\"),\n    parent=container_sprite,\n)\nright_align_sample_text.align = ap.SvgTextAlign.RIGHT\n\nap.save_overall_html(dest_dir_path=\"svg_text_align_note/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nSTAGE_WIDTH: int = 500\nSTAGE_HEIGHT: int = 120\nap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=STAGE_WIDTH,\n    stage_height=STAGE_HEIGHT,\n    stage_elem_id=\"stage\",\n)\ncontainer_sprite: ap.Sprite = ap.Sprite()\ncontainer_sprite.x = ap.Number(STAGE_WIDTH / 2)\n\nvertical_x0_line: ap.Line = ap.Line(\n    start_point=ap.Point2D(0, 0),\n    end_point=ap.Point2D(0, STAGE_HEIGHT),\n    line_color=ap.Color(\"#666\"),\n    parent=container_sprite,\n)\nx0_text: ap.SvgText = ap.SvgText(\n    text=\"Text\'s x=0 position\",\n    fill_color=ap.Color(\"#666\"),\n    x=5,\n    y=20,\n    parent=container_sprite,\n)\n\nleft_align_sample_text: ap.SvgText = ap.SvgText(\n    text=\"Left align sample (default)\",\n    x=0,\n    y=52,\n    fill_color=ap.Color(\"#aaa\"),\n    parent=container_sprite,\n)\n\ncenter_align_sample_text: ap.SvgText = ap.SvgText(\n    text=\"Center align sample\",\n    x=0,\n    y=72,\n    fill_color=ap.Color(\"#aaa\"),\n    parent=container_sprite,\n)\ncenter_align_sample_text.align = ap.SvgTextAlign.CENTER\n\nright_align_sample_text: ap.SvgText = ap.SvgText(\n    text=\"Right align sample\",\n    x=0,\n    y=92,\n    fill_color=ap.Color(\"#aaa\"),\n    parent=container_sprite,\n)\nright_align_sample_text.align = ap.SvgTextAlign.RIGHT\n\nap.save_overall_html(dest_dir_path=\"svg_text_align_note/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nSTAGE_WIDTH: int = 500\nSTAGE_HEIGHT: int = 120\nap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=STAGE_WIDTH,\n    stage_height=STAGE_HEIGHT,\n    stage_elem_id="stage",\n)\ncontainer_sprite: ap.Sprite = ap.Sprite()\ncontainer_sprite.x = ap.Number(STAGE_WIDTH / 2)\n\nvertical_x0_line: ap.Line = ap.Line(\n    start_point=ap.Point2D(0, 0),\n    end_point=ap.Point2D(0, STAGE_HEIGHT),\n    line_color=ap.Color("#666"),\n    parent=container_sprite,\n)\nx0_text: ap.SvgText = ap.SvgText(\n    text="Text\'s x=0 position",\n    fill_color=ap.Color("#666"),\n    x=5,\n    y=20,\n    parent=container_sprite,\n)\n\nleft_align_sample_text: ap.SvgText = ap.SvgText(\n    text="Left align sample (default)",\n    x=0,\n    y=52,\n    fill_color=ap.Color("#aaa"),\n    parent=container_sprite,\n)\n\ncenter_align_sample_text: ap.SvgText = ap.SvgText(\n    text="Center align sample",\n    x=0,\n    y=72,\n    fill_color=ap.Color("#aaa"),\n    parent=container_sprite,\n)\ncenter_align_sample_text.align = ap.SvgTextAlign.CENTER\n\nright_align_sample_text: ap.SvgText = ap.SvgText(\n    text="Right align sample",\n    x=0,\n    y=92,\n    fill_color=ap.Color("#aaa"),\n    parent=container_sprite,\n)\nright_align_sample_text.align = ap.SvgTextAlign.RIGHT\n\nap.save_overall_html(dest_dir_path="svg_text_align_note/")\n```': '```py\n# runnable\nimport apysc as ap\n\nSTAGE_WIDTH: int = 500\nSTAGE_HEIGHT: int = 120\nap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=STAGE_WIDTH,\n    stage_height=STAGE_HEIGHT,\n    stage_elem_id="stage",\n)\ncontainer_sprite: ap.Sprite = ap.Sprite()\ncontainer_sprite.x = ap.Number(STAGE_WIDTH / 2)\n\nvertical_x0_line: ap.Line = ap.Line(\n    start_point=ap.Point2D(0, 0),\n    end_point=ap.Point2D(0, STAGE_HEIGHT),\n    line_color=ap.Color("#666"),\n    parent=container_sprite,\n)\nx0_text: ap.SvgText = ap.SvgText(\n    text="Text\'s x=0 position",\n    fill_color=ap.Color("#666"),\n    x=5,\n    y=20,\n    parent=container_sprite,\n)\n\nleft_align_sample_text: ap.SvgText = ap.SvgText(\n    text="Left align sample (default)",\n    x=0,\n    y=52,\n    fill_color=ap.Color("#aaa"),\n    parent=container_sprite,\n)\n\ncenter_align_sample_text: ap.SvgText = ap.SvgText(\n    text="Center align sample",\n    x=0,\n    y=72,\n    fill_color=ap.Color("#aaa"),\n    parent=container_sprite,\n)\ncenter_align_sample_text.align = ap.SvgTextAlign.CENTER\n\nright_align_sample_text: ap.SvgText = ap.SvgText(\n    text="Right align sample",\n    x=0,\n    y=92,\n    fill_color=ap.Color("#aaa"),\n    parent=container_sprite,\n)\nright_align_sample_text.align = ap.SvgTextAlign.RIGHT\n\nap.save_overall_html(dest_dir_path="svg_text_align_note/")\n```',  # noqa
     ##################################################
     "## bold property interface example": "## bold 属性のインターフェイス例",
     ##################################################
-    "The `bold` property updates or gets the instance\'s `bold` text setting.": "`bold`属性ではインスタンスの太字設定の更新もしくは取得を行えます。",  # noqa
+    "The `bold` property updates or gets the instance's `bold` text setting.": "`bold`属性ではインスタンスの太字設定の更新もしくは取得を行えます。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Bold style sample\",\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\nsvg_text.bold = ap.Boolean(True)\nap.save_overall_html(dest_dir_path=\"svg_text_bold/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Bold style sample\",\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\nsvg_text.bold = ap.Boolean(True)\nap.save_overall_html(dest_dir_path=\"svg_text_bold/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Bold style sample",\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\nsvg_text.bold = ap.Boolean(True)\nap.save_overall_html(dest_dir_path="svg_text_bold/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Bold style sample",\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\nsvg_text.bold = ap.Boolean(True)\nap.save_overall_html(dest_dir_path="svg_text_bold/")\n```',  # noqa
     ##################################################
     "## italic property interface example": "## italic 属性のインターフェイス例",
     ##################################################
-    "The `italic` property updates or gets the instance\'s `italic` style setting.": "`italic`属性ではインスタンスの斜体の設定の更新もしくは取得を行えます。",  # noqa
+    "The `italic` property updates or gets the instance's `italic` style setting.": "`italic`属性ではインスタンスの斜体の設定の更新もしくは取得を行えます。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Italic style sample\",\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\nsvg_text.italic = ap.Boolean(True)\nap.save_overall_html(dest_dir_path=\"svg_text_italic/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Italic style sample\",\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\nsvg_text.italic = ap.Boolean(True)\nap.save_overall_html(dest_dir_path=\"svg_text_italic/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Italic style sample",\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\nsvg_text.italic = ap.Boolean(True)\nap.save_overall_html(dest_dir_path="svg_text_italic/")\n```': '```py\n# runnable\nimport apysc as ap\n\nap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Italic style sample",\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\nsvg_text.italic = ap.Boolean(True)\nap.save_overall_html(dest_dir_path="svg_text_italic/")\n```',  # noqa
     ##################################################
     "## rotation_around_center property interface example": "## rotation_around_center属性のインターフェイス例",  # noqa
     ##################################################
-    "The `rotation_around_center` property updates or gets the instance\'s rotation value (0 to 359) from the center point:": "`rotation_around_center`属性ではインスタンスの中央座標での回転量（0～359）の更新もしくは取得を行えます:",  # noqa
+    "The `rotation_around_center` property updates or gets the instance's rotation value (0 to 359) from the center point:": "`rotation_around_center`属性ではインスタンスの中央座標での回転量（0～359）の更新もしくは取得を行えます:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    x=100,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n    align=ap.SvgTextAlign.CENTER,\n)\n\n\ndef on_enter_frame(e: ap.EnterFrameEvent, optional: dict) -> None:\n    \"\"\"\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.EnterFrameEvent\n        Event instance.\n    optional : dict\n        Optional argument dictionary.\n    \"\"\"\n    svg_text.rotation_around_center += 1\n\n\nstage.enter_frame(handler=on_enter_frame)\nap.save_overall_html(dest_dir_path=\"svg_txt_rotation_around_center/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    x=100,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n    align=ap.SvgTextAlign.CENTER,\n)\n\n\ndef on_enter_frame(e: ap.EnterFrameEvent, optional: dict) -> None:\n    \"\"\"\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.EnterFrameEvent\n        Event instance.\n    optional : dict\n        Optional argument dictionary.\n    \"\"\"\n    svg_text.rotation_around_center += 1\n\n\nstage.enter_frame(handler=on_enter_frame)\nap.save_overall_html(dest_dir_path=\"svg_txt_rotation_around_center/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    x=100,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n    align=ap.SvgTextAlign.CENTER,\n)\n\n\ndef on_enter_frame(e: ap.EnterFrameEvent, optional: dict) -> None:\n    """\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.EnterFrameEvent\n        Event instance.\n    optional : dict\n        Optional argument dictionary.\n    """\n    svg_text.rotation_around_center += 1\n\n\nstage.enter_frame(handler=on_enter_frame)\nap.save_overall_html(dest_dir_path="svg_txt_rotation_around_center/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    x=100,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n    align=ap.SvgTextAlign.CENTER,\n)\n\n\ndef on_enter_frame(e: ap.EnterFrameEvent, optional: dict) -> None:\n    """\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.EnterFrameEvent\n        Event instance.\n    optional : dict\n        Optional argument dictionary.\n    """\n    svg_text.rotation_around_center += 1\n\n\nstage.enter_frame(handler=on_enter_frame)\nap.save_overall_html(dest_dir_path="svg_txt_rotation_around_center/")\n```',  # noqa
     ##################################################
     "## set_rotation_around_point and get_rotation_around_point methods interface example": "## set_rotation_around_pointとget_rotation_around_pointメソッドのインターフェイス例",  # noqa
     ##################################################
-    "The `set_rotation_around_point` method updates the instance\'s rotation value (0 to 359) from a specified point.": "`set_rotation_around_point`メソッドは指定された座標からのインスタンスの回転量（0～359）を更新します。",  # noqa
+    "The `set_rotation_around_point` method updates the instance's rotation value (0 to 359) from a specified point.": "`set_rotation_around_point`メソッドは指定された座標からのインスタンスの回転量（0～359）を更新します。",  # noqa
     ##################################################
-    "Similarly, the `get_rotation_around_point` method gets the instance\'s rotation value (0 to 359) from a specified point:": "同様に、`get_rotation_around_point`メソッドでは指定された座標のインスタンスの回転量（0～359）を取得します:",  # noqa
+    "Similarly, the `get_rotation_around_point` method gets the instance's rotation value (0 to 359) from a specified point:": "同様に、`get_rotation_around_point`メソッドでは指定された座標のインスタンスの回転量（0～359）を取得します:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=120,\n    stage_elem_id=\"stage\",\n)\nX: ap.Number = ap.Number(20)\nY: ap.Number = ap.Number(32)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    x=X,\n    y=Y,\n    fill_color=ap.Color(\"#aaa\"),\n)\n\n\ndef on_enter_frame(e: ap.EnterFrameEvent, optional: dict) -> None:\n    \"\"\"\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.EnterFrameEvent\n        Event instance.\n    optional : dict\n        Optional argument dictionary.\n    \"\"\"\n    rotation: ap.Int = (\n        svg_text.get_rotation_around_point(\n            x=X,\n            y=Y,\n        )\n        + 1\n    )\n    svg_text.set_rotation_around_point(\n        rotation=rotation,\n        x=X,\n        y=Y,\n    )\n\n\nstage.enter_frame(handler=on_enter_frame)\nap.save_overall_html(dest_dir_path=\"svg_txt_rotation_around_point/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=120,\n    stage_elem_id=\"stage\",\n)\nX: ap.Number = ap.Number(20)\nY: ap.Number = ap.Number(32)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    x=X,\n    y=Y,\n    fill_color=ap.Color(\"#aaa\"),\n)\n\n\ndef on_enter_frame(e: ap.EnterFrameEvent, optional: dict) -> None:\n    \"\"\"\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.EnterFrameEvent\n        Event instance.\n    optional : dict\n        Optional argument dictionary.\n    \"\"\"\n    rotation: ap.Int = (\n        svg_text.get_rotation_around_point(\n            x=X,\n            y=Y,\n        )\n        + 1\n    )\n    svg_text.set_rotation_around_point(\n        rotation=rotation,\n        x=X,\n        y=Y,\n    )\n\n\nstage.enter_frame(handler=on_enter_frame)\nap.save_overall_html(dest_dir_path=\"svg_txt_rotation_around_point/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=120,\n    stage_elem_id="stage",\n)\nX: ap.Number = ap.Number(20)\nY: ap.Number = ap.Number(32)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    x=X,\n    y=Y,\n    fill_color=ap.Color("#aaa"),\n)\n\n\ndef on_enter_frame(e: ap.EnterFrameEvent, optional: dict) -> None:\n    """\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.EnterFrameEvent\n        Event instance.\n    optional : dict\n        Optional argument dictionary.\n    """\n    rotation: ap.Int = (\n        svg_text.get_rotation_around_point(\n            x=X,\n            y=Y,\n        )\n        + 1\n    )\n    svg_text.set_rotation_around_point(\n        rotation=rotation,\n        x=X,\n        y=Y,\n    )\n\n\nstage.enter_frame(handler=on_enter_frame)\nap.save_overall_html(dest_dir_path="svg_txt_rotation_around_point/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=120,\n    stage_elem_id="stage",\n)\nX: ap.Number = ap.Number(20)\nY: ap.Number = ap.Number(32)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    x=X,\n    y=Y,\n    fill_color=ap.Color("#aaa"),\n)\n\n\ndef on_enter_frame(e: ap.EnterFrameEvent, optional: dict) -> None:\n    """\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.EnterFrameEvent\n        Event instance.\n    optional : dict\n        Optional argument dictionary.\n    """\n    rotation: ap.Int = (\n        svg_text.get_rotation_around_point(\n            x=X,\n            y=Y,\n        )\n        + 1\n    )\n    svg_text.set_rotation_around_point(\n        rotation=rotation,\n        x=X,\n        y=Y,\n    )\n\n\nstage.enter_frame(handler=on_enter_frame)\nap.save_overall_html(dest_dir_path="svg_txt_rotation_around_point/")\n```',  # noqa
     ##################################################
     "## Scale-related interfaces note": "## 拡縮関係のインターフェイスに対する特記事項",
     ##################################################
     "The scale-related interfaces are not recommended as the display may become distorted depending on the settings.": "拡縮関係のインターフェイスは設定次第では表示が崩れたりするため利用は非推奨です。",  # noqa
     ##################################################
     "## scale_x_from_center property interface example": "## scale_x_from_center属性のインターフェイス例",  # noqa
     ##################################################
-    "The `scale_x_from_center` property updates or gets the instance\'s scale-x from the center point:": "`scale_x_from_center`属性ではインスタンスの中央座標でのX軸の拡縮値の更新もしくは取得を行えます:",  # noqa
+    "The `scale_x_from_center` property updates or gets the instance's scale-x from the center point:": "`scale_x_from_center`属性ではインスタンスの中央座標でのX軸の拡縮値の更新もしくは取得を行えます:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\ndirection: ap.Int = ap.Int(-1)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\n\n\ndef on_enter_frame(e: ap.EnterFrameEvent, optional: dict) -> None:\n    \"\"\"\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.EnterFrameEvent\n        Event instance.\n    optional : dict\n        Optional argument dictionary.\n    \"\"\"\n    scale: ap.Number = svg_text.scale_x_from_center\n    with ap.If(scale > 1):\n        direction.value = -1\n    with ap.If(scale <= 0.3):\n        direction.value = 1\n    scale += direction * 0.005\n    svg_text.scale_x_from_center = scale\n\n\nstage.enter_frame(handler=on_enter_frame)\nap.save_overall_html(dest_dir_path=\"svg_txt_scale_x_from_center/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\ndirection: ap.Int = ap.Int(-1)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\n\n\ndef on_enter_frame(e: ap.EnterFrameEvent, optional: dict) -> None:\n    \"\"\"\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.EnterFrameEvent\n        Event instance.\n    optional : dict\n        Optional argument dictionary.\n    \"\"\"\n    scale: ap.Number = svg_text.scale_x_from_center\n    with ap.If(scale > 1):\n        direction.value = -1\n    with ap.If(scale <= 0.3):\n        direction.value = 1\n    scale += direction * 0.005\n    svg_text.scale_x_from_center = scale\n\n\nstage.enter_frame(handler=on_enter_frame)\nap.save_overall_html(dest_dir_path=\"svg_txt_scale_x_from_center/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\ndirection: ap.Int = ap.Int(-1)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\n\n\ndef on_enter_frame(e: ap.EnterFrameEvent, optional: dict) -> None:\n    """\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.EnterFrameEvent\n        Event instance.\n    optional : dict\n        Optional argument dictionary.\n    """\n    scale: ap.Number = svg_text.scale_x_from_center\n    with ap.If(scale > 1):\n        direction.value = -1\n    with ap.If(scale <= 0.3):\n        direction.value = 1\n    scale += direction * 0.005\n    svg_text.scale_x_from_center = scale\n\n\nstage.enter_frame(handler=on_enter_frame)\nap.save_overall_html(dest_dir_path="svg_txt_scale_x_from_center/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\ndirection: ap.Int = ap.Int(-1)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\n\n\ndef on_enter_frame(e: ap.EnterFrameEvent, optional: dict) -> None:\n    """\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.EnterFrameEvent\n        Event instance.\n    optional : dict\n        Optional argument dictionary.\n    """\n    scale: ap.Number = svg_text.scale_x_from_center\n    with ap.If(scale > 1):\n        direction.value = -1\n    with ap.If(scale <= 0.3):\n        direction.value = 1\n    scale += direction * 0.005\n    svg_text.scale_x_from_center = scale\n\n\nstage.enter_frame(handler=on_enter_frame)\nap.save_overall_html(dest_dir_path="svg_txt_scale_x_from_center/")\n```',  # noqa
     ##################################################
     "## set_scale_x_from_point and get_scale_x_from_point methods interface example": "## set_scale_x_from_pointとget_scale_x_from_pointメソッドのインターフェイス例",  # noqa
     ##################################################
-    "The `set_scale_x_from_point` method updates the instance\'s scale-x from a specified point.": "`set_scale_x_from_point`メソッドは指定されたX座標を基準としてX軸の拡縮値を更新します。",  # noqa
+    "The `set_scale_x_from_point` method updates the instance's scale-x from a specified point.": "`set_scale_x_from_point`メソッドは指定されたX座標を基準としてX軸の拡縮値を更新します。",  # noqa
     ##################################################
-    "Similarly, the `get_scale_x_from_point` method gets the instance\'s scale-x from a specified point:": "同様に、`get_scale_x_from_point`メソッドでは指定されたX座標を基準としたX軸の拡縮値を取得します:",  # noqa
+    "Similarly, the `get_scale_x_from_point` method gets the instance's scale-x from a specified point:": "同様に、`get_scale_x_from_point`メソッドでは指定されたX座標を基準としたX軸の拡縮値を取得します:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nX: ap.Number = ap.Number(20)\ndirection: ap.Int = ap.Int(-1)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    x=X,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\n\n\ndef on_enter_frame(e: ap.EnterFrameEvent, optional: dict) -> None:\n    \"\"\"\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.EnterFrameEvent\n        Event instance.\n    optional : dict\n        Optional argument dictionary.\n    \"\"\"\n    scale: ap.Number = svg_text.get_scale_x_from_point(x=X)\n    with ap.If(scale > 1):\n        direction.value = -1\n    with ap.If(scale <= 0.3):\n        direction.value = 1\n    scale += direction * 0.005\n    svg_text.set_scale_x_from_point(scale_x=scale, x=X)\n\n\nstage.enter_frame(handler=on_enter_frame)\nap.save_overall_html(dest_dir_path=\"svg_txt_scale_x_from_point/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nX: ap.Number = ap.Number(20)\ndirection: ap.Int = ap.Int(-1)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    x=X,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\n\n\ndef on_enter_frame(e: ap.EnterFrameEvent, optional: dict) -> None:\n    \"\"\"\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.EnterFrameEvent\n        Event instance.\n    optional : dict\n        Optional argument dictionary.\n    \"\"\"\n    scale: ap.Number = svg_text.get_scale_x_from_point(x=X)\n    with ap.If(scale > 1):\n        direction.value = -1\n    with ap.If(scale <= 0.3):\n        direction.value = 1\n    scale += direction * 0.005\n    svg_text.set_scale_x_from_point(scale_x=scale, x=X)\n\n\nstage.enter_frame(handler=on_enter_frame)\nap.save_overall_html(dest_dir_path=\"svg_txt_scale_x_from_point/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nX: ap.Number = ap.Number(20)\ndirection: ap.Int = ap.Int(-1)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    x=X,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\n\n\ndef on_enter_frame(e: ap.EnterFrameEvent, optional: dict) -> None:\n    """\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.EnterFrameEvent\n        Event instance.\n    optional : dict\n        Optional argument dictionary.\n    """\n    scale: ap.Number = svg_text.get_scale_x_from_point(x=X)\n    with ap.If(scale > 1):\n        direction.value = -1\n    with ap.If(scale <= 0.3):\n        direction.value = 1\n    scale += direction * 0.005\n    svg_text.set_scale_x_from_point(scale_x=scale, x=X)\n\n\nstage.enter_frame(handler=on_enter_frame)\nap.save_overall_html(dest_dir_path="svg_txt_scale_x_from_point/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nX: ap.Number = ap.Number(20)\ndirection: ap.Int = ap.Int(-1)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    x=X,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\n\n\ndef on_enter_frame(e: ap.EnterFrameEvent, optional: dict) -> None:\n    """\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.EnterFrameEvent\n        Event instance.\n    optional : dict\n        Optional argument dictionary.\n    """\n    scale: ap.Number = svg_text.get_scale_x_from_point(x=X)\n    with ap.If(scale > 1):\n        direction.value = -1\n    with ap.If(scale <= 0.3):\n        direction.value = 1\n    scale += direction * 0.005\n    svg_text.set_scale_x_from_point(scale_x=scale, x=X)\n\n\nstage.enter_frame(handler=on_enter_frame)\nap.save_overall_html(dest_dir_path="svg_txt_scale_x_from_point/")\n```',  # noqa
     ##################################################
     "## flip_x property interface example": "## flip_x属性のインターフェイス例",
     ##################################################
-    "The `flip_x` property updates or gets the instance\'s flip-x (reflecting state) boolean value:": "`flip_x`属性ではインスタンスのX軸の反転状況の真偽値の更新もしくは取得を行えます:",  # noqa
+    "The `flip_x` property updates or gets the instance's flip-x (reflecting state) boolean value:": "`flip_x`属性ではインスタンスのX軸の反転状況の真偽値の更新もしくは取得を行えます:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\n\n\ndef on_timer(e: ap.TimerEvent, options: dict) -> None:\n    \"\"\"\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.TimerEvent\n        Event instance.\n    options : dict\n        Optional argument dictionary.\n    \"\"\"\n    svg_text.flip_x = svg_text.flip_x.not_\n\n\nap.Timer(handler=on_timer, delay=1000).start()\nap.save_overall_html(dest_dir_path=\"svg_txt_flip_x/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\n\n\ndef on_timer(e: ap.TimerEvent, options: dict) -> None:\n    \"\"\"\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.TimerEvent\n        Event instance.\n    options : dict\n        Optional argument dictionary.\n    \"\"\"\n    svg_text.flip_x = svg_text.flip_x.not_\n\n\nap.Timer(handler=on_timer, delay=1000).start()\nap.save_overall_html(dest_dir_path=\"svg_txt_flip_x/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\n\n\ndef on_timer(e: ap.TimerEvent, options: dict) -> None:\n    """\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.TimerEvent\n        Event instance.\n    options : dict\n        Optional argument dictionary.\n    """\n    svg_text.flip_x = svg_text.flip_x.not_\n\n\nap.Timer(handler=on_timer, delay=1000).start()\nap.save_overall_html(dest_dir_path="svg_txt_flip_x/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\n\n\ndef on_timer(e: ap.TimerEvent, options: dict) -> None:\n    """\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.TimerEvent\n        Event instance.\n    options : dict\n        Optional argument dictionary.\n    """\n    svg_text.flip_x = svg_text.flip_x.not_\n\n\nap.Timer(handler=on_timer, delay=1000).start()\nap.save_overall_html(dest_dir_path="svg_txt_flip_x/")\n```',  # noqa
     ##################################################
     "## flip_y property interface example": "## flip_y属性のインターフェイス例",
     ##################################################
-    "The `flip_y` property updates or gets the instance\'s flip-y (reflecting state) boolean value:": "`flip_y`属性ではインスタンスのX軸の反転状況の真偽値の更新もしくは取得を行えます:",  # noqa
+    "The `flip_y` property updates or gets the instance's flip-y (reflecting state) boolean value:": "`flip_y`属性ではインスタンスのX軸の反転状況の真偽値の更新もしくは取得を行えます:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\n\n\ndef on_timer(e: ap.TimerEvent, options: dict) -> None:\n    \"\"\"\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.TimerEvent\n        Event instance.\n    options : dict\n        Optional argument dictionary.\n    \"\"\"\n    svg_text.flip_y = svg_text.flip_y.not_\n\n\nap.Timer(handler=on_timer, delay=1000).start()\nap.save_overall_html(dest_dir_path=\"svg_txt_flip_y/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text=\"Hello, world!\",\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\n\n\ndef on_timer(e: ap.TimerEvent, options: dict) -> None:\n    \"\"\"\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.TimerEvent\n        Event instance.\n    options : dict\n        Optional argument dictionary.\n    \"\"\"\n    svg_text.flip_y = svg_text.flip_y.not_\n\n\nap.Timer(handler=on_timer, delay=1000).start()\nap.save_overall_html(dest_dir_path=\"svg_txt_flip_y/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\n\n\ndef on_timer(e: ap.TimerEvent, options: dict) -> None:\n    """\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.TimerEvent\n        Event instance.\n    options : dict\n        Optional argument dictionary.\n    """\n    svg_text.flip_y = svg_text.flip_y.not_\n\n\nap.Timer(handler=on_timer, delay=1000).start()\nap.save_overall_html(dest_dir_path="svg_txt_flip_y/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText(\n    text="Hello, world!",\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\n\n\ndef on_timer(e: ap.TimerEvent, options: dict) -> None:\n    """\n    The handler to handle a timer event.\n\n    Parameters\n    ----------\n    e : ap.TimerEvent\n        Event instance.\n    options : dict\n        Optional argument dictionary.\n    """\n    svg_text.flip_y = svg_text.flip_y.not_\n\n\nap.Timer(handler=on_timer, delay=1000).start()\nap.save_overall_html(dest_dir_path="svg_txt_flip_y/")\n```',  # noqa
     ##################################################
     "## SvgText constructor API": "## SvgText クラスのコンストラクタのAPI",
     ##################################################
-    "<span class=\"inconspicuous-txt\">Note: the document build script generates and updates this API document section automatically. Maybe this section is duplicated compared with previous sections.</span>": "<span class=\"inconspicuous-txt\">特記事項: このAPIドキュメントはドキュメントビルド用のスクリプトによって自動で生成・同期されています。そのためもしかしたらこの節の内容は前節までの内容と重複している場合があります。</span>",  # noqa
+    '<span class="inconspicuous-txt">Note: the document build script generates and updates this API document section automatically. Maybe this section is duplicated compared with previous sections.</span>': '<span class="inconspicuous-txt">特記事項: このAPIドキュメントはドキュメントビルド用のスクリプトによって自動で生成・同期されています。そのためもしかしたらこの節の内容は前節までの内容と重複している場合があります。</span>',  # noqa
     ##################################################
     "**[Interface summary]**": "**[インターフェイス概要]**",
     ##################################################
     "The class for an SVG text.<hr>": "SVGテキストのためのクラスです。<hr>",
     ##################################################
     "**[Parameters]**": "**[引数]**",
     ##################################################
@@ -247,13 +247,13 @@
     ##################################################
     "  - A JavaScript variable name suffix string. This setting is sometimes useful for JavaScript debugging.": "  - JavaScript上の変数のサフィックスの設定です。この設定はJavaScriptのデバッグ時に役立つことがあります。",  # noqa
     ##################################################
     "<hr>": "<hr>",
     ##################################################
     "**[Notes]**": "**[特記事項]**",
     ##################################################
-    " ・SvgText\'s y-coordinate zero-position starts at the bottom of a text. So if you set y=0, a text becomes almost invisible.<hr>": " ・SVGTextクラスの座標の0の位置はテキストの下部からスタートします。そのためもしもy=0を指定した場合、テキストはほとんど見えない状態になります。<hr>",  # noqa
+    " ・SvgText's y-coordinate zero-position starts at the bottom of a text. So if you set y=0, a text becomes almost invisible.<hr>": " ・SVGTextクラスの座標の0の位置はテキストの下部からスタートします。そのためもしもy=0を指定した場合、テキストはほとんど見えない状態になります。<hr>",  # noqa
     ##################################################
     "**[Examples]**": "**[コードサンプル]**",
     ##################################################
-    "```py\n>>> import apysc as ap\n>>> stage: ap.Stage = ap.Stage(\n...     background_color=ap.Color(\"#333\"),\n...     stage_width=200,\n...     stage_height=50,\n...     stage_elem_id=\"stage\",\n... )\n>>> svg_text: ap.SvgText = ap.SvgText(\n...     text=\"Hello, world!\",\n...     font_size=20,\n...     fill_color=ap.Color(\"#0af\"),\n... )\n>>> svg_text.text\nString(\"Hello, world!\")\n\n>>> svg_text.font_size\nInt(20)\n\n>>> svg_text.fill_color\nColor(\"#00aaff\")\n```": "```py\n>>> import apysc as ap\n>>> stage: ap.Stage = ap.Stage(\n...     background_color=ap.Color(\"#333\"),\n...     stage_width=200,\n...     stage_height=50,\n...     stage_elem_id=\"stage\",\n... )\n>>> svg_text: ap.SvgText = ap.SvgText(\n...     text=\"Hello, world!\",\n...     font_size=20,\n...     fill_color=ap.Color(\"#0af\"),\n... )\n>>> svg_text.text\nString(\"Hello, world!\")\n\n>>> svg_text.font_size\nInt(20)\n\n>>> svg_text.fill_color\nColor(\"#00aaff\")\n```",  # noqa
+    '```py\n>>> import apysc as ap\n>>> stage: ap.Stage = ap.Stage(\n...     background_color=ap.Color("#333"),\n...     stage_width=200,\n...     stage_height=50,\n...     stage_elem_id="stage",\n... )\n>>> svg_text: ap.SvgText = ap.SvgText(\n...     text="Hello, world!",\n...     font_size=20,\n...     fill_color=ap.Color("#0af"),\n... )\n>>> svg_text.text\nString("Hello, world!")\n\n>>> svg_text.font_size\nInt(20)\n\n>>> svg_text.fill_color\nColor("#00aaff")\n```': '```py\n>>> import apysc as ap\n>>> stage: ap.Stage = ap.Stage(\n...     background_color=ap.Color("#333"),\n...     stage_width=200,\n...     stage_height=50,\n...     stage_elem_id="stage",\n... )\n>>> svg_text: ap.SvgText = ap.SvgText(\n...     text="Hello, world!",\n...     font_size=20,\n...     fill_color=ap.Color("#0af"),\n... )\n>>> svg_text.text\nString("Hello, world!")\n\n>>> svg_text.font_size\nInt(20)\n\n>>> svg_text.fill_color\nColor("#00aaff")\n```',  # noqa
 }
```

### Comparing `apysc-4.3.0/apysc/_translation/jp/svg_text_span.py` & `apysc-4.3.2/apysc/_translation/jp/svg_text_span.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,111 +19,111 @@
     ##################################################
     "You can create an `SvgText` instance with multiple `SvgTextSpan` class instances and set different text styles.": "複数の`SvgTextSpan`クラスのインスタンスを使ってそれぞれに異なるテキストのスタイルを設定した状態の`SvgText`のインスタンスを作成することができます。",  # noqa
     ##################################################
     "## Basic usage": "## 基本的な使い方",
     ##################################################
     "The `SvgTextSpan` class constructor requires the `text` argument.": "`SvgTextSpan`クラスのコンストラクタには`text`引数を必要とします。",  # noqa
     ##################################################
-    "The constructor also accepts each font\'s and style\'s argument, such as the `font_size`, `font_family`, `fill_color`, and `bold`.": "コンストラクタでは`font_size`や`font_family`、`fill_color`、`bold`などの各スタイル設定の引数を受け付けます。",  # noqa
+    "The constructor also accepts each font's and style's argument, such as the `font_size`, `font_family`, `fill_color`, and `bold`.": "コンストラクタでは`font_size`や`font_family`、`fill_color`、`bold`などの各スタイル設定の引数を受け付けます。",  # noqa
     ##################################################
-    "If you skip the style settings\' arguments, these settings become the parent SvgText\'s styles.": "もしもそれらのスタイル設定の引数指定を省略した場合、親のSVGTextのインスタンスのスタイルが反映されます。",  # noqa
+    "If you skip the style settings' arguments, these settings become the parent SvgText's styles.": "もしもそれらのスタイル設定の引数指定を省略した場合、親のSVGTextのインスタンスのスタイルが反映されます。",  # noqa
     ##################################################
     "You can use `SvgTextSpan` instances to create an `SvgText` instance with the `create_with_svg_text_spans` class method.": "また、複数の`SvgTextSpan`のインスタンスを使って`SvgText`のインスタンスの作成するには`create_with_svg_text_spans`のクラスメソッドを使うことで対応ができます。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[\n        ap.SvgTextSpan(text=\"Lorem \"),\n        ap.SvgTextSpan(text=\"ipsum \", font_size=20, fill_color=ap.Color(\"#0af\")),\n        ap.SvgTextSpan(text=\"dolor \", font_size=12),\n    ],\n    fill_color=ap.Color(\"#aaa\"),\n    font_size=16,\n    x=20,\n    y=32,\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_basic_usage/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[\n        ap.SvgTextSpan(text=\"Lorem \"),\n        ap.SvgTextSpan(text=\"ipsum \", font_size=20, fill_color=ap.Color(\"#0af\")),\n        ap.SvgTextSpan(text=\"dolor \", font_size=12),\n    ],\n    fill_color=ap.Color(\"#aaa\"),\n    font_size=16,\n    x=20,\n    y=32,\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_basic_usage/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[\n        ap.SvgTextSpan(text="Lorem "),\n        ap.SvgTextSpan(text="ipsum ", font_size=20, fill_color=ap.Color("#0af")),\n        ap.SvgTextSpan(text="dolor ", font_size=12),\n    ],\n    fill_color=ap.Color("#aaa"),\n    font_size=16,\n    x=20,\n    y=32,\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_basic_usage/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[\n        ap.SvgTextSpan(text="Lorem "),\n        ap.SvgTextSpan(text="ipsum ", font_size=20, fill_color=ap.Color("#0af")),\n        ap.SvgTextSpan(text="dolor ", font_size=12),\n    ],\n    fill_color=ap.Color("#aaa"),\n    font_size=16,\n    x=20,\n    y=32,\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_basic_usage/")\n```',  # noqa
     ##################################################
     "## Notes of the line breaking": "## 改行に対する特記事項",
     ##################################################
     "The `SvgTextSpan` class ignores line breaks.": "`SvgTextSpan`クラスは改行設定を無視します。",
     ##################################################
-    "For instance, the following example\'s text contains a line break (`\n`), but the text line becomes a single line.": "例えば、以下の例では改行用の文字列（`\n`）を含んでいますがテキストの行は単一行になっています。",  # noqa
+    "For instance, the following example's text contains a line break (`\n`), but the text line becomes a single line.": "例えば、以下の例では改行用の文字列（`\n`）を含んでいますがテキストの行は単一行になっています。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[\n        ap.SvgTextSpan(text=\"Lorem \n\"),\n        ap.SvgTextSpan(text=\"ipsum \n\"),\n        ap.SvgTextSpan(text=\"dolor\"),\n    ],\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_notes_of_the_line_break/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[\n        ap.SvgTextSpan(text=\"Lorem \n\"),\n        ap.SvgTextSpan(text=\"ipsum \n\"),\n        ap.SvgTextSpan(text=\"dolor\"),\n    ],\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_notes_of_the_line_break/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[\n        ap.SvgTextSpan(text="Lorem \n"),\n        ap.SvgTextSpan(text="ipsum \n"),\n        ap.SvgTextSpan(text="dolor"),\n    ],\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_notes_of_the_line_break/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[\n        ap.SvgTextSpan(text="Lorem \n"),\n        ap.SvgTextSpan(text="ipsum \n"),\n        ap.SvgTextSpan(text="dolor"),\n    ],\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_notes_of_the_line_break/")\n```',  # noqa
     ##################################################
     "If you want to add a line break, please use the `SvgText` class (not the `SvgTextSpan`) or create multiple `SvgText` instances.": "もしも改行を加えたい場合には`SvgTextSpan`クラスではなく`SvgText`クラスを使用するか、もしくは複数のインスタンスを作成して対応をお願いします。",  # noqa
     ##################################################
     "## text property interface example": "## text 属性のインターフェイス例",
     ##################################################
-    "The `text` property updates or gets the instance\'s text.": "`text`属性ではインスタンスのテキストの更新もしくは取得を行えます。",  # noqa
+    "The `text` property updates or gets the instance's text.": "`text`属性ではインスタンスのテキストの更新もしくは取得を行えます。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text=\"Lorem \")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text=\"ipsum\")\ntext_span_2.text = ap.String(\"dolor\")\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_text/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text=\"Lorem \")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text=\"ipsum\")\ntext_span_2.text = ap.String(\"dolor\")\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_text/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text="Lorem ")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text="ipsum")\ntext_span_2.text = ap.String("dolor")\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_text/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text="Lorem ")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text="ipsum")\ntext_span_2.text = ap.String("dolor")\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_text/")\n```',  # noqa
     ##################################################
     "## font_size property interface example": "## font_size 属性のインターフェイス例",
     ##################################################
-    "The `font_size` property updates or gets the instance\'s font size.": "`font_size`属性ではインスタンスのフォントサイズの更新もしくは取得を行えます。",  # noqa
+    "The `font_size` property updates or gets the instance's font size.": "`font_size`属性ではインスタンスのフォントサイズの更新もしくは取得を行えます。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text=\"Lorem \")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text=\"ipsum\")\ntext_span_2.font_size = ap.Int(25)\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_font_size/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text=\"Lorem \")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text=\"ipsum\")\ntext_span_2.font_size = ap.Int(25)\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_font_size/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text="Lorem ")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text="ipsum")\ntext_span_2.font_size = ap.Int(25)\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_font_size/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text="Lorem ")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text="ipsum")\ntext_span_2.font_size = ap.Int(25)\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_font_size/")\n```',  # noqa
     ##################################################
     "## font_family property interface example": "## font_family 属性のインターフェイス例",
     ##################################################
-    "The `font_family` property updates or gets the instance\'s font family.": "`font_family`属性ではインスタンスのフォントファミリー（フォントの指定）の更新もしくは取得を行えます。",  # noqa
+    "The `font_family` property updates or gets the instance's font family.": "`font_family`属性ではインスタンスのフォントファミリー（フォントの指定）の更新もしくは取得を行えます。",  # noqa
     ##################################################
     "This property requires an `Array` of each font name `String`.": "この属性は各フォント名の`String`型の文字列を格納した`Array`型の配列を必要とします。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text=\"Lorem \")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text=\"ipsum\")\ntext_span_2.font_family = ap.Array([ap.String(\"Impact\"), ap.String(\"Arial\")])\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_font_family/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text=\"Lorem \")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text=\"ipsum\")\ntext_span_2.font_family = ap.Array([ap.String(\"Impact\"), ap.String(\"Arial\")])\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_font_family/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text="Lorem ")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text="ipsum")\ntext_span_2.font_family = ap.Array([ap.String("Impact"), ap.String("Arial")])\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_font_family/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text="Lorem ")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text="ipsum")\ntext_span_2.font_family = ap.Array([ap.String("Impact"), ap.String("Arial")])\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_font_family/")\n```',  # noqa
     ##################################################
     "## fill_color property interface example": "## fill_color属性のインターフェイス例",
     ##################################################
-    "The `fill_color` property updates or gets the instance\'s fill color:": "`fill_color`属性は塗りの色の値の更新もしくは取得を行えます:",  # noqa
+    "The `fill_color` property updates or gets the instance's fill color:": "`fill_color`属性は塗りの色の値の更新もしくは取得を行えます:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text=\"Lorem \")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text=\"ipsum\")\ntext_span_2.fill_color = ap.Color(\"#0af\")\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_fill_color/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text=\"Lorem \")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text=\"ipsum\")\ntext_span_2.fill_color = ap.Color(\"#0af\")\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_fill_color/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text="Lorem ")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text="ipsum")\ntext_span_2.fill_color = ap.Color("#0af")\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_fill_color/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text="Lorem ")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text="ipsum")\ntext_span_2.fill_color = ap.Color("#0af")\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_fill_color/")\n```',  # noqa
     ##################################################
     "## fill_alpha property interface example": "## fill_alpha属性のインターフェイス例",
     ##################################################
-    "The `fill_alpha` property updates or gets the instance\'s fill alpha (opacity):": "`fill_alpha`属性は塗りの透明度の値の更新もしくは取得を行えます:",  # noqa
+    "The `fill_alpha` property updates or gets the instance's fill alpha (opacity):": "`fill_alpha`属性は塗りの透明度の値の更新もしくは取得を行えます:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text=\"Lorem \")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text=\"ipsum\")\ntext_span_2.fill_alpha = ap.Number(0.3)\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_fill_alpha/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text=\"Lorem \")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text=\"ipsum\")\ntext_span_2.fill_alpha = ap.Number(0.3)\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_fill_alpha/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text="Lorem ")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text="ipsum")\ntext_span_2.fill_alpha = ap.Number(0.3)\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_fill_alpha/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text="Lorem ")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text="ipsum")\ntext_span_2.fill_alpha = ap.Number(0.3)\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_fill_alpha/")\n```',  # noqa
     ##################################################
     "## line_color property interface example": "## line_color属性のインターフェイス例",
     ##################################################
-    "The `line_color` property updates or gets the instance\'s line color:": "`line_color`属性では線の色の値の更新もしくは取得を行えます:",  # noqa
+    "The `line_color` property updates or gets the instance's line color:": "`line_color`属性では線の色の値の更新もしくは取得を行えます:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(\n    text=\"Lorem \", line_thickness=1, font_size=20, bold=True\n)\ntext_span_1.line_color = ap.Color(\"#aaa\")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(\n    text=\"ipsum\", line_thickness=1, font_size=20, bold=True\n)\ntext_span_2.line_color = ap.Color(\"#0af\")\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.COLORLESS,\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_line_color/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(\n    text=\"Lorem \", line_thickness=1, font_size=20, bold=True\n)\ntext_span_1.line_color = ap.Color(\"#aaa\")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(\n    text=\"ipsum\", line_thickness=1, font_size=20, bold=True\n)\ntext_span_2.line_color = ap.Color(\"#0af\")\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.COLORLESS,\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_line_color/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(\n    text="Lorem ", line_thickness=1, font_size=20, bold=True\n)\ntext_span_1.line_color = ap.Color("#aaa")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(\n    text="ipsum", line_thickness=1, font_size=20, bold=True\n)\ntext_span_2.line_color = ap.Color("#0af")\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.COLORLESS,\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_line_color/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(\n    text="Lorem ", line_thickness=1, font_size=20, bold=True\n)\ntext_span_1.line_color = ap.Color("#aaa")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(\n    text="ipsum", line_thickness=1, font_size=20, bold=True\n)\ntext_span_2.line_color = ap.Color("#0af")\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.COLORLESS,\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_line_color/")\n```',  # noqa
     ##################################################
     "## line_alpha property interface example": "## line_alpha属性のインターフェイス例",
     ##################################################
-    "The `line_alpha` property updates or gets the instance\'s line alpha (opacity):": "`line_alpha`属性では線の透明度の値の更新もしくは取得を行えます:",  # noqa
+    "The `line_alpha` property updates or gets the instance's line alpha (opacity):": "`line_alpha`属性では線の透明度の値の更新もしくは取得を行えます:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(\n    text=\"Lorem \",\n    line_color=ap.Color(\"#0af\"),\n    line_thickness=1,\n    font_size=20,\n    bold=True,\n)\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(\n    text=\"ipsum\",\n    line_color=ap.Color(\"#0af\"),\n    line_thickness=1,\n    font_size=20,\n    bold=True,\n)\ntext_span_2.line_alpha = ap.Number(0.3)\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.COLORLESS,\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_line_alpha/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(\n    text=\"Lorem \",\n    line_color=ap.Color(\"#0af\"),\n    line_thickness=1,\n    font_size=20,\n    bold=True,\n)\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(\n    text=\"ipsum\",\n    line_color=ap.Color(\"#0af\"),\n    line_thickness=1,\n    font_size=20,\n    bold=True,\n)\ntext_span_2.line_alpha = ap.Number(0.3)\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.COLORLESS,\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_line_alpha/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(\n    text="Lorem ",\n    line_color=ap.Color("#0af"),\n    line_thickness=1,\n    font_size=20,\n    bold=True,\n)\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(\n    text="ipsum",\n    line_color=ap.Color("#0af"),\n    line_thickness=1,\n    font_size=20,\n    bold=True,\n)\ntext_span_2.line_alpha = ap.Number(0.3)\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.COLORLESS,\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_line_alpha/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(\n    text="Lorem ",\n    line_color=ap.Color("#0af"),\n    line_thickness=1,\n    font_size=20,\n    bold=True,\n)\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(\n    text="ipsum",\n    line_color=ap.Color("#0af"),\n    line_thickness=1,\n    font_size=20,\n    bold=True,\n)\ntext_span_2.line_alpha = ap.Number(0.3)\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.COLORLESS,\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_line_alpha/")\n```',  # noqa
     ##################################################
     "## line_thickness property interface example": "## line_thickness属性のインターフェイス例",
     ##################################################
-    "The `line_thickness` property updates or gets the instance\'s line thickness (line width):": "`line_thickness`属性では線の幅の更新もしくは取得を行えます:",  # noqa
+    "The `line_thickness` property updates or gets the instance's line thickness (line width):": "`line_thickness`属性では線の幅の更新もしくは取得を行えます:",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(\n    text=\"Lorem \",\n    line_color=ap.Color(\"#0af\"),\n    font_size=20,\n    bold=True,\n)\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(\n    text=\"ipsum\",\n    line_color=ap.Color(\"#0af\"),\n    font_size=20,\n    bold=True,\n)\ntext_span_1.line_thickness = ap.Int(3)\ntext_span_2.line_thickness = ap.Int(3)\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.COLORLESS,\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_line_thickness/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(\n    text=\"Lorem \",\n    line_color=ap.Color(\"#0af\"),\n    font_size=20,\n    bold=True,\n)\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(\n    text=\"ipsum\",\n    line_color=ap.Color(\"#0af\"),\n    font_size=20,\n    bold=True,\n)\ntext_span_1.line_thickness = ap.Int(3)\ntext_span_2.line_thickness = ap.Int(3)\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.COLORLESS,\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_line_thickness/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(\n    text="Lorem ",\n    line_color=ap.Color("#0af"),\n    font_size=20,\n    bold=True,\n)\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(\n    text="ipsum",\n    line_color=ap.Color("#0af"),\n    font_size=20,\n    bold=True,\n)\ntext_span_1.line_thickness = ap.Int(3)\ntext_span_2.line_thickness = ap.Int(3)\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.COLORLESS,\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_line_thickness/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(\n    text="Lorem ",\n    line_color=ap.Color("#0af"),\n    font_size=20,\n    bold=True,\n)\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(\n    text="ipsum",\n    line_color=ap.Color("#0af"),\n    font_size=20,\n    bold=True,\n)\ntext_span_1.line_thickness = ap.Int(3)\ntext_span_2.line_thickness = ap.Int(3)\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.COLORLESS,\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_line_thickness/")\n```',  # noqa
     ##################################################
     "## bold property interface example": "## bold 属性のインターフェイス例",
     ##################################################
-    "The `bold` property updates or gets the instance\'s `bold` text setting.": "`bold`属性ではインスタンスの太字設定の更新もしくは取得を行えます。",  # noqa
+    "The `bold` property updates or gets the instance's `bold` text setting.": "`bold`属性ではインスタンスの太字設定の更新もしくは取得を行えます。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text=\"Lorem \")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text=\"ipsum\")\ntext_span_2.bold = ap.Boolean(True)\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_bold/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text=\"Lorem \")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text=\"ipsum\")\ntext_span_2.bold = ap.Boolean(True)\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_bold/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text="Lorem ")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text="ipsum")\ntext_span_2.bold = ap.Boolean(True)\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_bold/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text="Lorem ")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text="ipsum")\ntext_span_2.bold = ap.Boolean(True)\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_bold/")\n```',  # noqa
     ##################################################
     "## italic property interface example": "## italic 属性のインターフェイス例",
     ##################################################
-    "The `italic` property updates or gets the instance\'s `italic` style setting.": "`italic`属性ではインスタンスの斜体の設定の更新もしくは取得を行えます。",  # noqa
+    "The `italic` property updates or gets the instance's `italic` style setting.": "`italic`属性ではインスタンスの斜体の設定の更新もしくは取得を行えます。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text=\"Lorem \")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text=\"ipsum\")\ntext_span_2.italic = ap.Boolean(True)\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_italic/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text=\"Lorem \")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text=\"ipsum\")\ntext_span_2.italic = ap.Boolean(True)\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_italic/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text="Lorem ")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text="ipsum")\ntext_span_2.italic = ap.Boolean(True)\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_italic/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text="Lorem ")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text="ipsum")\ntext_span_2.italic = ap.Boolean(True)\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_italic/")\n```',  # noqa
     ##################################################
     "## delta_x property interface example": "## delta_x 属性のインターフェイス例",
     ##################################################
-    "The `delta_x` property updates or gets the instance\'s delta-x (x-coordinate adjustment).": "`delta_x`属性ではインスタンスのX座標の調整値の更新もしくは取得を行えます。",  # noqa
+    "The `delta_x` property updates or gets the instance's delta-x (x-coordinate adjustment).": "`delta_x`属性ではインスタンスのX座標の調整値の更新もしくは取得を行えます。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text=\"Lorem \")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text=\"ipsum\")\ntext_span_2.delta_x = ap.Number(-20)\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_delta_x/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id=\"stage\",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text=\"Lorem \")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text=\"ipsum\")\ntext_span_2.delta_x = ap.Number(-20)\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_delta_x/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text="Lorem ")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text="ipsum")\ntext_span_2.delta_x = ap.Number(-20)\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_delta_x/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=50,\n    stage_elem_id="stage",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text="Lorem ")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text="ipsum")\ntext_span_2.delta_x = ap.Number(-20)\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_delta_x/")\n```',  # noqa
     ##################################################
     "## delta_y property interface example": "## delta_y 属性のインターフェイス例",
     ##################################################
-    "The `delta_y` property updates or gets the instance\'s delta-y (y-coordinate adjustment).": "`delta_y`属性ではインスタンスのY座標の調整値の更新もくしは取得を行えます。",  # noqa
+    "The `delta_y` property updates or gets the instance's delta-y (y-coordinate adjustment).": "`delta_y`属性ではインスタンスのY座標の調整値の更新もくしは取得を行えます。",  # noqa
     ##################################################
     "Note: This setting inherits a y-coordinate from the previous `SvgTextSpan` instance.": "特記事項: この設定は直前の`SvgTextSpan`インスタンスの設定を引き継ぎます。",  # noqa
     ##################################################
-    "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=80,\n    stage_elem_id=\"stage\",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text=\"Lorem \")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text=\"ipsum \")\ntext_span_3: ap.SvgTextSpan = ap.SvgTextSpan(text=\"dolar\")\n\ntext_span_2.delta_y = ap.Number(10)\ntext_span_3.delta_y = ap.Number(10)\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_delta_y/\")\n```": "```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color(\"#333\"),\n    stage_width=200,\n    stage_height=80,\n    stage_elem_id=\"stage\",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text=\"Lorem \")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text=\"ipsum \")\ntext_span_3: ap.SvgTextSpan = ap.SvgTextSpan(text=\"dolar\")\n\ntext_span_2.delta_y = ap.Number(10)\ntext_span_3.delta_y = ap.Number(10)\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color(\"#aaa\"),\n)\n\nap.save_overall_html(dest_dir_path=\"svg_txt_span_delta_y/\")\n```",  # noqa
+    '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=80,\n    stage_elem_id="stage",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text="Lorem ")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text="ipsum ")\ntext_span_3: ap.SvgTextSpan = ap.SvgTextSpan(text="dolar")\n\ntext_span_2.delta_y = ap.Number(10)\ntext_span_3.delta_y = ap.Number(10)\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_delta_y/")\n```': '```py\n# runnable\nimport apysc as ap\n\nstage: ap.Stage = ap.Stage(\n    background_color=ap.Color("#333"),\n    stage_width=200,\n    stage_height=80,\n    stage_elem_id="stage",\n)\ntext_span_1: ap.SvgTextSpan = ap.SvgTextSpan(text="Lorem ")\ntext_span_2: ap.SvgTextSpan = ap.SvgTextSpan(text="ipsum ")\ntext_span_3: ap.SvgTextSpan = ap.SvgTextSpan(text="dolar")\n\ntext_span_2.delta_y = ap.Number(10)\ntext_span_3.delta_y = ap.Number(10)\n\nsvg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n    text_spans=[text_span_1, text_span_2],\n    font_size=16,\n    x=20,\n    y=32,\n    fill_color=ap.Color("#aaa"),\n)\n\nap.save_overall_html(dest_dir_path="svg_txt_span_delta_y/")\n```',  # noqa
     ##################################################
     "## SvgTextSpan constructor API": "## SvgTextSpan クラスのコンストラクタのAPI",
     ##################################################
-    "<span class=\"inconspicuous-txt\">Note: the document build script generates and updates this API document section automatically. Maybe this section is duplicated compared with previous sections.</span>": "<span class=\"inconspicuous-txt\">特記事項: このAPIドキュメントはドキュメントビルド用のスクリプトによって自動で生成・同期されています。そのためもしかしたらこの節の内容は前節までの内容と重複している場合があります。</span>",  # noqa
+    '<span class="inconspicuous-txt">Note: the document build script generates and updates this API document section automatically. Maybe this section is duplicated compared with previous sections.</span>': '<span class="inconspicuous-txt">特記事項: このAPIドキュメントはドキュメントビルド用のスクリプトによって自動で生成・同期されています。そのためもしかしたらこの節の内容は前節までの内容と重複している場合があります。</span>',  # noqa
     ##################################################
     "**[Interface summary]**": "**[インターフェイス概要]**",
     ##################################################
     "The class for an SVG text-span (the child class of `SvgText`).<hr>": "`SvgText`の子となるSVGのtext-span要素のためのクラスです。<hr>",  # noqa
     ##################################################
     "**[Parameters]**": "**[引数]**",
     ##################################################
@@ -165,43 +165,43 @@
     ##################################################
     "- `italic`: Optional[Union[bool, Boolean]], optional": "- `italic`: Optional[Union[bool, Boolean]], optional",  # noqa
     ##################################################
     "  - A boolean, whether a text is an italic style or not (normal).": "  - テキストを斜体表示のスタイル設定を行うかどうかの真偽値。",  # noqa
     ##################################################
     "- `delta_x`: Union[float, Number], optional": "- `delta_x`: Union[float, Number], optional",  # noqa
     ##################################################
-    "  - A coordinate delta-x setting. Notes: This setting also changes a coordinate of subsequent `SvgTextSpan`\'s instance.": "  - X座標の調整値の設定。特記事項 : この設定は後に続く`SvgTextSpan`のインスタンスの座標も変更します。",  # noqa
+    "  - A coordinate delta-x setting. Notes: This setting also changes a coordinate of subsequent `SvgTextSpan`'s instance.": "  - X座標の調整値の設定。特記事項 : この設定は後に続く`SvgTextSpan`のインスタンスの座標も変更します。",  # noqa
     ##################################################
     "- `delta_y`: Union[float, Number], optional": "- `delta_y`: Union[float, Number], optional",  # noqa
     ##################################################
-    "  - A coordinate delta-y setting. Notes: This setting also changes a coordinate of subsequent `SvgTextSpan`\'s instance.": "  - Y座標の調整値の設定。特記事項 : この設定は後に続く`SvgTextSpan`のインスタンスの座標も更新します。",  # noqa
+    "  - A coordinate delta-y setting. Notes: This setting also changes a coordinate of subsequent `SvgTextSpan`'s instance.": "  - Y座標の調整値の設定。特記事項 : この設定は後に続く`SvgTextSpan`のインスタンスの座標も更新します。",  # noqa
     ##################################################
     "- `variable_name_suffix`: str, optional": "- `variable_name_suffix`: str, optional",  # noqa
     ##################################################
     "  - A JavaScript variable name suffix string. This setting is sometimes useful for JavaScript debugging.": "  - JavaScript上の変数のサフィックスの設定です。この設定はJavaScriptのデバッグ時に役立つことがあります。",  # noqa
     ##################################################
     "<hr>": "<hr>",
     ##################################################
     "**[Notes]**": "**[特記事項]**",
     ##################################################
     " ・If style settings are `None`, its styles inherit parent style settings.<hr>": " ・もしも各種スタイル設定に`None`が指定された場合、そのスタイルは親のスタイル設定を引き継ぎます。<hr>",  # noqa
     ##################################################
     "**[Examples]**": "**[コードサンプル]**",
     ##################################################
-    "```py\n>>> import apysc as ap\n>>> stage: ap.Stage = ap.Stage(\n...     background_color=ap.Color(\"#333\"), stage_width=200, stage_height=50\n... )\n>>> svg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n...     text_spans=[\n...         ap.SvgTextSpan(text=\"Hello, \"),\n...         ap.SvgTextSpan(text=\"Hello, \", font_size=14),\n...     ],\n...     font_size=20,\n...     fill_color=ap.Color(\"#0af\"),\n... )\n```": "```py\n>>> import apysc as ap\n>>> stage: ap.Stage = ap.Stage(\n...     background_color=ap.Color(\"#333\"), stage_width=200, stage_height=50\n... )\n>>> svg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n...     text_spans=[\n...         ap.SvgTextSpan(text=\"Hello, \"),\n...         ap.SvgTextSpan(text=\"Hello, \", font_size=14),\n...     ],\n...     font_size=20,\n...     fill_color=ap.Color(\"#0af\"),\n... )\n```",  # noqa
+    '```py\n>>> import apysc as ap\n>>> stage: ap.Stage = ap.Stage(\n...     background_color=ap.Color("#333"), stage_width=200, stage_height=50\n... )\n>>> svg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n...     text_spans=[\n...         ap.SvgTextSpan(text="Hello, "),\n...         ap.SvgTextSpan(text="Hello, ", font_size=14),\n...     ],\n...     font_size=20,\n...     fill_color=ap.Color("#0af"),\n... )\n```': '```py\n>>> import apysc as ap\n>>> stage: ap.Stage = ap.Stage(\n...     background_color=ap.Color("#333"), stage_width=200, stage_height=50\n... )\n>>> svg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n...     text_spans=[\n...         ap.SvgTextSpan(text="Hello, "),\n...         ap.SvgTextSpan(text="Hello, ", font_size=14),\n...     ],\n...     font_size=20,\n...     fill_color=ap.Color("#0af"),\n... )\n```',  # noqa
     ##################################################
     "<hr>": "<hr>",
     ##################################################
     "**[References]**": "**[関連資料]**",
     ##################################################
     "- [SvgText class](https://simon-ritchie.github.io/apysc/en/svg_text.html)": "- [SvgText クラス](https://simon-ritchie.github.io/apysc/jp/jp_svg_text.html)",  # noqa
     ##################################################
     "## SvgText create_with_svg_text_spans class method API": "## SvgText クラスの create_with_svg_text_spans クラスメソッドのAPI",  # noqa
     ##################################################
-    "<span class=\"inconspicuous-txt\">Note: the document build script generates and updates this API document section automatically. Maybe this section is duplicated compared with previous sections.</span>": "<span class=\"inconspicuous-txt\">特記事項: このAPIドキュメントはドキュメントビルド用のスクリプトによって自動で生成・同期されています。そのためもしかしたらこの節の内容は前節までの内容と重複している場合があります。</span>",  # noqa
+    '<span class="inconspicuous-txt">Note: the document build script generates and updates this API document section automatically. Maybe this section is duplicated compared with previous sections.</span>': '<span class="inconspicuous-txt">特記事項: このAPIドキュメントはドキュメントビルド用のスクリプトによって自動で生成・同期されています。そのためもしかしたらこの節の内容は前節までの内容と重複している場合があります。</span>',  # noqa
     ##################################################
     "**[Interface summary]**": "**[インターフェイス概要]**",
     ##################################################
     "Create an `SvgText` instance with specified text spans.<hr>": "指定された各text spanのインスタンスを使用して`SvgText`のインスタンスを生成します。<hr>",  # noqa
     ##################################################
     "**[Parameters]**": "**[引数]**",
     ##################################################
@@ -277,19 +277,19 @@
     ##################################################
     "  - A created `SvgText` instance.": "  - 生成された`SvgText`のインスタンス。",
     ##################################################
     "<hr>": "<hr>",
     ##################################################
     "**[Notes]**": "**[特記事項]**",
     ##################################################
-    " ・SvgText\'s y-coordinate zero-position starts at the bottom of a text. So if you set y=0, a text becomes almost invisible.<hr>": " ・SVGTextクラスの座標の0の位置はテキストの下部からスタートします。そのためもしもy=0を指定した場合、テキストはほとんど見えない状態になります。<hr>",  # noqa
+    " ・SvgText's y-coordinate zero-position starts at the bottom of a text. So if you set y=0, a text becomes almost invisible.<hr>": " ・SVGTextクラスの座標の0の位置はテキストの下部からスタートします。そのためもしもy=0を指定した場合、テキストはほとんど見えない状態になります。<hr>",  # noqa
     ##################################################
     "**[Examples]**": "**[コードサンプル]**",
     ##################################################
-    "```py\n>>> import apysc as ap\n>>> stage: ap.Stage = ap.Stage(\n...     background_color=ap.Color(\"#333\"),\n...     stage_width=200,\n...     stage_height=50,\n... )\n>>> svg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n...     text_spans=[\n...         ap.SvgTextSpan(text=\"Hello, \"),\n...         ap.SvgTextSpan(text=\"Hello, \", font_size=14),\n...     ],\n...     font_size=20,\n...     fill_color=ap.Color(\"#0af\"),\n... )\n```": "```py\n>>> import apysc as ap\n>>> stage: ap.Stage = ap.Stage(\n...     background_color=ap.Color(\"#333\"),\n...     stage_width=200,\n...     stage_height=50,\n... )\n>>> svg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n...     text_spans=[\n...         ap.SvgTextSpan(text=\"Hello, \"),\n...         ap.SvgTextSpan(text=\"Hello, \", font_size=14),\n...     ],\n...     font_size=20,\n...     fill_color=ap.Color(\"#0af\"),\n... )\n```",  # noqa
+    '```py\n>>> import apysc as ap\n>>> stage: ap.Stage = ap.Stage(\n...     background_color=ap.Color("#333"),\n...     stage_width=200,\n...     stage_height=50,\n... )\n>>> svg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n...     text_spans=[\n...         ap.SvgTextSpan(text="Hello, "),\n...         ap.SvgTextSpan(text="Hello, ", font_size=14),\n...     ],\n...     font_size=20,\n...     fill_color=ap.Color("#0af"),\n... )\n```': '```py\n>>> import apysc as ap\n>>> stage: ap.Stage = ap.Stage(\n...     background_color=ap.Color("#333"),\n...     stage_width=200,\n...     stage_height=50,\n... )\n>>> svg_text: ap.SvgText = ap.SvgText.create_with_svg_text_spans(\n...     text_spans=[\n...         ap.SvgTextSpan(text="Hello, "),\n...         ap.SvgTextSpan(text="Hello, ", font_size=14),\n...     ],\n...     font_size=20,\n...     fill_color=ap.Color("#0af"),\n... )\n```',  # noqa
     ##################################################
     "<hr>": "<hr>",
     ##################################################
     "**[References]**": "**[関連資料]**",
     ##################################################
     "- [SvgText class](https://simon-ritchie.github.io/apysc/en/svg_text.html)": "- [SvgText クラス](https://simon-ritchie.github.io/apysc/jp/jp_svg_text.html)",  # noqa
 }
```

### Comparing `apysc-4.3.0/apysc/_translation/jp/text_align.py` & `apysc-4.3.2/apysc/_translation/jp/text_align.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/text_align_last.py` & `apysc-4.3.2/apysc/_translation/jp/text_align_last.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/text_bold.py` & `apysc-4.3.2/apysc/_translation/jp/text_bold.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/text_fill_alpha.py` & `apysc-4.3.2/apysc/_translation/jp/text_fill_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/text_fill_color.py` & `apysc-4.3.2/apysc/_translation/jp/text_fill_color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/text_font_size.py` & `apysc-4.3.2/apysc/_translation/jp/text_font_size.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/text_italic.py` & `apysc-4.3.2/apysc/_translation/jp/text_italic.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/text_line_height.py` & `apysc-4.3.2/apysc/_translation/jp/text_line_height.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/text_underline.py` & `apysc-4.3.2/apysc/_translation/jp/text_underline.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/timedelta.py` & `apysc-4.3.2/apysc/_translation/jp/timedelta.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/timedelta_days.py` & `apysc-4.3.2/apysc/_translation/jp/timedelta_days.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/timedelta_total_seconds.py` & `apysc-4.3.2/apysc/_translation/jp/timedelta_total_seconds.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/timer.py` & `apysc-4.3.2/apysc/_translation/jp/timer.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/timer_complete.py` & `apysc-4.3.2/apysc/_translation/jp/timer_complete.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/timer_delay.py` & `apysc-4.3.2/apysc/_translation/jp/timer_delay.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/timer_event.py` & `apysc-4.3.2/apysc/_translation/jp/timer_event.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/timer_repeat_count.py` & `apysc-4.3.2/apysc/_translation/jp/timer_repeat_count.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/timer_reset.py` & `apysc-4.3.2/apysc/_translation/jp/timer_reset.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/timer_start_and_stop.py` & `apysc-4.3.2/apysc/_translation/jp/timer_start_and_stop.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/to_string.py` & `apysc-4.3.2/apysc/_translation/jp/to_string.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/trace.py` & `apysc-4.3.2/apysc/_translation/jp/trace.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/triangle.py` & `apysc-4.3.2/apysc/_translation/jp/triangle.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/true_and_false.py` & `apysc-4.3.2/apysc/_translation/jp/true_and_false.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/unbind_enter_frame_and_unbind_enter_frame_all.py` & `apysc-4.3.2/apysc/_translation/jp/unbind_enter_frame_and_unbind_enter_frame_all.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/unset_debug_mode.py` & `apysc-4.3.2/apysc/_translation/jp/unset_debug_mode.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/variable_name_suffix.py` & `apysc-4.3.2/apysc/_translation/jp/variable_name_suffix.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/what_apysc_can_do.py` & `apysc-4.3.2/apysc/_translation/jp/what_apysc_can_do.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_translation/jp/why_apysc_doesnt_use_python_builtin_data_type.py` & `apysc-4.3.2/apysc/_translation/jp/why_apysc_doesnt_use_python_builtin_data_type.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/_delete.py` & `apysc-4.3.2/apysc/_type/_delete.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/_return.py` & `apysc-4.3.2/apysc/_type/_return.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/any_value.py` & `apysc-4.3.2/apysc/_type/any_value.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/array.py` & `apysc-4.3.2/apysc/_type/array.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/attr_linking_mixin.py` & `apysc-4.3.2/apysc/_type/attr_linking_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/attr_to_apysc_val_from_builtin_mixin.py` & `apysc-4.3.2/apysc/_type/attr_to_apysc_val_from_builtin_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/blank_object_mixin.py` & `apysc-4.3.2/apysc/_type/blank_object_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/bool_const_mixin.py` & `apysc-4.3.2/apysc/_type/bool_const_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/boolean.py` & `apysc-4.3.2/apysc/_type/boolean.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/copy_mixin.py` & `apysc-4.3.2/apysc/_type/copy_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/deleted_object_mixin.py` & `apysc-4.3.2/apysc/_type/deleted_object_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/dictionary.py` & `apysc-4.3.2/apysc/_type/dictionary.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/expression_string.py` & `apysc-4.3.2/apysc/_type/expression_string.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/false.py` & `apysc-4.3.2/apysc/_type/false.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/initial_substitution_exp_mixin.py` & `apysc-4.3.2/apysc/_type/initial_substitution_exp_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/initialize_locals_and_globals_mixin.py` & `apysc-4.3.2/apysc/_type/initialize_locals_and_globals_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/int.py` & `apysc-4.3.2/apysc/_type/int.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/number.py` & `apysc-4.3.2/apysc/_type/number.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/number_value_mixin.py` & `apysc-4.3.2/apysc/_type/number_value_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/py_builtin_iter_disabling_mixin.py` & `apysc-4.3.2/apysc/_type/py_builtin_iter_disabling_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/revert_interface.py` & `apysc-4.3.2/apysc/_type/revert_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/revert_mixin.py` & `apysc-4.3.2/apysc/_type/revert_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/string.py` & `apysc-4.3.2/apysc/_type/string.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/string_apply_max_num_of_decimal_places_mixin.py` & `apysc-4.3.2/apysc/_type/string_apply_max_num_of_decimal_places_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/string_length_mixin.py` & `apysc-4.3.2/apysc/_type/string_length_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/string_lower_mixin.py` & `apysc-4.3.2/apysc/_type/string_lower_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/string_lstrip_mixin.py` & `apysc-4.3.2/apysc/_type/string_lstrip_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/string_rstrip_mixin.py` & `apysc-4.3.2/apysc/_type/string_rstrip_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/string_slice_mixin.py` & `apysc-4.3.2/apysc/_type/string_slice_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/string_split_mixin.py` & `apysc-4.3.2/apysc/_type/string_split_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/string_strip_mixin.py` & `apysc-4.3.2/apysc/_type/string_strip_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/string_upper_mixin.py` & `apysc-4.3.2/apysc/_type/string_upper_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/string_zfill_mixin.py` & `apysc-4.3.2/apysc/_type/string_zfill_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/to_fixed_mixin.py` & `apysc-4.3.2/apysc/_type/to_fixed_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/to_hex_mixin.py` & `apysc-4.3.2/apysc/_type/to_hex_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/to_number_mixin.py` & `apysc-4.3.2/apysc/_type/to_number_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/to_string_mixin.py` & `apysc-4.3.2/apysc/_type/to_string_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/true.py` & `apysc-4.3.2/apysc/_type/true.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/type_util.py` & `apysc-4.3.2/apysc/_type/type_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/value_util.py` & `apysc-4.3.2/apysc/_type/value_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/variable_name_mixin.py` & `apysc-4.3.2/apysc/_type/variable_name_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/variable_name_suffix_attr_or_var_mixin.py` & `apysc-4.3.2/apysc/_type/variable_name_suffix_attr_or_var_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/variable_name_suffix_mixin.py` & `apysc-4.3.2/apysc/_type/variable_name_suffix_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_type/variable_name_suffix_utils.py` & `apysc-4.3.2/apysc/_type/variable_name_suffix_utils.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_validation/arg_validation_decos.py` & `apysc-4.3.2/apysc/_validation/arg_validation_decos.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_validation/bool_validation.py` & `apysc-4.3.2/apysc/_validation/bool_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_validation/color_validation.py` & `apysc-4.3.2/apysc/_validation/color_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_validation/display_validation.py` & `apysc-4.3.2/apysc/_validation/display_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_validation/event_validation.py` & `apysc-4.3.2/apysc/_validation/event_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_validation/geom_validation.py` & `apysc-4.3.2/apysc/_validation/geom_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_validation/handler_validation.py` & `apysc-4.3.2/apysc/_validation/handler_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_validation/matrix_data_validation.py` & `apysc-4.3.2/apysc/_validation/matrix_data_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_validation/number_validation.py` & `apysc-4.3.2/apysc/_validation/number_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_validation/parent_validation.py` & `apysc-4.3.2/apysc/_validation/parent_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_validation/path_validation.py` & `apysc-4.3.2/apysc/_validation/path_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_validation/string_validation.py` & `apysc-4.3.2/apysc/_validation/string_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_validation/validation_common_utils.py` & `apysc-4.3.2/apysc/_validation/validation_common_utils.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc/_validation/variable_name_validation.py` & `apysc-4.3.2/apysc/_validation/variable_name_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.3.0/apysc.egg-info/PKG-INFO` & `apysc-4.3.2/apysc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apysc
-Version: 4.3.0
+Version: 4.3.2
 Summary: apysc is the Python's frontend library to create html and js file, that has the ActionScript 3 (as3)-like interface.
 Home-page: https://github.com/simon-ritchie/apysc
 Maintainer: simon-ritchie
 Maintainer-email: 
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

