# Comparing `tmp/badger-opt-1.0_1.tar.gz` & `tmp/badger_opt-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "badger-opt-1.0.tar", last modified: Tue Dec 12 04:38:59 2023, max compression
+gzip compressed data, was "badger_opt-1.0.2.tar", last modified: Mon May 20 18:23:46 2024, max compression
```

## Comparing `badger-opt-1.0_1.tar` & `badger_opt-1.0.2.tar`

### file list

```diff
@@ -1,166 +1,168 @@
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-12-12 04:38:59.358988 badger-opt-1.0/
--rw-r--r--   0 zhezhang (1762935258) 1704612529    35149 2023-11-06 22:02:45.000000 badger-opt-1.0/LICENSE
--rw-r--r--   0 zhezhang (1762935258) 1704612529      240 2023-12-12 03:35:16.000000 badger-opt-1.0/MANIFEST.in
--rw-r--r--   0 zhezhang (1762935258) 1704612529      620 2023-12-12 04:38:59.358801 badger-opt-1.0/PKG-INFO
--rw-r--r--   0 zhezhang (1762935258) 1704612529     5370 2023-12-08 21:14:51.000000 badger-opt-1.0/README.md
--rw-r--r--   0 zhezhang (1762935258) 1704612529      174 2023-12-12 04:38:59.359618 badger-opt-1.0/setup.cfg
--rw-r--r--   0 zhezhang (1762935258) 1704612529      938 2023-12-05 17:00:15.000000 badger-opt-1.0/setup.py
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-12-12 04:38:59.227712 badger-opt-1.0/src/
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-12-12 04:38:59.360556 badger-opt-1.0/src/badger/
--rw-r--r--   0 zhezhang (1762935258) 1704612529       72 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/__init__.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     5349 2023-12-06 18:20:14.000000 badger-opt-1.0/src/badger/__main__.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      495 2023-12-12 04:38:59.360659 badger-opt-1.0/src/badger/_version.py
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-12-12 04:38:59.256037 badger-opt-1.0/src/badger/actions/
--rw-r--r--   0 zhezhang (1762935258) 1704612529     1269 2023-12-11 23:16:34.000000 badger-opt-1.0/src/badger/actions/__init__.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     3559 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/actions/config.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     2430 2023-12-08 21:16:42.000000 badger-opt-1.0/src/badger/actions/doctor.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      685 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/actions/env.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      640 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/actions/generator.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     4759 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/actions/install.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      603 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/actions/intf.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     1401 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/actions/routine.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     4836 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/actions/run.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     1101 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/actions/uninstall.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     3896 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/archive.py
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-12-12 04:38:59.223889 badger-opt-1.0/src/badger/built_in_plugins/
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-12-12 04:38:59.223685 badger-opt-1.0/src/badger/built_in_plugins/environments/
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-12-12 04:38:59.259332 badger-opt-1.0/src/badger/built_in_plugins/environments/sphere_2d/
--rw-r--r--   0 zhezhang (1762935258) 1704612529       68 2023-12-08 08:30:51.000000 badger-opt-1.0/src/badger/built_in_plugins/environments/sphere_2d/README.md
--rw-r--r--   0 zhezhang (1762935258) 1704612529      870 2023-12-08 08:30:23.000000 badger-opt-1.0/src/badger/built_in_plugins/environments/sphere_2d/__init__.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      106 2023-12-08 08:30:48.000000 badger-opt-1.0/src/badger/built_in_plugins/environments/sphere_2d/configs.yaml
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-12-12 04:38:59.224023 badger-opt-1.0/src/badger/built_in_plugins/interfaces/
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-12-12 04:38:59.263104 badger-opt-1.0/src/badger/built_in_plugins/interfaces/default/
--rw-r--r--   0 zhezhang (1762935258) 1704612529       59 2023-12-08 08:27:18.000000 badger-opt-1.0/src/badger/built_in_plugins/interfaces/default/README.md
--rw-r--r--   0 zhezhang (1762935258) 1704612529      753 2023-12-08 08:28:30.000000 badger-opt-1.0/src/badger/built_in_plugins/interfaces/default/__init__.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529       62 2023-12-08 08:27:18.000000 badger-opt-1.0/src/badger/built_in_plugins/interfaces/default/configs.yaml
--rw-r--r--   0 zhezhang (1762935258) 1704612529     5400 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/core.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     9074 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/db.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     8786 2023-12-06 18:46:44.000000 badger-opt-1.0/src/badger/environment.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      943 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/errors.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      616 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/extension.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     6270 2023-12-05 18:43:47.000000 badger-opt-1.0/src/badger/factory.py
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-12-12 04:38:59.264193 badger-opt-1.0/src/badger/gui/
--rw-r--r--   0 zhezhang (1762935258) 1704612529        0 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/gui/__init__.py
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-12-12 04:38:59.265674 badger-opt-1.0/src/badger/gui/default/
--rw-r--r--   0 zhezhang (1762935258) 1704612529     2492 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/gui/default/__init__.py
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-12-12 04:38:59.292906 badger-opt-1.0/src/badger/gui/default/components/
--rw-r--r--   0 zhezhang (1762935258) 1704612529        0 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/gui/default/components/__init__.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     1602 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/gui/default/components/analysis_extensions.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     4648 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/gui/default/components/collapsible_box.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     1917 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/gui/default/components/constraint_item.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     5469 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/gui/default/components/data_table.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     2787 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/gui/default/components/eliding_label.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529    11842 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/gui/default/components/env_cbox.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     3704 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/gui/default/components/extensions_palette.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     2164 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/gui/default/components/filter_cbox.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     4522 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/gui/default/components/generator_cbox.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     5250 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/gui/default/components/history_navigator.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      589 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/gui/default/components/labeled_lineedit.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     5785 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/gui/default/components/obj_table.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     2421 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/gui/default/components/reorderable_table.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     1267 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/gui/default/components/robust_spinbox.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     3160 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/gui/default/components/routine_editor.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     4966 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/gui/default/components/routine_item.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529    24950 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/gui/default/components/routine_page.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     5028 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/gui/default/components/routine_runner.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529    38188 2023-12-08 21:31:29.000000 badger-opt-1.0/src/badger/gui/default/components/run_monitor.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      232 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/gui/default/components/search_bar.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      949 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/gui/default/components/state_item.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     1444 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/gui/default/components/status_bar.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     7164 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/gui/default/components/syntax.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     6667 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/gui/default/components/var_table.py
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-12-12 04:38:59.317593 badger-opt-1.0/src/badger/gui/default/images/
--rw-r--r--   0 zhezhang (1762935258) 1704612529    10986 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/gui/default/images/add.png
--rw-r--r--   0 zhezhang (1762935258) 1704612529    12456 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/gui/default/images/book-alt.png
--rw-r--r--   0 zhezhang (1762935258) 1704612529    11898 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/gui/default/images/book.png
--rw-r--r--   0 zhezhang (1762935258) 1704612529    19762 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/gui/default/images/crosshairs.png
--rw-r--r--   0 zhezhang (1762935258) 1704612529    13286 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/gui/default/images/export.png
--rw-r--r--   0 zhezhang (1762935258) 1704612529    16864 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/gui/default/images/extension-alt.png
--rw-r--r--   0 zhezhang (1762935258) 1704612529    14882 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/gui/default/images/extension.png
--rw-r--r--   0 zhezhang (1762935258) 1704612529    18562 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/gui/default/images/gear.png
--rw-r--r--   0 zhezhang (1762935258) 1704612529    46055 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/gui/default/images/icon.png
--rw-r--r--   0 zhezhang (1762935258) 1704612529    13127 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/gui/default/images/import.png
--rw-r--r--   0 zhezhang (1762935258) 1704612529    12838 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/gui/default/images/info.png
--rw-r--r--   0 zhezhang (1762935258) 1704612529     9713 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/gui/default/images/next.png
--rw-r--r--   0 zhezhang (1762935258) 1704612529    11997 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/gui/default/images/pause.png
--rw-r--r--   0 zhezhang (1762935258) 1704612529    11462 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/gui/default/images/play.png
--rw-r--r--   0 zhezhang (1762935258) 1704612529     9899 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/gui/default/images/previous.png
--rw-r--r--   0 zhezhang (1762935258) 1704612529    12675 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/gui/default/images/set.png
--rw-r--r--   0 zhezhang (1762935258) 1704612529    15884 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/gui/default/images/star.png
--rw-r--r--   0 zhezhang (1762935258) 1704612529     8425 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/gui/default/images/stop.png
--rw-r--r--   0 zhezhang (1762935258) 1704612529    22102 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/gui/default/images/tools.png
--rw-r--r--   0 zhezhang (1762935258) 1704612529    14125 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/gui/default/images/trash.png
--rw-r--r--   0 zhezhang (1762935258) 1704612529    18309 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/gui/default/images/undo.png
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-12-12 04:38:59.319556 badger-opt-1.0/src/badger/gui/default/pages/
--rw-r--r--   0 zhezhang (1762935258) 1704612529        0 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/gui/default/pages/__init__.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529    20558 2023-12-08 19:50:58.000000 badger-opt-1.0/src/badger/gui/default/pages/home_page.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     1291 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/gui/default/utils.py
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-12-12 04:38:59.327821 badger-opt-1.0/src/badger/gui/default/windows/
--rw-r--r--   0 zhezhang (1762935258) 1704612529        0 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/gui/default/windows/__init__.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     1808 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/gui/default/windows/docs_window.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     1961 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/gui/default/windows/edit_script_dialog.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     4716 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/gui/default/windows/lim_vrange_dialog.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     2132 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/gui/default/windows/main_window.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      833 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/gui/default/windows/review_dialog.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     6353 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/gui/default/windows/settings_dialog.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     5216 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/gui/default/windows/terminition_condition_dialog.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     3495 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/gui/default/windows/var_dialog.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     2624 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/interface.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      999 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/log.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     4314 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/logbook.py
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-12-12 04:38:59.330541 badger-opt-1.0/src/badger/logger/
--rw-r--r--   0 zhezhang (1762935258) 1704612529     4437 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/logger/__init__.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      259 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/logger/event.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      937 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/logger/observer.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     1616 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/logger/util.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     4752 2023-12-06 18:45:58.000000 badger-opt-1.0/src/badger/routine.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     5231 2023-12-08 19:11:43.000000 badger-opt-1.0/src/badger/settings.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      606 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/stats.py
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-12-12 04:38:59.345208 badger-opt-1.0/src/badger/tests/
--rw-r--r--   0 zhezhang (1762935258) 1704612529        0 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/tests/__init__.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     2094 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/tests/conftest.py
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-12-12 04:38:59.226243 badger-opt-1.0/src/badger/tests/mock/
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-12-12 04:38:59.345872 badger-opt-1.0/src/badger/tests/mock/configs/
--rw-r--r--   0 zhezhang (1762935258) 1704612529       43 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/tests/mock/configs/test.yaml
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-12-12 04:38:59.346556 badger-opt-1.0/src/badger/tests/mock/plugins/
--rw-r--r--   0 zhezhang (1762935258) 1704612529        0 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/tests/mock/plugins/__init__.py
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-12-12 04:38:59.227057 badger-opt-1.0/src/badger/tests/mock/plugins/environments/
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-12-12 04:38:59.348212 badger-opt-1.0/src/badger/tests/mock/plugins/environments/multiobjective_test/
--rw-r--r--   0 zhezhang (1762935258) 1704612529       82 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/tests/mock/plugins/environments/multiobjective_test/README.md
--rw-r--r--   0 zhezhang (1762935258) 1704612529      789 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/tests/mock/plugins/environments/multiobjective_test/__init__.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      109 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/tests/mock/plugins/environments/multiobjective_test/configs.yaml
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-12-12 04:38:59.350401 badger-opt-1.0/src/badger/tests/mock/plugins/environments/test/
--rw-r--r--   0 zhezhang (1762935258) 1704612529       82 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/tests/mock/plugins/environments/test/README.md
--rw-r--r--   0 zhezhang (1762935258) 1704612529      765 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/tests/mock/plugins/environments/test/__init__.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      109 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/tests/mock/plugins/environments/test/configs.yaml
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-12-12 04:38:59.227463 badger-opt-1.0/src/badger/tests/mock/plugins/interfaces/
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-12-12 04:38:59.352667 badger-opt-1.0/src/badger/tests/mock/plugins/interfaces/test/
--rw-r--r--   0 zhezhang (1762935258) 1704612529       56 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/tests/mock/plugins/interfaces/test/README.md
--rw-r--r--   0 zhezhang (1762935258) 1704612529      773 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/tests/mock/plugins/interfaces/test/__init__.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529       59 2023-11-06 22:02:45.000000 badger-opt-1.0/src/badger/tests/mock/plugins/interfaces/test/configs.yaml
--rw-r--r--   0 zhezhang (1762935258) 1704612529     1633 2023-12-11 23:31:58.000000 badger-opt-1.0/src/badger/tests/test_cli_basic.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     4416 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/tests/test_core.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      330 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/tests/test_data_viewer_extension.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      778 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/tests/test_db.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     4683 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/tests/test_env.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     2508 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/tests/test_environment.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     1358 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/tests/test_factory.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     1286 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/tests/test_gui_basic.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     1042 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/tests/test_home_page.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     3638 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/tests/test_intf.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     2253 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/tests/test_lib_basic.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     1549 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/tests/test_routine.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      471 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/tests/test_routine_editor.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     2747 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/tests/test_routine_page.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529      482 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/tests/test_routine_runner.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529    12791 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/tests/test_run_monitor.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     3775 2023-12-05 17:00:15.000000 badger-opt-1.0/src/badger/tests/utils.py
--rw-r--r--   0 zhezhang (1762935258) 1704612529     7662 2023-12-08 18:40:48.000000 badger-opt-1.0/src/badger/utils.py
-drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2023-12-12 04:38:59.357452 badger-opt-1.0/src/badger_opt.egg-info/
--rw-r--r--   0 zhezhang (1762935258) 1704612529      620 2023-12-12 04:38:59.000000 badger-opt-1.0/src/badger_opt.egg-info/PKG-INFO
--rw-r--r--   0 zhezhang (1762935258) 1704612529     5471 2023-12-12 04:38:59.000000 badger-opt-1.0/src/badger_opt.egg-info/SOURCES.txt
--rw-r--r--   0 zhezhang (1762935258) 1704612529        1 2023-12-12 04:38:59.000000 badger-opt-1.0/src/badger_opt.egg-info/dependency_links.txt
--rw-r--r--   0 zhezhang (1762935258) 1704612529       48 2023-12-12 04:38:59.000000 badger-opt-1.0/src/badger_opt.egg-info/entry_points.txt
--rw-r--r--   0 zhezhang (1762935258) 1704612529      112 2023-12-12 04:38:59.000000 badger-opt-1.0/src/badger_opt.egg-info/requires.txt
--rw-r--r--   0 zhezhang (1762935258) 1704612529        7 2023-12-12 04:38:59.000000 badger-opt-1.0/src/badger_opt.egg-info/top_level.txt
--rw-r--r--   0 zhezhang (1762935258) 1704612529    80044 2023-11-06 22:02:45.000000 badger-opt-1.0/versioneer.py
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2024-05-20 18:23:46.106402 badger_opt-1.0.2/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529    35149 2023-11-06 22:02:45.000000 badger_opt-1.0.2/LICENSE
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      240 2023-12-12 19:51:09.000000 badger_opt-1.0.2/MANIFEST.in
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      622 2024-05-20 18:23:46.106226 badger_opt-1.0.2/PKG-INFO
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     5368 2024-04-22 20:47:04.000000 badger_opt-1.0.2/README.md
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      174 2024-05-20 18:23:46.106943 badger_opt-1.0.2/setup.cfg
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      938 2023-12-12 19:27:52.000000 badger_opt-1.0.2/setup.py
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2024-05-20 18:23:45.972227 badger_opt-1.0.2/src/
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2024-05-20 18:23:46.107697 badger_opt-1.0.2/src/badger/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529       72 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/__init__.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     5349 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/__main__.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      497 2024-05-20 18:23:46.107877 badger_opt-1.0.2/src/badger/_version.py
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2024-05-20 18:23:45.998874 badger_opt-1.0.2/src/badger/actions/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     1269 2023-12-12 19:51:09.000000 badger_opt-1.0.2/src/badger/actions/__init__.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     3559 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/actions/config.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     2430 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/actions/doctor.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      685 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/actions/env.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      640 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/actions/generator.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     4759 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/actions/install.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      603 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/actions/intf.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     1401 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/actions/routine.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     4836 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/actions/run.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     1101 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/actions/uninstall.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     4509 2024-04-22 20:47:04.000000 badger_opt-1.0.2/src/badger/archive.py
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2024-05-20 18:23:45.966821 badger_opt-1.0.2/src/badger/built_in_plugins/
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2024-05-20 18:23:45.966488 badger_opt-1.0.2/src/badger/built_in_plugins/environments/
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2024-05-20 18:23:46.000801 badger_opt-1.0.2/src/badger/built_in_plugins/environments/sphere_2d/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529       68 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/built_in_plugins/environments/sphere_2d/README.md
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      870 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/built_in_plugins/environments/sphere_2d/__init__.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      106 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/built_in_plugins/environments/sphere_2d/configs.yaml
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2024-05-20 18:23:45.967323 badger_opt-1.0.2/src/badger/built_in_plugins/interfaces/
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2024-05-20 18:23:46.003082 badger_opt-1.0.2/src/badger/built_in_plugins/interfaces/default/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529       59 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/built_in_plugins/interfaces/default/README.md
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      753 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/built_in_plugins/interfaces/default/__init__.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529       62 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/built_in_plugins/interfaces/default/configs.yaml
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     5462 2024-05-20 18:21:05.000000 badger_opt-1.0.2/src/badger/core.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     9461 2024-05-20 18:21:05.000000 badger_opt-1.0.2/src/badger/db.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     8786 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/environment.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      943 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/errors.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      616 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/extension.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     6331 2024-04-26 15:48:01.000000 badger_opt-1.0.2/src/badger/factory.py
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2024-05-20 18:23:46.003724 badger_opt-1.0.2/src/badger/gui/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529        0 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/gui/__init__.py
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2024-05-20 18:23:46.005570 badger_opt-1.0.2/src/badger/gui/default/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     2492 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/gui/default/__init__.py
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2024-05-20 18:23:46.032381 badger_opt-1.0.2/src/badger/gui/default/components/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529        0 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/gui/default/components/__init__.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     1602 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/gui/default/components/analysis_extensions.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     4648 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/gui/default/components/collapsible_box.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     1917 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/gui/default/components/constraint_item.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     5469 2024-04-10 23:34:26.000000 badger_opt-1.0.2/src/badger/gui/default/components/data_table.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     3437 2024-04-30 08:20:51.000000 badger_opt-1.0.2/src/badger/gui/default/components/eliding_label.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529    12157 2024-04-22 20:59:30.000000 badger_opt-1.0.2/src/badger/gui/default/components/env_cbox.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     3704 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/gui/default/components/extensions_palette.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     2164 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/gui/default/components/filter_cbox.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     4674 2024-04-22 20:59:55.000000 badger_opt-1.0.2/src/badger/gui/default/components/generator_cbox.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     5927 2024-04-22 20:47:04.000000 badger_opt-1.0.2/src/badger/gui/default/components/history_navigator.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      589 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/gui/default/components/labeled_lineedit.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     5785 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/gui/default/components/obj_table.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     2421 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/gui/default/components/reorderable_table.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     1267 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/gui/default/components/robust_spinbox.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     3189 2024-04-22 20:47:04.000000 badger_opt-1.0.2/src/badger/gui/default/components/routine_editor.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     4966 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/gui/default/components/routine_item.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529    29065 2024-04-22 20:47:04.000000 badger_opt-1.0.2/src/badger/gui/default/components/routine_page.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     5466 2024-05-20 18:21:05.000000 badger_opt-1.0.2/src/badger/gui/default/components/routine_runner.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529    39503 2024-05-20 18:21:05.000000 badger_opt-1.0.2/src/badger/gui/default/components/run_monitor.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      232 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/gui/default/components/search_bar.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      949 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/gui/default/components/state_item.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     1497 2024-04-30 08:26:52.000000 badger_opt-1.0.2/src/badger/gui/default/components/status_bar.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     7164 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/gui/default/components/syntax.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     6667 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/gui/default/components/var_table.py
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2024-05-20 18:23:46.055083 badger_opt-1.0.2/src/badger/gui/default/images/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529    10986 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/gui/default/images/add.png
+-rw-r--r--   0 zhezhang (1762935258) 1704612529    12456 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/gui/default/images/book-alt.png
+-rw-r--r--   0 zhezhang (1762935258) 1704612529    11898 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/gui/default/images/book.png
+-rw-r--r--   0 zhezhang (1762935258) 1704612529    19762 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/gui/default/images/crosshairs.png
+-rw-r--r--   0 zhezhang (1762935258) 1704612529    13286 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/gui/default/images/export.png
+-rw-r--r--   0 zhezhang (1762935258) 1704612529    16864 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/gui/default/images/extension-alt.png
+-rw-r--r--   0 zhezhang (1762935258) 1704612529    14882 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/gui/default/images/extension.png
+-rw-r--r--   0 zhezhang (1762935258) 1704612529    18562 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/gui/default/images/gear.png
+-rw-r--r--   0 zhezhang (1762935258) 1704612529    46055 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/gui/default/images/icon.png
+-rw-r--r--   0 zhezhang (1762935258) 1704612529    13127 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/gui/default/images/import.png
+-rw-r--r--   0 zhezhang (1762935258) 1704612529    12838 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/gui/default/images/info.png
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     9713 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/gui/default/images/next.png
+-rw-r--r--   0 zhezhang (1762935258) 1704612529    11997 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/gui/default/images/pause.png
+-rw-r--r--   0 zhezhang (1762935258) 1704612529    11462 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/gui/default/images/play.png
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     9899 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/gui/default/images/previous.png
+-rw-r--r--   0 zhezhang (1762935258) 1704612529    12675 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/gui/default/images/set.png
+-rw-r--r--   0 zhezhang (1762935258) 1704612529    15884 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/gui/default/images/star.png
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     8425 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/gui/default/images/stop.png
+-rw-r--r--   0 zhezhang (1762935258) 1704612529    22102 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/gui/default/images/tools.png
+-rw-r--r--   0 zhezhang (1762935258) 1704612529    14125 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/gui/default/images/trash.png
+-rw-r--r--   0 zhezhang (1762935258) 1704612529    18309 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/gui/default/images/undo.png
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2024-05-20 18:23:46.056595 badger_opt-1.0.2/src/badger/gui/default/pages/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529        0 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/gui/default/pages/__init__.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529    22381 2024-05-20 18:21:05.000000 badger_opt-1.0.2/src/badger/gui/default/pages/home_page.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     2663 2024-05-08 20:08:22.000000 badger_opt-1.0.2/src/badger/gui/default/utils.py
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2024-05-20 18:23:46.067018 badger_opt-1.0.2/src/badger/gui/default/windows/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529        0 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/gui/default/windows/__init__.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     4100 2024-04-10 18:51:05.000000 badger_opt-1.0.2/src/badger/gui/default/windows/add_random_dialog.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     1808 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/gui/default/windows/docs_window.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     1961 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/gui/default/windows/edit_script_dialog.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     4716 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/gui/default/windows/lim_vrange_dialog.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     2132 2024-05-20 18:21:05.000000 badger_opt-1.0.2/src/badger/gui/default/windows/main_window.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     2662 2024-04-22 20:47:04.000000 badger_opt-1.0.2/src/badger/gui/default/windows/message_dialog.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      833 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/gui/default/windows/review_dialog.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     6353 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/gui/default/windows/settings_dialog.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     5216 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/gui/default/windows/terminition_condition_dialog.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     3495 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/gui/default/windows/var_dialog.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     2624 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/interface.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      999 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/log.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     4531 2024-04-22 20:47:04.000000 badger_opt-1.0.2/src/badger/logbook.py
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2024-05-20 18:23:46.071344 badger_opt-1.0.2/src/badger/logger/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     4437 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/logger/__init__.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      259 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/logger/event.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      937 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/logger/observer.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     1616 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/logger/util.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     4978 2024-05-20 18:21:05.000000 badger_opt-1.0.2/src/badger/routine.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     5231 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/settings.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      606 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/stats.py
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2024-05-20 18:23:46.089875 badger_opt-1.0.2/src/badger/tests/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529        0 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/tests/__init__.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     2094 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/tests/conftest.py
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2024-05-20 18:23:45.970709 badger_opt-1.0.2/src/badger/tests/mock/
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2024-05-20 18:23:46.090913 badger_opt-1.0.2/src/badger/tests/mock/configs/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529       43 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/tests/mock/configs/test.yaml
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2024-05-20 18:23:46.091789 badger_opt-1.0.2/src/badger/tests/mock/plugins/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529        0 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/tests/mock/plugins/__init__.py
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2024-05-20 18:23:45.971400 badger_opt-1.0.2/src/badger/tests/mock/plugins/environments/
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2024-05-20 18:23:46.094656 badger_opt-1.0.2/src/badger/tests/mock/plugins/environments/multiobjective_test/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529       82 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/tests/mock/plugins/environments/multiobjective_test/README.md
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      789 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/tests/mock/plugins/environments/multiobjective_test/__init__.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      109 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/tests/mock/plugins/environments/multiobjective_test/configs.yaml
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2024-05-20 18:23:46.096919 badger_opt-1.0.2/src/badger/tests/mock/plugins/environments/test/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529       82 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/tests/mock/plugins/environments/test/README.md
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      765 2024-05-20 18:21:05.000000 badger_opt-1.0.2/src/badger/tests/mock/plugins/environments/test/__init__.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      109 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/tests/mock/plugins/environments/test/configs.yaml
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2024-05-20 18:23:45.971910 badger_opt-1.0.2/src/badger/tests/mock/plugins/interfaces/
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2024-05-20 18:23:46.099253 badger_opt-1.0.2/src/badger/tests/mock/plugins/interfaces/test/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529       56 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/tests/mock/plugins/interfaces/test/README.md
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      773 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/tests/mock/plugins/interfaces/test/__init__.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529       59 2023-11-06 22:02:45.000000 badger_opt-1.0.2/src/badger/tests/mock/plugins/interfaces/test/configs.yaml
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     1774 2024-04-22 20:47:04.000000 badger_opt-1.0.2/src/badger/tests/test_cli_basic.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     4416 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/tests/test_core.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      330 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/tests/test_data_viewer_extension.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      778 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/tests/test_db.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     4683 2024-05-20 18:21:05.000000 badger_opt-1.0.2/src/badger/tests/test_env.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     2508 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/tests/test_environment.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     1358 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/tests/test_factory.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     5844 2024-05-20 18:21:05.000000 badger_opt-1.0.2/src/badger/tests/test_gui_basic.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     1042 2024-05-20 18:21:05.000000 badger_opt-1.0.2/src/badger/tests/test_home_page.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     3638 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/tests/test_intf.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     2253 2023-12-12 19:27:52.000000 badger_opt-1.0.2/src/badger/tests/test_lib_basic.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     1549 2024-05-20 18:21:05.000000 badger_opt-1.0.2/src/badger/tests/test_routine.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      471 2024-05-20 18:21:05.000000 badger_opt-1.0.2/src/badger/tests/test_routine_editor.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     6507 2024-05-20 18:21:05.000000 badger_opt-1.0.2/src/badger/tests/test_routine_page.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     3124 2024-05-20 18:21:05.000000 badger_opt-1.0.2/src/badger/tests/test_routine_runner.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529    16091 2024-05-20 18:21:05.000000 badger_opt-1.0.2/src/badger/tests/test_run_monitor.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     6035 2024-04-22 20:47:04.000000 badger_opt-1.0.2/src/badger/tests/utils.py
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     7662 2024-04-16 23:06:20.000000 badger_opt-1.0.2/src/badger/utils.py
+drwxr-xr-x   0 zhezhang (1762935258) 1704612529        0 2024-05-20 18:23:46.104899 badger_opt-1.0.2/src/badger_opt.egg-info/
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      622 2024-05-20 18:23:45.000000 badger_opt-1.0.2/src/badger_opt.egg-info/PKG-INFO
+-rw-r--r--   0 zhezhang (1762935258) 1704612529     5572 2024-05-20 18:23:45.000000 badger_opt-1.0.2/src/badger_opt.egg-info/SOURCES.txt
+-rw-r--r--   0 zhezhang (1762935258) 1704612529        1 2024-05-20 18:23:45.000000 badger_opt-1.0.2/src/badger_opt.egg-info/dependency_links.txt
+-rw-r--r--   0 zhezhang (1762935258) 1704612529       48 2024-05-20 18:23:45.000000 badger_opt-1.0.2/src/badger_opt.egg-info/entry_points.txt
+-rw-r--r--   0 zhezhang (1762935258) 1704612529      112 2024-05-20 18:23:45.000000 badger_opt-1.0.2/src/badger_opt.egg-info/requires.txt
+-rw-r--r--   0 zhezhang (1762935258) 1704612529        7 2024-05-20 18:23:45.000000 badger_opt-1.0.2/src/badger_opt.egg-info/top_level.txt
+-rw-r--r--   0 zhezhang (1762935258) 1704612529    80044 2023-11-06 22:02:45.000000 badger_opt-1.0.2/versioneer.py
```

### Comparing `badger-opt-1.0/LICENSE` & `badger_opt-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/PKG-INFO` & `badger_opt-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badger-opt
-Version: 1.0
+Version: 1.0.2
 Summary: Core of the Badger optimizer
 Home-page: https://github.com/SLAC-ML/Badger
 Author: Zhe Zhang
 Author-email: zhezhang@slac.stanford.edu
 License: GPL
 Requires-Python: >=3.9
 License-File: LICENSE
