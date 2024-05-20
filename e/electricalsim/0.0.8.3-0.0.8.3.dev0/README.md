# Comparing `tmp/electricalsim-0.0.8.3.tar.gz` & `tmp/electricalsim-0.0.8.3.dev0.tar.gz`

## Comparing `electricalsim-0.0.8.3.tar` & `electricalsim-0.0.8.3.dev0.tar`

### file list

```diff
@@ -1,154 +1,153 @@
--rw-r--r--   0        0        0    19579 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/README.md
--rw-r--r--   0        0        0    84223 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/img/10_PF4.png
--rw-r--r--   0        0        0    54206 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/img/11_PF_tooltips.png
--rw-r--r--   0        0        0    88072 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/img/12_App_settings.png
--rw-r--r--   0        0        0    65553 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/img/13_Disabling_nodes.png
--rw-r--r--   0        0        0   160217 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/img/14_Context_menu.png
--rw-r--r--   0        0        0    67750 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/img/14_Context_menu.svg
--rw-r--r--   0        0        0    10969 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/img/15_Extension_manager.png
--rw-r--r--   0        0        0   131148 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/img/1_Main_Window.png
--rw-r--r--   0        0        0   127556 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/img/1_Main_Window_dark.png
--rw-r--r--   0        0        0   132253 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/img/2_Dialogs.png
--rw-r--r--   0        0        0    15081 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/img/3_Widgets.png
--rw-r--r--   0        0        0   136762 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/img/4_Pandapower_DataFrames.png
--rw-r--r--   0        0        0    19729 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/img/5_Connections_angle_b.png
--rw-r--r--   0        0        0    23817 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/img/5_Connections_curved_b.png
--rw-r--r--   0        0        0    24398 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/img/5_Connections_straight_b.png
--rw-r--r--   0        0        0    10719 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/img/6_Line_and_transformer_nodes.png
--rw-r--r--   0        0        0   136386 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/img/7_PF1.png
--rw-r--r--   0        0        0   144782 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/img/8_PF2.png
--rw-r--r--   0        0        0    83704 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/img/9_PF3.png
--rwxr-xr-x   0        0        0    51862 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/img/Logo_CIESE_2021 y UTN_Sta_Fe.png
--rw-r--r--   0        0        0    33067 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/img/app_icon.png
--rw-r--r--   0        0        0    26932 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/img/dialog_connecting_buses.png
--rw-r--r--   0        0        0    27944 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/img/fuzzy_search.png
--rw-r--r--   0        0        0    19069 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/img/fuzzy_search2.png
--rw-r--r--   0        0        0    38748 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/img/slice_connections.png
--rw-r--r--   0        0        0    24015 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/Electrical_Grid_Simulator.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/__init__.py
--rw-r--r--   0        0        0     4821 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/config.ini
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/egs_create_shortcut.py
--rwxr-xr-x   0        0        0       98 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/egs_run.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/version.py
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/__init__.py
--rw-r--r--   0        0        0     7186 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/constants.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/errors.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/pkg_info.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/base/__init__.py
--rw-r--r--   0        0        0    15244 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/base/commands.py
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/base/factory.py
--rw-r--r--   0        0        0   103716 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/base/graph.py
--rw-r--r--   0        0        0     8997 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/base/menu.py
--rw-r--r--   0        0        0    20595 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/base/model.py
--rw-r--r--   0        0        0    14716 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/base/node.py
--rw-r--r--   0        0        0    16289 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/base/port.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/custom_widgets/__init__.py
--rw-r--r--   0        0        0    11668 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/custom_widgets/nodes_palette.py
--rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/custom_widgets/nodes_tree.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/__init__.py
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/custom_widget_color_picker.py
--rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/custom_widget_file_paths.py
--rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/custom_widget_slider.py
--rw-r--r--   0        0        0     9193 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/custom_widget_value_edit.py
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/custom_widget_vectors.py
--rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/node_property_factory.py
--rw-r--r--   0        0        0    28341 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/node_property_widgets.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/prop_widgets_abstract.py
--rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/prop_widgets_base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/nodes/__init__.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/nodes/backdrop_node.py
--rw-r--r--   0        0        0    28399 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/nodes/base_node.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/nodes/base_node_circle.py
--rw-r--r--   0        0        0     5646 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/nodes/group_node.py
--rw-r--r--   0        0        0     4288 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/nodes/port_node.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/qgraphics/__init__.py
--rw-r--r--   0        0        0     6851 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/qgraphics/node_abstract.py
--rw-r--r--   0        0        0    10831 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/qgraphics/node_backdrop.py
--rw-r--r--   0        0        0    36334 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/qgraphics/node_base.py
--rw-r--r--   0        0        0    20676 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/qgraphics/node_circle.py
--rw-r--r--   0        0        0    12036 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/qgraphics/node_group.py
--rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/qgraphics/node_overlay_disabled.py
--rw-r--r--   0        0        0     7932 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/qgraphics/node_port_in.py
--rw-r--r--   0        0        0     7931 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/qgraphics/node_port_out.py
--rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/qgraphics/node_text_item.py
--rw-r--r--   0        0        0    23168 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/qgraphics/pipe.py
--rw-r--r--   0        0        0    10316 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/qgraphics/port.py
--rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/qgraphics/slicer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/widgets/__init__.py
--rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/widgets/actions.py
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/widgets/dialogs.py
--rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/widgets/node_graph.py
--rw-r--r--   0        0        0    13621 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/widgets/node_widgets.py
--rw-r--r--   0        0        0     5527 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/widgets/scene.py
--rw-r--r--   0        0        0    11148 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/widgets/tab_search.py
--rw-r--r--   0        0        0    56457 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/widgets/viewer.py
--rw-r--r--   0        0        0     6732 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/widgets/viewer_nav.py
--rw-r--r--   0        0        0    17542 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/widgets/icons/node_base.png
--rw-r--r--   0        0        0     6915 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/extensions/extension_classes.py
--rw-r--r--   0        0        0     8997 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/hotkeys/hotkey_functions.py
--rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/hotkeys/hotkeys.json
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/icons/3w-transformer.svg
--rwxr-xr-x   0        0        0    82539 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/icons/CIESE_UTN_Sta_Fe.png
--rw-r--r--   0        0        0    33031 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/icons/app_icon.ico
--rw-r--r--   0        0        0    33067 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/icons/app_icon.png
--rwxr-xr-x   0        0        0    14363 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/icons/app_icon.svg
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/icons/demand.svg
--rw-r--r--   0        0        0     4380 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/icons/ext_grid.svg
--rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/icons/generator.svg
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/icons/icon_resources.qrc
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/icons/impedance.svg
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/icons/motor.svg
--rw-r--r--   0        0        0    80786 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/icons/rc_icons.py
--rw-r--r--   0        0        0    10748 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/icons/shunt.svg
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/icons/storage.svg
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/icons/switch_closed.svg
--rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/icons/switch_opened.svg
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/icons/transformer.svg
--rw-r--r--   0        0        0    16217 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/icons/ward.svg
--rw-r--r--   0        0        0    18881 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/icons/xward.svg
--rw-r--r--   0        0        0    31947 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/lib/auxiliary.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/lib/calculations.py
--rw-r--r--   0        0        0   234290 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/lib/electricalGraph.py
--rw-r--r--   0        0        0    87146 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/lib/main_components.py
--rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/lib/table_widget.py
--rw-r--r--   0        0        0    11797 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/about_dialog.ui
--rw-r--r--   0        0        0    17328 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/aload_dialog.ui
--rw-r--r--   0        0        0    17419 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/asgen_dialog.ui
--rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/bus_dialog.ui
--rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/choose_bus_switch.ui
--rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/choose_generator_type.ui
--rw-r--r--   0        0        0     4964 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/choose_line_type.ui
--rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/choose_load_type.ui
--rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/choose_transformer_type.ui
--rw-r--r--   0        0        0     8047 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/connecting_buses_dialog.ui
--rw-r--r--   0        0        0    23084 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/dcline_dialog.ui
--rw-r--r--   0        0        0   152121 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/dialogs.py
--rw-r--r--   0        0        0    35106 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/ext_grid_dialog.ui
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/extension.ui
--rw-r--r--   0        0        0    33034 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/gen_dialog.ui
--rw-r--r--   0        0        0    16772 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/impedance_dialog.ui
--rw-r--r--   0        0        0    31104 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/line_dialog.ui
--rw-r--r--   0        0        0    25616 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/load_dialog.ui
--rw-r--r--   0        0        0    12940 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/main_window.ui
--rw-r--r--   0        0        0    23184 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/motor_dialog.ui
--rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/network_settings_dialog.ui
--rw-r--r--   0        0        0    34604 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/pf_settings_widget.ui
--rw-r--r--   0        0        0    50076 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/power_flow_dialog.ui
--rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/search_node_dialog.ui
--rw-r--r--   0        0        0    14082 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/settings_dialog.ui
--rw-r--r--   0        0        0    38654 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/sgen_dialog.ui
--rw-r--r--   0        0        0    11331 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/shunt_dialog.ui
--rw-r--r--   0        0        0    10554 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/stdline_dialog.ui
--rw-r--r--   0        0        0    10807 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/stdtransformer3w_dialog.ui
--rw-r--r--   0        0        0    30234 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/stdtransformer_dialog.ui
--rw-r--r--   0        0        0    26339 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/storage_dialog.ui
--rw-r--r--   0        0        0     8989 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/switch_dialog.ui
--rw-r--r--   0        0        0    65860 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/transformer3w_dialog.ui
--rw-r--r--   0        0        0    56751 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/transformer_dialog.ui
--rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/ward_dialog.ui
--rw-r--r--   0        0        0    15494 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/src/electricalsim/ui/xward_dialog.ui
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/LICENSE
--rw-r--r--   0        0        0     5788 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/README_PyPI.md
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/pyproject.toml
--rw-r--r--   0        0        0     7062 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3/PKG-INFO
+-rw-r--r--   0        0        0    19579 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/README.md
+-rw-r--r--   0        0        0    84223 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/img/10_PF4.png
+-rw-r--r--   0        0        0    54206 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/img/11_PF_tooltips.png
+-rw-r--r--   0        0        0    88072 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/img/12_App_settings.png
+-rw-r--r--   0        0        0    65553 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/img/13_Disabling_nodes.png
+-rw-r--r--   0        0        0   160217 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/img/14_Context_menu.png
+-rw-r--r--   0        0        0    67750 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/img/14_Context_menu.svg
+-rw-r--r--   0        0        0    10969 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/img/15_Extension_manager.png
+-rw-r--r--   0        0        0   131148 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/img/1_Main_Window.png
+-rw-r--r--   0        0        0   127556 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/img/1_Main_Window_dark.png
+-rw-r--r--   0        0        0   132253 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/img/2_Dialogs.png
+-rw-r--r--   0        0        0    15081 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/img/3_Widgets.png
+-rw-r--r--   0        0        0   136762 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/img/4_Pandapower_DataFrames.png
+-rw-r--r--   0        0        0    19729 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/img/5_Connections_angle_b.png
+-rw-r--r--   0        0        0    23817 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/img/5_Connections_curved_b.png
+-rw-r--r--   0        0        0    24398 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/img/5_Connections_straight_b.png
+-rw-r--r--   0        0        0    10719 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/img/6_Line_and_transformer_nodes.png
+-rw-r--r--   0        0        0   136386 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/img/7_PF1.png
+-rw-r--r--   0        0        0   144782 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/img/8_PF2.png
+-rw-r--r--   0        0        0    83704 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/img/9_PF3.png
+-rwxr-xr-x   0        0        0    51862 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/img/Logo_CIESE_2021 y UTN_Sta_Fe.png
+-rw-r--r--   0        0        0    33067 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/img/app_icon.png
+-rw-r--r--   0        0        0    26932 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/img/dialog_connecting_buses.png
+-rw-r--r--   0        0        0    27944 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/img/fuzzy_search.png
+-rw-r--r--   0        0        0    19069 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/img/fuzzy_search2.png
+-rw-r--r--   0        0        0    38748 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/img/slice_connections.png
+-rw-r--r--   0        0        0    23988 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/Electrical_Grid_Simulator.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/__init__.py
+-rw-r--r--   0        0        0     4821 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/config.ini
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/egs_create_shortcut.py
+-rwxr-xr-x   0        0        0       98 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/egs_run.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/version.py
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/__init__.py
+-rw-r--r--   0        0        0     7186 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/constants.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/errors.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/pkg_info.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/base/__init__.py
+-rw-r--r--   0        0        0    15244 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/base/commands.py
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/base/factory.py
+-rw-r--r--   0        0        0   103716 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/base/graph.py
+-rw-r--r--   0        0        0     8997 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/base/menu.py
+-rw-r--r--   0        0        0    20595 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/base/model.py
+-rw-r--r--   0        0        0    14716 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/base/node.py
+-rw-r--r--   0        0        0    16289 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/base/port.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/custom_widgets/__init__.py
+-rw-r--r--   0        0        0    11668 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/custom_widgets/nodes_palette.py
+-rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/custom_widgets/nodes_tree.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/__init__.py
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/custom_widget_color_picker.py
+-rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/custom_widget_file_paths.py
+-rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/custom_widget_slider.py
+-rw-r--r--   0        0        0     9193 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/custom_widget_value_edit.py
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/custom_widget_vectors.py
+-rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/node_property_factory.py
+-rw-r--r--   0        0        0    28341 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/node_property_widgets.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/prop_widgets_abstract.py
+-rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/prop_widgets_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/nodes/__init__.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/nodes/backdrop_node.py
+-rw-r--r--   0        0        0    28399 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/nodes/base_node.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/nodes/base_node_circle.py
+-rw-r--r--   0        0        0     5646 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/nodes/group_node.py
+-rw-r--r--   0        0        0     4288 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/nodes/port_node.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/qgraphics/__init__.py
+-rw-r--r--   0        0        0     6851 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/qgraphics/node_abstract.py
+-rw-r--r--   0        0        0    10831 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/qgraphics/node_backdrop.py
+-rw-r--r--   0        0        0    36334 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/qgraphics/node_base.py
+-rw-r--r--   0        0        0    20676 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/qgraphics/node_circle.py
+-rw-r--r--   0        0        0    12036 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/qgraphics/node_group.py
+-rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/qgraphics/node_overlay_disabled.py
+-rw-r--r--   0        0        0     7932 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/qgraphics/node_port_in.py
+-rw-r--r--   0        0        0     7931 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/qgraphics/node_port_out.py
+-rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/qgraphics/node_text_item.py
+-rw-r--r--   0        0        0    23168 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/qgraphics/pipe.py
+-rw-r--r--   0        0        0    10316 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/qgraphics/port.py
+-rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/qgraphics/slicer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/widgets/__init__.py
+-rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/widgets/actions.py
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/widgets/dialogs.py
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/widgets/node_graph.py
+-rw-r--r--   0        0        0    13621 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/widgets/node_widgets.py
+-rw-r--r--   0        0        0     5527 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/widgets/scene.py
+-rw-r--r--   0        0        0    11148 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/widgets/tab_search.py
+-rw-r--r--   0        0        0    56457 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/widgets/viewer.py
+-rw-r--r--   0        0        0     6732 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/widgets/viewer_nav.py
+-rw-r--r--   0        0        0    17542 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/widgets/icons/node_base.png
+-rw-r--r--   0        0        0     6915 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/extensions/extension_classes.py
+-rw-r--r--   0        0        0     8997 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/hotkeys/hotkey_functions.py
+-rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/hotkeys/hotkeys.json
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/icons/3w-transformer.svg
+-rwxr-xr-x   0        0        0    82539 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/icons/CIESE_UTN_Sta_Fe.png
+-rw-r--r--   0        0        0    33031 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/icons/app_icon.ico
+-rw-r--r--   0        0        0    33067 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/icons/app_icon.png
+-rwxr-xr-x   0        0        0    14363 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/icons/app_icon.svg
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/icons/demand.svg
+-rw-r--r--   0        0        0     4380 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/icons/ext_grid.svg
+-rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/icons/generator.svg
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/icons/impedance.png
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/icons/impedance.svg
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/icons/motor.svg
+-rw-r--r--   0        0        0    10748 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/icons/shunt.svg
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/icons/storage.svg
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/icons/switch_closed.svg
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/icons/switch_opened.svg
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/icons/transformer.svg
+-rw-r--r--   0        0        0    16217 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/icons/ward.svg
+-rw-r--r--   0        0        0    18881 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/icons/xward.svg
+-rw-r--r--   0        0        0    31947 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/lib/auxiliary.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/lib/calculations.py
+-rw-r--r--   0        0        0   233770 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/lib/electricalGraph.py
+-rw-r--r--   0        0        0    86926 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/lib/main_components.py
+-rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/lib/table_widget.py
+-rw-r--r--   0        0        0    11797 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/about_dialog.ui
+-rw-r--r--   0        0        0    17328 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/aload_dialog.ui
+-rw-r--r--   0        0        0    17419 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/asgen_dialog.ui
+-rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/bus_dialog.ui
+-rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/choose_bus_switch.ui
+-rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/choose_generator_type.ui
+-rw-r--r--   0        0        0     4964 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/choose_line_type.ui
+-rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/choose_load_type.ui
+-rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/choose_transformer_type.ui
+-rw-r--r--   0        0        0     8047 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/connecting_buses_dialog.ui
+-rw-r--r--   0        0        0    23084 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/dcline_dialog.ui
+-rw-r--r--   0        0        0   152121 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/dialogs.py
+-rw-r--r--   0        0        0    35106 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/ext_grid_dialog.ui
+-rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/extension.ui
+-rw-r--r--   0        0        0    33034 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/gen_dialog.ui
+-rw-r--r--   0        0        0    16772 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/impedance_dialog.ui
+-rw-r--r--   0        0        0    31104 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/line_dialog.ui
+-rw-r--r--   0        0        0    25616 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/load_dialog.ui
+-rw-r--r--   0        0        0    12940 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/main_window.ui
+-rw-r--r--   0        0        0    23184 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/motor_dialog.ui
+-rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/network_settings_dialog.ui
+-rw-r--r--   0        0        0    34604 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/pf_settings_widget.ui
+-rw-r--r--   0        0        0    50076 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/power_flow_dialog.ui
+-rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/search_node_dialog.ui
+-rw-r--r--   0        0        0    14082 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/settings_dialog.ui
+-rw-r--r--   0        0        0    38654 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/sgen_dialog.ui
+-rw-r--r--   0        0        0    11331 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/shunt_dialog.ui
+-rw-r--r--   0        0        0    10554 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/stdline_dialog.ui
+-rw-r--r--   0        0        0    10807 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/stdtransformer3w_dialog.ui
+-rw-r--r--   0        0        0    30234 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/stdtransformer_dialog.ui
+-rw-r--r--   0        0        0    26339 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/storage_dialog.ui
+-rw-r--r--   0        0        0     8989 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/switch_dialog.ui
+-rw-r--r--   0        0        0    65860 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/transformer3w_dialog.ui
+-rw-r--r--   0        0        0    56751 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/transformer_dialog.ui
+-rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/ward_dialog.ui
+-rw-r--r--   0        0        0    15494 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/src/electricalsim/ui/xward_dialog.ui
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/LICENSE
+-rw-r--r--   0        0        0     5788 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/README_PyPI.md
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/pyproject.toml
+-rw-r--r--   0        0        0     7067 2020-02-02 00:00:00.000000 electricalsim-0.0.8.3.dev0/PKG-INFO
```

### Comparing `electricalsim-0.0.8.3/README.md` & `electricalsim-0.0.8.3.dev0/README.md`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/img/10_PF4.png` & `electricalsim-0.0.8.3.dev0/img/10_PF4.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/img/11_PF_tooltips.png` & `electricalsim-0.0.8.3.dev0/img/11_PF_tooltips.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/img/12_App_settings.png` & `electricalsim-0.0.8.3.dev0/img/12_App_settings.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/img/13_Disabling_nodes.png` & `electricalsim-0.0.8.3.dev0/img/13_Disabling_nodes.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/img/14_Context_menu.png` & `electricalsim-0.0.8.3.dev0/img/14_Context_menu.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/img/14_Context_menu.svg` & `electricalsim-0.0.8.3.dev0/img/14_Context_menu.svg`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/img/15_Extension_manager.png` & `electricalsim-0.0.8.3.dev0/img/15_Extension_manager.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/img/1_Main_Window.png` & `electricalsim-0.0.8.3.dev0/img/1_Main_Window.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/img/1_Main_Window_dark.png` & `electricalsim-0.0.8.3.dev0/img/1_Main_Window_dark.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/img/2_Dialogs.png` & `electricalsim-0.0.8.3.dev0/img/2_Dialogs.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/img/3_Widgets.png` & `electricalsim-0.0.8.3.dev0/img/3_Widgets.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/img/4_Pandapower_DataFrames.png` & `electricalsim-0.0.8.3.dev0/img/4_Pandapower_DataFrames.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/img/5_Connections_angle_b.png` & `electricalsim-0.0.8.3.dev0/img/5_Connections_angle_b.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/img/5_Connections_curved_b.png` & `electricalsim-0.0.8.3.dev0/img/5_Connections_curved_b.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/img/5_Connections_straight_b.png` & `electricalsim-0.0.8.3.dev0/img/5_Connections_straight_b.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/img/6_Line_and_transformer_nodes.png` & `electricalsim-0.0.8.3.dev0/img/6_Line_and_transformer_nodes.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/img/7_PF1.png` & `electricalsim-0.0.8.3.dev0/img/7_PF1.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/img/8_PF2.png` & `electricalsim-0.0.8.3.dev0/img/8_PF2.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/img/9_PF3.png` & `electricalsim-0.0.8.3.dev0/img/9_PF3.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/img/Logo_CIESE_2021 y UTN_Sta_Fe.png` & `electricalsim-0.0.8.3.dev0/img/Logo_CIESE_2021 y UTN_Sta_Fe.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/img/app_icon.png` & `electricalsim-0.0.8.3.dev0/img/app_icon.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/img/dialog_connecting_buses.png` & `electricalsim-0.0.8.3.dev0/img/dialog_connecting_buses.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/img/fuzzy_search.png` & `electricalsim-0.0.8.3.dev0/img/fuzzy_search.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/img/fuzzy_search2.png` & `electricalsim-0.0.8.3.dev0/img/fuzzy_search2.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/img/slice_connections.png` & `electricalsim-0.0.8.3.dev0/img/slice_connections.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/Electrical_Grid_Simulator.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/Electrical_Grid_Simulator.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 import qdarktheme  # Always import after Qt
 import qtawesome as qta
 
 from lib.electricalGraph import ElectricalGraph
 from lib.table_widget import TableWidgetWithMenu
 from lib.auxiliary import QVLine, QMainWindow2, return_config
 from lib.calculations import Run_PF