```

### Comparing `badger-opt-1.0/README.md` & `badger_opt-1.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 <div align="center">
   <h1 align="center">
-    Badger: The Missing Optimizer in ACR
+    Badger: The Go-To Optimizer in ACR
     <br />
     <br />
-    <a href="https://slac-ml.github.io/Badger">
+    <a href="https://slaclab.github.io/Badger">
       <img src="pics/badger.png" alt="Badger" height=128>
     </a>
   </h1>
 </div>
 
 ![Badger main GUI](pics/main.png)
 
 <div align="center">
 
 | Documentation | Package | Downloads | Version | Platforms |
 | --- | --- | --- | --- | --- |
-| [![Documentation](https://img.shields.io/badge/Badger-documentation-blue.svg)](https://slac-ml.github.io/Badger/) | [![Conda Recipe](https://img.shields.io/badge/recipe-badger-opt.svg)](https://anaconda.org/conda-forge/badger-opt) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/badger-opt.svg)](https://anaconda.org/conda-forge/badger-opt) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/badger-opt.svg)](https://anaconda.org/conda-forge/badger-opt) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/badger-opt.svg)](https://anaconda.org/conda-forge/badger-opt) |
+| [![Documentation](https://img.shields.io/badge/Badger-documentation-blue.svg)](https://slaclab.github.io/Badger/) | [![Conda Recipe](https://img.shields.io/badge/recipe-badger-opt.svg)](https://anaconda.org/conda-forge/badger-opt) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/badger-opt.svg)](https://anaconda.org/conda-forge/badger-opt) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/badger-opt.svg)](https://anaconda.org/conda-forge/badger-opt) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/badger-opt.svg)](https://anaconda.org/conda-forge/badger-opt) |
 
 </div>
 
 ## Introduction
 
 Badger is an optimization interface tailored for the Accelerator Control Room (ACR)[^1]. It places a strong emphasis on extensibility, easily expandable through the plugin system, and flexibility, offering complete GUI, CLI, and API support.
 
@@ -35,15 +35,15 @@
 - **History Exploration:** Browse through past runs effortlessly.
 - **Optimal Solution Navigation:** Jump to or set optimal solutions.
 - **State Recovery:** Easily recover machine states after an optimization run.
 - **Constraint Support:** Accommodate both soft and hard constraints.
 - **Data Preservation:** Preserve all raw data for comprehensive analysis.
 - **Advanced Extensions:** Benefit from extensions for sophisticated optimization data analysis and visualization.
 
-For additional details about Badger and its capabilities, please refer to [Badger's online documentation](https://slac-ml.github.io/Badger/).
+For additional details about Badger and its capabilities, please refer to [Badger's online documentation](https://slaclab.github.io/Badger/).
 
 ## Installation
 
 Using `conda`
 
 ```shell
 conda install -c conda-forge badger-opt
@@ -61,15 +61,15 @@
 
 Once Badger is installed, launch the GUI by running the following command in the terminal:
 
 ```bash
 badger -g
 ```
 
-Then following [this simple GUI tutorial](https://slac-ml.github.io/Badger/docs/next/getting-started/tutorial_0) to run your first optimizaion in Badger within a couple of minutes!
+Then following [this simple GUI tutorial](https://slaclab.github.io/Badger/docs/next/getting-started/tutorial_0) to run your first optimizaion in Badger within a couple of minutes!
 
 ## Citation
 
 If you use Badger for your research, please consider adding the following citation to your publications.
 
 ```
 Zhang, Z., et al. "Badger: The missing optimizer in ACR",
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-                  ************ BBaaddggeerr:: TThhee MMiissssiinngg OOppttiimmiizzeerr iinn AACCRR
+                   ************ BBaaddggeerr:: TThhee GGoo--TToo OOppttiimmiizzeerr iinn AACCRR
 
                                 _[[_BB_aa_dd_gg_ee_rr_]] ************
 ![Badger main GUI](pics/main.png)
 | Documentation | Package | Downloads | Version | Platforms | | --- | --- | --
    - | --- | --- | | [![Documentation](https://img.shields.io/badge/Badger-
-documentation-blue.svg)](https://slac-ml.github.io/Badger/) | [![Conda Recipe]
+documentation-blue.svg)](https://slaclab.github.io/Badger/) | [![Conda Recipe]
   (https://img.shields.io/badge/recipe-badger-opt.svg)](https://anaconda.org/
 conda-forge/badger-opt) | [![Conda Downloads](https://img.shields.io/conda/dn/
 conda-forge/badger-opt.svg)](https://anaconda.org/conda-forge/badger-opt) | [!
  [Conda Version](https://img.shields.io/conda/vn/conda-forge/badger-opt.svg)]
  (https://anaconda.org/conda-forge/badger-opt) | [![Conda Platforms](https://
   img.shields.io/conda/pn/conda-forge/badger-opt.svg)](https://anaconda.org/
                            conda-forge/badger-opt) |
@@ -34,21 +34,21 @@
 ** Browse through past runs effortlessly. - **Optimal Solution Navigation:**
 Jump to or set optimal solutions. - **State Recovery:** Easily recover machine
 states after an optimization run. - **Constraint Support:** Accommodate both
 soft and hard constraints. - **Data Preservation:** Preserve all raw data for
 comprehensive analysis. - **Advanced Extensions:** Benefit from extensions for
 sophisticated optimization data analysis and visualization. For additional
 details about Badger and its capabilities, please refer to [Badger's online
-documentation](https://slac-ml.github.io/Badger/). ## Installation Using
+documentation](https://slaclab.github.io/Badger/). ## Installation Using
 `conda` ```shell conda install -c conda-forge badger-opt ``` or `pip` ```shell
 pip install badger-opt ``` Currently Badger only officially support Linux.
 Badger on MacOS and Windows could be potentially unstable. ## Run an
 optimization Once Badger is installed, launch the GUI by running the following
 command in the terminal: ```bash badger -g ``` Then following [this simple GUI
-tutorial](https://slac-ml.github.io/Badger/docs/next/getting-started/
+tutorial](https://slaclab.github.io/Badger/docs/next/getting-started/
 tutorial_0) to run your first optimizaion in Badger within a couple of minutes!
 ## Citation If you use Badger for your research, please consider adding the
 following citation to your publications. ``` Zhang, Z., et al. "Badger: The
 missing optimizer in ACR", in Proc. IPAC'22, Bangkok. doi:10.18429/JACoW-
 IPAC2022-TUPOST058 ``` BibTex entry: ```bibtex @inproceedings{Badger, author =
 {Z. Zhang and M. BÃ¶se and A.L. Edelen and J.R. Garrahan and Y. Hidaka and C.E.
 Mayes and S.A. Miskovich and D.F. Ratner and R.J. Roussel and J. Shtalenkova
```

### Comparing `badger-opt-1.0/setup.py` & `badger_opt-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/__main__.py` & `badger_opt-1.0.2/src/badger/__main__.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/actions/__init__.py` & `badger_opt-1.0.2/src/badger/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/actions/config.py` & `badger_opt-1.0.2/src/badger/actions/config.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/actions/doctor.py` & `badger_opt-1.0.2/src/badger/actions/doctor.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/actions/env.py` & `badger_opt-1.0.2/src/badger/actions/env.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/actions/generator.py` & `badger_opt-1.0.2/src/badger/actions/generator.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/actions/install.py` & `badger_opt-1.0.2/src/badger/actions/install.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/actions/intf.py` & `badger_opt-1.0.2/src/badger/actions/intf.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/actions/routine.py` & `badger_opt-1.0.2/src/badger/actions/routine.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/actions/run.py` & `badger_opt-1.0.2/src/badger/actions/run.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/actions/uninstall.py` & `badger_opt-1.0.2/src/badger/actions/uninstall.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/archive.py` & `badger_opt-1.0.2/src/badger/archive.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import warnings
 import logging
 logger = logging.getLogger(__name__)
 from .db import save_run, remove_run_by_filename
 from .utils import ts_float_to_str
 from .settings import read_value
 from .routine import Routine
 from .errors import BadgerConfigError
@@ -86,15 +87,25 @@
 
     filename = os.path.join(BADGER_ARCHIVE_ROOT,
                             first_level,
                             second_level,
                             third_level,
                             run_fname)
 
-    routine = Routine.from_file(filename)
+    # TODO: create utility function to catch warnings to remove code
+    # duplication
+    with warnings.catch_warnings(record=True) as caught_warnings:
+        routine = Routine.from_file(filename)
+
+        # Check if any user warnings were caught
+        for warning in caught_warnings:
+            if warning.category == UserWarning:
+                pass
+            else:
+                print(f"Caught user warning: {warning.message}")
 
     return routine
 
 
 def delete_run(run_fname):
     tokens = run_fname.split('-')
     first_level = tokens[1]
@@ -112,7 +123,16 @@
     try:
         os.remove(os.path.join(prefix, pickle_fname))
     except FileNotFoundError:
         pass
 
     # Remove the yaml data file
     os.remove(os.path.join(prefix, run_fname))
+
+
+def get_base_run_filename(run_filename):
+    if run_filename.endswith(' (failed to load)'):
+        base_name = run_filename[:-17]
+    else:
+        base_name = run_filename
+
+    return base_name
```

### Comparing `badger-opt-1.0/src/badger/built_in_plugins/environments/sphere_2d/__init__.py` & `badger_opt-1.0.2/src/badger/built_in_plugins/environments/sphere_2d/__init__.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/built_in_plugins/interfaces/default/__init__.py` & `badger_opt-1.0.2/src/badger/built_in_plugins/interfaces/default/__init__.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/core.py` & `badger_opt-1.0.2/src/badger/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,19 +26,22 @@
         else:
             break
 
 
 def convert_to_solution(result: DataFrame, routine: Routine):
     vocs = routine.vocs
     try:
-        best_idx, _ = vocs.select_best(routine.sorted_data, n=1)
-        if best_idx != len(routine.data) - 1:
+        best_idx, _, _ = vocs.select_best(routine.sorted_data, n=1)
+        if best_idx.size > 0:
+            if best_idx != len(routine.data) - 1:
+                is_optimal = False
+            else:
+                is_optimal = True
+        else:  # no feasible solution
             is_optimal = False
-        else:
-            is_optimal = True
     except NotImplementedError:
         is_optimal = False  # disable the optimal highlight for MO problems
 
     vars = list(result[vocs.variable_names].to_numpy()[0])
     objs = list(result[vocs.objective_names].to_numpy()[0])
     cons = list(result[vocs.constraint_names].to_numpy()[0])
     stas = list(result[vocs.observable_names].to_numpy()[0])
@@ -107,15 +110,14 @@
                      routine.vocs.constraint_names,
                      routine.vocs.observable_names)
     opt_logger.update(Events.OPTIMIZATION_START, solution_meta)
 
     # evaluate initial points:
     # Nikita: more care about the setting var logic,
     # wait or consider timeout/retry
-    # TODO: need to evaluate a single point at the time
     for _, ele in initial_points.iterrows():
         result = routine.evaluate_data(ele.to_dict())
         solution = convert_to_solution(result, routine)
         opt_logger.update(Events.OPTIMIZATION_STEP, solution)
         if evaluate_callback:
             evaluate_callback(result)
```

### Comparing `badger-opt-1.0/src/badger/db.py` & `badger_opt-1.0.2/src/badger/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import warnings
 from datetime import datetime
 import logging
 logger = logging.getLogger(__name__)
 import yaml
 import sqlite3
 from .routine import Routine
 from .settings import read_value
@@ -162,15 +163,25 @@
     records = cur.fetchall()
     con.close()
 
     if len(records) == 1:
         # return yaml.safe_load(records[0][1]), records[0][2]
         routine_dict = yaml.safe_load(records[0][1])
         # routine_dict['evaluator'] = None
-        return Routine(**routine_dict), records[0][2]
+        with warnings.catch_warnings(record=True) as caught_warnings:
+            routine = Routine(**routine_dict)
+
+            # Check if any user warnings were caught
+            for warning in caught_warnings:
+                if warning.category == UserWarning:
+                    pass
+                else:
+                    print(f"Caught user warning: {warning.message}")
+
+            return routine, records[0][2]
     elif len(records) == 0:
         # logger.warning(f'Routine {name} not found in the database!')
         return None, None
     else:
         raise BadgerDBError(
             f'Multiple routines with name {name} found in the database!')
```

### Comparing `badger-opt-1.0/src/badger/environment.py` & `badger_opt-1.0.2/src/badger/environment.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/errors.py` & `badger_opt-1.0.2/src/badger/errors.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/extension.py` & `badger_opt-1.0.2/src/badger/extension.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/factory.py` & `badger_opt-1.0.2/src/badger/factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,18 @@
 
 LOAD_LOCAL_ALGO = False
 ALGO_EXCLUDED = [
     'bayesian_exploration',
     'cnsga',
     'mggpo',
     'time_dependent_upper_confidence_bound',
-    'multi_fidelity'
+    'multi_fidelity',
+    'neldermead',
+    'mobo',
+    'upper_confidence_bound',
 ]
 
 # Check badger plugin root
 BADGER_PLUGIN_ROOT = read_value('BADGER_PLUGIN_ROOT')
 if BADGER_PLUGIN_ROOT is None:
     raise BadgerConfigError('Please set the BADGER_PLUGIN_ROOT env var!')
 elif not os.path.exists(BADGER_PLUGIN_ROOT):
```

### Comparing `badger-opt-1.0/src/badger/gui/default/__init__.py` & `badger_opt-1.0.2/src/badger/gui/default/__init__.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/components/analysis_extensions.py` & `badger_opt-1.0.2/src/badger/gui/default/components/analysis_extensions.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/components/collapsible_box.py` & `badger_opt-1.0.2/src/badger/gui/default/components/collapsible_box.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/components/constraint_item.py` & `badger_opt-1.0.2/src/badger/gui/default/components/constraint_item.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/components/data_table.py` & `badger_opt-1.0.2/src/badger/gui/default/components/data_table.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/components/eliding_label.py` & `badger_opt-1.0.2/src/badger/gui/default/components/eliding_label.py`

 * *Files 13% similar despite different names*

```diff
@@ -92,7 +92,27 @@
                 line.draw(painter, QtCore.QPoint(0, 0))
 
         text_layout.endLayout()
 
         if did_elide != self.is_elided:
             self.is_elided = did_elide
             self.elision_changed.emit(did_elide)
+
+
+class SimpleElidedLabel(QtWidgets.QLabel):
+    def __init__(self, text="", parent=None):
+        super(SimpleElidedLabel, self).__init__(parent)
+        self._text = text
+
+    def setText(self, text):
+        self._text = text
+        super(SimpleElidedLabel, self).setText(self.elidedText())
+
+    def resizeEvent(self, event):
+        super(SimpleElidedLabel, self).setText(self.elidedText())
+        super(SimpleElidedLabel, self).resizeEvent(event)
+
+    def elidedText(self):
+        metrics = QtGui.QFontMetrics(self.font())
+        elided = metrics.elidedText(
+            self._text, QtCore.Qt.ElideRight, self.width())
+        return elided
```

### Comparing `badger-opt-1.0/src/badger/gui/default/components/env_cbox.py` & `badger_opt-1.0.2/src/badger/gui/default/components/env_cbox.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from PyQt5.QtWidgets import QVBoxLayout, QHBoxLayout, QPushButton, QWidget, QPlainTextEdit, QLineEdit
 from PyQt5.QtWidgets import QComboBox, QCheckBox, QStyledItemDelegate, QLabel, QListWidget, QFrame
 from PyQt5.QtCore import QRegExp
+
 from .collapsible_box import CollapsibleBox
 from .var_table import VariableTable
 from .obj_table import ObjectiveTable
 from .data_table import init_data_table, update_init_data_table
+from ..utils import MouseWheelWidgetAdjustmentGuard, NoHoverFocusComboBox
 from ....settings import read_value
 from ....utils import strtobool
 
 LABEL_WIDTH = 80
 
 class BadgerEnvBox(CollapsibleBox):
     def __init__(self, parent=None, envs=[]):
@@ -23,18 +25,19 @@
         vbox = QVBoxLayout()
 
         name = QWidget()
         hbox_name = QHBoxLayout(name)
         hbox_name.setContentsMargins(0, 0, 0, 0)
         lbl = QLabel('Name')
         lbl.setFixedWidth(LABEL_WIDTH)
-        self.cb = cb = QComboBox()
+        self.cb = cb = NoHoverFocusComboBox()
         cb.setItemDelegate(QStyledItemDelegate())
         cb.addItems(self.envs)
         cb.setCurrentIndex(-1)
+        cb.installEventFilter(MouseWheelWidgetAdjustmentGuard(cb))
         self.btn_env_play = btn_env_play = QPushButton('Open Playground')
         btn_env_play.setFixedSize(128, 24)
         if not strtobool(read_value('BADGER_ENABLE_ADVANCED')):
             btn_env_play.hide()
         hbox_name.addWidget(lbl)
         hbox_name.addWidget(cb, 1)
         hbox_name.addWidget(btn_env_play)
@@ -120,19 +123,22 @@
         action_init = QWidget()
         hbox_action_init = QHBoxLayout(action_init)
         hbox_action_init.setContentsMargins(0, 0, 0, 0)
         self.btn_add_row = btn_add_row = QPushButton('Add Row')
         btn_add_row.setFixedSize(96, 24)
         self.btn_add_curr = btn_add_curr = QPushButton('Add Current')
         btn_add_curr.setFixedSize(96, 24)
+        self.btn_add_rand = btn_add_rand = QPushButton('Add Random')
+        btn_add_rand.setFixedSize(96, 24)
         self.btn_clear = btn_clear = QPushButton('Clear All')
         btn_clear.setFixedSize(96, 24)
         hbox_action_init.addWidget(btn_add_row)
         hbox_action_init.addStretch()
         hbox_action_init.addWidget(btn_add_curr)
+        hbox_action_init.addWidget(btn_add_rand)
         hbox_action_init.addWidget(btn_clear)
         vbox_init.addWidget(action_init)
         self.init_table = init_data_table()
         vbox_init.addWidget(self.init_table)
         cbox_init.setContentLayout(vbox_init)
         cbox_init.expand()
 
@@ -215,15 +221,15 @@
         sta_panel = QWidget()
         vbox_more.addWidget(sta_panel, 1)
         hbox_sta = QHBoxLayout(sta_panel)
         hbox_sta.setContentsMargins(0, 0, 0, 0)
         lbl_sta_col = QWidget()
         vbox_lbl_sta = QVBoxLayout(lbl_sta_col)
         vbox_lbl_sta.setContentsMargins(0, 0, 0, 0)
-        lbl_sta = QLabel('Constants')
+        lbl_sta = QLabel('Observables')
         lbl_sta.setFixedWidth(LABEL_WIDTH)
         vbox_lbl_sta.addWidget(lbl_sta)
         vbox_lbl_sta.addStretch(1)
         hbox_sta.addWidget(lbl_sta_col)
 
         edit_sta_col = QWidget()
         vbox_sta_edit = QVBoxLayout(edit_sta_col)
@@ -233,19 +239,19 @@
         hbox_action_sta.setContentsMargins(0, 0, 0, 0)
         vbox_sta_edit.addWidget(action_sta)
         self.btn_add_sta = btn_add_sta = QPushButton('Add')
         btn_add_sta.setFixedSize(96, 24)
         btn_add_sta.setDisabled(True)
         hbox_action_sta.addWidget(btn_add_sta)
         hbox_action_sta.addStretch()
-        self.list_sta = QListWidget()
-        self.list_sta.setMaximumHeight(80)
-        # self.list_sta.setFixedHeight(64)
-        self.list_sta.setViewportMargins(2, 2, 17, 2)
-        vbox_sta_edit.addWidget(self.list_sta)
+        self.list_obs = QListWidget()
+        self.list_obs.setMaximumHeight(80)
+        # self.list_obs.setFixedHeight(64)
+        self.list_obs.setViewportMargins(2, 2, 17, 2)
+        vbox_sta_edit.addWidget(self.list_obs)
         # vbox_sta_edit.addStretch()
         hbox_sta.addWidget(edit_sta_col)
         cbox_more.setContentLayout(vbox_more)
 
         self.setContentLayout(vbox)
 
     def config_logic(self):
@@ -301,8 +307,8 @@
         height = max(28, min(height, 192))
         list.setFixedHeight(height)
 
     def fit_content(self):
         return
         self._fit_content(self.list_obj)
         self._fit_content(self.list_con)
-        self._fit_content(self.list_sta)
+        self._fit_content(self.list_obs)
```

### Comparing `badger-opt-1.0/src/badger/gui/default/components/extensions_palette.py` & `badger_opt-1.0.2/src/badger/gui/default/components/extensions_palette.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/components/filter_cbox.py` & `badger_opt-1.0.2/src/badger/gui/default/components/filter_cbox.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/components/generator_cbox.py` & `badger_opt-1.0.2/src/badger/gui/default/components/generator_cbox.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from PyQt5.QtWidgets import QVBoxLayout, QHBoxLayout, QPushButton, QWidget, QPlainTextEdit
 from PyQt5.QtWidgets import QComboBox, QCheckBox, QStyledItemDelegate, QLabel
 from .collapsible_box import CollapsibleBox
+from ..utils import MouseWheelWidgetAdjustmentGuard, NoHoverFocusComboBox
 from ....settings import read_value
 from ....utils import strtobool
 
 
 class BadgerAlgoBox(CollapsibleBox):
 
     def __init__(self, parent=None, generators=[], scaling_functions=[]):
@@ -20,18 +21,19 @@
 
         # Algo selector
         name = QWidget()
         hbox_name = QHBoxLayout(name)
         hbox_name.setContentsMargins(0, 0, 0, 0)
         lbl = QLabel('Name')
         lbl.setFixedWidth(64)
-        self.cb = cb = QComboBox()
+        self.cb = cb = NoHoverFocusComboBox()
         cb.setItemDelegate(QStyledItemDelegate())
         cb.addItems(self.generators)
         cb.setCurrentIndex(-1)
+        cb.installEventFilter(MouseWheelWidgetAdjustmentGuard(cb))
         hbox_name.addWidget(lbl)
         hbox_name.addWidget(cb, 1)
         self.btn_docs = btn_docs = QPushButton('Open Docs')
         btn_docs.setFixedSize(128, 24)
         hbox_name.addWidget(btn_docs)
         vbox.addWidget(name)
```

### Comparing `badger-opt-1.0/src/badger/gui/default/components/history_navigator.py` & `badger_opt-1.0.2/src/badger/gui/default/components/history_navigator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from PyQt5.QtWidgets import QComboBox, QTreeWidget, QTreeWidgetItem
 from PyQt5.QtCore import QModelIndex, Qt
+from ....archive import get_base_run_filename
 from ....utils import run_names_to_dict
 
 
 # Modified based on the following solution
 # https://stackoverflow.com/a/9672359/4263605
 class HistoryNavigator(QComboBox):
     def __init__(self):
@@ -36,65 +37,70 @@
                     return itemIndex, row
         return parent, None
 
     def currentIsFirst(self):
         if not self.runs:
             return True
 
-        run = self.currentText()
+        run = get_base_run_filename(self.currentText())
         try:
             idx = self.runs.index(run)
             if idx == 0:
                 return True
             else:
                 return False
         except:  # run is empty string
             return True
 
     def currentIsLast(self):
         if not self.runs:
             return True
 
-        run = self.currentText()
+        run = get_base_run_filename(self.currentText())
         try:
             idx = self.runs.index(run)
             tot = len(self.runs)
             if idx == tot - 1:
                 return True
             else:
                 return False
         except:  # run is empty string
             return True
 
     def _firstMatchingSelectableItem(self, text, parent=QModelIndex()):
         for i in range(self.model().rowCount(parent)):
             itemIndex = self.model().index(i, 0, parent)
             item = self.view().itemFromIndex(itemIndex)
-            if (item.flags() & Qt.ItemIsSelectable) and item.text(0) == text:
+            if (item.flags() & Qt.ItemIsSelectable) and item.text(0).startswith(text):
                 return parent, i
             else:
                 itemIndex, row = self._firstMatchingSelectableItem(text, itemIndex)
                 if row is not None:
                     return itemIndex, row
         return parent, None
 
     def _nextSelectableItem(self, parent=QModelIndex()):
-        run_curr = self.currentText()
+        run_curr = get_base_run_filename(self.currentText())
         idx = self.runs.index(run_curr)
         run_next = self.runs[idx + 1]
 
         return self._firstMatchingSelectableItem(run_next)
 
     def _previousSelectableItem(self, parent=QModelIndex()):
-        run_curr = self.currentText()
+        run_curr = get_base_run_filename(self.currentText())
         idx = self.runs.index(run_curr)
         run_prev = self.runs[idx - 1]
 
         return self._firstMatchingSelectableItem(run_prev)
 
+    def _currentSelectableItem(self, parent=QModelIndex()):
+        run_curr = get_base_run_filename(self.currentText())
+
+        return self._firstMatchingSelectableItem(run_curr)
+
     def updateItems(self, runs=None):
         self.view().clear()
 
         self.runs = runs  # store the runs for nav
         if runs is None:
             return
 
@@ -146,7 +152,16 @@
             self.setCurrentIndex(row)
 
     def selectPreviousItem(self):
         parent, row = self._previousSelectableItem()
         if row is not None:
             self.setRootModelIndex(parent)
             self.setCurrentIndex(row)
+
+    def changeCurrentItem(self, text, color=None):
+        parent, row = self._currentSelectableItem()
+        if row is not None:
+            itemIndex = self.model().index(row, 0, parent)
+            item = self.view().itemFromIndex(itemIndex)
+            item.setText(0, text)
+            if color:
+                item.setForeground(0, color)
```

### Comparing `badger-opt-1.0/src/badger/gui/default/components/labeled_lineedit.py` & `badger_opt-1.0.2/src/badger/gui/default/components/labeled_lineedit.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/components/obj_table.py` & `badger_opt-1.0.2/src/badger/gui/default/components/obj_table.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/components/reorderable_table.py` & `badger_opt-1.0.2/src/badger/gui/default/components/reorderable_table.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/components/robust_spinbox.py` & `badger_opt-1.0.2/src/badger/gui/default/components/robust_spinbox.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/components/routine_editor.py` & `badger_opt-1.0.2/src/badger/gui/default/components/routine_editor.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,20 +69,20 @@
         hbox_action.addWidget(btn_save)
         vbox.addWidget(action_bar)
 
     def config_logic(self):
         self.btn_cancel.clicked.connect(self.cancel_create_routine)
         self.btn_save.clicked.connect(self.save_routine)
 
-    def set_routine(self, routine: Routine):
+    def set_routine(self, routine: Routine, silent=False):
         try:
             self.routine_edit.setText(routine.yaml())
         except AttributeError:
             self.routine_edit.setText("")
-        self.routine_page.refresh_ui(routine)
+        self.routine_page.refresh_ui(routine, silent=silent)
 
     def edit_routine(self):
         self.stacks.setCurrentIndex(1)
 
     def del_routine(self):
         if self.routine_page.delete() == 0:
             self.sig_deleted.emit()
```

### Comparing `badger-opt-1.0/src/badger/gui/default/components/routine_item.py` & `badger_opt-1.0.2/src/badger/gui/default/components/routine_item.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/components/routine_page.py` & `badger_opt-1.0.2/src/badger/gui/default/components/routine_page.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,38 @@
+import warnings
 import sqlite3
 import traceback
-from typing import List
 
 import numpy as np
 import pandas as pd
 from PyQt5.QtCore import Qt, pyqtSignal
 from PyQt5.QtWidgets import QGroupBox, QLineEdit, QLabel, QPushButton
 from PyQt5.QtWidgets import QListWidgetItem, QMessageBox, QWidget
 from PyQt5.QtWidgets import QVBoxLayout, QHBoxLayout
 from PyQt5.QtWidgets import QTableWidgetItem, QPlainTextEdit, QSizePolicy
 from coolname import generate_slug
 from pydantic import ValidationError
 from xopt import VOCS
-from xopt.generators import get_generator_defaults
+from xopt.generators import get_generator_defaults, all_generator_names
+from xopt.utils import get_local_region
 
 from .generator_cbox import BadgerAlgoBox
 from .constraint_item import constraint_item
 from .data_table import get_table_content_as_dict, set_init_data_table
 from .env_cbox import BadgerEnvBox
 from .filter_cbox import BadgerFilterBox
 from .state_item import state_item
 from ..windows.docs_window import BadgerDocsWindow
 from ..windows.edit_script_dialog import BadgerEditScriptDialog
 from ..windows.lim_vrange_dialog import BadgerLimitVariableRangeDialog
 from ..windows.review_dialog import BadgerReviewDialog
 from ..windows.var_dialog import BadgerVariableDialog
+from ..windows.add_random_dialog import BadgerAddRandomDialog
+from ..windows.message_dialog import BadgerScrollableMessageBox
+from ..utils import filter_generator_config
 from ....db import save_routine, remove_routine, update_routine
 from ....environment import instantiate_env
 from ....errors import BadgerRoutineError
 from ....factory import list_generators, list_env, get_env
 from ....routine import Routine
 from ....settings import read_value
 from ....utils import get_yaml_string, load_config, strtobool
@@ -52,14 +56,18 @@
         self.routine = None
         self.script = ''
         self.window_docs = BadgerDocsWindow(self, '')
 
         # Limit variable ranges
         self.limit_option = None
 
+        # Add radom points config
+        self.add_rand_config = None
+        self.rc_dialog = None
+
         self.init_ui()
         self.config_logic()
 
     def init_ui(self):
         # Set up the layout
         vbox = QVBoxLayout(self)
         vbox.setContentsMargins(11, 11, 19, 11)
@@ -142,30 +150,36 @@
         self.env_box.cb.currentIndexChanged.connect(self.select_env)
         self.env_box.btn_env_play.clicked.connect(self.open_playground)
         self.env_box.btn_add_var.clicked.connect(self.add_var)
         self.env_box.btn_lim_vrange.clicked.connect(self.limit_variable_ranges)
         self.env_box.btn_add_con.clicked.connect(self.add_constraint)
         self.env_box.btn_add_sta.clicked.connect(self.add_state)
         self.env_box.btn_add_curr.clicked.connect(self.fill_curr_in_init_table)
+        self.env_box.btn_add_rand.clicked.connect(self.show_add_rand_dialog)
         self.env_box.btn_clear.clicked.connect(self.clear_init_table)
         self.env_box.btn_add_row.clicked.connect(self.add_row_to_init_table)
 
-    def refresh_ui(self, routine: Routine = None):
+    def refresh_ui(self, routine: Routine = None, silent: bool = False):
         self.routine = routine  # save routine for future reference
 
         self.generators = list_generators()
         self.envs = list_env()
-        # Clean up the constraints/states list
+        # Clean up the constraints/observables list
         self.env_box.list_con.clear()
-        self.env_box.list_sta.clear()
+        self.env_box.list_obs.clear()
 
         if routine is None:
             # Reset the generator and env configs
             self.generator_box.cb.setCurrentIndex(-1)
             self.env_box.cb.setCurrentIndex(-1)
+            init_table = self.env_box.init_table
+            init_table.clear()
+            init_table.horizontalHeader().setVisible(False)
+            init_table.setRowCount(10)
+            init_table.setColumnCount(0)
 
             # Reset the routine configs check box status
             self.env_box.check_only_var.setChecked(False)
             self.env_box.check_only_obj.setChecked(False)
 
             # Reset the save settings
             name = generate_slug(2)
@@ -176,19 +190,35 @@
 
             return
 
         # Enable description edition
         self.btn_descr_update.setDisabled(False)
         # Fill in the generator and env configs
         name_generator = routine.generator.name
-        idx_generator = self.generators.index(name_generator)
+        try:
+            idx_generator = self.generators.index(name_generator)
+        except ValueError as e:
+            if not silent:  # show the error message if not in silent mode
+                details = traceback.format_exc()
+                dialog = BadgerScrollableMessageBox(
+                    title='Error!',
+                    text=str(e),
+                    parent=self
+                )
+                dialog.setIcon(QMessageBox.Critical)
+                dialog.setDetailedText(details)
+                dialog.exec_()
+
+            idx_generator = -1
+
         self.generator_box.cb.setCurrentIndex(idx_generator)
         # self.generator_box.edit.setPlainText(routine.generator.yaml())
-        self.generator_box.edit.setPlainText(
-            get_yaml_string(routine.generator.model_dump()))
+        filtered_config = filter_generator_config(
+            name_generator, routine.generator.model_dump())
+        self.generator_box.edit.setPlainText(get_yaml_string(filtered_config))
         self.script = routine.script
 
         name_env = routine.environment.name
         idx_env = self.envs.index(name_env)
         self.env_box.cb.setCurrentIndex(idx_env)
         env_params = routine.environment.model_dump()
         del env_params["interface"]
@@ -218,17 +248,17 @@
             for name, val in constraints.items():
                 relation, thres = val
                 critical = name in routine.critical_constraint_names
                 relation = ['GREATER_THAN', 'LESS_THAN',
                             'EQUAL_TO'].index(relation)
                 self.add_constraint(name, relation, thres, critical)
 
-        constants = routine.vocs.constants
-        if len(constants):
-            for name_sta, val in constants.items():
+        observables = routine.vocs.observable_names
+        if len(observables):
+            for name_sta in observables:
                 self.add_state(name_sta)
 
         # Config the metadata
         self.edit_save.setPlaceholderText(generate_slug(2))
         self.edit_save.setText(routine.name)
         self.edit_descr.setPlainText(routine.description)
 
@@ -242,15 +272,22 @@
         if i == -1:
             self.generator_box.edit.setPlainText('')
             self.generator_box.cb_scaling.setCurrentIndex(-1)
             return
 
         name = self.generators[i]
         default_config = get_generator_defaults(name)
-        self.generator_box.edit.setPlainText(get_yaml_string(default_config))
+
+        # Patch for BOs that make the low noise prior False by default
+        if name in all_generator_names['bo']:
+            default_config['gp_constructor']['use_low_noise_prior'] = False
+
+        # Patch to only show part of the config
+        filtered_config = filter_generator_config(name, default_config)
+        self.generator_box.edit.setPlainText(get_yaml_string(filtered_config))
 
         # Update the docs
         self.window_docs.update_docs(name)
 
     def toggle_use_script(self):
         if self.generator_box.check_use_script.isChecked():
             self.generator_box.btn_edit_script.show()
@@ -366,15 +403,15 @@
             obj = {}
             obj[name] = 'MINIMIZE'  # default rule
             objs_env.append(obj)
         self.env_box.check_only_obj.setChecked(False)
         self.env_box.obj_table.update_objectives(objs_env)
 
         self.env_box.list_con.clear()
-        self.env_box.list_sta.clear()
+        self.env_box.list_obs.clear()
         self.env_box.fit_content()
         # self.routine = None
 
     def get_init_table_header(self):
         table = self.env_box.init_table
         header_list = []
         for col in range(table.columnCount()):
@@ -397,14 +434,57 @@
             if np.all([not table.item(row, col).text() for col in range(table.columnCount())]):
                 # Fill the row with content_list
                 for col, name in enumerate(vname_selected):
                     item = QTableWidgetItem(str(var_curr[name]))
                     table.setItem(row, col, item)
                 break  # Stop after filling the first non-empty row
 
+    def save_add_rand_config(self, add_rand_config):
+        self.add_rand_config = add_rand_config
+
+    def add_rand_in_init_table(self):
+        # Get current point
+        env = self.create_env()
+        vname_selected = self.get_init_table_header()
+        var_curr = env._get_variables(vname_selected)
+
+        # get small region around current point to sample
+        vocs, _ = self._compose_vocs()
+        n_point = self.add_rand_config['n_points']
+        fraction = self.add_rand_config['fraction']
+        random_sample_region = get_local_region(var_curr, vocs,
+                                                fraction=fraction)
+        random_points = vocs.random_inputs(n_point,
+                                           custom_bounds=random_sample_region)
+
+        # Add points to the table
+        table = self.env_box.init_table
+        for row in range(table.rowCount()):
+            # Check if the row is empty
+            if np.all([not table.item(row, col).text() for col in range(table.columnCount())]):
+                # Fill the row with content_list
+                try:
+                    point = random_points.pop(0)
+                    for col, name in enumerate(vname_selected):
+                        item = QTableWidgetItem(str(point[name]))
+                        table.setItem(row, col, item)
+                except IndexError:  # No more points to add
+                    break
+
+    def show_add_rand_dialog(self):
+        dlg = BadgerAddRandomDialog(
+            self, self.add_rand_in_init_table,
+            self.save_add_rand_config, self.add_rand_config,
+        )
+        self.rc_dialog = dlg
+        try:
+            dlg.exec()
+        finally:
+            self.rc_dialog = None
+
     def clear_init_table(self):
         table = self.env_box.init_table
         for row in range(table.rowCount()):
             for col in range(table.columnCount()):
                 item = table.item(row, col)
                 if item:
                     item.setText('')  # Set the cell content to an empty string
@@ -516,24 +596,24 @@
 
     def add_state(self, name=None):
         if self.configs is None:
             return
 
         var_names = [next(iter(d)) for d in self.configs['variables']]
         options = self.configs['observations'] + var_names
-        item = QListWidgetItem(self.env_box.list_sta)
+        item = QListWidgetItem(self.env_box.list_obs)
         sta_item = state_item(options,
-                              lambda: self.env_box.list_sta.takeItem(
-                                  self.env_box.list_sta.row(item)), name)
+                              lambda: self.env_box.list_obs.takeItem(
+                                  self.env_box.list_obs.row(item)), name)
         item.setSizeHint(sta_item.sizeHint())
-        self.env_box.list_sta.addItem(item)
-        self.env_box.list_sta.setItemWidget(item, sta_item)
+        self.env_box.list_obs.addItem(item)
+        self.env_box.list_obs.setItemWidget(item, sta_item)
         self.env_box.fit_content()
 
-    def _compose_vocs(self) -> (VOCS, List[str]):
+    def _compose_vocs(self) -> (VOCS, list[str]):
         # Compose the VOCS settings
         variables = self.env_box.var_table.export_variables()
         objectives = self.env_box.obj_table.export_objectives()
 
         constraints = {}
         critical_constraints = []
         for i in range(self.env_box.list_con.count()):
@@ -543,27 +623,27 @@
             con_name = item_widget.cb_obs.currentText()
             relation = CONS_RELATION_DICT[item_widget.cb_rel.currentText()]
             value = item_widget.sb.value()
             constraints[con_name] = [relation, value]
             if critical:
                 critical_constraints.append(con_name)
 
-        states = {}
-        for i in range(self.env_box.list_sta.count()):
-            raise NotImplementedError("constants/states has not been implemented yet!")
-            #item = self.env_box.list_sta.item(i)
-            #item_widget = self.env_box.list_sta.itemWidget(item)
-            #sta_name = item_widget.cb_sta.currentText()
-            #states[sta_name] =
+        observables = []
+        for i in range(self.env_box.list_obs.count()):
+            item = self.env_box.list_obs.item(i)
+            item_widget = self.env_box.list_obs.itemWidget(item)
+            obs_name = item_widget.cb_sta.currentText()
+            observables.append(obs_name)
 
         vocs = VOCS(
             variables=variables,
             objectives=objectives,
-            constraints={},
-            constants={}
+            constraints=constraints,
+            constants={},
+            observables=observables,
         )
 
         return vocs, critical_constraints
 
     def _compose_routine(self) -> Routine:
         # Compose the routine
         name = self.edit_save.text() or self.edit_save.placeholderText()
@@ -573,14 +653,22 @@
             raise BadgerRoutineError("no generator selected")
         if self.env_box.cb.currentIndex() == -1:
             raise BadgerRoutineError("no environment selected")
 
         generator_name = self.generators[self.generator_box.cb.currentIndex()]
         env_name = self.envs[self.env_box.cb.currentIndex()]
         generator_params = load_config(self.generator_box.edit.toPlainText())
+        # Patch the BO generators to make sure use_low_noise_prior is False
+        if generator_name in all_generator_names['bo']:
+            if 'gp_constructor' not in generator_params:
+                generator_params['gp_constructor'] = {
+                    'name': 'standard',  # have to add name too for pydantic validation
+                    'use_low_noise_prior': False,
+                }
+            # or else we use whatever specified by the users
         env_params = load_config(self.env_box.edit.toPlainText())
 
         # VOCS
         vocs, critical_constraints = self._compose_vocs()
 
         # Initial points
         init_points_df = pd.DataFrame.from_dict(
@@ -596,27 +684,37 @@
 
         # Script that generates generator params
         if self.generator_box.check_use_script.isChecked():
             script = self.script
         else:
             script = None
 
-        return Routine(
-            # Xopt part
-            vocs=vocs,
-            generator={"name": generator_name} | generator_params,
-            # Badger part
-            name=name,
-            description=description,
-            environment={"name": env_name} | env_params,
-            initial_points=init_points_df.astype("double"),
-            critical_constraint_names=critical_constraints,
-            tags=None,
-            script=script,
-        )
+        with warnings.catch_warnings(record=True) as caught_warnings:
+            routine = Routine(
+                # Xopt part
+                vocs=vocs,
+                generator={"name": generator_name} | generator_params,
+                # Badger part
+                name=name,
+                description=description,
+                environment={"name": env_name} | env_params,
+                initial_points=init_points_df.astype("double"),
+                critical_constraint_names=critical_constraints,
+                tags=None,
+                script=script,
+            )
+
+            # Check if any user warnings were caught
+            for warning in caught_warnings:
+                if warning.category == UserWarning:
+                    pass
+                else:
+                    print(f"Caught user warning: {warning.message}")
+
+            return routine
 
     def review(self):
         try:
             routine = self._compose_routine()
         except:
             return QMessageBox.critical(
                 self,
@@ -632,16 +730,16 @@
         routine.description = self.edit_descr.toPlainText()
         try:
             update_routine(routine)
             # Notify routine list to update
             self.sig_updated.emit(routine.name, routine.description)
             QMessageBox.information(
                 self,
-                'Update succeeded!',
-                f'Routine {self.routine.name} description was updated successfully!'
+                'Update success!',
+                f'Routine {self.routine.name} description was updated!'
             )
         except Exception:
             return QMessageBox.critical(
                 self,
                 'Update failed!',
                 traceback.format_exc()
             )
```

### Comparing `badger-opt-1.0/src/badger/gui/default/components/routine_runner.py` & `badger_opt-1.0.2/src/badger/gui/default/components/routine_runner.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import logging
 
 logger = logging.getLogger(__name__)
 import time
+import traceback
 from pandas import DataFrame
+import torch  # for converting dtype str to torch object
 from PyQt5.QtCore import pyqtSignal, QObject, QRunnable
 from ....core import run_routine, Routine
 from ....errors import BadgerRunTerminatedError
+from ....tests.utils import get_current_vars
 
 
 class BadgerRoutineSignals(QObject):
     env_ready = pyqtSignal(list)
     finished = pyqtSignal()
     progress = pyqtSignal()
     error = pyqtSignal(Exception)
@@ -60,14 +63,25 @@
     def set_termination_condition(self, termination_condition):
         self.termination_condition = termination_condition
 
     def run(self) -> None:
         self.start_time = time.time()
         self.last_dump_time = None  # reset the timer
 
+        # Patch for converting dtype str to torch object
+        try:
+            dtype = self.routine.generator.turbo_controller.tkwargs['dtype']
+            self.routine.generator.turbo_controller.tkwargs['dtype'] = eval(dtype)
+        except AttributeError:
+            pass
+        except KeyError:
+            pass
+        except TypeError:
+            pass
+
         try:
             self.save_init_vars()
 
             self.routine.data = None  # reset data
             run_routine(
                 self.routine,
                 active_callback=self.check_run_status,
@@ -75,15 +89,16 @@
                 evaluate_callback=self.after_evaluate,
                 states_callback=self.states_ready
             )
         except BadgerRunTerminatedError as e:
             self.signals.finished.emit()
             self.signals.info.emit(str(e))
         except Exception as e:
-            print(e)
+            traceback_info = traceback.format_exc()
+            e._details = traceback_info
             self.signals.finished.emit()
             self.signals.error.emit(e)
 
     def before_evaluate(self, candidates: DataFrame):
         # vars: ndarray
         while self.is_paused:
             time.sleep(0)
@@ -139,17 +154,15 @@
             return 2
         elif self.is_paused:
             return 1
         else:
             return 0  # continue to run
 
     def save_init_vars(self):
-        var_names = self.routine.vocs.variable_names
-        var_dict = self.routine.environment._get_variables(var_names)
-        init_vars = list(var_dict.values())
+        init_vars = get_current_vars(self.routine)
         self.signals.env_ready.emit(init_vars)
 
     def states_ready(self, states):
         self.states = states
 
     def ctrl_routine(self, pause):
         self.is_paused = pause
```

### Comparing `badger-opt-1.0/src/badger/gui/default/components/run_monitor.py` & `badger_opt-1.0.2/src/badger/gui/default/components/run_monitor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import os
 import traceback
 from importlib import resources
 import numpy as np
 import pandas as pd
-from PyQt5.QtWidgets import QVBoxLayout, QHBoxLayout, QWidget, QPushButton, QCheckBox
+from PyQt5.QtWidgets import QVBoxLayout, QHBoxLayout, QWidget, QTextEdit, QCheckBox
 from PyQt5.QtWidgets import QMessageBox, QComboBox, QLabel, QStyledItemDelegate
-from PyQt5.QtWidgets import QToolButton, QMenu, QAction
-from PyQt5.QtCore import pyqtSignal, QThreadPool, QSize
+from PyQt5.QtWidgets import QToolButton, QMenu, QAction, QScrollArea
+from PyQt5.QtCore import pyqtSignal, QThreadPool
 from PyQt5.QtGui import QFont, QIcon
 import pyqtgraph as pg
 from xopt import VOCS
 
 from .extensions_palette import ExtensionsPalette
 from .routine_runner import BadgerRoutineRunner
 from ..utils import create_button
 from ..windows.terminition_condition_dialog import BadgerTerminationConditionDialog
+from ..windows.message_dialog import BadgerScrollableMessageBox
 from ....routine import Routine
 # from ...utils import AURORA_PALETTE, FROST_PALETTE
 from ....logbook import send_to_logbook, BADGER_LOGBOOK_ROOT
 from ....archive import archive_run, BADGER_ARCHIVE_ROOT
+from ....tests.utils import get_current_vars
 
 # disable chained assignment warning from pydantic
 pd.options.mode.chained_assignment = None  # default='warn'
 
 
 stylesheet_del = '''
 QPushButton:hover:pressed
@@ -104,14 +106,15 @@
 
 class BadgerOptMonitor(QWidget):
     sig_pause = pyqtSignal(bool)  # True: pause, False: resume
     sig_stop = pyqtSignal()
     sig_lock = pyqtSignal(bool)  # True: lock GUI, False: unlock GUI
     sig_new_run = pyqtSignal()
     sig_run_name = pyqtSignal(str)  # filename of the new run
+    sig_status = pyqtSignal(str)  # status information
     sig_inspect = pyqtSignal(int)  # index of the inspector
     sig_progress = pyqtSignal(pd.DataFrame)  # new evaluated solution
     sig_del = pyqtSignal()
 
     def __init__(self):
         super().__init__()
         # self.setAttribute(Qt.WA_DeleteOnClose, True)
@@ -147,15 +150,18 @@
         self.post_run_actions = []
 
         self.init_ui()
         self.config_logic()
 
     @property
     def vocs(self) -> VOCS:
-        return self.routine.vocs
+        if self.routine is None:
+            return None
+        else:
+            return self.routine.vocs
 
     def init_ui(self):
         # Load all icons
         icon_ref = resources.files(__package__) / '../images/play.png'
         with resources.as_file(icon_ref) as icon_path:
             self.icon_play = QIcon(str(icon_path))
         icon_ref = resources.files(__package__) / '../images/pause.png'
@@ -400,46 +406,50 @@
 
         """
         if routine is None:
             # if no routines are specified, clear the current plots
             self.plot_var.clear()
             self.plot_obj.clear()
 
-            # if constraints are active clear them
+            # if constraints are active delete them
             try:
-                self.plot_con.clear()
-                self.plot_con.addItem(self.inspector_constraint)
-            except AttributeError:
+                self.monitor.removeItem(self.plot_con)
+                self.plot_con.removeItem(self.inspector_constraint)
+                del self.plot_con
+            except:
                 pass
 
-            # if statics exist clear that plot
+            # if statics exist delete that plot
             try:
-                self.plot_sta.clear()
-                self.plot_sta.addItem(self.inspector_state)
-            except AttributeError:
+                self.monitor.removeItem(self.plot_obs)
+                self.plot_obs.removeItem(self.inspector_state)
+                del self.plot_obs
+            except:
                 pass
 
             # if no routine is loaded set button to disabled
             self.btn_del.setDisabled(True)
             self.btn_log.setDisabled(True)
             self.btn_reset.setDisabled(True)
             self.btn_ctrl.setDisabled(True)
             self.btn_stop.setDisabled(True)
             self.btn_opt.setDisabled(True)
             self.btn_set.setDisabled(True)
 
+            self.routine = None
+
             return
 
         self.routine = routine
 
         # Retrieve data information
         objective_names = self.vocs.objective_names
         variable_names = self.vocs.variable_names
         constraint_names = self.vocs.constraint_names
-        sta_names = self.vocs.constant_names
+        sta_names = self.vocs.observable_names
 
         # Configure variable plots
         self.curves_variable = self._configure_plot(
             self.plot_var, self.inspector_variable, variable_names
         )
 
         # Configure objective plots
@@ -449,20 +459,19 @@
 
         # Configure constraint plots
         if constraint_names:
             try:
                 self.plot_con
             except:
                 self.plot_con = plot_con = add_axes(
-                    self.monitor, "Constraints", 'Evaluation History (C)',
+                    self.monitor, "constraints", 'Evaluation History (C)',
                     self.inspector_constraint, row=1, col=0
                 )
                 plot_con.setXLink(self.plot_obj)
 
-            # Configure objective plots
             self.curves_constraint = self._configure_plot(
                 self.plot_con, self.inspector_constraint, constraint_names
             )
 
         else:
             try:
                 self.monitor.removeItem(self.plot_con)
@@ -470,34 +479,30 @@
                 del self.plot_con
             except:
                 pass
 
         # Configure state plots
         if sta_names:
             try:
-                self.plot_sta
+                self.plot_obs
             except:
-                self.plot_sta = plot_sta = add_axes(
-                    self.monitor, "Constants", 'Evaluation History (S)',
-                    self.inspector_state, row=1, col=0
+                self.plot_obs = plot_obs = add_axes(
+                    self.monitor, "observables", 'Evaluation History (S)',
+                    self.inspector_state, row=2, col=0
                 )
-                plot_sta.setXLink(self.plot_obj)
+                plot_obs.setXLink(self.plot_obj)
 
-            self.curves_sta = []
-            for i, sta_name in enumerate(sta_names):
-                color = self.colors[i % len(self.colors)]
-                symbol = self.symbols[i % len(self.colors)]
-                _curve = self.plot_sta.plot(pen=pg.mkPen(color, width=3),
-                                            name=sta_name)
-                self.curves_sta.append(_curve)
+            self.curves_sta = self._configure_plot(
+                self.plot_obs, self.inspector_state, sta_names
+            )
         else:
             try:
-                self.monitor.removeItem(self.plot_sta)
-                self.plot_sta.removeItem(self.inspector_state)
-                del self.plot_sta
+                self.monitor.removeItem(self.plot_obs)
+                self.plot_obs.removeItem(self.inspector_state)
+                del self.plot_obs
             except:
                 pass
 
         # Reset inspectors
         self.inspector_objective.setValue(0)
         self.inspector_variable.setValue(0)
         self.inspector_constraint.setValue(0)
@@ -562,14 +567,15 @@
         if self.routine_runner:
             self.sig_pause.disconnect()
             self.sig_stop.disconnect()
             self.routine_runner = None
 
     def start(self, use_termination_condition=False):
         self.sig_new_run.emit()
+        self.sig_status.emit(f'Running routine {self.routine.name}...')
         self.init_plots(self.routine)
         self.init_routine_runner()
         if use_termination_condition:
             self.routine_runner.set_termination_condition(self.termination_condition)
         self.running = True  # if a routine runner is working
         self.thread_pool.start(self.routine_runner)
 
@@ -591,16 +597,16 @@
     def enable_auto_range(self):
         # Enable autorange
         self.plot_obj.enableAutoRange()
         self.plot_var.enableAutoRange()
         if self.vocs.constraint_names:
             self.plot_con.enableAutoRange()
 
-        # if self.sta_names:
-        #    self.plot_sta.enableAutoRange()
+        if self.vocs.observable_names:
+           self.plot_obs.enableAutoRange()
 
     def open_extensions_palette(self):
         self.extensions_palette.show()
 
     def extension_window_closed(self, child_window):
         self.active_extensions.remove(child_window)
         self.extensions_palette.update_palette()
@@ -653,16 +659,15 @@
         if self.x_plot_relative:
             input_data[variable_names] = input_data[variable_names] - \
                                         input_data[variable_names].iloc[0]
 
         set_data(variable_names, self.curves_variable, input_data, ts)
         set_data(self.vocs.objective_names, self.curves_objective, data_copy, ts)
         set_data(self.vocs.constraint_names, self.curves_constraint, data_copy, ts)
-
-        # TODO: add tracking of observables
+        set_data(self.vocs.observable_names, self.curves_sta, data_copy, ts)
 
     def check_critical(self):
         """
         Check if a critical constraint has been violated in the last data point,
         and take appropriate actions if so.
 
         If there are no critical constraints, the function will return without taking
@@ -685,31 +690,33 @@
         pause and stop actions.
 
         """
 
         # if there are no critical constraints then skip
         if len(self.routine.critical_constraint_names) == 0:
             return
-        else:
-            feas = self.vocs.feasibility_data(self.routine.data.iloc[-1])
-            violated_critical = ~feas[self.routine.critical_constraint_names].any()
 
-            if not violated_critical:
-                return
+        feas = self.vocs.feasibility_data(self.routine.data.tail(1), prefix='')
+        feasible = feas['feasible'].iloc[0].item()
+        if feasible:
+            return
 
         # if code reaches this point there is a critical constraint violated
         self.sig_pause.emit(True)
         self.btn_ctrl.setIcon(self.icon_play)
         self.btn_ctrl.setToolTip('Resume')
         self.btn_ctrl._status = 'play'
 
-        msg = str(feas)
+        # Show the list of critical violated constraints
+        feas_crit = feas[self.routine.critical_constraint_names]
+        violated_crit = feas_crit.columns[~feas_crit.iloc[0]].tolist()
+        msg = '\n'.join(violated_crit)
         reply = QMessageBox.warning(self,
                                     'Run Paused',
-                                    f'Critical constraint was violated: {msg}\nTerminate the run?',
+                                    f'The following critical constraints were violated:\n\n{msg}\n\nTerminate the run?',
                                     QMessageBox.Yes | QMessageBox.No, QMessageBox.Yes)
         if reply == QMessageBox.Yes:
             self.sig_stop.emit()
 
     def update_analysis_extensions(self):
         for ele in self.active_extensions:
             try:
@@ -755,57 +762,65 @@
             filename = run['filename'][:-4] + 'pickle'
             try:
                 env.interface.stop_recording(os.path.join(path, filename))
             except AttributeError:  # recording was not enabled
                 pass
 
             self.sig_run_name.emit(run['filename'])
-            if not self.testing:
-                QMessageBox.information(
-                    self, 'Success!',
-                    f'Archive succeeded: Run data archived to {BADGER_ARCHIVE_ROOT}')
+            self.sig_status.emit(f'Archive success: Run data archived to {BADGER_ARCHIVE_ROOT}')
+            # if not self.testing:
+            #     QMessageBox.information(
+            #         self, 'Success!',
+            #         f'Archive success: Run data archived to {BADGER_ARCHIVE_ROOT}')
 
         except Exception as e:
             self.sig_run_name.emit(None)
-            if not self.testing:
-                QMessageBox.critical(self, 'Archive failed!',
-                                     f'Archive failed: {str(e)}')
+            self.sig_status.emit(f'Archive failed: {str(e)}')
+            # if not self.testing:
+            #     QMessageBox.critical(self, 'Archive failed!',
+            #                          f'Archive failed: {str(e)}')
         finally:
             for action in self.post_run_actions:
                 action()
 
     def destroy_unused_env(self):
         if not self.running:
             try:
                 del self.routine.environment
             except AttributeError:  # env already destroyed
                 pass
 
     def on_error(self, error):
-        QMessageBox.critical(self, 'Error!', str(error))
+        details = error._details if hasattr(error, '_details') else None
+
+        dialog = BadgerScrollableMessageBox(
+            title='Error!',
+            text=str(error),
+            parent=self
+        )
+        dialog.setIcon(QMessageBox.Critical)
+        dialog.setDetailedText(details)
+        dialog.exec_()
 
     # Do not show info -- too distracting
     def on_info(self, msg):
         pass
-        # QMessageBox.information(self, 'Info', msg)
 
     def logbook(self):
         try:
-            if self.routine_runner:
-                routine = self.routine_runner.name
-                data = self.routine_runner.data.to_dict('list')
-            else:
-                routine = self.routine
-                data = self.data
-            send_to_logbook(routine, data, self.monitor)
+            send_to_logbook(self.routine, self.monitor)
         except Exception as e:
-            QMessageBox.critical(self, 'Log failed!', str(e))
+            self.sig_status.emit(f'Log failed: {str(e)}')
+            # QMessageBox.critical(self, 'Log failed!', str(e))
+
+            return
 
-        QMessageBox.information(
-            self, 'Success!', f'Log saved to {BADGER_LOGBOOK_ROOT}')
+        self.sig_status.emit(f'Log success: Log saved to {BADGER_LOGBOOK_ROOT}')
+        # QMessageBox.information(
+        #     self, 'Success!', f'')
 
     def ctrl_routine(self):
         if self.btn_ctrl._status == 'pause':
             self.sig_pause.emit(True)
             self.btn_ctrl.setIcon(self.icon_play)
             self.btn_ctrl.setToolTip('Resume')
             self.btn_ctrl._status = 'play'
@@ -815,50 +830,53 @@
             self.btn_ctrl.setToolTip('Pause')
             self.btn_ctrl._status = 'pause'
 
     def ins_obj_dragged(self, ins_obj):
         self.inspector_variable.setValue(ins_obj.value())
         if self.vocs.constraint_names:
             self.inspector_constraint.setValue(ins_obj.value())
-        # if self.sta_names:
-        #    self.inspector_state.setValue(ins_obj.value())
+        if self.vocs.observable_names:
+            self.inspector_state.setValue(ins_obj.value())
 
     def ins_con_dragged(self, ins_con):
         self.inspector_variable.setValue(ins_con.value())
         self.inspector_objective.setValue(ins_con.value())
-        # if self.sta_names:
-        #    self.inspector_state.setValue(ins_con.value())
+        if self.vocs.observable_names:
+            self.inspector_state.setValue(ins_con.value())
 
     def ins_sta_dragged(self, ins_sta):
         self.inspector_variable.setValue(ins_sta.value())
         self.inspector_objective.setValue(ins_sta.value())
-        # if self.vocs.constraint_names:
-        #    self.inspector_constraint.setValue(ins_sta.value())
+        if self.vocs.constraint_names:
+            self.inspector_constraint.setValue(ins_sta.value())
 
     def ins_var_dragged(self, ins_var):
         self.inspector_objective.setValue(ins_var.value())
         if self.vocs.constraint_names:
             self.inspector_constraint.setValue(ins_var.value())
-        # if self.sta_names:
-        #    self.inspector_state.setValue(ins_var.value())
+        if self.vocs.observable_names:
+            self.inspector_state.setValue(ins_var.value())
 
     def ins_drag_done(self, ins):
         self.sync_ins(ins.value())
 
     def sync_ins(self, pos):
         if self.plot_x_axis:  # x-axis is time
             value, idx = self.closest_ts(pos)
         else:
-            ts = self.extract_timestamp()
-            value = idx = np.clip(np.round(pos), 0, len(ts) - 1)
+            try:
+                ts = self.extract_timestamp()
+                value = idx = np.clip(np.round(pos), 0, len(ts) - 1)
+            except:  # no data
+                value = idx = np.round(pos)
         self.inspector_objective.setValue(value)
-        if self.vocs.constraint_names:
+        if self.vocs and self.vocs.constraint_names:
             self.inspector_constraint.setValue(value)
-        # if self.sta_names:
-        #    self.inspector_state.setValue(value)
+        if self.vocs and self.vocs.observable_names:
+            self.inspector_state.setValue(value)
         self.inspector_variable.setValue(value)
 
         self.sig_inspect.emit(idx)
 
     def closest_ts(self, t):
         # Get the closest timestamp in data regarding t
         ts = self.extract_timestamp()
@@ -872,32 +890,39 @@
                                      'Reset Environment',
                                      f'Are you sure you want to reset the env vars '
                                      f'back to {self.init_vars}?',
                                      QMessageBox.Yes | QMessageBox.No, QMessageBox.No)
         if reply != QMessageBox.Yes:
             return
 
-        # TODO: Should just get vars from env! Current values are not always
-        # ones in the latest solution
-        # current_vars = self.routine.data.iloc[-1].to_dict(orient="records")
-        current_vars = self.routine.sorted_data[
-            self.vocs.variable_names].iloc[-1].to_numpy().tolist()
+        curr_vars = get_current_vars(self.routine)
 
-        # evaluate the initial variables -- do not store the result
-        # self.routine.evaluate(self.init_vars)
         self.routine.environment._set_variables(
             dict(zip(self.vocs.variable_names, self.init_vars)))
 
-        QMessageBox.information(self, 'Reset Environment',
-                                f'Env vars {current_vars} -> {self.init_vars}')
+        self.jump_to_solution(0)
+        self.sig_inspect.emit(0)
+        # Center around the zero position
+        if self.plot_x_axis:  # x-axis is time
+            pos, _ = self.closest_ts(self.inspector_objective.value())
+        else:
+            pos = int(self.inspector_objective.value())
+        x_range = self.plot_var.getViewBox().viewRange()[0]
+        delta = (x_range[1] - x_range[0]) / 2
+        self.plot_var.setXRange(pos - delta, pos + delta, padding=0)
+
+        self.sig_status.emit(f'Reset environment: Env vars {curr_vars} -> {self.init_vars}')
+        # QMessageBox.information(self, 'Reset Environment',
+        #                         f'Env vars {curr_vars} -> {self.init_vars}')
 
     def jump_to_optimal(self):
         try:
-            best_idx, _ = self.routine.vocs.select_best(
+            best_idx, _, _ = self.routine.vocs.select_best(
                 self.routine.sorted_data, n=1)
+            # print(best_idx, _)
             best_idx = int(best_idx[0])
 
             self.jump_to_solution(best_idx)
             self.sig_inspect.emit(best_idx)
         except NotImplementedError:
             QMessageBox.warning(
                 self, 'Jump to optimum',
@@ -910,73 +935,77 @@
             value = ts[idx] - ts[0]
         else:
             value = idx
 
         self.inspector_objective.setValue(value)
         if self.vocs.constraint_names:
             self.inspector_constraint.setValue(value)
-        # if self.sta_names:
-        #    self.inspector_state.setValue(value)
+        if self.vocs.observable_names:
+            self.inspector_state.setValue(value)
         self.inspector_variable.setValue(value)
 
     def set_vars(self):
         df = self.routine.sorted_data
         if self.plot_x_axis:  # x-axis is time
             pos, idx = self.closest_ts(self.inspector_objective.value())
         else:
             pos = idx = int(self.inspector_objective.value())
         variable_names = self.vocs.variable_names
         solution = df[variable_names].to_numpy()[idx]
 
         reply = QMessageBox.question(self,
                                      'Apply Solution',
-                                     f'Are you sure you want to apply the current solution at {solution} to env?',
+                                     f'Are you sure you want to apply the selected solution at {solution} to env?',
                                      QMessageBox.Yes | QMessageBox.No, QMessageBox.No)
         if reply != QMessageBox.Yes:
             return
 
+        curr_vars = get_current_vars(self.routine)
         self.routine.environment._set_variables(
             dict(zip(variable_names, solution)))
         # center around the inspector
         x_range = self.plot_var.getViewBox().viewRange()[0]
         delta = (x_range[1] - x_range[0]) / 2
-        self.plot_var.setXRange(pos - delta, pos + delta)
+        self.plot_var.setXRange(pos - delta, pos + delta, padding=0)
+
+        updated_vars = get_current_vars(self.routine)
+        self.sig_status.emit(f'Dial in solution: Env vars {curr_vars} -> {updated_vars}')
         # QMessageBox.information(
         #     self, 'Set Environment', f'Env vars have been set to {solution}')
 
     def select_x_axis(self, i):
         self.plot_x_axis = i
 
         # Switch the x-axis labels
         if i:
             self.plot_var.setLabel('bottom', 'time (s)')
             self.plot_obj.setLabel('bottom', 'time (s)')
             if self.vocs.constraint_names:
                 self.plot_con.setLabel('bottom', 'time (s)')
-            # if self.sta_names:
-            #    self.plot_sta.setLabel('bottom', 'time (s)')
+            if self.vocs.observable_names:
+                self.plot_obs.setLabel('bottom', 'time (s)')
         else:
             self.plot_var.setLabel('bottom', 'iterations')
             self.plot_obj.setLabel('bottom', 'iterations')
             if self.vocs.constraint_names:
                 self.plot_con.setLabel('bottom', 'iterations')
-            # if self.sta_names:
-            #     self.plot_sta.setLabel('bottom', 'iterations')
+            if self.vocs.observable_names:
+                self.plot_obs.setLabel('bottom', 'iterations')
 
         # Update inspector line position
         if i:
             ts = self.extract_timestamp()
             value = ts[int(self.inspector_objective.value())] - ts[0]
         else:
             _, value = self.closest_ts(self.inspector_objective.value())
         self.inspector_objective.setValue(value)
         if self.vocs.constraint_names:
             self.inspector_constraint.setValue(value)
-        # if self.sta_names:
-        #    self.inspector_state.setValue(value)
+        if self.vocs.observable_names:
+            self.inspector_state.setValue(value)
         self.inspector_variable.setValue(value)
 
         self.update_curves()
         self.enable_auto_range()
 
     def select_x_plot_y_axis(self, i):
         self.x_plot_y_axis = i
@@ -985,26 +1014,26 @@
     def toggle_x_plot_y_axis_relative(self):
         self.x_plot_relative = self.check_relative.isChecked()
         self.update_curves()
 
     def on_mouse_click(self, event):
         # https://stackoverflow.com/a/64081483
         coor_obj = self.plot_obj.vb.mapSceneToView(event._scenePos)
-        if self.vocs.constraint_names:
+        if self.vocs and self.vocs.constraint_names:
             coor_con = self.plot_con.vb.mapSceneToView(event._scenePos)
-        # if self.sta_names:
-        #    coor_sta = self.plot_sta.vb.mapSceneToView(event._scenePos)
+        if self.vocs and self.vocs.observable_names:
+            coor_sta = self.plot_obs.vb.mapSceneToView(event._scenePos)
         coor_var = self.plot_var.vb.mapSceneToView(event._scenePos)
 
         flag = self.plot_obj.viewRect().contains(coor_obj) or \
-               self.plot_var.viewRect().contains(coor_var)
-        if self.vocs.constraint_names:
+            self.plot_var.viewRect().contains(coor_var)
+        if self.vocs and self.vocs.constraint_names:
             flag = flag or self.plot_con.viewRect().contains(coor_con)
-        # if self.sta_names:
-        #    flag = flag or self.plot_sta.viewRect().contains(coor_sta)
+        if self.vocs and self.vocs.observable_names:
+            flag = flag or self.plot_obs.viewRect().contains(coor_sta)
 
         if flag:
             self.sync_ins(coor_obj.x())
 
     def delete_run(self):
         self.sig_del.emit()
```

### Comparing `badger-opt-1.0/src/badger/gui/default/components/state_item.py` & `badger_opt-1.0.2/src/badger/gui/default/components/state_item.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/components/status_bar.py` & `badger_opt-1.0.2/src/badger/gui/default/components/status_bar.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from importlib import resources
 from PyQt5.QtWidgets import QHBoxLayout, QWidget, QPushButton
-from PyQt5.QtWidgets import QLabel
 from PyQt5.QtWidgets import QSizePolicy
 from PyQt5.QtGui import QIcon
 from PyQt5.QtCore import Qt, QSize
 from ..windows.settings_dialog import BadgerSettingsDialog
+from .eliding_label import SimpleElidedLabel
 
 
 class BadgerStatusBar(QWidget):
     def __init__(self):
         super().__init__()
 
         self.init_ui()
@@ -18,29 +18,30 @@
         icon_ref = resources.files(__package__) / '../images/gear.png'
         with resources.as_file(icon_ref) as icon_path:
             self.icon_settings = QIcon(str(icon_path))
 
         hbox = QHBoxLayout(self)
         hbox.setContentsMargins(0, 0, 0, 0)
 
-        self.summary = summary = QLabel()
+        self.summary = summary = SimpleElidedLabel()
+        # summary.setStyleSheet("background-color: orange;")  # for debugging
+        summary.setAlignment(Qt.AlignCenter)
 
         self.btn_settings = btn_settings = QPushButton()
         btn_settings.setFixedSize(24, 24)
         btn_settings.setIcon(self.icon_settings)
         btn_settings.setIconSize(QSize(12, 12))
         btn_settings.setToolTip('Badger settings')
 
-        summary.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Preferred)
-        summary.setAlignment(Qt.AlignCenter)
         hbox.addWidget(summary, 1)
         hbox.addWidget(btn_settings)
 
     def config_logic(self):
         self.btn_settings.clicked.connect(self.go_settings)
 
     def set_summary(self, text):
         self.summary.setText(text)
+        self.setToolTip(text)
 
     def go_settings(self):
         dlg = BadgerSettingsDialog(self)
         dlg.exec()
```

### Comparing `badger-opt-1.0/src/badger/gui/default/components/syntax.py` & `badger_opt-1.0.2/src/badger/gui/default/components/syntax.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/components/var_table.py` & `badger_opt-1.0.2/src/badger/gui/default/components/var_table.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/images/add.png` & `badger_opt-1.0.2/src/badger/gui/default/images/add.png`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/images/book-alt.png` & `badger_opt-1.0.2/src/badger/gui/default/images/book-alt.png`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/images/book.png` & `badger_opt-1.0.2/src/badger/gui/default/images/book.png`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/images/crosshairs.png` & `badger_opt-1.0.2/src/badger/gui/default/images/crosshairs.png`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/images/export.png` & `badger_opt-1.0.2/src/badger/gui/default/images/export.png`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/images/extension-alt.png` & `badger_opt-1.0.2/src/badger/gui/default/images/extension-alt.png`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/images/extension.png` & `badger_opt-1.0.2/src/badger/gui/default/images/extension.png`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/images/gear.png` & `badger_opt-1.0.2/src/badger/gui/default/images/gear.png`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/images/icon.png` & `badger_opt-1.0.2/src/badger/gui/default/images/icon.png`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/images/import.png` & `badger_opt-1.0.2/src/badger/gui/default/images/import.png`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/images/info.png` & `badger_opt-1.0.2/src/badger/gui/default/images/info.png`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/images/next.png` & `badger_opt-1.0.2/src/badger/gui/default/images/next.png`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/images/pause.png` & `badger_opt-1.0.2/src/badger/gui/default/images/pause.png`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/images/play.png` & `badger_opt-1.0.2/src/badger/gui/default/images/play.png`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/images/previous.png` & `badger_opt-1.0.2/src/badger/gui/default/images/previous.png`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/images/set.png` & `badger_opt-1.0.2/src/badger/gui/default/images/set.png`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/images/star.png` & `badger_opt-1.0.2/src/badger/gui/default/images/star.png`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/images/stop.png` & `badger_opt-1.0.2/src/badger/gui/default/images/stop.png`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/images/tools.png` & `badger_opt-1.0.2/src/badger/gui/default/images/tools.png`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/images/trash.png` & `badger_opt-1.0.2/src/badger/gui/default/images/trash.png`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/images/undo.png` & `badger_opt-1.0.2/src/badger/gui/default/images/undo.png`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/pages/home_page.py` & `badger_opt-1.0.2/src/badger/gui/default/pages/home_page.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import os
+import traceback
 from importlib import resources
 from pandas import DataFrame
 
 from PyQt5.QtWidgets import QWidget, QVBoxLayout, QHBoxLayout, QMessageBox
 from PyQt5.QtWidgets import QPushButton, QSplitter, QTabWidget, QShortcut
 from PyQt5.QtWidgets import QListWidget, QListWidgetItem, QLabel, QFileDialog
 from PyQt5.QtCore import Qt, pyqtSignal
-from PyQt5.QtGui import QKeySequence, QIcon, QFont
+from PyQt5.QtGui import QKeySequence, QIcon
+# from PyQt5.QtGui import QBrush, QColor
+from ..windows.message_dialog import BadgerScrollableMessageBox
 from ..components.search_bar import search_bar
 from ..components.data_table import data_table, update_table, reset_table, add_row
 from ..components.routine_item import BadgerRoutineItem
 from ..components.history_navigator import HistoryNavigator
 from ..components.run_monitor import BadgerOptMonitor
 from ..components.routine_editor import BadgerRoutineEditor
 from ..components.status_bar import BadgerStatusBar
 from ..components.filter_cbox import BadgerFilterBox
 from ..utils import create_button
 from ....db import list_routine, load_routine, remove_routine, get_runs_by_routine, get_runs
 from ....db import import_routines, export_routines
-from ....archive import load_run, delete_run
+from ....archive import load_run, delete_run, get_base_run_filename
 from ....utils import get_header, strtobool
 from ....settings import read_value
 
 
 stylesheet = '''
 QPushButton:hover:pressed
 {
@@ -43,14 +46,16 @@
 
     def __init__(self):
         super().__init__()
 
         self.mode = 'regular'  # home page mode
         self.splitter_state = None  # store the run splitter state
         self.tab_state = None  # store the tabs state before creating new routine
+        self.current_routine = None  # current routine
+        self.go_run_failed = False  # flag to indicate go_run failed
 
         self.init_ui()
         self.config_logic()
 
         self.load_all_runs()
 
     def init_ui(self):
@@ -222,14 +227,15 @@
         self.btn_prev.clicked.connect(self.go_prev_run)
         self.btn_next.clicked.connect(self.go_next_run)
 
         self.run_monitor.sig_inspect.connect(self.inspect_solution)
         self.run_monitor.sig_lock.connect(self.toggle_lock)
         self.run_monitor.sig_new_run.connect(self.new_run)
         self.run_monitor.sig_run_name.connect(self.run_name)
+        self.run_monitor.sig_status.connect(self.update_status)
         self.run_monitor.sig_progress.connect(self.progress)
         self.run_monitor.sig_del.connect(self.delete_run)
 
         self.routine_editor.sig_saved.connect(self.routine_saved)
         self.routine_editor.sig_canceled.connect(self.done_create_routine)
         self.routine_editor.sig_deleted.connect(self.routine_deleted)
         self.routine_editor.routine_page.sig_updated.connect(self.routine_description_updated)
@@ -254,22 +260,24 @@
         self.routine_editor.set_routine(None)
         self.tab_state = self.tabs.currentIndex()
         self.tabs.setCurrentIndex(1)
         self.mode = 'new routine'
         self.routine_editor.switch_mode(self.mode)
         self.toggle_lock(True, 0)
 
-    def select_routine(self, routine_item: QListWidgetItem):
+    def select_routine(self, routine_item: QListWidgetItem, force=False):
+        # force: if True, select the target routine_item even if
+        #        it's selected already
         if self.prev_routine_item:
             try:
                 self.routine_list.itemWidget(self.prev_routine_item).deactivate()
             except ValueError:
                 pass
 
-            if self.prev_routine_item.routine_name == routine_item.routine_name:  #
+            if (not force) and (self.prev_routine_item.routine_name == routine_item.routine_name):
                 # click a routine again to deselect
                 self.prev_routine_item = None
                 self.current_routine = None
                 self.load_all_runs()
                 if not self.cb_history.count():
                     self.go_run(-1)  # sometimes we need to trigger this manually
                 self.sig_routine_activated.emit(False)
@@ -285,15 +293,18 @@
         self.cb_history.updateItems(runs)
         if not self.cb_history.count():
             self.go_run(-1)  # sometimes we need to trigger this manually
 
         if not runs:  # auto plot will not be triggered
             self.run_monitor.init_plots(routine)
 
-        self.routine_list.itemWidget(routine_item).activate()
+        if self.go_run_failed:  # failed to load run, do not select the routine
+            self.go_run_failed = False
+        else:
+            self.routine_list.itemWidget(routine_item).activate()
 
     def build_routine_list(self,
                            routines: list[str],
                            timestamps: list[str],
                            descriptions: list[str]):
         try:
             selected_routine = self.prev_routine_item.routine_name
@@ -341,34 +352,63 @@
         #     return
 
         self.btn_prev.setDisabled(self.cb_history.currentIsFirst())
         self.btn_next.setDisabled(self.cb_history.currentIsLast())
 
         if i == -1:
             update_table(self.run_table)
+            try:
+                self.current_routine.data = None  # reset the data
+            except AttributeError:  # current routine is None
+                pass
             self.run_monitor.init_plots(self.current_routine)
             if not self.current_routine:
                 self.routine_editor.clear()
-                self.status_bar.set_summary('no active routine')
+                self.status_bar.set_summary('No active routine')
             else:
-                self.status_bar.set_summary(f'current routine: {self.current_routine.name}')
+                self.status_bar.set_summary(f'Current routine: {self.current_routine.name}')
             return
 
-        run_filename = self.cb_history.currentText()
+        run_filename = get_base_run_filename(self.cb_history.currentText())
         try:
             _routine = load_run(run_filename)
             routine, _ = load_routine(_routine.name)  # get the initial routine
-            routine.data = _routine.data
-        except (IndexError, AttributeError):
+            # TODO: figure out how to recover the original routine
+            if routine is None:  # routine not found, could be deleted
+                routine = _routine  # make do w/ the routine saved in run
+            else:
+                routine.data = _routine.data
+        except IndexError:
             return
+        except Exception as e:  # failed to load the run
+            details = traceback.format_exc()
+            dialog = BadgerScrollableMessageBox(
+                title='Error!',
+                text=str(e),
+                parent=self
+            )
+            dialog.setIcon(QMessageBox.Critical)
+            dialog.setDetailedText(details)
+            dialog.exec_()
+            self.go_run_failed = True
+
+            # Show info in the nav bar
+            # red_brush = QBrush(QColor(255, 0, 0))  # red color
+            self.cb_history.changeCurrentItem(
+                f'{run_filename} (failed to load)',
+                # color=red_brush)
+                color=None)
+
+            return
+
         self.current_routine = routine  # update the current routine
         update_table(self.run_table, routine.sorted_data)
         self.run_monitor.init_plots(routine, run_filename)
-        self.routine_editor.set_routine(routine)
-        self.status_bar.set_summary(f'current routine: {self.current_routine.name}')
+        self.routine_editor.set_routine(routine, silent=True)
+        self.status_bar.set_summary(f'Current routine: {self.current_routine.name}')
 
     def go_prev_run(self):
         self.cb_history.selectPreviousItem()
 
     def go_next_run(self):
         self.cb_history.selectNextItem()
 
@@ -418,24 +458,27 @@
     def run_name(self, name):
         if self.prev_routine_item:
             runs = get_runs_by_routine(self.current_routine.name)
         else:
             runs = get_runs()
         self.cb_history.updateItems(runs)
 
+    def update_status(self, info):
+        self.status_bar.set_summary(info)
+
     def progress(self, solution: DataFrame):
         vocs = self.current_routine.vocs
         vars = list(solution[vocs.variable_names].to_numpy()[0])
         objs = list(solution[vocs.objective_names].to_numpy()[0])
         cons = list(solution[vocs.constraint_names].to_numpy()[0])
         stas = list(solution[vocs.observable_names].to_numpy()[0])
         add_row(self.run_table, objs + cons + vars + stas)
 
     def delete_run(self):
-        run_name = self.cb_history.currentText()
+        run_name = get_base_run_filename(self.cb_history.currentText())
 
         reply = QMessageBox.question(
             self, 'Delete run',
             f'Are you sure you want to delete run {run_name}?',
             QMessageBox.Yes | QMessageBox.No, QMessageBox.No)
         if reply != QMessageBox.Yes:
             return
@@ -449,15 +492,15 @@
             runs = get_runs_by_routine(self.current_routine.name)
         self.cb_history.updateItems(runs)
         if not self.cb_history.count():
             self.go_run(-1)  # sometimes we need to trigger this manually
 
     def routine_saved(self):
         self.refresh_routine_list()
-        self.select_routine(self.routine_list.item(0))
+        self.select_routine(self.routine_list.item(0), force=True)
         self.tab_state = 0  # force jump to run monitor
         self.done_create_routine()
 
     def done_create_routine(self):
         if self.mode == 'new routine':
             self.mode = 'regular'
             self.routine_editor.switch_mode(self.mode)
@@ -509,15 +552,15 @@
             filename = filename + '.db'
 
         try:
             routines, _, _ = self.get_current_routines()
             export_routines(filename, routines)
 
             QMessageBox.information(
-                self, 'Success!', f'Export succeeded: filtered routines exported to {filename}')
+                self, 'Success!', f'Export success: filtered routines exported to {filename}')
         except Exception as e:
             QMessageBox.critical(self, 'Export failed!', f'Export failed: {str(e)}')
 
     def import_routines(self):
         options = QFileDialog.Options()
         options |= QFileDialog.DontUseNativeDialog
         filename, _ = QFileDialog.getOpenFileName(self, 'Import Badger routines',
@@ -531,10 +574,10 @@
         if not ext:
             filename = filename + '.db'
 
         try:
             import_routines(filename)
 
             QMessageBox.information(
-                self, 'Success!', f'Import succeeded: imported all routines from {filename}')
+                self, 'Success!', f'Import success: imported all routines from {filename}')
         except Exception as e:
             QMessageBox.warning(self, 'Heads-up!', f'Failed to import the following routines since they already existed: \n{str(e)}')
```

### Comparing `badger-opt-1.0/src/badger/gui/default/windows/docs_window.py` & `badger_opt-1.0.2/src/badger/gui/default/windows/docs_window.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/windows/edit_script_dialog.py` & `badger_opt-1.0.2/src/badger/gui/default/windows/edit_script_dialog.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/windows/lim_vrange_dialog.py` & `badger_opt-1.0.2/src/badger/gui/default/windows/lim_vrange_dialog.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/windows/main_window.py` & `badger_opt-1.0.2/src/badger/gui/default/windows/main_window.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/windows/review_dialog.py` & `badger_opt-1.0.2/src/badger/gui/default/windows/review_dialog.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/windows/settings_dialog.py` & `badger_opt-1.0.2/src/badger/gui/default/windows/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/windows/terminition_condition_dialog.py` & `badger_opt-1.0.2/src/badger/gui/default/windows/terminition_condition_dialog.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/gui/default/windows/var_dialog.py` & `badger_opt-1.0.2/src/badger/gui/default/windows/var_dialog.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/interface.py` & `badger_opt-1.0.2/src/badger/interface.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/log.py` & `badger_opt-1.0.2/src/badger/log.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/logbook.py` & `badger_opt-1.0.2/src/badger/logbook.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,36 +13,41 @@
     raise BadgerConfigError('Please set the BADGER_LOGBOOK_ROOT env var!')
 elif not os.path.exists(BADGER_LOGBOOK_ROOT):
     os.makedirs(BADGER_LOGBOOK_ROOT)
     logger.info(
         f'Badger logbook root {BADGER_LOGBOOK_ROOT} created')
 
 
-def send_to_logbook(routine, data, widget=None):
+def send_to_logbook(routine, widget=None):
     from xml.etree import ElementTree
     from re import sub
 
-    obj_names = [next(iter(d))
-        for d in routine['config']['objectives']]
-
     log_text = ''
-    routine_name = routine['name']
-    generator_name = routine['generator']
+    routine_name = routine.name
+    generator_name = routine.generator.name
     data_path = BADGER_ARCHIVE_ROOT
-    obj_name = obj_names[0]
-    obj_start = data[obj_name][0]
-    obj_end = data[obj_name][-1]
-    duration = data['timestamp'][-1] - data['timestamp'][0]
+    obj_name = routine.vocs.objective_names[0]
+    env_name = routine.environment.name
+
+    idx_opt, obj_opt, _ = routine.vocs.select_best(routine.sorted_data, n=1)
+    idx_opt = int(idx_opt[0])
+    obj_opt = obj_opt[0]
+
+    data = routine.data
+    obj_start = data[obj_name].iloc[0]
+    duration = data['timestamp'].iloc[-1] - data['timestamp'].iloc[0]
     n_point = len(data['timestamp'])
     if n_point > 0:
-        log_text = f'Gain ({obj_name}): {round(obj_start, 4)} -> {round(obj_end, 4)}\n'
+        log_text = f'Gain ({obj_name}): {round(obj_start, 4)} -> {round(obj_opt, 4)}\n'
     log_text += f'Time cost: {round(duration, 2)}s\n'
     log_text += f'Points requested: {n_point}\n'
+    log_text += f'Optimal solution index: {idx_opt}\n'
     log_text += f'Routine name: {routine_name}\n'
-    log_text += f'Type of optimization: {generator_name}\n'
+    log_text += f'Environment name: {env_name}\n'
+    log_text += f'Optimization algorithm: {generator_name}\n'
     log_text += f'Data location: {data_path}\n'
     try:
         log_text += f'Log location: {BADGER_LOGBOOK_ROOT}\n'
     except:
         pass
 
     # Generate the xml data
```

### Comparing `badger-opt-1.0/src/badger/logger/__init__.py` & `badger_opt-1.0.2/src/badger/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/logger/observer.py` & `badger_opt-1.0.2/src/badger/logger/observer.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/logger/util.py` & `badger_opt-1.0.2/src/badger/logger/util.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/routine.py` & `badger_opt-1.0.2/src/badger/routine.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,18 @@
             if "data" in data:
                 if isinstance(data["data"], dict):
                     try:
                         data["data"] = pd.DataFrame(data["data"])
                     except IndexError:
                         data["data"] = pd.DataFrame(data["data"], index=[0])
 
-                    data["generator"].add_data(data["data"])
+                    # Add data one row at a time to avoid generator issues
+                    for i in range(len(data["data"])):
+                        row_df = data["data"].iloc[[i]]
+                        data["generator"].add_data(row_df)
 
             # instantiate env
             if isinstance(data["environment"], dict):
                 # TODO: Actually we need this interface info, but
                 # should be put somewhere else (in parallel with env?)
                 try:
                     del data["environment"]["interface"]
@@ -100,16 +103,17 @@
                 v = pd.DataFrame(v, index=[0])
 
         return v
 
     @property
     def sorted_data(self):
         data_copy = deepcopy(self.data)
-        data_copy.index = data_copy.index.astype(int)
-        data_copy.sort_index(inplace=True)
+        if data_copy is not None:
+            data_copy.index = data_copy.index.astype(int)
+            data_copy.sort_index(inplace=True)
 
         return data_copy
 
     def json(self, **kwargs) -> str:
         """Handle custom serialization of environment"""
 
         result = super().json(**kwargs)
```

### Comparing `badger-opt-1.0/src/badger/settings.py` & `badger_opt-1.0.2/src/badger/settings.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/stats.py` & `badger_opt-1.0.2/src/badger/stats.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/tests/conftest.py` & `badger_opt-1.0.2/src/badger/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/tests/mock/plugins/environments/multiobjective_test/__init__.py` & `badger_opt-1.0.2/src/badger/tests/mock/plugins/environments/multiobjective_test/__init__.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/tests/mock/plugins/environments/test/__init__.py` & `badger_opt-1.0.2/src/badger/tests/mock/plugins/environments/test/__init__.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/tests/mock/plugins/interfaces/test/__init__.py` & `badger_opt-1.0.2/src/badger/tests/mock/plugins/interfaces/test/__init__.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/tests/test_cli_basic.py` & `badger_opt-1.0.2/src/badger/tests/test_cli_basic.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,22 +30,26 @@
         _ = float(version)
         assert outlines[1] == f"version: '{version}'"
     except ValueError:
         assert outlines[1] == f'version: {version}'
 
 
 def test_list_algo():
+    from badger.factory import ALGO_EXCLUDED
+
     command = ['badger', 'generator']
     out, err, exitcode = capture(command)
 
     assert exitcode == 0
 
     # Check output lines
     outlines = out.splitlines()
-    assert '- upper_confidence_bound' in outlines
+    for algo in ['expected_improvement', 'neldermead', 'rcds']:
+        if algo not in ALGO_EXCLUDED:
+            assert f'- {algo}' in outlines
 
 
 # def test_cli_run(mock_config_root):
 #     command = ['badger', 'run', '-a', 'upper_confidence_bound', '-ap',
 #                '{max_evaluations: 10}',  '-e', 'silly', '-c',
 #                os.path.join(mock_config_root, 'test.yaml'), '-y']
 #     out, err, exitcode = capture(command)
```

### Comparing `badger-opt-1.0/src/badger/tests/test_core.py` & `badger_opt-1.0.2/src/badger/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/tests/test_db.py` & `badger_opt-1.0.2/src/badger/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/tests/test_env.py` & `badger_opt-1.0.2/src/badger/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/tests/test_environment.py` & `badger_opt-1.0.2/src/badger/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/tests/test_factory.py` & `badger_opt-1.0.2/src/badger/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/tests/test_home_page.py` & `badger_opt-1.0.2/src/badger/tests/test_home_page.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/tests/test_intf.py` & `badger_opt-1.0.2/src/badger/tests/test_intf.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/tests/test_lib_basic.py` & `badger_opt-1.0.2/src/badger/tests/test_lib_basic.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/tests/test_routine.py` & `badger_opt-1.0.2/src/badger/tests/test_routine.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger/tests/test_run_monitor.py` & `badger_opt-1.0.2/src/badger/tests/test_run_monitor.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import pytest
 import time
+import warnings
 from unittest.mock import patch
 
 import numpy as np
 
 from PyQt5.QtCore import QPointF, Qt, QTimer
 from PyQt5.QtGui import QMouseEvent
 from PyQt5.QtTest import QSignalSpy, QTest
@@ -25,14 +27,29 @@
 
     if add_data:
         assert len(routine.data) == 10
 
     return monitor
 
 
+def create_test_run_monitor_critical():
+    from badger.gui.default.components.run_monitor import BadgerOptMonitor
+    from badger.tests.utils import create_routine_critical, fix_db_path_issue
+
+    fix_db_path_issue()
+
+    monitor = BadgerOptMonitor()
+    monitor.testing = True
+
+    routine = create_routine_critical()
+    monitor.init_plots(routine)
+
+    return monitor
+
+
 def test_run_monitor(qtbot):
     from badger.gui.default.components.run_monitor import BadgerOptMonitor
     from badger.tests.utils import create_routine, fix_db_path_issue
 
     fix_db_path_issue()
 
     monitor = BadgerOptMonitor()
@@ -298,17 +315,17 @@
     curr_vars = get_current_vars(monitor.routine)
     assert np.all(curr_vars == last_vars)
 
     # Reset env and confirm
     spy = QSignalSpy(monitor.btn_reset.clicked)
 
     with patch("PyQt5.QtWidgets.QMessageBox.question", return_value=QMessageBox.Yes):
-        with patch("PyQt5.QtWidgets.QMessageBox.information") as mock_info:
-            qtbot.mouseClick(monitor.btn_reset, Qt.MouseButton.LeftButton)
-            mock_info.assert_called_once()
+        # with patch("PyQt5.QtWidgets.QMessageBox.information") as mock_info:
+        qtbot.mouseClick(monitor.btn_reset, Qt.MouseButton.LeftButton)
+        # mock_info.assert_called_once()
 
     assert len(spy) == 1
 
     # Check if the env has been reset
     curr_vars = get_current_vars(monitor.routine)
     assert np.all(curr_vars == init_vars)
 
@@ -319,39 +336,41 @@
     monitor = create_test_run_monitor()
 
     # Check if current env vars matches the last solution in data
     last_vars = get_vars_in_row(monitor.routine, idx=-1)
     curr_vars = get_current_vars(monitor.routine)
     assert np.all(curr_vars == last_vars)
 
-    # Dial in the solution at the inspector line (should be the first solution)
+    # Dial in the third solution
     current_x_view_range = monitor.plot_var.getViewBox().viewRange()[0]
 
+    monitor.inspector_objective.setValue(2)
+
     spy = QSignalSpy(monitor.btn_set.clicked)
     with patch("PyQt5.QtWidgets.QMessageBox.question", return_value=QMessageBox.Yes):
         qtbot.mouseClick(monitor.btn_set, Qt.MouseButton.LeftButton)
     assert len(spy) == 1
 
     new_x_view_range = monitor.plot_var.getViewBox().viewRange()[0]
 
     assert new_x_view_range != current_x_view_range
 
     # Test if the solution has been dialed in
-    first_vars = get_vars_in_row(monitor.routine, idx=0)
+    third_vars = get_vars_in_row(monitor.routine, idx=2)
     curr_vars = get_current_vars(monitor.routine)
-    assert np.all(curr_vars == first_vars)
+    assert np.all(curr_vars == third_vars)
 
-    monitor.plot_x_axis = False
+    # monitor.plot_x_axis = False
 
-    with patch("PyQt5.QtWidgets.QMessageBox.question", return_value=QMessageBox.Yes):
-        qtbot.mouseClick(monitor.btn_set, Qt.MouseButton.LeftButton)
+    # with patch("PyQt5.QtWidgets.QMessageBox.question", return_value=QMessageBox.Yes):
+    #     qtbot.mouseClick(monitor.btn_set, Qt.MouseButton.LeftButton)
 
-    not_time_x_view_range = monitor.plot_var.getViewBox().viewRange()[0]
+    # not_time_x_view_range = monitor.plot_var.getViewBox().viewRange()[0]
 
-    assert new_x_view_range != not_time_x_view_range
+    # assert new_x_view_range != not_time_x_view_range
 
 
 def test_run_until(qtbot):
     monitor = create_test_run_monitor(add_data=False)
 
     def handle_dialog():
         while monitor.tc_dialog is None:
@@ -402,7 +421,95 @@
     # assert isinstance(monitor.active_extensions[0], ParetoFrontViewer)
     # assert len(monitor.active_extensions) == 1
 
     # test closing window -- should remove element from active extensions
     # monitor.active_extensions[0].close()
     # assert len(monitor.active_extensions) == 0
     # assert monitor.extensions_palette.n_active_extensions == 0
+
+
+def test_critical_constraints(qtbot):
+    monitor = create_test_run_monitor_critical()
+
+    def handle_dialog():
+        while monitor.tc_dialog is None:
+            QApplication.processEvents()
+
+        # Set max evaluation to 5, then run the optimization
+        monitor.tc_dialog.sb_max_eval.setValue(5)
+
+        qtbot.mouseClick(monitor.tc_dialog.btn_run, Qt.MouseButton.LeftButton)
+
+    QTimer.singleShot(0, handle_dialog)
+    monitor.run_until_action.trigger()
+
+    # Check if critical violation alert being triggered
+    with patch("PyQt5.QtWidgets.QMessageBox.warning", return_value=QMessageBox.Yes):
+        # Have to keep it run to correctly trigger/dismiss the dialog
+        while monitor.running:
+            qtbot.wait(100)
+
+    assert len(monitor.routine.data) == 1  # early-termination due to violation
+
+
+def test_ucb_user_warning():
+    from badger.tests.utils import create_routine_constrained_ucb
+
+    with warnings.catch_warnings(record=True) as caught_warnings:
+        _ = create_routine_constrained_ucb()
+
+        # Check if the user warning is caught
+        assert len(caught_warnings) == 1
+        assert caught_warnings[0].category == UserWarning
+
+
+# Note: this test will delete all the previous runs
+# you might want to run this test last
+def test_del_last_run(qtbot):
+    from badger.gui.default.windows.main_window import BadgerMainWindow
+    from badger.tests.utils import fix_db_path_issue, create_routine
+
+    fix_db_path_issue()
+
+    window = BadgerMainWindow()
+    qtbot.addWidget(window)
+
+    # Run a routine
+    routine = create_routine()
+    home_page = window.home_page
+    home_page.current_routine = routine
+    monitor = home_page.run_monitor
+    monitor.testing = True
+    monitor.termination_condition = {
+        "tc_idx": 0,
+        "max_eval": 3,
+    }
+    home_page.go_run(-1)
+    monitor.start(True)
+    while monitor.running:
+        qtbot.wait(100)
+
+    # Variables/objectives/constraints monitor should contain some data
+    assert len(monitor.plot_var.items) > 0
+    assert len(monitor.plot_obj.items) > 0
+    assert len(monitor.plot_con.items) > 0
+
+    # Delete all the runs and check if the monitors have been cleared
+    with patch("PyQt5.QtWidgets.QMessageBox.question",
+               return_value=QMessageBox.Yes):
+        while home_page.cb_history.count():
+            qtbot.mouseClick(monitor.btn_del, Qt.MouseButton.LeftButton)
+
+    # Should have no constraints/observables monitor
+    with pytest.raises(AttributeError):
+        _ = monitor.plot_con
+    with pytest.raises(AttributeError):
+        _ = monitor.plot_obs
+    # Variables/objectives monitor should be cleared
+    assert len(monitor.plot_var.items) == 0
+    assert len(monitor.plot_obj.items) == 0
+
+
+# TODO: Test if logbook entry is created correctly and put into the
+# correct location when the logbook button is clicked
+def test_send_to_logbook(qtbot):
+    pass
```

### Comparing `badger-opt-1.0/src/badger/tests/utils.py` & `badger_opt-1.0.2/src/badger/tests/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
 
 def create_routine_turbo():
     from badger.routine import Routine
 
     test_routine = {
         "name": "routine-for-turbo-test",
-        "generator": "upper_confidence_bound",
+        "generator": "expected_improvement",
         "env": "test",
         "generator_params": {
             "turbo_controller": "optimize",
             "gp_constructor": {
                 "name": "standard",
                 "use_low_noise_prior": True,
             },
@@ -125,14 +125,103 @@
         vocs=vocs,
         generator=generator,
         environment={"name": "test"},
         initial_points=pd.DataFrame(test_routine["config"]["init_points"])
     )
 
 
+def create_routine_critical():
+    from badger.routine import Routine
+
+    test_routine = {
+        "name": "routine-for-critical-test",
+        "generator": "random",
+        "env": "test",
+        "generator_params": {},
+        "env_params": {},
+        "vocs": {
+            "variables": {
+                "x0": [-1, 1],
+                "x1": [-1, 1],
+                "x2": [-1, 1],
+                "x3": [-1, 1]
+            },
+            "objectives": {"f": "MAXIMIZE"},
+            "constraints": {"c": ["LESS_THAN", 0]}
+        },
+        "init_points": {
+            "x0": [0.5],
+            "x1": [0.5],
+            "x2": [0.5],
+            "x3": [0.5]
+        },
+    }
+
+    vocs = VOCS(**test_routine["vocs"])
+
+    generator = RandomGenerator(vocs=vocs)
+
+    return Routine(
+        name="test",
+        vocs=vocs,
+        generator=generator,
+        environment={"name": "test"},
+        initial_points=pd.DataFrame(test_routine["init_points"]),
+        critical_constraint_names=["c"]
+    )
+
+
+def create_routine_constrained_ucb():
+    from badger.routine import Routine
+
+    test_routine = {
+        "name": "routine-for-ucb-cons-test",
+        "generator": "expected_improvement",
+        "env": "test",
+        "generator_params": {
+            "turbo_controller": "optimize",
+            "gp_constructor": {
+                "name": "standard",
+                "use_low_noise_prior": True,
+            },
+            "beta": 2.0,
+        },
+        "env_params": {},
+        "vocs": {
+            "variables": {
+                "x0": [-1, 1],
+                "x1": [-1, 1],
+                "x2": [-1, 1],
+                "x3": [-1, 1]
+            },
+            "objectives": {"f": "MAXIMIZE"},
+            "constraints": {"c": ["GREATER_THAN", 0]}
+        },
+        "init_points": {
+            "x0": [0.5],
+            "x1": [0.5],
+            "x2": [0.5],
+            "x3": [0.5]
+        },
+    }
+
+    vocs = VOCS(**test_routine["vocs"])
+
+    generator = UpperConfidenceBoundGenerator(
+        vocs=vocs, **test_routine["generator_params"])
+
+    return Routine(
+        name="test",
+        vocs=vocs,
+        generator=generator,
+        environment={"name": "test"},
+        initial_points=pd.DataFrame(test_routine["init_points"])
+    )
+
+
 def fix_db_path_issue():
     from badger.db import BADGER_DB_ROOT
 
     os.makedirs(BADGER_DB_ROOT, exist_ok=True)
 
 
 def get_current_vars(routine):
```

### Comparing `badger-opt-1.0/src/badger/utils.py` & `badger_opt-1.0.2/src/badger/utils.py`

 * *Files identical despite different names*

### Comparing `badger-opt-1.0/src/badger_opt.egg-info/PKG-INFO` & `badger_opt-1.0.2/src/badger_opt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badger-opt
-Version: 1.0
+Version: 1.0.2
 Summary: Core of the Badger optimizer
 Home-page: https://github.com/SLAC-ML/Badger
 Author: Zhe Zhang
 Author-email: zhezhang@slac.stanford.edu
 License: GPL
 Requires-Python: >=3.9
 License-File: LICENSE
```

### Comparing `badger-opt-1.0/src/badger_opt.egg-info/SOURCES.txt` & `badger_opt-1.0.2/src/badger_opt.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -85,18 +85,20 @@
 src/badger/gui/default/images/stop.png
 src/badger/gui/default/images/tools.png
 src/badger/gui/default/images/trash.png
 src/badger/gui/default/images/undo.png
 src/badger/gui/default/pages/__init__.py
 src/badger/gui/default/pages/home_page.py
 src/badger/gui/default/windows/__init__.py
+src/badger/gui/default/windows/add_random_dialog.py
 src/badger/gui/default/windows/docs_window.py
 src/badger/gui/default/windows/edit_script_dialog.py
 src/badger/gui/default/windows/lim_vrange_dialog.py
 src/badger/gui/default/windows/main_window.py
+src/badger/gui/default/windows/message_dialog.py
 src/badger/gui/default/windows/review_dialog.py
 src/badger/gui/default/windows/settings_dialog.py
 src/badger/gui/default/windows/terminition_condition_dialog.py
 src/badger/gui/default/windows/var_dialog.py
 src/badger/logger/__init__.py
 src/badger/logger/event.py
 src/badger/logger/observer.py
```

### Comparing `badger-opt-1.0/versioneer.py` & `badger_opt-1.0.2/versioneer.py`

 * *Files identical despite different names*