-from icons import rc_icons
 
 if sys.version_info < (3, 10):
     from importlib_metadata import entry_points
 else:
     from importlib.metadata import entry_points
```

### Comparing `electricalsim-0.0.8.3/src/electricalsim/config.ini` & `electricalsim-0.0.8.3.dev0/src/electricalsim/config.ini`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/egs_create_shortcut.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/egs_create_shortcut.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/__init__.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/__init__.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/constants.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/constants.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/base/commands.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/base/commands.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/base/factory.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/base/factory.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/base/graph.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/base/graph.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/base/menu.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/base/menu.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/base/model.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/base/model.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/base/node.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/base/node.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/base/port.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/base/port.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/custom_widgets/nodes_palette.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/custom_widgets/nodes_palette.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/custom_widgets/nodes_tree.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/custom_widgets/nodes_tree.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/custom_widget_color_picker.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/custom_widget_color_picker.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/custom_widget_file_paths.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/custom_widget_file_paths.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/custom_widget_slider.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/custom_widget_slider.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/custom_widget_value_edit.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/custom_widget_value_edit.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/custom_widget_vectors.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/custom_widget_vectors.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/node_property_factory.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/node_property_factory.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/node_property_widgets.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/node_property_widgets.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/prop_widgets_abstract.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/prop_widgets_abstract.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/prop_widgets_base.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/custom_widgets/properties_bin/prop_widgets_base.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/nodes/backdrop_node.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/nodes/backdrop_node.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/nodes/base_node.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/nodes/base_node_circle.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/nodes/base_node_circle.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/nodes/group_node.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/nodes/group_node.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/nodes/port_node.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/nodes/port_node.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/qgraphics/node_abstract.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/qgraphics/node_abstract.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/qgraphics/node_backdrop.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/qgraphics/node_backdrop.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/qgraphics/node_base.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/qgraphics/node_base.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/qgraphics/node_circle.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/qgraphics/node_circle.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/qgraphics/node_group.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/qgraphics/node_group.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/qgraphics/node_overlay_disabled.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/qgraphics/node_overlay_disabled.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/qgraphics/node_port_in.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/qgraphics/node_port_in.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/qgraphics/node_port_out.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/qgraphics/node_port_out.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/qgraphics/node_text_item.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/qgraphics/node_text_item.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/qgraphics/pipe.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/qgraphics/pipe.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/qgraphics/port.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/qgraphics/port.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/qgraphics/slicer.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/qgraphics/slicer.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/widgets/actions.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/widgets/actions.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/widgets/dialogs.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/widgets/dialogs.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/widgets/node_graph.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/widgets/node_graph.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/widgets/node_widgets.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/widgets/node_widgets.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/widgets/scene.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/widgets/scene.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/widgets/tab_search.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/widgets/tab_search.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/widgets/viewer.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/widgets/viewer.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/widgets/viewer_nav.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/widgets/viewer_nav.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/NodeGraphQt6/widgets/icons/node_base.png` & `electricalsim-0.0.8.3.dev0/src/electricalsim/NodeGraphQt6/widgets/icons/node_base.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/extensions/extension_classes.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/extensions/extension_classes.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/hotkeys/hotkey_functions.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/hotkeys/hotkey_functions.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/hotkeys/hotkeys.json` & `electricalsim-0.0.8.3.dev0/src/electricalsim/hotkeys/hotkeys.json`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/icons/3w-transformer.svg` & `electricalsim-0.0.8.3.dev0/src/electricalsim/icons/3w-transformer.svg`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/icons/CIESE_UTN_Sta_Fe.png` & `electricalsim-0.0.8.3.dev0/src/electricalsim/icons/CIESE_UTN_Sta_Fe.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/icons/app_icon.ico` & `electricalsim-0.0.8.3.dev0/src/electricalsim/icons/app_icon.ico`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/icons/app_icon.png` & `electricalsim-0.0.8.3.dev0/src/electricalsim/icons/app_icon.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/icons/app_icon.svg` & `electricalsim-0.0.8.3.dev0/src/electricalsim/icons/app_icon.svg`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/icons/demand.svg` & `electricalsim-0.0.8.3.dev0/src/electricalsim/icons/demand.svg`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/icons/ext_grid.svg` & `electricalsim-0.0.8.3.dev0/src/electricalsim/icons/ext_grid.svg`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/icons/generator.svg` & `electricalsim-0.0.8.3.dev0/src/electricalsim/icons/generator.svg`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/icons/impedance.svg` & `electricalsim-0.0.8.3.dev0/src/electricalsim/icons/impedance.svg`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/icons/motor.svg` & `electricalsim-0.0.8.3.dev0/src/electricalsim/icons/motor.svg`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/icons/shunt.svg` & `electricalsim-0.0.8.3.dev0/src/electricalsim/icons/shunt.svg`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/icons/storage.svg` & `electricalsim-0.0.8.3.dev0/src/electricalsim/icons/storage.svg`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/icons/switch_closed.svg` & `electricalsim-0.0.8.3.dev0/src/electricalsim/icons/switch_closed.svg`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/icons/switch_opened.svg` & `electricalsim-0.0.8.3.dev0/src/electricalsim/icons/switch_opened.svg`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/icons/transformer.svg` & `electricalsim-0.0.8.3.dev0/src/electricalsim/icons/transformer.svg`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/icons/ward.svg` & `electricalsim-0.0.8.3.dev0/src/electricalsim/icons/ward.svg`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/icons/xward.svg` & `electricalsim-0.0.8.3.dev0/src/electricalsim/icons/xward.svg`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/lib/auxiliary.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/lib/auxiliary.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/lib/electricalGraph.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/lib/electricalGraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -3169,18 +3169,16 @@
             node.set_property('min_q_mvar', np.round(dialog.min_q_mvar.value(), 5), push_undo=False)
             node.set_property('max_vm_pu', np.round(dialog.max_vm_pu.value(), 5), push_undo=False)
             node.set_property('min_vm_pu', np.round(dialog.min_vm_pu.value(), 5), push_undo=False)
             node.set_property('controllable', dialog.controllable.isChecked(), push_undo=False)
 
             node.p_mw_widget.get_custom_widget().setMinimum(node.get_property('min_p_mw'))
             node.p_mw_widget.get_custom_widget().setMaximum(node.get_property('max_p_mw'))
-            node.p_mw_widget.get_custom_widget().setValue(node.get_property('p_mw'))
             node.vm_pu_widget.get_custom_widget().setMinimum(node.get_property('min_vm_pu'))
             node.vm_pu_widget.get_custom_widget().setMaximum(node.get_property('max_vm_pu'))
-            node.vm_pu_widget.get_custom_widget().setValue(node.get_property('vm_pu'))
 
             gen_index = node.get_property('gen_index')
             if gen_index is not None and node.connected_to_network():
                 for name in node.electrical_properties:
                     self.net.gen.loc[gen_index, name] = node.get_property(name)
 
             self.session_change_warning()
@@ -3299,18 +3297,16 @@
             node.set_property('min_q_mvar', np.round(dialog.min_q_mvar.value(), 5), push_undo=False)
 
             node.set_property('controllable', dialog.controllable.isChecked(), push_undo=False)
             node.set_property('current_source', dialog.current_source.isChecked(), push_undo=False)
 
             node.p_mw_widget.get_custom_widget().setMinimum(node.get_property('min_p_mw'))
             node.p_mw_widget.get_custom_widget().setMaximum(node.get_property('max_p_mw'))
-            node.p_mw_widget.get_custom_widget().setValue(node.get_property('p_mw'))
             node.q_mvar_widget.get_custom_widget().setMinimum(node.get_property('min_q_mvar'))
             node.q_mvar_widget.get_custom_widget().setMaximum(node.get_property('max_q_mvar'))
-            node.q_mvar_widget.get_custom_widget().setValue(node.get_property('q_mvar'))
 
             gen_index = node.get_property('gen_index')
             if gen_index is not None and node.connected_to_network():
                 for name in node.electrical_properties:
                     self.net.sgen.loc[gen_index, name] = node.get_property(name)
 
             self.session_change_warning()
@@ -3508,18 +3504,16 @@
             node.set_property('max_q_mvar', np.round(dialog.max_q_mvar.value(), 5), push_undo=False)
             node.set_property('min_q_mvar', np.round(dialog.min_q_mvar.value(), 5), push_undo=False)
 
             node.set_property('controllable', dialog.controllable.isChecked(), push_undo=False)
 
             node.p_mw_widget.get_custom_widget().setMinimum(node.get_property('min_p_mw'))
             node.p_mw_widget.get_custom_widget().setMaximum(node.get_property('max_p_mw'))
-            node.p_mw_widget.get_custom_widget().setValue(node.get_property('p_mw'))
             node.q_mvar_widget.get_custom_widget().setMinimum(node.get_property('min_q_mvar'))
             node.q_mvar_widget.get_custom_widget().setMaximum(node.get_property('max_q_mvar'))
-            node.q_mvar_widget.get_custom_widget().setValue(node.get_property('q_mvar'))
 
             load_index = node.get_property('load_index')
             if load_index is not None and node.connected_to_network():
                 for name in node.electrical_properties:
                     self.net.load.loc[load_index, name] = node.get_property(name)
 
             self.session_change_warning()
```

### Comparing `electricalsim-0.0.8.3/src/electricalsim/lib/main_components.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/lib/main_components.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,17 +405,16 @@
         Add an image to the node.
         
         image_name: Image file name from de 'icons' folder.
         """
     
         self.image_widget = ImageWrapper(self.view)
         self.image_widget.set_name('image')
-        # icon_path = os.path.join(icons_dir, image_name)
-        # style = f"image: url('{icon_path}');"
-        style = "image: url(:/" + image_name + ");"
+        icon_path = os.path.join(icons_dir, image_name)
+        style = f"image: url('{icon_path}');"
         self.image_widget.set_value(style)
         self.add_custom_widget(self.image_widget, tab=None)
         model = self.model
         self.set_model(model)
 
 
 class BusNode(BaseNode2):
@@ -610,15 +609,15 @@
         self.electrical_properties = ('rft_pu', 'xft_pu', 'sn_mva', 'rtf_pu',
                                       'xtf_pu', 'rft0_pu', 'xft0_pu',
                                       'rtf0_pu', 'xtf0_pu')
         for name in self.electrical_properties:
             self.create_property(name, None)
             
         self.create_property('impedance_index', None)
-        self.add_image('impedance.svg')
+        self.add_image('impedance.png')
             
     def connected_to_network(self):
         """
         Returns True if the impedance node is connected to the network (to buses).
         Returns False otherwise.
         """
         inputs_connected = len(self.connected_input_nodes()[self.input_port])
@@ -1381,17 +1380,16 @@
         # self.image_widget.set_value(pixmap)
         # self.add_custom_widget(self.image_widget, tab=None)
         # model = self.model
         # self.set_model(model)
         
         self.image_widget = ImageWrapper(self.view)
         self.image_widget.set_name('image')
-        # icon_path = os.path.join(icons_dir, 'demand.svg')
-        # style = f"image: url('{icon_path}')"
-        style = "image: url(:/demand.svg);"
+        icon_path = os.path.join(icons_dir, 'demand.svg')
+        style = f"image: url('{icon_path}')"
         self.image_widget.set_value(style)
         self.add_custom_widget(self.image_widget, tab=None)
         model = self.model
         self.set_model(model)
                 
         # add custom widget to node with "node.view" as the parent.
         self.p_mw_widget = QSpinBoxWrapper(self.view, widget_type=QtWidgets.QDoubleSpinBox())
@@ -2003,22 +2001,20 @@
         """
         index = self.get_property('switch_index')
         new_value = self.get_property('closed')
         if index in self.graph.net.switch.index:
             self.graph.net.switch.loc[index, 'closed'] = new_value
         if new_value:
             self.set_color(0, 0, 255)
-            # icon_path = os.path.join(icons_dir, 'switch_closed.svg')
-            style = "image: url(:/switch_closed.svg);"
+            icon_path = os.path.join(icons_dir, 'switch_closed.svg')
         else:
             self.set_color(178, 199, 218)
-            # icon_path = os.path.join(icons_dir, 'switch_opened.svg')
-            style = "image: url(:/switch_opened.svg);"
+            icon_path = os.path.join(icons_dir, 'switch_opened.svg')
             
-        # style = f"image: url('{icon_path}')"
+        style = f"image: url('{icon_path}')"
         self.image_widget.set_value(style)
             
     def connected_to_network(self):
         """
         Returns True if the switch node is connected to the network.
         Returns False otherwise.
         """
```

### Comparing `electricalsim-0.0.8.3/src/electricalsim/lib/table_widget.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/lib/table_widget.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/about_dialog.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/about_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/aload_dialog.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/aload_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/asgen_dialog.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/asgen_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/bus_dialog.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/bus_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/choose_bus_switch.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/choose_bus_switch.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/choose_generator_type.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/choose_generator_type.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/choose_line_type.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/choose_line_type.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/choose_load_type.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/choose_load_type.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/choose_transformer_type.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/choose_transformer_type.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/connecting_buses_dialog.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/connecting_buses_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/dcline_dialog.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/dcline_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/dialogs.py` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/ext_grid_dialog.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/ext_grid_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/extension.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/extension.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/gen_dialog.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/gen_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/impedance_dialog.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/impedance_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/line_dialog.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/line_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/load_dialog.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/load_dialog.ui`

 * *Files 0% similar despite different names*

#### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/load_dialog.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/load_dialog.ui`

```diff
@@ -127,15 +127,15 @@
                       <property name="minimum">
                         <double>0.000100000000000</double>
                       </property>
                       <property name="maximum">
                         <double>100.000000000000000</double>
                       </property>
                       <property name="singleStep">
-                        <double>1.000000000000000</double>
+                        <double>0.010000000000000</double>
                       </property>
                       <property name="value">
                         <double>13.199999999999999</double>
                       </property>
                     </widget>
                   </item>
                 </layout>
```

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/main_window.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/main_window.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/motor_dialog.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/motor_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/network_settings_dialog.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/network_settings_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/pf_settings_widget.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/pf_settings_widget.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/power_flow_dialog.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/power_flow_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/search_node_dialog.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/search_node_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/settings_dialog.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/settings_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/sgen_dialog.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/sgen_dialog.ui`

 * *Files 0% similar despite different names*

#### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/sgen_dialog.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/sgen_dialog.ui`

```diff
@@ -127,15 +127,15 @@
                       <property name="minimum">
                         <double>0.000100000000000</double>
                       </property>
                       <property name="maximum">
                         <double>100.000000000000000</double>
                       </property>
                       <property name="singleStep">
-                        <double>1.000000000000000</double>
+                        <double>0.010000000000000</double>
                       </property>
                       <property name="value">
                         <double>13.199999999999999</double>
                       </property>
                     </widget>
                   </item>
                 </layout>
```

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/shunt_dialog.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/shunt_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/stdline_dialog.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/stdline_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/stdtransformer3w_dialog.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/stdtransformer3w_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/stdtransformer_dialog.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/stdtransformer_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/storage_dialog.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/storage_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/switch_dialog.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/switch_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/transformer3w_dialog.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/transformer3w_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/transformer_dialog.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/transformer_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/ward_dialog.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/ward_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/src/electricalsim/ui/xward_dialog.ui` & `electricalsim-0.0.8.3.dev0/src/electricalsim/ui/xward_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/LICENSE` & `electricalsim-0.0.8.3.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/README_PyPI.md` & `electricalsim-0.0.8.3.dev0/README_PyPI.md`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.8.3/pyproject.toml` & `electricalsim-0.0.8.3.dev0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "electricalsim"
-version = "0.0.8.3"
+version = "0.0.8.3-dev"
 author = "Dr. Ing. Ariel S. Loyarte"
 authors = [
   { name="Dr. Ing. Ariel S. Loyarte", email="aloyarte@frsf.utn.edu.ar" },
 ]
 description = "Graphical user interface for simulating electrical networks based on the pandapower library"
 readme = "README_PyPI.md"
 requires-python = ">=3.8,<3.12"
```

### Comparing `electricalsim-0.0.8.3/PKG-INFO` & `electricalsim-0.0.8.3.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: electricalsim
-Version: 0.0.8.3
+Version: 0.0.8.3.dev0
 Summary: Graphical user interface for simulating electrical networks based on the pandapower library
 Project-URL: Homepage, https://github.com/aloytag/electrical-grid-simulator
 Project-URL: Bug Tracker, https://github.com/aloytag/electrical-grid-simulator/issues
 Project-URL: Repository, https://github.com/aloytag/electrical-grid-simulator
 Author-email: "Dr. Ing. Ariel S. Loyarte" <aloyarte@frsf.utn.edu.ar>
 License: MIT
 License-File: LICENSE
```

