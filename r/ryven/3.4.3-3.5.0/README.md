# Comparing `tmp/ryven-3.4.3.tar.gz` & `tmp/ryven-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryven-3.4.3.tar", last modified: Fri Oct 27 21:53:02 2023, max compression
+gzip compressed data, was "ryven-3.5.0.tar", last modified: Mon May 20 15:51:22 2024, max compression
```

## Comparing `ryven-3.4.3.tar` & `ryven-3.5.0.tar`

### file list

```diff
@@ -1,205 +1,213 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:02.978658 ryven-3.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-10-27 21:52:50.000000 ryven-3.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      405 2023-10-27 21:52:50.000000 ryven-3.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      640 2023-10-27 21:53:02.978658 ryven-3.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       99 2023-10-27 21:52:50.000000 ryven-3.4.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:02.946657 ryven-3.4.3/ryven/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:02.942657 ryven-3.4.3/ryven/example_nodes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:02.946657 ryven-3.4.3/ryven/example_nodes/OpenCV/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/example_nodes/OpenCV/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    37537 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/example_nodes/OpenCV/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6103 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/example_nodes/OpenCV/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:02.946657 ryven-3.4.3/ryven/example_nodes/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/example_nodes/linalg/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/example_nodes/linalg/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/example_nodes/linalg/nodes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:02.946657 ryven-3.4.3/ryven/example_nodes/std/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/example_nodes/std/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/example_nodes/std/basic_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/example_nodes/std/control_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)    15986 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/example_nodes/std/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/example_nodes/std/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    17061 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/example_nodes/std/special_nodes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:02.950657 ryven-3.4.3/ryven/examples_projects/
--rw-r--r--   0 runner    (1001) docker     (127)    63369 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/examples_projects/basics.json
--rw-r--r--   0 runner    (1001) docker     (127)    40944 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/examples_projects/matrices.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:02.950657 ryven-3.4.3/ryven/gui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:02.950657 ryven-3.4.3/ryven/gui/code_editor/
--rw-r--r--   0 runner    (1001) docker     (127)     4103 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/gui/code_editor/CodeEditorWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     9118 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/gui/code_editor/CodePreviewWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/gui/code_editor/EditSrcCodeInfoDialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4407 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/gui/code_editor/SourceCodeUpdater.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/gui/code_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/gui/code_editor/codes_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:02.950657 ryven-3.4.3/ryven/gui/code_editor/pygments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/gui/code_editor/pygments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/gui/code_editor/pygments/dracula.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/gui/code_editor/pygments/light.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/gui/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/gui/flow_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)    10700 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/gui/main_console.py
--rw-r--r--   0 runner    (1001) docker     (127)    16256 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/gui/main_window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:02.950657 ryven-3.4.3/ryven/gui/startup_dialog/
--rw-r--r--   0 runner    (1001) docker     (127)    27649 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/gui/startup_dialog/StartupDialog.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/gui/startup_dialog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11684 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/gui/std_input_widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:02.950657 ryven-3.4.3/ryven/gui/styling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/gui/styling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3363 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/gui/styling/design_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/gui/styling/window_theme.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:02.950657 ryven-3.4.3/ryven/gui/uic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/gui/uic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/gui/uic/flow.ui
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/gui/uic/main_window.ui
--rw-r--r--   0 runner    (1001) docker     (127)     5290 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/gui/uic/ui_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)    10872 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/gui/uic/ui_main_window.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/gui_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:02.950657 ryven-3.4.3/ryven/main/
--rw-r--r--   0 runner    (1001) docker     (127)     7214 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/main/Ryven.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/main/RyvenConsole.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17755 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/main/args_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/main/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:02.954657 ryven-3.4.3/ryven/main/packages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/main/packages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:02.954657 ryven-3.4.3/ryven/main/packages/built_in/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/main/packages/built_in/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5417 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/main/packages/built_in/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     6956 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/main/packages/built_in/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/main/packages/gui_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/main/packages/node_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     7393 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/main/packages/nodes_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     7355 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/main/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/node_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:02.942657 ryven-3.4.3/ryven/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:02.954657 ryven-3.4.3/ryven/resources/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:02.954657 ryven-3.4.3/ryven/resources/fonts/asap/
--rw-r--r--   0 runner    (1001) docker     (127)   102416 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/asap/Asap-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   111664 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/asap/Asap-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   109800 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/asap/Asap-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   102444 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/asap/Asap-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   111808 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/asap/Asap-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   101032 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/asap/Asap-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   102688 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/asap/Asap-SemiBold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   112712 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/asap/Asap-SemiBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/asap/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/asap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:02.962657 ryven-3.4.3/ryven/resources/fonts/poppins/
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/poppins/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (127)   138520 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-Black.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   155420 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-BlackItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   140724 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   159688 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   139684 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-ExtraBold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   158172 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-ExtraBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   147416 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-ExtraLight.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   170376 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-ExtraLightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   166604 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   145936 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   168408 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   142980 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   164976 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   144776 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   141612 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-SemiBold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   161360 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-SemiBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   148440 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-Thin.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   171772 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-ThinItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/poppins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:02.970657 ryven-3.4.3/ryven/resources/fonts/source_code_pro/
--rw-r--r--   0 runner    (1001) docker     (127)     4528 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/source_code_pro/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (127)   191284 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/source_code_pro/SourceCodePro-Black.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   155056 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/source_code_pro/SourceCodePro-BlackItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   191568 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/source_code_pro/SourceCodePro-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   155288 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/source_code_pro/SourceCodePro-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   193360 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/source_code_pro/SourceCodePro-ExtraLight.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   156884 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/source_code_pro/SourceCodePro-ExtraLightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   161376 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/source_code_pro/SourceCodePro-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   193160 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/source_code_pro/SourceCodePro-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   156984 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/source_code_pro/SourceCodePro-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   191984 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/source_code_pro/SourceCodePro-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   156156 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/source_code_pro/SourceCodePro-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   192740 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/source_code_pro/SourceCodePro-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   191792 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/source_code_pro/SourceCodePro-SemiBold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   155568 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/source_code_pro/SourceCodePro-SemiBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/fonts/source_code_pro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:02.970657 ryven-3.4.3/ryven/resources/pics/
--rw-r--r--   0 runner    (1001) docker     (127)    61897 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/pics/Ryven_icon.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   391573 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/pics/Ryven_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)   786058 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/pics/Ryven_icon_blurred.png
--rw-r--r--   0 runner    (1001) docker     (127)    46855 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/pics/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:02.970657 ryven-3.4.3/ryven/resources/stylesheets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:02.974657 ryven-3.4.3/ryven/resources/stylesheets/icons/
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/branch-closed.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/branch-end.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4043 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/branch-more.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/branch-open.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/checkbox_checked.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4412 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/checkbox_indeterminate.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/checkbox_unchecked.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/close.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/downarrow.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/downarrow2.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3750 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/float.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/leftarrow.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/leftarrow2.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:02.978658 ryven-3.4.3/ryven/resources/stylesheets/icons/orig/
--rw-r--r--   0 runner    (1001) docker     (127)     7477 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/orig/base.svg
--rw-r--r--   0 runner    (1001) docker     (127)     8852 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/orig/branch-closed.svg
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/orig/branch-end.svg
--rw-r--r--   0 runner    (1001) docker     (127)     8525 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/orig/branch-more.svg
--rw-r--r--   0 runner    (1001) docker     (127)     9148 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/orig/branch-open.svg
--rw-r--r--   0 runner    (1001) docker     (127)     8691 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/orig/checkbox_checked.svg
--rw-r--r--   0 runner    (1001) docker     (127)     8910 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/orig/checkbox_indeterminate.svg
--rw-r--r--   0 runner    (1001) docker     (127)     8619 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/orig/checkbox_unchecked.svg
--rw-r--r--   0 runner    (1001) docker     (127)     8056 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/orig/close.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7801 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/orig/downarrow.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/orig/downarrow2.svg
--rw-r--r--   0 runner    (1001) docker     (127)     8239 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/orig/float.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7797 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/orig/leftarrow.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/orig/leftarrow2.svg
--rw-r--r--   0 runner    (1001) docker     (127)     8522 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/orig/radiobutton_checked.svg
--rw-r--r--   0 runner    (1001) docker     (127)     8215 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/orig/radiobutton_unchecked.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7800 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/orig/rightarrow.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/orig/rightarrow2.svg
--rw-r--r--   0 runner    (1001) docker     (127)    10503 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/orig/sizegrip.svg
--rw-r--r--   0 runner    (1001) docker     (127)     8109 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/orig/slider.svg
--rw-r--r--   0 runner    (1001) docker     (127)     9268 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/orig/splitter-horizontal.svg
--rw-r--r--   0 runner    (1001) docker     (127)     9323 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/orig/splitter-vertical.svg
--rw-r--r--   0 runner    (1001) docker     (127)     8050 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/orig/tab_close.svg
--rw-r--r--   0 runner    (1001) docker     (127)    11390 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/orig/toolbar-handle-horizontal.svg
--rw-r--r--   0 runner    (1001) docker     (127)    11636 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/orig/toolbar-handle-vertical.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7797 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/orig/uparrow.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/orig/uparrow2.svg
--rw-r--r--   0 runner    (1001) docker     (127)     8027 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/orig/vline.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/radiobutton_checked.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/radiobutton_unchecked.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/rightarrow.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/rightarrow2.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6014 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/sizegrip.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/slider.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/splitter-horizontal.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/splitter-vertical.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/tab_close.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6903 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/toolbar-handle-horizontal.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7149 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/toolbar-handle-vertical.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/uparrow.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/uparrow2.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/icons/vline.svg
--rw-r--r--   0 runner    (1001) docker     (127)    22441 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/resources/stylesheets/style_template.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:02.978658 ryven-3.4.3/ryven/unused/
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/unused/EditVal_Dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/unused/NodeDetailsWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/unused/NodesTreeListWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)   574832 2023-10-27 21:52:50.000000 ryven-3.4.3/ryven/unused/test.stl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:02.946657 ryven-3.4.3/ryven.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2023-10-27 21:53:02.000000 ryven-3.4.3/ryven.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7805 2023-10-27 21:53:02.000000 ryven-3.4.3/ryven.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-27 21:53:02.000000 ryven-3.4.3/ryven.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-10-27 21:53:02.000000 ryven-3.4.3/ryven.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-10-27 21:53:02.000000 ryven-3.4.3/ryven.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-10-27 21:53:02.000000 ryven-3.4.3/ryven.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      809 2023-10-27 21:53:02.978658 ryven-3.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      800 2023-10-27 21:52:50.000000 ryven-3.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:22.442077 ryven-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-20 15:51:15.000000 ryven-3.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-20 15:51:15.000000 ryven-3.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-20 15:51:22.442077 ryven-3.5.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:22.402077 ryven-3.5.0/ryven/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:22.398077 ryven-3.5.0/ryven/example_nodes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:22.402077 ryven-3.5.0/ryven/example_nodes/OpenCV/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/example_nodes/OpenCV/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    37537 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/example_nodes/OpenCV/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/example_nodes/OpenCV/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:22.402077 ryven-3.5.0/ryven/example_nodes/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/example_nodes/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/example_nodes/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/example_nodes/examples/basic_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/example_nodes/examples/control_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16458 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/example_nodes/examples/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/example_nodes/examples/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17174 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/example_nodes/examples/special_nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:22.406077 ryven-3.5.0/ryven/example_nodes/inspector_example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/example_nodes/inspector_example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/example_nodes/inspector_example/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/example_nodes/inspector_example/nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:22.406077 ryven-3.5.0/ryven/example_nodes/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/example_nodes/linalg/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/example_nodes/linalg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/example_nodes/linalg/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11370 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/example_nodes/linalg/matrices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/example_nodes/linalg/nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:22.406077 ryven-3.5.0/ryven/example_projects/
+-rw-r--r--   0 runner    (1001) docker     (127)    72609 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/example_projects/basics.json
+-rw-r--r--   0 runner    (1001) docker     (127)    43593 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/example_projects/matrices.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:22.406077 ryven-3.5.0/ryven/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:22.406077 ryven-3.5.0/ryven/gui/code_editor/
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/gui/code_editor/CodeEditorWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10859 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/gui/code_editor/CodePreviewWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/gui/code_editor/EditSrcCodeInfoDialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/gui/code_editor/SourceCodeUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/gui/code_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/gui/code_editor/codes_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:22.410077 ryven-3.5.0/ryven/gui/code_editor/pygments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/gui/code_editor/pygments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/gui/code_editor/pygments/dracula.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/gui/code_editor/pygments/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/gui/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/gui/flow_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10826 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/gui/main_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23459 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/gui/main_window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:22.410077 ryven-3.5.0/ryven/gui/startup_dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)    29064 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/gui/startup_dialog/StartupDialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/gui/startup_dialog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11659 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/gui/std_input_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:22.410077 ryven-3.5.0/ryven/gui/styling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/gui/styling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/gui/styling/design_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/gui/styling/window_theme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:22.410077 ryven-3.5.0/ryven/gui/uic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/gui/uic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/gui/uic/flow.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/gui/uic/flow_window.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     7963 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/gui/uic/main_window.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/gui/uic/ui_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5496 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/gui/uic/ui_flow_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/gui/uic/ui_main_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/gui_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:22.410077 ryven-3.5.0/ryven/main/
+-rw-r--r--   0 runner    (1001) docker     (127)     8658 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/main/Ryven.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/main/RyvenConsole.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18131 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/main/args_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/main/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:22.414077 ryven-3.5.0/ryven/main/packages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/main/packages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:22.414077 ryven-3.5.0/ryven/main/packages/built_in/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/main/packages/built_in/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/main/packages/built_in/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/main/packages/built_in/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/main/packages/gui_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/main/packages/node_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/main/packages/nodes_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8877 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/main/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/node_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:22.398077 ryven-3.5.0/ryven/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:22.414077 ryven-3.5.0/ryven/resources/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:22.414077 ryven-3.5.0/ryven/resources/fonts/asap/
+-rw-r--r--   0 runner    (1001) docker     (127)   102416 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/asap/Asap-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   111664 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/asap/Asap-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   109800 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/asap/Asap-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   102444 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/asap/Asap-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   111808 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/asap/Asap-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   101032 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/asap/Asap-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   102688 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/asap/Asap-SemiBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   112712 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/asap/Asap-SemiBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/asap/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/asap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:22.422077 ryven-3.5.0/ryven/resources/fonts/poppins/
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/poppins/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   138520 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-Black.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   155420 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-BlackItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   140724 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   159688 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   139684 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-ExtraBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   158172 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-ExtraBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   147416 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-ExtraLight.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   170376 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-ExtraLightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   166604 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   145936 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   168408 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   142980 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   164976 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   144776 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   141612 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-SemiBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   161360 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-SemiBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   148440 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-Thin.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   171772 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-ThinItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/poppins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:22.426077 ryven-3.5.0/ryven/resources/fonts/source_code_pro/
+-rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/source_code_pro/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   191284 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/source_code_pro/SourceCodePro-Black.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   155056 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/source_code_pro/SourceCodePro-BlackItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   191568 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/source_code_pro/SourceCodePro-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   155288 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/source_code_pro/SourceCodePro-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   193360 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/source_code_pro/SourceCodePro-ExtraLight.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   156884 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/source_code_pro/SourceCodePro-ExtraLightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   161376 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/source_code_pro/SourceCodePro-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   193160 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/source_code_pro/SourceCodePro-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   156984 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/source_code_pro/SourceCodePro-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   191984 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/source_code_pro/SourceCodePro-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   156156 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/source_code_pro/SourceCodePro-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   192740 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/source_code_pro/SourceCodePro-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   191792 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/source_code_pro/SourceCodePro-SemiBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   155568 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/source_code_pro/SourceCodePro-SemiBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/fonts/source_code_pro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:22.430077 ryven-3.5.0/ryven/resources/pics/
+-rw-r--r--   0 runner    (1001) docker     (127)    61897 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/pics/Ryven_icon.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   391573 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/pics/Ryven_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)   786058 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/pics/Ryven_icon_blurred.png
+-rw-r--r--   0 runner    (1001) docker     (127)    46855 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/pics/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:22.430077 ryven-3.5.0/ryven/resources/stylesheets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:22.434077 ryven-3.5.0/ryven/resources/stylesheets/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/branch-closed.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/branch-end.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/branch-more.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/branch-open.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/checkbox_checked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/checkbox_indeterminate.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/checkbox_unchecked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/close.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/downarrow.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/downarrow2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/float.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/leftarrow.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/leftarrow2.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:22.442077 ryven-3.5.0/ryven/resources/stylesheets/icons/orig/
+-rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/orig/base.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8852 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/orig/branch-closed.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/orig/branch-end.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8525 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/orig/branch-more.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     9148 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/orig/branch-open.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8691 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/orig/checkbox_checked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8910 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/orig/checkbox_indeterminate.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8619 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/orig/checkbox_unchecked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/orig/close.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/orig/downarrow.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/orig/downarrow2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/orig/float.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7797 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/orig/leftarrow.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/orig/leftarrow2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8522 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/orig/radiobutton_checked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/orig/radiobutton_unchecked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7800 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/orig/rightarrow.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/orig/rightarrow2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/orig/sizegrip.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/orig/slider.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     9268 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/orig/splitter-horizontal.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/orig/splitter-vertical.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8050 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/orig/tab_close.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11390 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/orig/toolbar-handle-horizontal.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11636 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/orig/toolbar-handle-vertical.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7797 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/orig/uparrow.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/orig/uparrow2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/orig/vline.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/radiobutton_checked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/radiobutton_unchecked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/rightarrow.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/rightarrow2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/sizegrip.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/slider.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/splitter-horizontal.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/splitter-vertical.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/tab_close.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6903 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/toolbar-handle-horizontal.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/toolbar-handle-vertical.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/uparrow.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/uparrow2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/icons/vline.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    22460 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/resources/stylesheets/style_template.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:22.442077 ryven-3.5.0/ryven/unused/
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/unused/EditVal_Dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/unused/NodeDetailsWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/unused/NodesTreeListWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)   574832 2024-05-20 15:51:15.000000 ryven-3.5.0/ryven/unused/test.stl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:22.442077 ryven-3.5.0/ryven.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-20 15:51:22.000000 ryven-3.5.0/ryven.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8140 2024-05-20 15:51:22.000000 ryven-3.5.0/ryven.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 15:51:22.000000 ryven-3.5.0/ryven.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-20 15:51:22.000000 ryven-3.5.0/ryven.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-20 15:51:22.000000 ryven-3.5.0/ryven.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 15:51:22.000000 ryven-3.5.0/ryven.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-20 15:51:22.442077 ryven-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-20 15:51:15.000000 ryven-3.5.0/setup.py
```

### Comparing `ryven-3.4.3/LICENSE` & `ryven-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/PKG-INFO` & `ryven-3.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: ryven
-Version: 3.4.3
+Version: 3.5.0
 Summary: Flow-based visual scripting for Python
 Home-page: https://github.com/leon-thomm/Ryven
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
-Requires-Dist: ryvencore-qt==0.4.*
-Requires-Dist: ryvencore==0.4.*
+Requires-Dist: ryvencore-qt==0.5.*
+Requires-Dist: ryvencore==0.5.*
 Requires-Dist: Jinja2
 Requires-Dist: Pygments
 Requires-Dist: textdistance
 Requires-Dist: packaging
```

### Comparing `ryven-3.4.3/ryven/example_nodes/OpenCV/nodes.py` & `ryven-3.5.0/ryven/example_nodes/OpenCV/nodes.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/example_nodes/OpenCV/widgets.py` & `ryven-3.5.0/ryven/example_nodes/OpenCV/widgets.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/example_nodes/linalg/gui.py` & `ryven-3.5.0/ryven/example_nodes/linalg/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from ryven.gui_env import *
+import numpy as np
 
 from qtpy.QtWidgets import QTextEdit
 from qtpy.QtGui import QFontMetrics
 
-import numpy as np
+from ryven.gui_env import *
 
+from . import matrices as nodes
 
 class MatrixWidget(NodeMainWidget, QTextEdit):
 
     def __init__(self, params, base_width=50, base_height=50):
         NodeMainWidget.__init__(self, params)
         QTextEdit.__init__(self)
 
@@ -122,30 +123,15 @@
     def set_state(self, data):
         self.setText(data['text'])
         self.resize_to_content(data['text'].splitlines())
         if not data['shown']:
             self.hide()
 
 
-class EditMatrixWidget(MatrixWidget):
-    def __init__(self, params):
-        super().__init__(params, 100, 80)
-
-        self.setReadOnly(False)
-        self.textChanged.connect(self.text_changed)
-
-    def text_changed(self):
-        self.node.parse_matrix(self.toPlainText())
-        self.resize_to_content(lines=self.toPlainText().splitlines())
-
-    def focusOutEvent(self, e):
-        self.update_matrix(self.node.expression_matrix)
-        QTextEdit.focusOutEvent(self, e)
-
-
+@node_gui(nodes.MatrixNodeBase)
 class MatrixNodeBaseGui(NodeGUI):
     main_widget_class = MatrixWidget
     main_widget_pos = 'below ports'
     color = '#3344ff'
 
     def __init__(self, params):
         super().__init__(params)
@@ -182,17 +168,28 @@
     def set_state(self, data):
         super().set_state(data)
         if data['main_widget_hidden']:
             self.ac_hide_mw()
         # shown by default
 
 
+class EditMatrixWidget(MatrixWidget):
+    def __init__(self, params):
+        super().__init__(params, 100, 80)
+
+        self.setReadOnly(False)
+        self.textChanged.connect(self.text_changed)
+
+    def text_changed(self):
+        self.node.parse_matrix(self.toPlainText())
+        self.resize_to_content(lines=self.toPlainText().splitlines())
+
+    def focusOutEvent(self, e):
+        self.update_matrix(self.node.expression_matrix)
+        QTextEdit.focusOutEvent(self, e)
+
+
+@node_gui(nodes.EditMatrixNode)
 class EditMatrixNodeGui(MatrixNodeBaseGui):
     main_widget_class = EditMatrixWidget
     main_widget_pos = 'below ports'
     color = '#3344ff'
-
-
-export_guis([
-    MatrixNodeBaseGui,
-    EditMatrixNodeGui,
-])
```

### Comparing `ryven-3.4.3/ryven/example_nodes/linalg/nodes.py` & `ryven-3.5.0/ryven/example_nodes/linalg/matrices.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
+import numpy as np
+from itertools import chain
 from typing import Optional, List
 
 import ryvencore.addons.Variables
 
 from ryven.node_env import *
-guis = import_guis(__file__)
-
-import numpy as np
-from itertools import chain
 
 
 class MatrixData(Data):
     # currently, there should not be any implicit
     # data sharing between nodes, because their
     # operations are copying the data anyway
 
@@ -23,22 +21,21 @@
     """
     Base class for nodes handling matrices.
     It implements basic forward propagation of a mutated matrix,
     defined by some operation in the get_mat() method, and a GUI
     for displaying the matrix.
     """
 
-    version = 'v0.2'
+    version = 'v0.3'
     init_inputs = [
         NodeInputType()
     ]
     init_outputs = [
         NodeOutputType()
     ]
-    GUI = guis.MatrixNodeBaseGui
 
     def __init__(self, params):
         super().__init__(params)
         self.mat = None
 
     def get_mat(self):
         """
@@ -301,15 +298,14 @@
     title = 'Matrix'
     identifier = 'EditMatrix_Node'
     legacy_identifiers = ['Matrix_Node', 'linalg.Matrix_Node']
     init_inputs = []
     init_outputs = [
         NodeOutputType()
     ]
-    GUI = guis.EditMatrixNodeGui
 
     def __init__(self, params):
         super().__init__(params)
 
         self.expression_matrix: Optional[np.ndarray] = None
         self.evaluated_matrix: Optional[MatrixData] = None
 
@@ -435,33 +431,34 @@
         return data
 
     def set_state(self, data, version):
         self.expression_matrix = deserialize(data['expression matrix'])
         self.register_vars_and_eval_matrix()
 
 
-export_nodes([
-    EditMatrixNode,
-    ShowMatrix,
-    Conjugate,
-    Transpose,
-    DetOfMatrix,
-    DotProduct,
-    HermMatrix,
-    IDMatrix,
-    ImagMatrix,
-    RealMatrix,
-    InnerProduct,
-    OuterProduct,
-    InverseMatrix,
-    KronMatrix,
-    MaskLower,
-    MaskUpper,
-    MatMul,
-    MatPower,
-    NullMatrix,
-    OnesMatrix,
-    RandomMatrix,
-    SolveLEq,
-],
+export_nodes(
+    node_types=[
+        EditMatrixNode,
+        ShowMatrix,
+        Conjugate,
+        Transpose,
+        DetOfMatrix,
+        DotProduct,
+        HermMatrix,
+        IDMatrix,
+        ImagMatrix,
+        RealMatrix,
+        InnerProduct,
+        OuterProduct,
+        InverseMatrix,
+        KronMatrix,
+        MaskLower,
+        MaskUpper,
+        MatMul,
+        MatPower,
+        NullMatrix,
+        OnesMatrix,
+        RandomMatrix,
+        SolveLEq,
+    ],
     data_types=[MatrixData]
 )
```

### Comparing `ryven-3.4.3/ryven/example_nodes/std/basic_operators.py` & `ryven-3.5.0/ryven/example_nodes/examples/basic_operators.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 from ryven.node_env import *
 
-guis = import_guis(__file__)
-
 
 class OperatorNodeBase(Node):
     """
     Base class for nodes implementing a binary operation.
     """
 
-    version = 'v0.2'
+    version = 'v0.3'
     init_inputs = [
         NodeInputType(),
         NodeInputType(),
     ]
     init_outputs = [
         NodeOutputType(),
     ]
-    GUI = guis.OperatorNodeBaseGui
 
     def __init__(self, params):
         super().__init__(params)
 
         self.num_inputs = 0
 
     def place_event(self):
@@ -46,15 +43,15 @@
 
 """
     logical operators
 """
 
 
 class LogicNodeBase(OperatorNodeBase):
-    GUI = guis.LogicNodeBaseGui
+    pass
 
 
 class NOT_Node(LogicNodeBase):
     title = 'not'
 
     def apply_op(self, elements: list):
         return all([not bool(e) for e in elements])
@@ -119,15 +116,15 @@
 
 """
     arithmetic operators
 """
 
 
 class ArithmeticNodeBase(OperatorNodeBase):
-    GUI = guis.ArithNodeBaseGui
+    pass
 
 
 class Plus_Node(ArithmeticNodeBase):
     title = '+'
 
     def apply_op(self, elements: list):
         v = elements[0]
@@ -190,15 +187,14 @@
 
 """
     comparison operators
 """
 
 
 class ComparatorNodeBase(OperatorNodeBase):
-    GUI = guis.CompNodeBaseGui
 
     def apply_op(self, elements: list):
         # if len(elements) > 0:
         b = True
         for i in range(1, len(elements)):
             b = b and (self.comp(elements[i-1], elements[i]))
         return b
@@ -260,13 +256,24 @@
 ]
 
 
 """
     export
 """
 
-
-nodes = [
+node_types = [
     *logic_nodes,
     *arithmetic_nodes,
     *comparator_nodes,
 ]
+
+# account for old package name
+for n in node_types:
+    n.legacy_identifiers = [
+        *getattr(n, 'legacy_identifiers', []),
+        f'std.{n.__class__.__name__}',
+    ]
+
+export_nodes(
+    node_types=node_types,
+    sub_pkg_name='basic_operators'
+)
```

### Comparing `ryven-3.4.3/ryven/example_nodes/std/control_structures.py` & `ryven-3.5.0/ryven/example_nodes/examples/control_structures.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from ryven.node_env import *
 
-guis = import_guis(__file__)
-
 
 class CSNodeBase(Node):
-    version = 'v0.2'
-    GUI = guis.CSNodeBaseGui
+    version = 'v0.3'
+
 
 class If_Node(CSNodeBase):
     title = 'branch'
     init_inputs = [
         NodeInputType(type_='exec'),
         NodeInputType(label='cond'),
     ]
@@ -36,15 +34,14 @@
         NodeInputType(label='to'),
     ]
     init_outputs = [
         NodeOutputType('loop', type_='exec'),
         NodeOutputType('i', type_='data'),
         NodeOutputType('finished', type_='exec'),
     ]
-    GUI = guis.ForLoopGui
 
     def __init__(self, params):
         super().__init__(params)
 
         self.dims = 1
 
     def add_dimension(self):
@@ -99,15 +96,14 @@
         NodeInputType(label='elements'),
     ]
     init_outputs = [
         NodeOutputType('loop', type_='exec'),
         NodeOutputType('e', type_='data'),
         NodeOutputType('finished', type_='exec'),
     ]
-    GUI = guis.ForEachLoopGui
 
     def update_event(self, inp=-1):
         for e in self.input(0).payload:
             self.set_output_val(1, e)
             self.exec_output(0)
 
         self.exec_output(2)
@@ -144,15 +140,26 @@
 
     def update_event(self, inp=-1):
         self.exec_output(0)
         while self.input(0).payload:
             self.exec_output(0)
         self.exec_output(1)
 
-
-nodes = [
+node_types = [
     If_Node,
     ForLoop_Node,
     ForEachLoop_Node,
     WhileLoop_Node,
     DoWhileLoop_Node,
 ]
+
+# account for old package name
+for n in node_types:
+    n.legacy_identifiers = [
+        *getattr(n, 'legacy_identifiers', []),
+        f'std.{n.__class__.__name__}',
+    ]
+
+export_nodes(
+    node_types=node_types,
+    sub_pkg_name='control_structures'
+)
```

### Comparing `ryven-3.4.3/ryven/example_nodes/std/gui.py` & `ryven-3.5.0/ryven/example_nodes/examples/gui.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import re
 
-from ryven.gui_env import *
-
-from special_nodes import *
-
 from qtpy.QtGui import QFont
 from qtpy.QtCore import Qt, Signal, QEvent
 from qtpy.QtWidgets import QPushButton, QComboBox, QSlider, QTextEdit, QPlainTextEdit, QWidget, QVBoxLayout, QLineEdit, \
     QDialog, QMessageBox
 
+from ryven.gui_env import *
+
+from . import special_nodes as special_nodes
+from . import basic_operators as operator_nodes
+from . import control_structures as control_nodes
+
 
 """
     generic base classes
 """
 
 
 class GuiBase(NodeGUI):
@@ -20,14 +22,15 @@
 
 
 """
     operator nodes
 """
 
 
+@node_gui(operator_nodes.OperatorNodeBase)
 class OperatorNodeBaseGui(GuiBase):
     input_widget_classes = {
         'in': inp_widgets.Builder.evaled_line_edit(size='s', resizing=True),
     }
     # init_input_widgets = {
     #     0: {'name': 'in', 'pos': 'besides'},
     #     1: {'name': 'in', 'pos': 'besides'},
@@ -64,36 +67,41 @@
     def rebuild_remove_actions(self):
         self.actions['remove input'] = {}
         for i in range(self.node.num_inputs):
             self.actions[f'remove input'][f'{i}'] = \
                 {'method': self.remove_operand_input, 'data': i}
 
 
+@node_gui(operator_nodes.LogicNodeBase)
 class LogicNodeBaseGui(OperatorNodeBaseGui):
     color = '#f58142'
 
 
+@node_gui(operator_nodes.ArithmeticNodeBase)
 class ArithNodeBaseGui(OperatorNodeBaseGui):
     color = '#58db53'
 
 
+@node_gui(operator_nodes.ComparatorNodeBase)
 class CompNodeBaseGui(OperatorNodeBaseGui):
     color = '#a1574c'
 
 
 """
     control structures
 """
 
 
+@node_gui(control_nodes.CSNodeBase)
 class CSNodeBaseGui(GuiBase):
     style = 'normal'
     color = '#b33a27'
 
 
+@node_gui(control_nodes.ForLoop_Node)
 class ForLoopGui(CSNodeBaseGui):
     input_widget_classes = {
         'RangeFrom': inp_widgets.Builder.int_spinbox(0, (0, 1000000)),
         'RangeTo': inp_widgets.Builder.int_spinbox(10, (0, 1000000)),
     }
     init_input_widgets = {
         1: {'name': 'RangeFrom', 'pos': 'besides'},
@@ -123,32 +131,35 @@
     def rebuild_remove_actions(self):
         self.actions['remove dimension'] = {}
         for i in range(1, self.dims):
             self.actions[f'remove dimension'][f'{i + 1}'] = \
                 {'method': self.remove_dimension, 'data': i + 1}
 
 
+@node_gui(control_nodes.ForEachLoop_Node)
 class ForEachLoopGui(CSNodeBaseGui):
     input_widget_classes = {
         'List': inp_widgets.Builder.evaled_line_edit(),
     }
     init_input_widgets = {
         1: {'name': 'List', 'pos': 'besides'},
     }
 
 
 """
     special nodes
 """
 
 
+@node_gui(special_nodes.NodeBase)
 class SpecialNodeGuiBase(GuiBase):
     color = '#FFCA00'
 
 
+@node_gui(special_nodes.DualNodeBase)
 class DualNodeBaseGui(SpecialNodeGuiBase):
     def initialized(self):
         super().initialized()
         self.clean_actions()
 
     def clean_actions(self):
         if 'make passive' in self.actions:
@@ -168,14 +179,15 @@
 
     def make_active(self):
         del self.actions['make active']
         self.actions['make passive'] = {'method': self.make_passive}
         self.node.make_active()
 
 
+@node_gui(special_nodes.Checkpoint_Node)
 class CheckpointNodeGui(DualNodeBaseGui):
     style = 'small'
     display_title = ''
 
     def initialized(self):
         super().initialized()
         self.actions['add output'] = {'method': self.add_output}
@@ -193,23 +205,24 @@
     def rebuild_remove_actions(self):
         self.actions['remove output'] = {}
         for i in range(len(self.node.outputs)):
             self.actions['remove output'][f'{i}'] = \
                 {'method': self.remove_output, 'data': i}
 
 
-class ButtonNode_MainWidget(QPushButton, NodeMainWidget):
+class ButtonNode_MainWidget(NodeMainWidget, QPushButton):
 
     def __init__(self, params):
         NodeMainWidget.__init__(self, params)
         QPushButton.__init__(self)
 
         self.clicked.connect(self.update_node)
 
 
+@node_gui(special_nodes.Button_Node)
 class ButtonNodeGui(SpecialNodeGuiBase):
     main_widget_class = ButtonNode_MainWidget
     main_widget_pos = 'between ports'
     color = '#99dd55'
 
 
 class ClockNode_MainWidget(NodeMainWidget, QPushButton):
@@ -217,14 +230,15 @@
     def __init__(self, params):
         NodeMainWidget.__init__(self, params)
         QPushButton.__init__(self)
 
         self.clicked.connect(self.node.toggle)
 
 
+@node_gui(special_nodes.Clock_Node)
 class ClockNodeGui(SpecialNodeGuiBase):
     main_widget_class = ClockNode_MainWidget
     main_widget_pos = 'below ports'
     input_widget_classes = {
         'delay': inp_widgets.Builder.int_slider(1, (0, 10000)),
         'iter': inp_widgets.Builder.int_spinbox(-1, (-1, 1000)),
     }
@@ -243,14 +257,15 @@
     def start(self):
         self.node.start()
 
     def stop(self):
         self.node.stop()
 
 
+@node_gui(special_nodes.Log_Node)
 class LogNodeGui(SpecialNodeGuiBase):
     color = '#5d95de'
 
 
 class SliderNode_MainWidget(NodeMainWidget, QSlider):
     def __init__(self, params):
         NodeMainWidget.__init__(self, params)
@@ -261,14 +276,15 @@
         self.valueChanged.connect(self.value_changed)
 
     def value_changed(self, v):
         self.node.val = v/1000
         self.update_node()
 
 
+@node_gui(special_nodes.Slider_Node)
 class SliderNodeGui(SpecialNodeGuiBase):
     main_widget_class = SliderNode_MainWidget
     main_widget_pos = 'below ports'
     input_widget_classes = {
         'scale': inp_widgets.Builder.int_spinbox(1, (1, 99)),
         'round': inp_widgets.Builder.bool_checkbox(True),
     }
@@ -277,14 +293,15 @@
         1: {'name': 'round', 'pos': 'besides'},
     }
 
     def initialized(self):
         self.main_widget().setValue(self.node.val*1000)
 
 
+@node_gui(special_nodes._DynamicPorts_Node)
 class DynamicPortsGui(SpecialNodeGuiBase):
     def __init__(self, params):
         super().__init__(params)
 
         self.actions['add input'] = {'method': self.add_input}
         self.actions['remove input'] = {}
         self.actions['add output'] = {'method': self.add_output}
@@ -330,14 +347,15 @@
             'text': self.toPlainText(),
         }
 
     def set_state(self, data: dict):
         self.setPlainText(data['text'])
 
 
+@node_gui(special_nodes.Exec_Node)
 class ExecNodeGui(DynamicPortsGui):
     main_widget_class = ExecNode_MainWidget
     main_widget_pos = 'between ports'
 
 
 class EvalNode_MainWidget(NodeMainWidget, QPlainTextEdit):
     def __init__(self, params):
@@ -358,14 +376,15 @@
             'text': self.toPlainText(),
         }
 
     def set_state(self, data: dict):
         self.setPlainText(data['text'])
 
 
+@node_gui(special_nodes.Eval_Node)
 class EvalNodeGui(SpecialNodeGuiBase):
     main_widget_class = EvalNode_MainWidget
     main_widget_pos = 'between ports'
 
     def __init__(self, params):
         super().__init__(params)
 
@@ -379,41 +398,14 @@
             {'method': self.remove_input, 'data': index}
 
     def remove_input(self, index: int):
         self.node.remove_param_input(index)
         del self.actions['remove input'][str(index)]
 
 
-class InterpreterConsole(NodeMainWidget, QWidget):
-    def __init__(self, params):
-        NodeMainWidget.__init__(self, params)
-        QWidget.__init__(self)
-
-        self.inp_line_edit = ConsoleInpLineEdit()
-        self.output_text_edit = ConsoleOutDisplay()
-
-        self.inp_line_edit.returned.connect(self.node.process_input)
-
-        self.setLayout(QVBoxLayout())
-        self.layout().addWidget(self.output_text_edit)
-        self.layout().addWidget(self.inp_line_edit)
-
-        self.last_hist_len = 0
-
-    def interp_updated(self):
-
-        if self.last_hist_len < len(self.node.hist):
-            self.output_text_edit.appendPlainText('\n'.join(self.node.hist[self.last_hist_len:]))
-        else:
-            self.output_text_edit.clear()
-            self.output_text_edit.setPlainText('\n'.join(self.node.hist))
-
-        self.last_hist_len = len(self.node.hist)
-
-
 class ConsoleInpLineEdit(QLineEdit):
 
     returned = Signal(str)
 
     def __init__(self):
         super().__init__()
 
@@ -479,31 +471,61 @@
     def __init__(self):
         super().__init__()
 
         self.setReadOnly(True)
         self.setFont(QFont('Source Code Pro', 9))
 
 
+class InterpreterConsole(NodeMainWidget, QWidget):
+    def __init__(self, params):
+        NodeMainWidget.__init__(self, params)
+        QWidget.__init__(self)
+
+        self.inp_line_edit = ConsoleInpLineEdit()
+        self.output_text_edit = ConsoleOutDisplay()
+
+        self.inp_line_edit.returned.connect(self.node.process_input)
+
+        self.setLayout(QVBoxLayout())
+        self.layout().addWidget(self.output_text_edit)
+        self.layout().addWidget(self.inp_line_edit)
+
+        self.last_hist_len = 0
+
+    def interp_updated(self):
+
+        if self.last_hist_len < len(self.node.hist):
+            self.output_text_edit.appendPlainText('\n'.join(self.node.hist[self.last_hist_len:]))
+        else:
+            self.output_text_edit.clear()
+            self.output_text_edit.setPlainText('\n'.join(self.node.hist))
+
+        self.last_hist_len = len(self.node.hist)
+
+
+@node_gui(special_nodes.Interpreter_Node)
 class InterpreterConsoleGui(SpecialNodeGuiBase):
     main_widget_class = InterpreterConsole
     main_widget_pos = 'between ports'
 
 
+@node_gui(special_nodes.Storage_Node)
 class StorageNodeGui(SpecialNodeGuiBase):
     color = '#aadd55'
 
     def __init__(self, params):
         super().__init__(params)
 
         self.actions['clear'] = {'method': self.clear}
 
     def clear(self):
         self.node.clear()
 
 
+@node_gui(special_nodes.LinkIN_Node)
 class LinkIN_NodeGui(SpecialNodeGuiBase):
     def __init__(self, params):
         super().__init__(params)
 
         self.actions['add input'] = {'method': self.add_inp}
         self.actions['remove inp'] = {}
         self.actions['copy ID'] = {'method': self.copy_ID}
@@ -521,14 +543,15 @@
         }
 
     def remove_inp(self, index: int):
         self.node.remove_input(index)
         del self.actions['remove inp'][str(index)]
 
 
+@node_gui(special_nodes.LinkOUT_Node)
 class LinkOUT_NodeGui(SpecialNodeGuiBase):
 
     class IDInpDialog(QDialog):
         def __init__(self):
             super().__init__()
             self.id_str = None
             self.setLayout(QVBoxLayout())
@@ -546,50 +569,16 @@
         self.actions['link to ID'] = {'method': self.link_to_ID}
 
     def link_to_ID(self):
         d = self.IDInpDialog()
         d.exec_()
 
         if d.id_str is not None:
-            n = LinkIN_Node.INSTANCES.get(d.id_str)
+            n = special_nodes.LinkIN_Node.INSTANCES.get(d.id_str)
             if n is not None:
                 self.node.link_to(n)
             else:
                 QMessageBox.warning(
                     self,
                     title='link failed',
                     text=f'No node with ID "{d.id_str}" found'
                 )
-
-
-"""
-    export
-"""
-
-
-export_guis([
-    DualNodeBaseGui,
-
-    CheckpointNodeGui,
-    OperatorNodeBaseGui,
-    LogicNodeBaseGui,
-    ArithNodeBaseGui,
-    CompNodeBaseGui,
-
-    CSNodeBaseGui,
-    ForLoopGui,
-    ForEachLoopGui,
-
-    SpecialNodeGuiBase,
-    ButtonNodeGui,
-    ClockNodeGui,
-    LogNodeGui,
-    SliderNodeGui,
-    DynamicPortsGui,
-    ExecNodeGui,
-    EvalNodeGui,
-    InterpreterConsoleGui,
-    StorageNodeGui,
-    LinkIN_NodeGui,
-    LinkOUT_NodeGui,
-])
-
```

### Comparing `ryven-3.4.3/ryven/example_nodes/std/special_nodes.py` & `ryven-3.5.0/ryven/example_nodes/examples/special_nodes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,26 @@
+from typing import Dict, Set
 import code
 from contextlib import redirect_stdout, redirect_stderr
 from packaging.version import Version
 
 from ryvencore.addons.Logging import LoggingAddon
 from ryven.node_env import *
 
-guis = import_guis(__file__)
-
 
 class NodeBase(Node):
-    version = 'v0.2'
-    GUI = guis.SpecialNodeGuiBase
+    version = 'v0.3'
 
     def have_gui(self):
         return hasattr(self, 'gui')
 
 
 class DualNodeBase(NodeBase):
     """For nodes that can be active and passive"""
 
-    GUI = guis.DualNodeBaseGui
-
     def __init__(self, params, active=True):
         super().__init__(params)
 
         self.active = active
 
     def make_passive(self):
         self.delete_input(0)
@@ -51,16 +47,15 @@
     title = 'checkpoint'
     init_inputs = [
         NodeInputType(type_='data'),
     ]
     init_outputs = [
         NodeOutputType(type_='data'),
     ]
-    GUI = guis.CheckpointNodeGui
-
+    
     def __init__(self, params):
         super().__init__(params)
 
         self.active = False
 
     """
     state transitions
@@ -113,15 +108,14 @@
 
 class Button_Node(NodeBase):
     title = 'Button'
     init_inputs = []
     init_outputs = [
         NodeOutputType(type_='exec')
     ]
-    GUI = guis.ButtonNodeGui
 
     def update_event(self, inp=-1):
         self.exec_output(0)
 
 
 class Print_Node(DualNodeBase):
     title = 'Print'
@@ -149,18 +143,17 @@
     init_inputs = [
         NodeInputType(type_='exec'),
         NodeInputType('msg', type_='data'),
     ]
     init_outputs = [
         NodeOutputType(type_='exec'),
     ]
-    GUI = guis.LogNodeGui
 
-    logs = {}   # {int: Logger}
-    in_use = set()  # make sure we don't reuse numbers on copy & paste
+    logs: Dict[int, logging.Logger] = {}   # {int: Logger}
+    in_use: Set[int] = set()  # make sure we don't reuse numbers on copy & paste
 
     def __init__(self, params):
         super().__init__(params, active=True)
 
         self.number: int = None
         self.logger: logging.Logger = None
 
@@ -198,28 +191,30 @@
         else:
             # number already in use; generate a new one
             # happens on copy & paste
             self.number = len(self.logs)
 
         # the logging addon will have re-created the logger
         # for us already
-        self.logs[self.number] = \
-            self.logs_ext().new_logger(self, 'Log Node')
+        l = self.logs_ext().new_logger(self, 'Log Node')
+        if l is None:
+            print(f'WARNING: logger {self.number} for Log Node {self} already exists')
+        else:
+            self.logs[self.number] = l
 
 
 class Clock_Node(NodeBase):
     title = 'clock'
     init_inputs = [
         NodeInputType('delay'),
         NodeInputType('iterations'),
     ]
     init_outputs = [
         NodeOutputType(type_='exec')
     ]
-    GUI = guis.ClockNodeGui
 
     # When running with GUI, this node uses QTime which doesn't
     # block the GUI. When running without GUI, it uses time.sleep()
 
     def __init__(self, params):
         super().__init__(params)
 
@@ -278,15 +273,14 @@
     init_inputs = [
         NodeInputType('scl'),
         NodeInputType('round'),
     ]
     init_outputs = [
         NodeOutputType(),
     ]
-    GUI = guis.SliderNodeGui
 
     def __init__(self, params):
         super().__init__(params)
 
         self.val = 0
 
     def place_event(self):
@@ -304,15 +298,14 @@
     def set_state(self, data: dict, version):
         self.val = data['val']
 
 
 class _DynamicPorts_Node(NodeBase):
     init_inputs = []
     init_outputs = []
-    GUI = guis.DynamicPortsGui
 
     def add_input(self):
         self.create_input()
 
     def remove_input(self, index):
         self.delete_input(index)
 
@@ -321,15 +314,14 @@
 
     def remove_output(self, index):
         self.delete_output(index)
 
 
 class Exec_Node(_DynamicPorts_Node):
     title = 'exec'
-    GUI = guis.ExecNodeGui
 
     def __init__(self, params):
         super().__init__(params)
 
         self.code = None
 
     def update_event(self, inp=-1):
@@ -350,15 +342,14 @@
     title = 'eval'
     init_inputs = [
         # NodeInputType(),
     ]
     init_outputs = [
         NodeOutputType(),
     ]
-    GUI = guis.EvalNodeGui
 
     def __init__(self, params):
         super().__init__(params)
 
         self.number_param_inputs = 0
         self.expression_code = None
 
@@ -397,15 +388,14 @@
     """
     Provides a python interpreter via a basic console with access to the
     node's properties.
     """
     title = 'interpreter'
     init_inputs = []
     init_outputs = []
-    GUI = guis.InterpreterConsoleGui
 
     """
     commands
     """
 
     def clear(self):
         self.hist.clear()
@@ -435,28 +425,28 @@
     def _hist_updated(self):
         if self.have_gui():
             self.gui.main_widget().interp_updated()
 
     def process_input(self, cmds: str):
         m = self.COMMANDS.get(cmds)
         if m is not None:
-            m()
+            m(self)
         else:
             for l in cmds.splitlines():
                 self.write(l)  # print input
                 self.buffer.append(l)
             src = '\n'.join(self.buffer)
 
             def run_src():
                 more_inp_required = self.interp.runsource(src, '<console>')
                 if not more_inp_required:
                     self.buffer.clear()
 
             if self.session.gui:
-                with redirect_stdout(self), redirect_stderr(self):
+                with redirect_stdout(self), redirect_stderr(self):  # type: ignore
                     run_src()
             else:
                 run_src()
 
     def write(self, line: str):
         self.hist.append(line)
         self._hist_updated()
@@ -471,15 +461,14 @@
     title = 'store'
     init_inputs = [
         NodeInputType(),
     ]
     init_outputs = [
         NodeOutputType(),
     ]
-    GUI = guis.StorageNodeGui
 
     def __init__(self, params):
         super().__init__(params)
 
         self.storage = []
 
     def clear(self):
@@ -512,18 +501,17 @@
     """
 
     title = 'link IN'
     init_inputs = [
         NodeInputType(),
     ]
     init_outputs = []  # no outputs
-    GUI = guis.LinkIN_NodeGui
 
     # instances registration
-    INSTANCES = {}  # {UUID: node}
+    INSTANCES: Dict[str, Node] = {}
 
     def __init__(self, params):
         super().__init__(params)
 
         # register
         self.ID: uuid.UUID = uuid.uuid4()
         self.INSTANCES[str(self.ID)] = self
@@ -571,20 +559,19 @@
             self.linked_node = None
 
 
 class LinkOUT_Node(NodeBase):
     """The complement to the link IN node"""
 
     title = 'link OUT'
-    init_inputs = []  # no inputs
-    init_outputs = []  # will be synchronized with linked IN node
-    GUI = guis.LinkOUT_NodeGui
+    init_inputs: List[NodeInputType] = []  # no inputs
+    init_outputs: List[NodeOutputType] = []  # will be synchronized with linked IN node
 
-    INSTANCES = []
-    PENDING_LINK_BUILDS = {}
+    INSTANCES: List['LinkOUT_Node'] = []
+    PENDING_LINK_BUILDS: Dict['LinkOUT_Node', str] = {}
     # because a link OUT node might get initialized BEFORE it's corresponding
     # link IN, it then stores itself together with the ID of the link IN it's
     # waiting for in PENDING_LINK_BUILDS
 
     @classmethod
     def new_link_in_loaded(cls, n: LinkIN_Node):
         for out_node, in_ID in cls.PENDING_LINK_BUILDS.items():
@@ -652,21 +639,33 @@
     def remove_event(self):
         # break existent link
         if self.linked_node:
             self.linked_node.linked_node = None
             self.linked_node = None
 
 
-nodes = [
+node_types = [
     Checkpoint_Node,
     Button_Node,
     Print_Node,
     Log_Node,
     Clock_Node,
     Slider_Node,
     Exec_Node,
     Eval_Node,
     Storage_Node,
     LinkIN_Node,
     LinkOUT_Node,
     Interpreter_Node,
 ]
+
+# account for old package name
+for n in node_types:
+    n.legacy_identifiers = [
+        *getattr(n, 'legacy_identifiers', []),
+        f'std.{n.__class__.__name__}',
+    ]
+
+export_nodes(
+    node_types=node_types,
+    sub_pkg_name='special_nodes',
+)
```

### Comparing `ryven-3.4.3/ryven/examples_projects/basics.json` & `ryven-3.5.0/ryven/example_projects/basics.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5661653265116897%*

 * *Differences: {"'addons'": "{'Variables': {'custom state': {'5': {'a': {'GID': 538, 'serialized': "*

 * *             "'gASVIgoAAAAAAABdlChN2wtN3AtN3QtN3gtN3wtN4AtN4QtN4gtN4wtN5AtN5QtN5gtN5wtN6AtN6QtN6gtN6wtN7AtN7QtN7gtN7wtN8AtN8QtN8gtN8wtN9AtN9QtN9gtN9wtN+AtN+QtN+gtN+wtN/AtN/QtN/gtN/wtNAAxNAQxNAgxNAwxNBAxNBQxNBgxNBwxNCAxNCQxNCgxNCwxNDAxNDQxNDgxNDwxNEAxNEQxNEgxNEwxNFAxNFQxNFgxNFwxNGAxNGQxNGgxNGwxNHAxNHQxNHgxNHwxNIAxNIQxNIgxNIwxNJAxNJQxNJgxNJwxNKAxNKQxNKgxNKwxNLAxNLQxNLgxNLwxNMAxNMQxNMgxNMwxNNAxNNQxNNgxNNwxNOAxNOQxNOgxNOwxNPAx […]*

```diff
@@ -5,31 +5,67 @@
             "GID": 4,
             "custom state": {},
             "version": "0.0.1"
         },
         "Variables": {
             "GID": 3,
             "custom state": {
+                "117": {},
                 "5": {
                     "a": {
-                        "GID": 4629,
+                        "GID": 538,
                         "identifier": "Data",
-                        "serialized": "gASVSAgAAAAAAABdlChN2wtN3AtN3QtN3gtN3wtN4AtN4QtN4gtN4wtN5AtN5QtN5gtN5wtN6AtN6QtN6gtN6wtN7AtN7QtN7gtN7wtN8AtN8QtN8gtN8wtN9AtN9QtN9gtN9wtN+AtN+QtN+gtN+wtN/AtN/QtN/gtN/wtNAAxNAQxNAgxNAwxNBAxNBQxNBgxNBwxNCAxNCQxNCgxNCwxNDAxNDQxNDgxNDwxNEAxNEQxNEgxNEwxNFAxNFQxNFgxNFwxNGAxNGQxNGgxNGwxNHAxNHQxNHgxNHwxNIAxNIQxNIgxNIwxNJAxNJQxNJgxNJwxNKAxNKQxNKgxNKwxNLAxNLQxNLgxNLwxNMAxNMQxNMgxNMwxNNAxNNQxNNgxNNwxNOAxNOQxNOgxNOwxNPAxNPQxNPgxNPgxNPwxNQAxNQQxNQgxNQwxNRAxNRQxNRgxNRwxNSAxNSQxNSgxNSwxNTAxNTQxNTgxNTwxNUAxNUQxNUgxNUwxNVAxNVQxNVgxNVwxNWAxNWQxNWgxNWwxNXAxNXQxNXgxNXwxNYAxNYQxNYgxNYwxNZAxNZQxNZgxNZwxNaAxNaQxNagxNawxNbAxNbQxNbgxNbwxNcAxNcQxNcgxNcwxNdAxNdQxNdgxNdwxNeAxNeQxNegxNewxNfAxNfQxNfgxNfwxNgAxNgQxNggxNgwxNhAxNhQxNhgxNhwxNiAxNiQxNigxNiwxNjAxNjQxNjgxNjwxNkAxNkQxNkgxNkwxNlAxNlQxNlgxNlwxNmAxNmQxNmgxNmwxNnAxNnQxNngxNnwxNoAxNoQxNogxNowxNpAxNpQxNpgxNpwxNqAxNqQxNqgxNqwxNrAxNrQxNrgxNrwxNsAxNsQxNsgxNswxNtAxNtQxNtgxNtwxNuAxNuQxNugxNuwxNvAxNvQxNvgxNvwxNwAxNwQxNwgxNwwxNxAxNxQxNxgxNxwxNyAxNyQxNygxNywxNzAxNzQxNzgxNzwxN0AxN0QxN0gxN0wxN1AxN1QxN1gxN1wxN2AxN2QxN2gxN2wxN3AxN3QxN3gxN3wxN4AxN4QxN4gxN4wxN5AxN5QxN5gxN5wxN6AxN6QxN6gxN6wxN7AxN7QxN7gxN7wxN8AxN8QxN8gxN8wxN9AxN9QxN9gxN9wxN+AxN+QxN+gxN+wxN/AxN/QxN/gxN/wxNAA1NAQ1NAg1NAw1NBA1NBQ1NBg1NBw1NCA1NCQ1NCg1NCw1NDA1NDQ1NDg1NDw1NEA1NEQ1NEg1NEw1NFA1NFQ1NFg1NFw1NGA1NGQ1NGg1NGw1NHA1NHQ1NHg1NHw1NIA1NIQ1NIg1NIw1NJA1NJQ1NJg1NJw1NKA1NKQ1NKg1NKw1NLA1NLQ1NLg1NLw1NMA1NMQ1NMg1NMw1NNA1NNQ1NNg1NNw1NOA1NOQ1NOg1NOw1NPA1NPQ1NPg1NPw1NQA1NQQ1NQg1NQw1NRA1NRQ1NRg1NRw1NSA1NSQ1NSg1NSw1NTA1NTQ1NTg1NTw1NUA1NUQ1NUg1NUw1NVA1NVQ1NVg1NVw1NWA1NWQ1NWg1NWw1NXA1NXQ1NXg1NXw1NYA1NYQ1NYg1NYw1NZA1NZQ1NZg1NZw1NaA1NaQ1Nag1Naw1NbA1NbQ1Nbg1Nbw1NcA1NcQ1Ncg1Ncw1NdA1NdQ1Ndg1Ndw1NeA1NeQ1Neg1New1NfA1NfQ1Nfg1Nfw1NgA1NgQ1Ngg1Ngw1NhA1NhQ1Nhg1Nhw1NiA1NiQ1Nig1Niw1NjA1NjQ1Njg1Njw1NkA1NkQ1Nkg1Nkw1NlA1NlQ1Nlg1Nlw1NmA1NmQ1Nmg1Nmw1NnA1NnQ1Nng1Nnw1NoA1NoQ1Nog1Now1NpA1NpQ1Npg1Npw1NqA1NqQ1Nqg1Nqw1NrA1NrQ1Nrg1Nrw1NsA1NsQ1Nsg1Nsw1NtA1NtQ1Ntg1Ntw1NuA1NuQ1Nug1Nuw1NvA1NvQ1Nvg1Nvw1NwA1NwQ1Nwg1Nww1NxA1NxQ1Nxg1Nxw1NyA1NyQ1Nyg1Nyw1NzA1NzQ1Nzg1Nzw1N0A1N0Q1N0g1N0w1N1A1N1Q1N1g1N1w1N2A1N2Q1N2g1N2w1N3A1N3Q1N3g1N3w1N4A1N4Q1N4g1N4w1N5A1N5Q1N5g1N5w1N6A1N6Q1N6g1N6w1N7A1N7Q1N7g1N7w1N8A1N8Q1N8g1N8w1N9A1N9Q1N9g1N9w1N+A1N+Q1N+g1N+w1N/A1N/Q1N/g1N/w1NAA5NAQ5NAg5NAw5NBA5NBQ5NBg5NBw5NCA5NCQ5NCg5NCw5NDA5NDQ5NDg5NDw5NEA5NEQ5NEg5NEw5NFA5NFQ5NFg5NFw5NGA5NGQ5NGg5NGw5NHA5NHQ5NHg5NHw5NIA5NIQ5NIg5NIw5NJA5NJQ5NJg5NJw5NKA5NKQ5NKg5NKw5NLA5NLQ5NLg5NLw5NMA5NMQ5NMg5NMw5NNA5NNQ5NNg5NNw5NOA5NOQ5NOg5NOw5NPA5NPQ5NPg5NPw5NQA5NQQ5NQg5NQw5NRA5NRQ5NRg5NRw5NSA5NSQ5NSg5NSw5NTA5NTQ5NTg5NTw5NUA5NUQ5NUg5NUw5NVA5NVQ5NVg5NVw5NWA5NWQ5NWg5NWw5NXA5NXQ5NXg5NXw5NYA5NYQ5NYg5NYw5NZA5NZQ5NZg5NZw5NaA5NaQ5Nag5Naw5NbA5NbQ5Nbg5Nbw5NcA5NcQ5Ncg5Ncw5NdA5NdQ5Ndg5Ndw5NeA5NeQ5Neg5New5NfA5NfQ5Nfg5Nfw5NgA5NgQ5Ngg5Ngw5NhA5NhQ5Nhg5Nhw5NiA5NiQ5Nig5Niw5NjA5NjQ5Njg5Njw5NkA5NkQ5Nkg5Nkw5NlA5NlQ5Nlg5Nlw5NmA5NmQ5Nmg5lLg=="
+                        "serialized": "gASVIgoAAAAAAABdlChN2wtN3AtN3QtN3gtN3wtN4AtN4QtN4gtN4wtN5AtN5QtN5gtN5wtN6AtN6QtN6gtN6wtN7AtN7QtN7gtN7wtN8AtN8QtN8gtN8wtN9AtN9QtN9gtN9wtN+AtN+QtN+gtN+wtN/AtN/QtN/gtN/wtNAAxNAQxNAgxNAwxNBAxNBQxNBgxNBwxNCAxNCQxNCgxNCwxNDAxNDQxNDgxNDwxNEAxNEQxNEgxNEwxNFAxNFQxNFgxNFwxNGAxNGQxNGgxNGwxNHAxNHQxNHgxNHwxNIAxNIQxNIgxNIwxNJAxNJQxNJgxNJwxNKAxNKQxNKgxNKwxNLAxNLQxNLgxNLwxNMAxNMQxNMgxNMwxNNAxNNQxNNgxNNwxNOAxNOQxNOgxNOwxNPAxNPQxNPgxNPgxNPwxNQAxNQQxNQgxNQwxNRAxNRQxNRgxNRwxNSAxNSQxNSgxNSwxNTAxNTQxNTgxNTwxNUAxNUQxNUgxNUwxNVAxNVQxNVgxNVwxNWAxNWQxNWgxNWwxNXAxNXQxNXgxNXwxNYAxNYQxNYgxNYwxNZAxNZQxNZgxNZwxNaAxNaQxNagxNawxNbAxNbQxNbgxNbwxNcAxNcQxNcgxNcwxNdAxNdQxNdgxNdwxNeAxNeQxNegxNewxNfAxNfQxNfgxNfwxNgAxNgQxNggxNgwxNhAxNhQxNhgxNhwxNiAxNiQxNigxNiwxNjAxNjQxNjgxNjwxNkAxNkQxNkgxNkwxNlAxNlQxNlgxNlwxNmAxNmQxNmgxNmwxNnAxNnQxNngxNnwxNoAxNoQxNogxNowxNpAxNpQxNpgxNpwxNqAxNqQxNqgxNqwxNrAxNrQxNrgxNrwxNsAxNsQxNsgxNswxNtAxNtQxNtgxNtwxNuAxNuQxNugxNuwxNvAxNvQxNvgxNvwxNwAxNwQxNwgxNwwxNxAxNxQxNxgxNxwxNyAxNyQxNygxNywxNzAxNzQxNzgxNzwxN0AxN0QxN0gxN0wxN1AxN1QxN1gxN1wxN2AxN2QxN2gxN2wxN3AxN3QxN3gxN3wxN4AxN4QxN4gxN4wxN5AxN5QxN5gxN5wxN6AxN6QxN6gxN6wxN7AxN7QxN7gxN7wxN8AxN8QxN8gxN8wxN9AxN9QxN9gxN9wxN+AxN+QxN+gxN+wxN/AxN/QxN/gxN/wxNAA1NAQ1NAg1NAw1NBA1NBQ1NBg1NBw1NCA1NCQ1NCg1NCw1NDA1NDQ1NDg1NDw1NEA1NEQ1NEg1NEw1NFA1NFQ1NFg1NFw1NGA1NGQ1NGg1NGw1NHA1NHQ1NHg1NHw1NIA1NIQ1NIg1NIw1NJA1NJQ1NJg1NJw1NKA1NKQ1NKg1NKw1NLA1NLQ1NLg1NLw1NMA1NMQ1NMg1NMw1NNA1NNQ1NNg1NNw1NOA1NOQ1NOg1NOw1NPA1NPQ1NPg1NPw1NQA1NQQ1NQg1NQw1NRA1NRQ1NRg1NRw1NSA1NSQ1NSg1NSw1NTA1NTQ1NTg1NTw1NUA1NUQ1NUg1NUw1NVA1NVQ1NVg1NVw1NWA1NWQ1NWg1NWw1NXA1NXQ1NXg1NXw1NYA1NYQ1NYg1NYw1NZA1NZQ1NZg1NZw1NaA1NaQ1Nag1Naw1NbA1NbQ1Nbg1Nbw1NcA1NcQ1Ncg1Ncw1NdA1NdQ1Ndg1Ndw1NeA1NeQ1Neg1New1NfA1NfQ1Nfg1Nfw1NgA1NgQ1Ngg1Ngw1NhA1NhQ1Nhg1Nhw1NiA1NiQ1Nig1Niw1NjA1NjQ1Njg1Njw1NkA1NkQ1Nkg1Nkw1NlA1NlQ1Nlg1Nlw1NmA1NmQ1Nmg1Nmw1NnA1NnQ1Nng1Nnw1NoA1NoQ1Nog1Now1NpA1NpQ1Npg1Npw1NqA1NqQ1Nqg1Nqw1NrA1NrQ1Nrg1Nrw1NsA1NsQ1Nsg1Nsw1NtA1NtQ1Ntg1Ntw1NuA1NuQ1Nug1Nuw1NvA1NvQ1Nvg1Nvw1NwA1NwQ1Nwg1Nww1NxA1NxQ1Nxg1Nxw1NyA1NyQ1Nyg1Nyw1NzA1NzQ1Nzg1Nzw1N0A1N0Q1N0g1N0w1N1A1N1Q1N1g1N1w1N2A1N2Q1N2g1N2w1N3A1N3Q1N3g1N3w1N4A1N4Q1N4g1N4w1N5A1N5Q1N5g1N5w1N6A1N6Q1N6g1N6w1N7A1N7Q1N7g1N7w1N8A1N8Q1N8g1N8w1N9A1N9Q1N9g1N9w1N+A1N+Q1N+g1N+w1N/A1N/Q1N/g1N/w1NAA5NAQ5NAg5NAw5NBA5NBQ5NBg5NBw5NCA5NCQ5NCg5NCw5NDA5NDQ5NDg5NDw5NEA5NEQ5NEg5NEw5NFA5NFQ5NFg5NFw5NGA5NGQ5NGg5NGw5NHA5NHQ5NHg5NHw5NIA5NIQ5NIg5NIw5NJA5NJQ5NJg5NJw5NKA5NKQ5NKg5NKw5NLA5NLQ5NLg5NLw5NMA5NMQ5NMg5NMw5NNA5NNQ5NNg5NNw5NOA5NOQ5NOg5NOw5NPA5NPQ5NPg5NPw5NQA5NQQ5NQg5NQw5NRA5NRQ5NRg5NRw5NSA5NSQ5NSg5NSw5NTA5NTQ5NTg5NTw5NUA5NUQ5NUg5NUw5NVA5NVQ5NVg5NVw5NWA5NWQ5NWg5NWw5NXA5NXQ5NXg5NXw5NYA5NYQ5NYg5NYw5NZA5NZQ5NZg5NZw5NaA5NaQ5Nag5Naw5NbA5NbQ5Nbg5Nbw5NcA5NcQ5Ncg5Ncw5NdA5NdQ5Ndg5Ndw5NeA5NeQ5Neg5New5NfA5NfQ5Nfg5Nfw5NgA5NgQ5Ngg5Ngw5NhA5NhQ5Nhg5Nhw5NiA5NiQ5Nig5Niw5NjA5NjQ5Njg5Njw5NkA5NkQ5Nkg5Nkw5NlA5NlQ5Nlg5Nlw5NmA5NmQ5Nmg5Nmw5Nmw5NnA5NnA5NnQ5NnQ5Nng5Nng5Nnw5Nnw5NoA5NoA5NoQ5NoQ5Nog5Nog5Now5Now5NpA5NpA5NpQ5NpQ5Npg5Npg5Npw5Npw5NqA5NqA5NqQ5NqQ5Nqg5Nqg5Nqw5Nqw5NrA5NrA5NrQ5NrQ5Nrg5Nrg5Nrw5Nrw5NsA5NsA5NsQ5NsQ5Nsg5Nsg5Nsw5Nsw5NtA5NtA5NtQ5NtQ5Ntg5Ntg5Ntw5Ntw5NuA5NuA5NuQ5NuQ5Nug5Nug5Nuw5Nuw5NvA5NvA5NvQ5NvQ5Nvg5Nvg5Nvw5Nvw5NwA5NwA5NwQ5NwQ5Nwg5Nwg5Nww5Nww5NxA5NxA5NxQ5NxQ5Nxg5Nxg5Nxw5Nxw5NyA5NyA5NyQ5NyQ5Nyg5Nyg5Nyw5Nyw5NzA5NzA5NzQ5NzQ5Nzg5Nzg5Nzw5Nzw5N0A5N0A5N0Q5N0Q5N0g5N0g5N0w5N0w5N1A5N1A5N1Q5N1Q5N1g5N1g5N1w5N1w5N2A5N2A5N2Q5N2Q5N2g5N2g5N2w5N2w5N3A5N3A5N3Q5N3Q5N3g5N3g5N3w5N3w5N4A5N4A5N4Q5N4Q5N4g5N4g5N4w5N4w5N5A5N5A5N5Q5N5Q5N5g5N5g5N5w5N5w5N6A5N6A5N6Q5N6Q5lLg=="
                     },
                     "ctr": {
-                        "GID": 4625,
+                        "GID": 523,
                         "identifier": "Data",
-                        "serialized": "gASVBAAAAAAAAABNmg4u"
+                        "serialized": "gASVBAAAAAAAAABN6Q4u"
                     }
-                },
-                "83": {}
+                }
             },
             "version": "0.4"
         }
     },
+    "flow_uis": {
+        "117": {
+            "geometry": "01d9d0cb0003000000000000000000000000048d000001b70000000000000000ffffffffffffffff000000000000000008d000000000000000000000048d000001b7",
+            "state": "000000ff00000000fd0000000100000001000000d8000001b8fc0200000001fc00000000000001b8000000d10000005bfa000000000200000006fb0000001c0069006e00730070006500630074006f0072005f0064006f0063006b0100000000ffffffff000000b200fffffffb000000220075006e0064006f005f0068006900730074006f00720079005f0064006f0063006b0100000000ffffffff0000005600fffffffb0000001a00730065007400740069006e00670073005f0064006f0063006b0100000000ffffffff0000003c0000003cfb0000001c007600610072006900610062006c00650073005f0064006f0063006b0100000000ffffffff0000007f00fffffffb00000016006c006f0067006700650072005f0064006f0063006b0100000000ffffffff0000004800fffffffb000000160073006f0075007200630065005f0064006f0063006b0100000000ffffffff0000009000ffffff000003a2000001b800000004000000040000000800000008fc00000000",
+            "view": {
+                "h_scroll": 139,
+                "m11": 1.250765972982705,
+                "m12": 0.0,
+                "m13": 0.0,
+                "m21": 0.0,
+                "m22": 1.250765972982705,
+                "m23": 0.0,
+                "m31": 0.0,
+                "m32": 0.0,
+                "m33": 1.0,
+                "v_scroll": 207
+            }
+        },
+        "5": {
+            "geometry": "01d9d0cb0003000000000000000000000000048d000001b70000000000000000ffffffffffffffff000000000000000008d000000000000000000000048d000001b7",
+            "state": "000000ff00000000fd0000000100000001000000d8000001b8fc0200000001fc00000000000001b8000000d10000005bfa000000000200000006fb0000001c0069006e00730070006500630074006f0072005f0064006f0063006b0100000000ffffffff000000b200fffffffb000000220075006e0064006f005f0068006900730074006f00720079005f0064006f0063006b0100000000ffffffff0000005600fffffffb0000001a00730065007400740069006e00670073005f0064006f0063006b0100000000ffffffff0000003c0000003cfb0000001c007600610072006900610062006c00650073005f0064006f0063006b0100000000ffffffff0000007f00fffffffb00000016006c006f0067006700650072005f0064006f0063006b0100000000ffffffff0000004800fffffffb000000160073006f0075007200630065005f0064006f0063006b0100000000ffffffff0000009000ffffff000003a2000001b800000004000000040000000800000008fc00000000",
+            "view": {
+                "h_scroll": 6,
+                "m11": 0.9712579279921432,
+                "m12": 0.0,
+                "m13": 0.0,
+                "m21": 0.0,
+                "m22": 0.9712579279921432,
+                "m23": 0.0,
+                "m31": 0.0,
+                "m32": 0.0,
+                "m33": 1.0,
+                "v_scroll": 30
+            }
+        }
+    },
     "flows": {
         "hello world": {
             "GID": 5,
             "algorithm mode": "data",
             "connections": [
                 {
                     "connected input port index": 1,
@@ -121,35 +157,36 @@
                         "update shape": {
                             "method": "update_shape"
                         }
                     },
                     "additional data": {},
                     "collapsed": false,
                     "display title": "store",
-                    "identifier": "std.Storage_Node",
+                    "identifier": "examples.special_nodes.Storage_Node",
                     "inputs": [
                         {
                             "GID": 9,
                             "has widget": false,
                             "label": "",
                             "type": "data"
                         }
                     ],
+                    "inspector widget": {},
                     "outputs": [
                         {
                             "GID": 10,
                             "label": "",
                             "type": "data"
                         }
                     ],
                     "pos x": 475.4795814751692,
                     "pos y": 264.55248052403067,
-                    "state data": "gASVUggAAAAAAAB9lIwEZGF0YZRdlChN2wtN3AtN3QtN3gtN3wtN4AtN4QtN4gtN4wtN5AtN5QtN5gtN5wtN6AtN6QtN6gtN6wtN7AtN7QtN7gtN7wtN8AtN8QtN8gtN8wtN9AtN9QtN9gtN9wtN+AtN+QtN+gtN+wtN/AtN/QtN/gtN/wtNAAxNAQxNAgxNAwxNBAxNBQxNBgxNBwxNCAxNCQxNCgxNCwxNDAxNDQxNDgxNDwxNEAxNEQxNEgxNEwxNFAxNFQxNFgxNFwxNGAxNGQxNGgxNGwxNHAxNHQxNHgxNHwxNIAxNIQxNIgxNIwxNJAxNJQxNJgxNJwxNKAxNKQxNKgxNKwxNLAxNLQxNLgxNLwxNMAxNMQxNMgxNMwxNNAxNNQxNNgxNNwxNOAxNOQxNOgxNOwxNPAxNPQxNPgxNPgxNPwxNQAxNQQxNQgxNQwxNRAxNRQxNRgxNRwxNSAxNSQxNSgxNSwxNTAxNTQxNTgxNTwxNUAxNUQxNUgxNUwxNVAxNVQxNVgxNVwxNWAxNWQxNWgxNWwxNXAxNXQxNXgxNXwxNYAxNYQxNYgxNYwxNZAxNZQxNZgxNZwxNaAxNaQxNagxNawxNbAxNbQxNbgxNbwxNcAxNcQxNcgxNcwxNdAxNdQxNdgxNdwxNeAxNeQxNegxNewxNfAxNfQxNfgxNfwxNgAxNgQxNggxNgwxNhAxNhQxNhgxNhwxNiAxNiQxNigxNiwxNjAxNjQxNjgxNjwxNkAxNkQxNkgxNkwxNlAxNlQxNlgxNlwxNmAxNmQxNmgxNmwxNnAxNnQxNngxNnwxNoAxNoQxNogxNowxNpAxNpQxNpgxNpwxNqAxNqQxNqgxNqwxNrAxNrQxNrgxNrwxNsAxNsQxNsgxNswxNtAxNtQxNtgxNtwxNuAxNuQxNugxNuwxNvAxNvQxNvgxNvwxNwAxNwQxNwgxNwwxNxAxNxQxNxgxNxwxNyAxNyQxNygxNywxNzAxNzQxNzgxNzwxN0AxN0QxN0gxN0wxN1AxN1QxN1gxN1wxN2AxN2QxN2gxN2wxN3AxN3QxN3gxN3wxN4AxN4QxN4gxN4wxN5AxN5QxN5gxN5wxN6AxN6QxN6gxN6wxN7AxN7QxN7gxN7wxN8AxN8QxN8gxN8wxN9AxN9QxN9gxN9wxN+AxN+QxN+gxN+wxN/AxN/QxN/gxN/wxNAA1NAQ1NAg1NAw1NBA1NBQ1NBg1NBw1NCA1NCQ1NCg1NCw1NDA1NDQ1NDg1NDw1NEA1NEQ1NEg1NEw1NFA1NFQ1NFg1NFw1NGA1NGQ1NGg1NGw1NHA1NHQ1NHg1NHw1NIA1NIQ1NIg1NIw1NJA1NJQ1NJg1NJw1NKA1NKQ1NKg1NKw1NLA1NLQ1NLg1NLw1NMA1NMQ1NMg1NMw1NNA1NNQ1NNg1NNw1NOA1NOQ1NOg1NOw1NPA1NPQ1NPg1NPw1NQA1NQQ1NQg1NQw1NRA1NRQ1NRg1NRw1NSA1NSQ1NSg1NSw1NTA1NTQ1NTg1NTw1NUA1NUQ1NUg1NUw1NVA1NVQ1NVg1NVw1NWA1NWQ1NWg1NWw1NXA1NXQ1NXg1NXw1NYA1NYQ1NYg1NYw1NZA1NZQ1NZg1NZw1NaA1NaQ1Nag1Naw1NbA1NbQ1Nbg1Nbw1NcA1NcQ1Ncg1Ncw1NdA1NdQ1Ndg1Ndw1NeA1NeQ1Neg1New1NfA1NfQ1Nfg1Nfw1NgA1NgQ1Ngg1Ngw1NhA1NhQ1Nhg1Nhw1NiA1NiQ1Nig1Niw1NjA1NjQ1Njg1Njw1NkA1NkQ1Nkg1Nkw1NlA1NlQ1Nlg1Nlw1NmA1NmQ1Nmg1Nmw1NnA1NnQ1Nng1Nnw1NoA1NoQ1Nog1Now1NpA1NpQ1Npg1Npw1NqA1NqQ1Nqg1Nqw1NrA1NrQ1Nrg1Nrw1NsA1NsQ1Nsg1Nsw1NtA1NtQ1Ntg1Ntw1NuA1NuQ1Nug1Nuw1NvA1NvQ1Nvg1Nvw1NwA1NwQ1Nwg1Nww1NxA1NxQ1Nxg1Nxw1NyA1NyQ1Nyg1Nyw1NzA1NzQ1Nzg1Nzw1N0A1N0Q1N0g1N0w1N1A1N1Q1N1g1N1w1N2A1N2Q1N2g1N2w1N3A1N3Q1N3g1N3w1N4A1N4Q1N4g1N4w1N5A1N5Q1N5g1N5w1N6A1N6Q1N6g1N6w1N7A1N7Q1N7g1N7w1N8A1N8Q1N8g1N8w1N9A1N9Q1N9g1N9w1N+A1N+Q1N+g1N+w1N/A1N/Q1N/g1N/w1NAA5NAQ5NAg5NAw5NBA5NBQ5NBg5NBw5NCA5NCQ5NCg5NCw5NDA5NDQ5NDg5NDw5NEA5NEQ5NEg5NEw5NFA5NFQ5NFg5NFw5NGA5NGQ5NGg5NGw5NHA5NHQ5NHg5NHw5NIA5NIQ5NIg5NIw5NJA5NJQ5NJg5NJw5NKA5NKQ5NKg5NKw5NLA5NLQ5NLg5NLw5NMA5NMQ5NMg5NMw5NNA5NNQ5NNg5NNw5NOA5NOQ5NOg5NOw5NPA5NPQ5NPg5NPw5NQA5NQQ5NQg5NQw5NRA5NRQ5NRg5NRw5NSA5NSQ5NSg5NSw5NTA5NTQ5NTg5NTw5NUA5NUQ5NUg5NUw5NVA5NVQ5NVg5NVw5NWA5NWQ5NWg5NWw5NXA5NXQ5NXg5NXw5NYA5NYQ5NYg5NYw5NZA5NZQ5NZg5NZw5NaA5NaQ5Nag5Naw5NbA5NbQ5Nbg5Nbw5NcA5NcQ5Ncg5Ncw5NdA5NdQ5Ndg5Ndw5NeA5NeQ5Neg5New5NfA5NfQ5Nfg5Nfw5NgA5NgQ5Ngg5Ngw5NhA5NhQ5Nhg5Nhw5NiA5NiQ5Nig5Niw5NjA5NjQ5Njg5Njw5NkA5NkQ5Nkg5Nkw5NlA5NlQ5Nlg5Nlw5NmA5NmQ5Nmg5lcy4=",
+                    "state data": "gASVLAoAAAAAAAB9lIwEZGF0YZRdlChN2wtN3AtN3QtN3gtN3wtN4AtN4QtN4gtN4wtN5AtN5QtN5gtN5wtN6AtN6QtN6gtN6wtN7AtN7QtN7gtN7wtN8AtN8QtN8gtN8wtN9AtN9QtN9gtN9wtN+AtN+QtN+gtN+wtN/AtN/QtN/gtN/wtNAAxNAQxNAgxNAwxNBAxNBQxNBgxNBwxNCAxNCQxNCgxNCwxNDAxNDQxNDgxNDwxNEAxNEQxNEgxNEwxNFAxNFQxNFgxNFwxNGAxNGQxNGgxNGwxNHAxNHQxNHgxNHwxNIAxNIQxNIgxNIwxNJAxNJQxNJgxNJwxNKAxNKQxNKgxNKwxNLAxNLQxNLgxNLwxNMAxNMQxNMgxNMwxNNAxNNQxNNgxNNwxNOAxNOQxNOgxNOwxNPAxNPQxNPgxNPgxNPwxNQAxNQQxNQgxNQwxNRAxNRQxNRgxNRwxNSAxNSQxNSgxNSwxNTAxNTQxNTgxNTwxNUAxNUQxNUgxNUwxNVAxNVQxNVgxNVwxNWAxNWQxNWgxNWwxNXAxNXQxNXgxNXwxNYAxNYQxNYgxNYwxNZAxNZQxNZgxNZwxNaAxNaQxNagxNawxNbAxNbQxNbgxNbwxNcAxNcQxNcgxNcwxNdAxNdQxNdgxNdwxNeAxNeQxNegxNewxNfAxNfQxNfgxNfwxNgAxNgQxNggxNgwxNhAxNhQxNhgxNhwxNiAxNiQxNigxNiwxNjAxNjQxNjgxNjwxNkAxNkQxNkgxNkwxNlAxNlQxNlgxNlwxNmAxNmQxNmgxNmwxNnAxNnQxNngxNnwxNoAxNoQxNogxNowxNpAxNpQxNpgxNpwxNqAxNqQxNqgxNqwxNrAxNrQxNrgxNrwxNsAxNsQxNsgxNswxNtAxNtQxNtgxNtwxNuAxNuQxNugxNuwxNvAxNvQxNvgxNvwxNwAxNwQxNwgxNwwxNxAxNxQxNxgxNxwxNyAxNyQxNygxNywxNzAxNzQxNzgxNzwxN0AxN0QxN0gxN0wxN1AxN1QxN1gxN1wxN2AxN2QxN2gxN2wxN3AxN3QxN3gxN3wxN4AxN4QxN4gxN4wxN5AxN5QxN5gxN5wxN6AxN6QxN6gxN6wxN7AxN7QxN7gxN7wxN8AxN8QxN8gxN8wxN9AxN9QxN9gxN9wxN+AxN+QxN+gxN+wxN/AxN/QxN/gxN/wxNAA1NAQ1NAg1NAw1NBA1NBQ1NBg1NBw1NCA1NCQ1NCg1NCw1NDA1NDQ1NDg1NDw1NEA1NEQ1NEg1NEw1NFA1NFQ1NFg1NFw1NGA1NGQ1NGg1NGw1NHA1NHQ1NHg1NHw1NIA1NIQ1NIg1NIw1NJA1NJQ1NJg1NJw1NKA1NKQ1NKg1NKw1NLA1NLQ1NLg1NLw1NMA1NMQ1NMg1NMw1NNA1NNQ1NNg1NNw1NOA1NOQ1NOg1NOw1NPA1NPQ1NPg1NPw1NQA1NQQ1NQg1NQw1NRA1NRQ1NRg1NRw1NSA1NSQ1NSg1NSw1NTA1NTQ1NTg1NTw1NUA1NUQ1NUg1NUw1NVA1NVQ1NVg1NVw1NWA1NWQ1NWg1NWw1NXA1NXQ1NXg1NXw1NYA1NYQ1NYg1NYw1NZA1NZQ1NZg1NZw1NaA1NaQ1Nag1Naw1NbA1NbQ1Nbg1Nbw1NcA1NcQ1Ncg1Ncw1NdA1NdQ1Ndg1Ndw1NeA1NeQ1Neg1New1NfA1NfQ1Nfg1Nfw1NgA1NgQ1Ngg1Ngw1NhA1NhQ1Nhg1Nhw1NiA1NiQ1Nig1Niw1NjA1NjQ1Njg1Njw1NkA1NkQ1Nkg1Nkw1NlA1NlQ1Nlg1Nlw1NmA1NmQ1Nmg1Nmw1NnA1NnQ1Nng1Nnw1NoA1NoQ1Nog1Now1NpA1NpQ1Npg1Npw1NqA1NqQ1Nqg1Nqw1NrA1NrQ1Nrg1Nrw1NsA1NsQ1Nsg1Nsw1NtA1NtQ1Ntg1Ntw1NuA1NuQ1Nug1Nuw1NvA1NvQ1Nvg1Nvw1NwA1NwQ1Nwg1Nww1NxA1NxQ1Nxg1Nxw1NyA1NyQ1Nyg1Nyw1NzA1NzQ1Nzg1Nzw1N0A1N0Q1N0g1N0w1N1A1N1Q1N1g1N1w1N2A1N2Q1N2g1N2w1N3A1N3Q1N3g1N3w1N4A1N4Q1N4g1N4w1N5A1N5Q1N5g1N5w1N6A1N6Q1N6g1N6w1N7A1N7Q1N7g1N7w1N8A1N8Q1N8g1N8w1N9A1N9Q1N9g1N9w1N+A1N+Q1N+g1N+w1N/A1N/Q1N/g1N/w1NAA5NAQ5NAg5NAw5NBA5NBQ5NBg5NBw5NCA5NCQ5NCg5NCw5NDA5NDQ5NDg5NDw5NEA5NEQ5NEg5NEw5NFA5NFQ5NFg5NFw5NGA5NGQ5NGg5NGw5NHA5NHQ5NHg5NHw5NIA5NIQ5NIg5NIw5NJA5NJQ5NJg5NJw5NKA5NKQ5NKg5NKw5NLA5NLQ5NLg5NLw5NMA5NMQ5NMg5NMw5NNA5NNQ5NNg5NNw5NOA5NOQ5NOg5NOw5NPA5NPQ5NPg5NPw5NQA5NQQ5NQg5NQw5NRA5NRQ5NRg5NRw5NSA5NSQ5NSg5NSw5NTA5NTQ5NTg5NTw5NUA5NUQ5NUg5NUw5NVA5NVQ5NVg5NVw5NWA5NWQ5NWg5NWw5NXA5NXQ5NXg5NXw5NYA5NYQ5NYg5NYw5NZA5NZQ5NZg5NZw5NaA5NaQ5Nag5Naw5NbA5NbQ5Nbg5Nbw5NcA5NcQ5Ncg5Ncw5NdA5NdQ5Ndg5Ndw5NeA5NeQ5Neg5New5NfA5NfQ5Nfg5Nfw5NgA5NgQ5Ngg5Ngw5NhA5NhQ5Nhg5Nhw5NiA5NiQ5Nig5Niw5NjA5NjQ5Njg5Njw5NkA5NkQ5Nkg5Nkw5NlA5NlQ5Nlg5Nlw5NmA5NmQ5Nmg5Nmw5Nmw5NnA5NnA5NnQ5NnQ5Nng5Nng5Nnw5Nnw5NoA5NoA5NoQ5NoQ5Nog5Nog5Now5Now5NpA5NpA5NpQ5NpQ5Npg5Npg5Npw5Npw5NqA5NqA5NqQ5NqQ5Nqg5Nqg5Nqw5Nqw5NrA5NrA5NrQ5NrQ5Nrg5Nrg5Nrw5Nrw5NsA5NsA5NsQ5NsQ5Nsg5Nsg5Nsw5Nsw5NtA5NtA5NtQ5NtQ5Ntg5Ntg5Ntw5Ntw5NuA5NuA5NuQ5NuQ5Nug5Nug5Nuw5Nuw5NvA5NvA5NvQ5NvQ5Nvg5Nvg5Nvw5Nvw5NwA5NwA5NwQ5NwQ5Nwg5Nwg5Nww5Nww5NxA5NxA5NxQ5NxQ5Nxg5Nxg5Nxw5Nxw5NyA5NyA5NyQ5NyQ5Nyg5Nyg5Nyw5Nyw5NzA5NzA5NzQ5NzQ5Nzg5Nzg5Nzw5Nzw5N0A5N0A5N0Q5N0Q5N0g5N0g5N0w5N0w5N1A5N1A5N1Q5N1Q5N1g5N1g5N1w5N1w5N2A5N2A5N2Q5N2Q5N2g5N2g5N2w5N2w5N3A5N3A5N3Q5N3Q5N3g5N3g5N3w5N3w5N4A5N4A5N4Q5N4Q5N4g5N4g5N4w5N4w5N5A5N5A5N5Q5N5Q5N5g5N5g5N5w5N5w5N6A5N6A5N6Q5N6Q5lcy4=",
                     "unconnected ports hidden": false,
-                    "version": "v0.2"
+                    "version": "v0.3"
                 },
                 {
                     "GID": 13,
                     "Variables": {
                         "subscriptions": {}
                     },
                     "actions": {
@@ -169,36 +206,37 @@
                         "update shape": {
                             "method": "update_shape"
                         }
                     },
                     "additional data": {},
                     "collapsed": false,
                     "display title": "eval",
-                    "identifier": "std.Eval_Node",
+                    "identifier": "examples.special_nodes.Eval_Node",
                     "inputs": [
                         {
                             "GID": 15,
                             "has widget": false,
                             "label": "",
                             "type": "data"
                         }
                     ],
+                    "inspector widget": {},
                     "main widget data": "gASVGAAAAAAAAAB9lIwEdGV4dJSMCmlucFswXVstMV2Ucy4=",
                     "outputs": [
                         {
                             "GID": 16,
                             "label": "",
                             "type": "data"
                         }
                     ],
                     "pos x": 462.86363383615935,
                     "pos y": 370.17323807221123,
                     "state data": "gASVOQAAAAAAAAB9lCiMEG51bSBwYXJhbSBpbnB1dHOUSwGMD2V4cHJlc3Npb24gY29kZZSMCmlucFswXVstMV2UdS4=",
                     "unconnected ports hidden": false,
-                    "version": "v0.2"
+                    "version": "v0.3"
                 },
                 {
                     "GID": 17,
                     "Variables": {
                         "subscriptions": {}
                     },
                     "actions": {
@@ -223,14 +261,15 @@
                         {
                             "GID": 19,
                             "has widget": false,
                             "label": "",
                             "type": "data"
                         }
                     ],
+                    "inspector widget": {},
                     "main widget data": "gAR9lC4=",
                     "outputs": [],
                     "pos x": 796.5680046166863,
                     "pos y": 369.6301042263301,
                     "state data": "gAR9lC4=",
                     "unconnected ports hidden": false,
                     "version": "v0.2"
@@ -253,61 +292,62 @@
                         "update shape": {
                             "method": "update_shape"
                         }
                     },
                     "additional data": {},
                     "collapsed": false,
                     "display title": "slider",
-                    "identifier": "std.Slider_Node",
+                    "identifier": "examples.special_nodes.Slider_Node",
                     "inputs": [
                         {
                             "GID": 24,
                             "default": {
-                                "GID": 27,
+                                "GID": 30,
                                 "identifier": "Data",
                                 "serialized": "gARLAS4="
                             },
                             "has widget": true,
                             "label": "scl",
                             "type": "data",
-                            "widget data": "gASVagAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTRsSjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUSwF1YnMu",
+                            "widget data": "gASVagAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTSQCjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUSwF1YnMu",
                             "widget name": "scale",
                             "widget pos": "besides"
                         },
                         {
-                            "GID": 25,
+                            "GID": 26,
                             "default": {
-                                "GID": 123,
+                                "GID": 32,
                                 "identifier": "Data",
                                 "serialized": "gASJLg=="
                             },
                             "has widget": true,
                             "label": "round",
                             "type": "data",
-                            "widget data": "gASVaQAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTRwSjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUiXVicy4=",
+                            "widget data": "gASVaQAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTSUCjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUiXVicy4=",
                             "widget name": "round",
                             "widget pos": "besides"
                         }
                     ],
+                    "inspector widget": {},
                     "main widget data": "gAR9lC4=",
                     "outputs": [
                         {
-                            "GID": 26,
+                            "GID": 28,
                             "label": "",
                             "type": "data"
                         }
                     ],
                     "pos x": 273.19774517706185,
                     "pos y": 503.4372312306748,
-                    "state data": "gASVEwAAAAAAAAB9lIwDdmFslEc/6FocrAgxJ3Mu",
+                    "state data": "gASVEwAAAAAAAAB9lIwDdmFslEc/4zMzMzMzM3Mu",
                     "unconnected ports hidden": false,
-                    "version": "v0.2"
+                    "version": "v0.3"
                 },
                 {
-                    "GID": 29,
+                    "GID": 33,
                     "Variables": {
                         "subscriptions": {}
                     },
                     "actions": {
                         "change title": {
                             "method": "change_title"
                         },
@@ -323,30 +363,31 @@
                     },
                     "additional data": {},
                     "collapsed": false,
                     "display title": "result",
                     "identifier": "built_in.Result_Node",
                     "inputs": [
                         {
-                            "GID": 31,
+                            "GID": 35,
                             "has widget": false,
                             "label": "",
                             "type": "data"
                         }
                     ],
+                    "inspector widget": {},
                     "main widget data": "gAR9lC4=",
                     "outputs": [],
                     "pos x": 571.2515010942456,
                     "pos y": 555.0662156323955,
                     "state data": "gAR9lC4=",
                     "unconnected ports hidden": false,
                     "version": "v0.2"
                 },
                 {
-                    "GID": 32,
+                    "GID": 36,
                     "Variables": {
                         "subscriptions": {}
                     },
                     "actions": {
                         "change title": {
                             "method": "change_title"
                         },
@@ -362,57 +403,58 @@
                     },
                     "additional data": {},
                     "collapsed": false,
                     "display title": "set var",
                     "identifier": "built_in.SetVar_Node",
                     "inputs": [
                         {
-                            "GID": 38,
+                            "GID": 42,
                             "default": {
-                                "GID": 3801,
+                                "GID": 47,
                                 "identifier": "Data",
                                 "serialized": "gASVBQAAAAAAAACMAWGULg=="
                             },
                             "has widget": true,
                             "label": "var",
                             "type": "data",
-                            "widget data": "gASVbAAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTR0SjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUjAFhlHVicy4=",
+                            "widget data": "gASVbAAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTSYCjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUjAFhlHVicy4=",
                             "widget name": "varname",
                             "widget pos": "besides"
                         },
                         {
-                            "GID": 39,
+                            "GID": 44,
                             "default": {
-                                "GID": 4628,
+                                "GID": 537,
                                 "identifier": "Data",
-                                "serialized": "gASVjRAAAAAAAABYhhAAAFszMDM1LCAzMDM2LCAzMDM3LCAzMDM4LCAzMDM5LCAzMDQwLCAzMDQxLCAzMDQyLCAzMDQzLCAzMDQ0LCAzMDQ1LCAzMDQ2LCAzMDQ3LCAzMDQ4LCAzMDQ5LCAzMDUwLCAzMDUxLCAzMDUyLCAzMDUzLCAzMDU0LCAzMDU1LCAzMDU2LCAzMDU3LCAzMDU4LCAzMDU5LCAzMDYwLCAzMDYxLCAzMDYyLCAzMDYzLCAzMDY0LCAzMDY1LCAzMDY2LCAzMDY3LCAzMDY4LCAzMDY5LCAzMDcwLCAzMDcxLCAzMDcyLCAzMDczLCAzMDc0LCAzMDc1LCAzMDc2LCAzMDc3LCAzMDc4LCAzMDc5LCAzMDgwLCAzMDgxLCAzMDgyLCAzMDgzLCAzMDg0LCAzMDg1LCAzMDg2LCAzMDg3LCAzMDg4LCAzMDg5LCAzMDkwLCAzMDkxLCAzMDkyLCAzMDkzLCAzMDk0LCAzMDk1LCAzMDk2LCAzMDk3LCAzMDk4LCAzMDk5LCAzMTAwLCAzMTAxLCAzMTAyLCAzMTAzLCAzMTA0LCAzMTA1LCAzMTA2LCAzMTA3LCAzMTA4LCAzMTA5LCAzMTEwLCAzMTExLCAzMTEyLCAzMTEzLCAzMTE0LCAzMTE1LCAzMTE2LCAzMTE3LCAzMTE4LCAzMTE5LCAzMTIwLCAzMTIxLCAzMTIyLCAzMTIzLCAzMTI0LCAzMTI1LCAzMTI2LCAzMTI3LCAzMTI4LCAzMTI5LCAzMTMwLCAzMTMxLCAzMTMyLCAzMTMzLCAzMTM0LCAzMTM0LCAzMTM1LCAzMTM2LCAzMTM3LCAzMTM4LCAzMTM5LCAzMTQwLCAzMTQxLCAzMTQyLCAzMTQzLCAzMTQ0LCAzMTQ1LCAzMTQ2LCAzMTQ3LCAzMTQ4LCAzMTQ5LCAzMTUwLCAzMTUxLCAzMTUyLCAzMTUzLCAzMTU0LCAzMTU1LCAzMTU2LCAzMTU3LCAzMTU4LCAzMTU5LCAzMTYwLCAzMTYxLCAzMTYyLCAzMTYzLCAzMTY0LCAzMTY1LCAzMTY2LCAzMTY3LCAzMTY4LCAzMTY5LCAzMTcwLCAzMTcxLCAzMTcyLCAzMTczLCAzMTc0LCAzMTc1LCAzMTc2LCAzMTc3LCAzMTc4LCAzMTc5LCAzMTgwLCAzMTgxLCAzMTgyLCAzMTgzLCAzMTg0LCAzMTg1LCAzMTg2LCAzMTg3LCAzMTg4LCAzMTg5LCAzMTkwLCAzMTkxLCAzMTkyLCAzMTkzLCAzMTk0LCAzMTk1LCAzMTk2LCAzMTk3LCAzMTk4LCAzMTk5LCAzMjAwLCAzMjAxLCAzMjAyLCAzMjAzLCAzMjA0LCAzMjA1LCAzMjA2LCAzMjA3LCAzMjA4LCAzMjA5LCAzMjEwLCAzMjExLCAzMjEyLCAzMjEzLCAzMjE0LCAzMjE1LCAzMjE2LCAzMjE3LCAzMjE4LCAzMjE5LCAzMjIwLCAzMjIxLCAzMjIyLCAzMjIzLCAzMjI0LCAzMjI1LCAzMjI2LCAzMjI3LCAzMjI4LCAzMjI5LCAzMjMwLCAzMjMxLCAzMjMyLCAzMjMzLCAzMjM0LCAzMjM1LCAzMjM2LCAzMjM3LCAzMjM4LCAzMjM5LCAzMjQwLCAzMjQxLCAzMjQyLCAzMjQzLCAzMjQ0LCAzMjQ1LCAzMjQ2LCAzMjQ3LCAzMjQ4LCAzMjQ5LCAzMjUwLCAzMjUxLCAzMjUyLCAzMjUzLCAzMjU0LCAzMjU1LCAzMjU2LCAzMjU3LCAzMjU4LCAzMjU5LCAzMjYwLCAzMjYxLCAzMjYyLCAzMjYzLCAzMjY0LCAzMjY1LCAzMjY2LCAzMjY3LCAzMjY4LCAzMjY5LCAzMjcwLCAzMjcxLCAzMjcyLCAzMjczLCAzMjc0LCAzMjc1LCAzMjc2LCAzMjc3LCAzMjc4LCAzMjc5LCAzMjgwLCAzMjgxLCAzMjgyLCAzMjgzLCAzMjg0LCAzMjg1LCAzMjg2LCAzMjg3LCAzMjg4LCAzMjg5LCAzMjkwLCAzMjkxLCAzMjkyLCAzMjkzLCAzMjk0LCAzMjk1LCAzMjk2LCAzMjk3LCAzMjk4LCAzMjk5LCAzMzAwLCAzMzAxLCAzMzAyLCAzMzAzLCAzMzA0LCAzMzA1LCAzMzA2LCAzMzA3LCAzMzA4LCAzMzA5LCAzMzEwLCAzMzExLCAzMzEyLCAzMzEzLCAzMzE0LCAzMzE1LCAzMzE2LCAzMzE3LCAzMzE4LCAzMzE5LCAzMzIwLCAzMzIxLCAzMzIyLCAzMzIzLCAzMzI0LCAzMzI1LCAzMzI2LCAzMzI3LCAzMzI4LCAzMzI5LCAzMzMwLCAzMzMxLCAzMzMyLCAzMzMzLCAzMzM0LCAzMzM1LCAzMzM2LCAzMzM3LCAzMzM4LCAzMzM5LCAzMzQwLCAzMzQxLCAzMzQyLCAzMzQzLCAzMzQ0LCAzMzQ1LCAzMzQ2LCAzMzQ3LCAzMzQ4LCAzMzQ5LCAzMzUwLCAzMzUxLCAzMzUyLCAzMzUzLCAzMzU0LCAzMzU1LCAzMzU2LCAzMzU3LCAzMzU4LCAzMzU5LCAzMzYwLCAzMzYxLCAzMzYyLCAzMzYzLCAzMzY0LCAzMzY1LCAzMzY2LCAzMzY3LCAzMzY4LCAzMzY5LCAzMzcwLCAzMzcxLCAzMzcyLCAzMzczLCAzMzc0LCAzMzc1LCAzMzc2LCAzMzc3LCAzMzc4LCAzMzc5LCAzMzgwLCAzMzgxLCAzMzgyLCAzMzgzLCAzMzg0LCAzMzg1LCAzMzg2LCAzMzg3LCAzMzg4LCAzMzg5LCAzMzkwLCAzMzkxLCAzMzkyLCAzMzkzLCAzMzk0LCAzMzk1LCAzMzk2LCAzMzk3LCAzMzk4LCAzMzk5LCAzNDAwLCAzNDAxLCAzNDAyLCAzNDAzLCAzNDA0LCAzNDA1LCAzNDA2LCAzNDA3LCAzNDA4LCAzNDA5LCAzNDEwLCAzNDExLCAzNDEyLCAzNDEzLCAzNDE0LCAzNDE1LCAzNDE2LCAzNDE3LCAzNDE4LCAzNDE5LCAzNDIwLCAzNDIxLCAzNDIyLCAzNDIzLCAzNDI0LCAzNDI1LCAzNDI2LCAzNDI3LCAzNDI4LCAzNDI5LCAzNDMwLCAzNDMxLCAzNDMyLCAzNDMzLCAzNDM0LCAzNDM1LCAzNDM2LCAzNDM3LCAzNDM4LCAzNDM5LCAzNDQwLCAzNDQxLCAzNDQyLCAzNDQzLCAzNDQ0LCAzNDQ1LCAzNDQ2LCAzNDQ3LCAzNDQ4LCAzNDQ5LCAzNDUwLCAzNDUxLCAzNDUyLCAzNDUzLCAzNDU0LCAzNDU1LCAzNDU2LCAzNDU3LCAzNDU4LCAzNDU5LCAzNDYwLCAzNDYxLCAzNDYyLCAzNDYzLCAzNDY0LCAzNDY1LCAzNDY2LCAzNDY3LCAzNDY4LCAzNDY5LCAzNDcwLCAzNDcxLCAzNDcyLCAzNDczLCAzNDc0LCAzNDc1LCAzNDc2LCAzNDc3LCAzNDc4LCAzNDc5LCAzNDgwLCAzNDgxLCAzNDgyLCAzNDgzLCAzNDg0LCAzNDg1LCAzNDg2LCAzNDg3LCAzNDg4LCAzNDg5LCAzNDkwLCAzNDkxLCAzNDkyLCAzNDkzLCAzNDk0LCAzNDk1LCAzNDk2LCAzNDk3LCAzNDk4LCAzNDk5LCAzNTAwLCAzNTAxLCAzNTAyLCAzNTAzLCAzNTA0LCAzNTA1LCAzNTA2LCAzNTA3LCAzNTA4LCAzNTA5LCAzNTEwLCAzNTExLCAzNTEyLCAzNTEzLCAzNTE0LCAzNTE1LCAzNTE2LCAzNTE3LCAzNTE4LCAzNTE5LCAzNTIwLCAzNTIxLCAzNTIyLCAzNTIzLCAzNTI0LCAzNTI1LCAzNTI2LCAzNTI3LCAzNTI4LCAzNTI5LCAzNTMwLCAzNTMxLCAzNTMyLCAzNTMzLCAzNTM0LCAzNTM1LCAzNTM2LCAzNTM3LCAzNTM4LCAzNTM5LCAzNTQwLCAzNTQxLCAzNTQyLCAzNTQzLCAzNTQ0LCAzNTQ1LCAzNTQ2LCAzNTQ3LCAzNTQ4LCAzNTQ5LCAzNTUwLCAzNTUxLCAzNTUyLCAzNTUzLCAzNTU0LCAzNTU1LCAzNTU2LCAzNTU3LCAzNTU4LCAzNTU5LCAzNTYwLCAzNTYxLCAzNTYyLCAzNTYzLCAzNTY0LCAzNTY1LCAzNTY2LCAzNTY3LCAzNTY4LCAzNTY5LCAzNTcwLCAzNTcxLCAzNTcyLCAzNTczLCAzNTc0LCAzNTc1LCAzNTc2LCAzNTc3LCAzNTc4LCAzNTc5LCAzNTgwLCAzNTgxLCAzNTgyLCAzNTgzLCAzNTg0LCAzNTg1LCAzNTg2LCAzNTg3LCAzNTg4LCAzNTg5LCAzNTkwLCAzNTkxLCAzNTkyLCAzNTkzLCAzNTk0LCAzNTk1LCAzNTk2LCAzNTk3LCAzNTk4LCAzNTk5LCAzNjAwLCAzNjAxLCAzNjAyLCAzNjAzLCAzNjA0LCAzNjA1LCAzNjA2LCAzNjA3LCAzNjA4LCAzNjA5LCAzNjEwLCAzNjExLCAzNjEyLCAzNjEzLCAzNjE0LCAzNjE1LCAzNjE2LCAzNjE3LCAzNjE4LCAzNjE5LCAzNjIwLCAzNjIxLCAzNjIyLCAzNjIzLCAzNjI0LCAzNjI1LCAzNjI2LCAzNjI3LCAzNjI4LCAzNjI5LCAzNjMwLCAzNjMxLCAzNjMyLCAzNjMzLCAzNjM0LCAzNjM1LCAzNjM2LCAzNjM3LCAzNjM4LCAzNjM5LCAzNjQwLCAzNjQxLCAzNjQyLCAzNjQzLCAzNjQ0LCAzNjQ1LCAzNjQ2LCAzNjQ3LCAzNjQ4LCAzNjQ5LCAzNjUwLCAzNjUxLCAzNjUyLCAzNjUzLCAzNjU0LCAzNjU1LCAzNjU2LCAzNjU3LCAzNjU4LCAzNjU5LCAzNjYwLCAzNjYxLCAzNjYyLCAzNjYzLCAzNjY0LCAzNjY1LCAzNjY2LCAzNjY3LCAzNjY4LCAzNjY5LCAzNjcwLCAzNjcxLCAzNjcyLCAzNjczLCAzNjc0LCAzNjc1LCAzNjc2LCAzNjc3LCAzNjc4LCAzNjc5LCAzNjgwLCAzNjgxLCAzNjgyLCAzNjgzLCAzNjg0LCAzNjg1LCAzNjg2LCAzNjg3LCAzNjg4LCAzNjg5LCAzNjkwLCAzNjkxLCAzNjkyLCAzNjkzLCAzNjk0LCAzNjk1LCAzNjk2LCAzNjk3LCAzNjk4LCAzNjk5LCAzNzAwLCAzNzAxLCAzNzAyLCAzNzAzLCAzNzA0LCAzNzA1LCAzNzA2LCAzNzA3LCAzNzA4LCAzNzA5LCAzNzEwLCAzNzExLCAzNzEyLCAzNzEzLCAzNzE0LCAzNzE1LCAzNzE2LCAzNzE3LCAzNzE4LCAzNzE5LCAzNzIwLCAzNzIxLCAzNzIyLCAzNzIzLCAzNzI0LCAzNzI1LCAzNzI2LCAzNzI3LCAzNzI4LCAzNzI5LCAzNzMwLCAzNzMxLCAzNzMyLCAzNzMzLCAzNzM0LCAzNzM1LCAzNzM2LCAzNzM3LCAzNzM4XZQu"
+                                "serialized": "gASVQRQAAAAAAABYOhQAAFszMDM1LCAzMDM2LCAzMDM3LCAzMDM4LCAzMDM5LCAzMDQwLCAzMDQxLCAzMDQyLCAzMDQzLCAzMDQ0LCAzMDQ1LCAzMDQ2LCAzMDQ3LCAzMDQ4LCAzMDQ5LCAzMDUwLCAzMDUxLCAzMDUyLCAzMDUzLCAzMDU0LCAzMDU1LCAzMDU2LCAzMDU3LCAzMDU4LCAzMDU5LCAzMDYwLCAzMDYxLCAzMDYyLCAzMDYzLCAzMDY0LCAzMDY1LCAzMDY2LCAzMDY3LCAzMDY4LCAzMDY5LCAzMDcwLCAzMDcxLCAzMDcyLCAzMDczLCAzMDc0LCAzMDc1LCAzMDc2LCAzMDc3LCAzMDc4LCAzMDc5LCAzMDgwLCAzMDgxLCAzMDgyLCAzMDgzLCAzMDg0LCAzMDg1LCAzMDg2LCAzMDg3LCAzMDg4LCAzMDg5LCAzMDkwLCAzMDkxLCAzMDkyLCAzMDkzLCAzMDk0LCAzMDk1LCAzMDk2LCAzMDk3LCAzMDk4LCAzMDk5LCAzMTAwLCAzMTAxLCAzMTAyLCAzMTAzLCAzMTA0LCAzMTA1LCAzMTA2LCAzMTA3LCAzMTA4LCAzMTA5LCAzMTEwLCAzMTExLCAzMTEyLCAzMTEzLCAzMTE0LCAzMTE1LCAzMTE2LCAzMTE3LCAzMTE4LCAzMTE5LCAzMTIwLCAzMTIxLCAzMTIyLCAzMTIzLCAzMTI0LCAzMTI1LCAzMTI2LCAzMTI3LCAzMTI4LCAzMTI5LCAzMTMwLCAzMTMxLCAzMTMyLCAzMTMzLCAzMTM0LCAzMTM0LCAzMTM1LCAzMTM2LCAzMTM3LCAzMTM4LCAzMTM5LCAzMTQwLCAzMTQxLCAzMTQyLCAzMTQzLCAzMTQ0LCAzMTQ1LCAzMTQ2LCAzMTQ3LCAzMTQ4LCAzMTQ5LCAzMTUwLCAzMTUxLCAzMTUyLCAzMTUzLCAzMTU0LCAzMTU1LCAzMTU2LCAzMTU3LCAzMTU4LCAzMTU5LCAzMTYwLCAzMTYxLCAzMTYyLCAzMTYzLCAzMTY0LCAzMTY1LCAzMTY2LCAzMTY3LCAzMTY4LCAzMTY5LCAzMTcwLCAzMTcxLCAzMTcyLCAzMTczLCAzMTc0LCAzMTc1LCAzMTc2LCAzMTc3LCAzMTc4LCAzMTc5LCAzMTgwLCAzMTgxLCAzMTgyLCAzMTgzLCAzMTg0LCAzMTg1LCAzMTg2LCAzMTg3LCAzMTg4LCAzMTg5LCAzMTkwLCAzMTkxLCAzMTkyLCAzMTkzLCAzMTk0LCAzMTk1LCAzMTk2LCAzMTk3LCAzMTk4LCAzMTk5LCAzMjAwLCAzMjAxLCAzMjAyLCAzMjAzLCAzMjA0LCAzMjA1LCAzMjA2LCAzMjA3LCAzMjA4LCAzMjA5LCAzMjEwLCAzMjExLCAzMjEyLCAzMjEzLCAzMjE0LCAzMjE1LCAzMjE2LCAzMjE3LCAzMjE4LCAzMjE5LCAzMjIwLCAzMjIxLCAzMjIyLCAzMjIzLCAzMjI0LCAzMjI1LCAzMjI2LCAzMjI3LCAzMjI4LCAzMjI5LCAzMjMwLCAzMjMxLCAzMjMyLCAzMjMzLCAzMjM0LCAzMjM1LCAzMjM2LCAzMjM3LCAzMjM4LCAzMjM5LCAzMjQwLCAzMjQxLCAzMjQyLCAzMjQzLCAzMjQ0LCAzMjQ1LCAzMjQ2LCAzMjQ3LCAzMjQ4LCAzMjQ5LCAzMjUwLCAzMjUxLCAzMjUyLCAzMjUzLCAzMjU0LCAzMjU1LCAzMjU2LCAzMjU3LCAzMjU4LCAzMjU5LCAzMjYwLCAzMjYxLCAzMjYyLCAzMjYzLCAzMjY0LCAzMjY1LCAzMjY2LCAzMjY3LCAzMjY4LCAzMjY5LCAzMjcwLCAzMjcxLCAzMjcyLCAzMjczLCAzMjc0LCAzMjc1LCAzMjc2LCAzMjc3LCAzMjc4LCAzMjc5LCAzMjgwLCAzMjgxLCAzMjgyLCAzMjgzLCAzMjg0LCAzMjg1LCAzMjg2LCAzMjg3LCAzMjg4LCAzMjg5LCAzMjkwLCAzMjkxLCAzMjkyLCAzMjkzLCAzMjk0LCAzMjk1LCAzMjk2LCAzMjk3LCAzMjk4LCAzMjk5LCAzMzAwLCAzMzAxLCAzMzAyLCAzMzAzLCAzMzA0LCAzMzA1LCAzMzA2LCAzMzA3LCAzMzA4LCAzMzA5LCAzMzEwLCAzMzExLCAzMzEyLCAzMzEzLCAzMzE0LCAzMzE1LCAzMzE2LCAzMzE3LCAzMzE4LCAzMzE5LCAzMzIwLCAzMzIxLCAzMzIyLCAzMzIzLCAzMzI0LCAzMzI1LCAzMzI2LCAzMzI3LCAzMzI4LCAzMzI5LCAzMzMwLCAzMzMxLCAzMzMyLCAzMzMzLCAzMzM0LCAzMzM1LCAzMzM2LCAzMzM3LCAzMzM4LCAzMzM5LCAzMzQwLCAzMzQxLCAzMzQyLCAzMzQzLCAzMzQ0LCAzMzQ1LCAzMzQ2LCAzMzQ3LCAzMzQ4LCAzMzQ5LCAzMzUwLCAzMzUxLCAzMzUyLCAzMzUzLCAzMzU0LCAzMzU1LCAzMzU2LCAzMzU3LCAzMzU4LCAzMzU5LCAzMzYwLCAzMzYxLCAzMzYyLCAzMzYzLCAzMzY0LCAzMzY1LCAzMzY2LCAzMzY3LCAzMzY4LCAzMzY5LCAzMzcwLCAzMzcxLCAzMzcyLCAzMzczLCAzMzc0LCAzMzc1LCAzMzc2LCAzMzc3LCAzMzc4LCAzMzc5LCAzMzgwLCAzMzgxLCAzMzgyLCAzMzgzLCAzMzg0LCAzMzg1LCAzMzg2LCAzMzg3LCAzMzg4LCAzMzg5LCAzMzkwLCAzMzkxLCAzMzkyLCAzMzkzLCAzMzk0LCAzMzk1LCAzMzk2LCAzMzk3LCAzMzk4LCAzMzk5LCAzNDAwLCAzNDAxLCAzNDAyLCAzNDAzLCAzNDA0LCAzNDA1LCAzNDA2LCAzNDA3LCAzNDA4LCAzNDA5LCAzNDEwLCAzNDExLCAzNDEyLCAzNDEzLCAzNDE0LCAzNDE1LCAzNDE2LCAzNDE3LCAzNDE4LCAzNDE5LCAzNDIwLCAzNDIxLCAzNDIyLCAzNDIzLCAzNDI0LCAzNDI1LCAzNDI2LCAzNDI3LCAzNDI4LCAzNDI5LCAzNDMwLCAzNDMxLCAzNDMyLCAzNDMzLCAzNDM0LCAzNDM1LCAzNDM2LCAzNDM3LCAzNDM4LCAzNDM5LCAzNDQwLCAzNDQxLCAzNDQyLCAzNDQzLCAzNDQ0LCAzNDQ1LCAzNDQ2LCAzNDQ3LCAzNDQ4LCAzNDQ5LCAzNDUwLCAzNDUxLCAzNDUyLCAzNDUzLCAzNDU0LCAzNDU1LCAzNDU2LCAzNDU3LCAzNDU4LCAzNDU5LCAzNDYwLCAzNDYxLCAzNDYyLCAzNDYzLCAzNDY0LCAzNDY1LCAzNDY2LCAzNDY3LCAzNDY4LCAzNDY5LCAzNDcwLCAzNDcxLCAzNDcyLCAzNDczLCAzNDc0LCAzNDc1LCAzNDc2LCAzNDc3LCAzNDc4LCAzNDc5LCAzNDgwLCAzNDgxLCAzNDgyLCAzNDgzLCAzNDg0LCAzNDg1LCAzNDg2LCAzNDg3LCAzNDg4LCAzNDg5LCAzNDkwLCAzNDkxLCAzNDkyLCAzNDkzLCAzNDk0LCAzNDk1LCAzNDk2LCAzNDk3LCAzNDk4LCAzNDk5LCAzNTAwLCAzNTAxLCAzNTAyLCAzNTAzLCAzNTA0LCAzNTA1LCAzNTA2LCAzNTA3LCAzNTA4LCAzNTA5LCAzNTEwLCAzNTExLCAzNTEyLCAzNTEzLCAzNTE0LCAzNTE1LCAzNTE2LCAzNTE3LCAzNTE4LCAzNTE5LCAzNTIwLCAzNTIxLCAzNTIyLCAzNTIzLCAzNTI0LCAzNTI1LCAzNTI2LCAzNTI3LCAzNTI4LCAzNTI5LCAzNTMwLCAzNTMxLCAzNTMyLCAzNTMzLCAzNTM0LCAzNTM1LCAzNTM2LCAzNTM3LCAzNTM4LCAzNTM5LCAzNTQwLCAzNTQxLCAzNTQyLCAzNTQzLCAzNTQ0LCAzNTQ1LCAzNTQ2LCAzNTQ3LCAzNTQ4LCAzNTQ5LCAzNTUwLCAzNTUxLCAzNTUyLCAzNTUzLCAzNTU0LCAzNTU1LCAzNTU2LCAzNTU3LCAzNTU4LCAzNTU5LCAzNTYwLCAzNTYxLCAzNTYyLCAzNTYzLCAzNTY0LCAzNTY1LCAzNTY2LCAzNTY3LCAzNTY4LCAzNTY5LCAzNTcwLCAzNTcxLCAzNTcyLCAzNTczLCAzNTc0LCAzNTc1LCAzNTc2LCAzNTc3LCAzNTc4LCAzNTc5LCAzNTgwLCAzNTgxLCAzNTgyLCAzNTgzLCAzNTg0LCAzNTg1LCAzNTg2LCAzNTg3LCAzNTg4LCAzNTg5LCAzNTkwLCAzNTkxLCAzNTkyLCAzNTkzLCAzNTk0LCAzNTk1LCAzNTk2LCAzNTk3LCAzNTk4LCAzNTk5LCAzNjAwLCAzNjAxLCAzNjAyLCAzNjAzLCAzNjA0LCAzNjA1LCAzNjA2LCAzNjA3LCAzNjA4LCAzNjA5LCAzNjEwLCAzNjExLCAzNjEyLCAzNjEzLCAzNjE0LCAzNjE1LCAzNjE2LCAzNjE3LCAzNjE4LCAzNjE5LCAzNjIwLCAzNjIxLCAzNjIyLCAzNjIzLCAzNjI0LCAzNjI1LCAzNjI2LCAzNjI3LCAzNjI4LCAzNjI5LCAzNjMwLCAzNjMxLCAzNjMyLCAzNjMzLCAzNjM0LCAzNjM1LCAzNjM2LCAzNjM3LCAzNjM4LCAzNjM5LCAzNjQwLCAzNjQxLCAzNjQyLCAzNjQzLCAzNjQ0LCAzNjQ1LCAzNjQ2LCAzNjQ3LCAzNjQ4LCAzNjQ5LCAzNjUwLCAzNjUxLCAzNjUyLCAzNjUzLCAzNjU0LCAzNjU1LCAzNjU2LCAzNjU3LCAzNjU4LCAzNjU5LCAzNjYwLCAzNjYxLCAzNjYyLCAzNjYzLCAzNjY0LCAzNjY1LCAzNjY2LCAzNjY3LCAzNjY4LCAzNjY5LCAzNjcwLCAzNjcxLCAzNjcyLCAzNjczLCAzNjc0LCAzNjc1LCAzNjc2LCAzNjc3LCAzNjc4LCAzNjc5LCAzNjgwLCAzNjgxLCAzNjgyLCAzNjgzLCAzNjg0LCAzNjg1LCAzNjg2LCAzNjg3LCAzNjg4LCAzNjg5LCAzNjkwLCAzNjkxLCAzNjkyLCAzNjkzLCAzNjk0LCAzNjk1LCAzNjk2LCAzNjk3LCAzNjk4LCAzNjk5LCAzNzAwLCAzNzAxLCAzNzAyLCAzNzAzLCAzNzA0LCAzNzA1LCAzNzA2LCAzNzA3LCAzNzA4LCAzNzA5LCAzNzEwLCAzNzExLCAzNzEyLCAzNzEzLCAzNzE0LCAzNzE1LCAzNzE2LCAzNzE3LCAzNzE4LCAzNzE5LCAzNzIwLCAzNzIxLCAzNzIyLCAzNzIzLCAzNzI0LCAzNzI1LCAzNzI2LCAzNzI3LCAzNzI4LCAzNzI5LCAzNzMwLCAzNzMxLCAzNzMyLCAzNzMzLCAzNzM0LCAzNzM1LCAzNzM2LCAzNzM3LCAzNzM4LCAzNzM5LCAzNzM5LCAzNzQwLCAzNzQwLCAzNzQxLCAzNzQxLCAzNzQyLCAzNzQyLCAzNzQzLCAzNzQzLCAzNzQ0LCAzNzQ0LCAzNzQ1LCAzNzQ1LCAzNzQ2LCAzNzQ2LCAzNzQ3LCAzNzQ3LCAzNzQ4LCAzNzQ4LCAzNzQ5LCAzNzQ5LCAzNzUwLCAzNzUwLCAzNzUxLCAzNzUxLCAzNzUyLCAzNzUyLCAzNzUzLCAzNzUzLCAzNzU0LCAzNzU0LCAzNzU1LCAzNzU1LCAzNzU2LCAzNzU2LCAzNzU3LCAzNzU3LCAzNzU4LCAzNzU4LCAzNzU5LCAzNzU5LCAzNzYwLCAzNzYwLCAzNzYxLCAzNzYxLCAzNzYyLCAzNzYyLCAzNzYzLCAzNzYzLCAzNzY0LCAzNzY0LCAzNzY1LCAzNzY1LCAzNzY2LCAzNzY2LCAzNzY3LCAzNzY3LCAzNzY4LCAzNzY4LCAzNzY5LCAzNzY5LCAzNzcwLCAzNzcwLCAzNzcxLCAzNzcxLCAzNzcyLCAzNzcyLCAzNzczLCAzNzczLCAzNzc0LCAzNzc0LCAzNzc1LCAzNzc1LCAzNzc2LCAzNzc2LCAzNzc3LCAzNzc3LCAzNzc4LCAzNzc4LCAzNzc5LCAzNzc5LCAzNzgwLCAzNzgwLCAzNzgxLCAzNzgxLCAzNzgyLCAzNzgyLCAzNzgzLCAzNzgzLCAzNzg0LCAzNzg0LCAzNzg1LCAzNzg1LCAzNzg2LCAzNzg2LCAzNzg3LCAzNzg3LCAzNzg4LCAzNzg4LCAzNzg5LCAzNzg5LCAzNzkwLCAzNzkwLCAzNzkxLCAzNzkxLCAzNzkyLCAzNzkyLCAzNzkzLCAzNzkzLCAzNzk0LCAzNzk0LCAzNzk1LCAzNzk1LCAzNzk2LCAzNzk2LCAzNzk3LCAzNzk3LCAzNzk4LCAzNzk4LCAzNzk5LCAzNzk5LCAzODAwLCAzODAwLCAzODAxLCAzODAxLCAzODAyLCAzODAyLCAzODAzLCAzODAzLCAzODA0LCAzODA0LCAzODA1LCAzODA1LCAzODA2LCAzODA2LCAzODA3LCAzODA3LCAzODA4LCAzODA4LCAzODA5LCAzODA5LCAzODEwLCAzODEwLCAzODExLCAzODExLCAzODEyLCAzODEyLCAzODEzLCAzODEzLCAzODE0LCAzODE0LCAzODE1LCAzODE1LCAzODE2LCAzODE2LCAzODE3LCAzODE3XZQu"
                             },
                             "has widget": true,
                             "label": "val",
                             "type": "data",
-                            "widget data": "gASV9BAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTR4SjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUWIYQAABbMzAzNSwgMzAzNiwgMzAzNywgMzAzOCwgMzAzOSwgMzA0MCwgMzA0MSwgMzA0MiwgMzA0MywgMzA0NCwgMzA0NSwgMzA0NiwgMzA0NywgMzA0OCwgMzA0OSwgMzA1MCwgMzA1MSwgMzA1MiwgMzA1MywgMzA1NCwgMzA1NSwgMzA1NiwgMzA1NywgMzA1OCwgMzA1OSwgMzA2MCwgMzA2MSwgMzA2MiwgMzA2MywgMzA2NCwgMzA2NSwgMzA2NiwgMzA2NywgMzA2OCwgMzA2OSwgMzA3MCwgMzA3MSwgMzA3MiwgMzA3MywgMzA3NCwgMzA3NSwgMzA3NiwgMzA3NywgMzA3OCwgMzA3OSwgMzA4MCwgMzA4MSwgMzA4MiwgMzA4MywgMzA4NCwgMzA4NSwgMzA4NiwgMzA4NywgMzA4OCwgMzA4OSwgMzA5MCwgMzA5MSwgMzA5MiwgMzA5MywgMzA5NCwgMzA5NSwgMzA5NiwgMzA5NywgMzA5OCwgMzA5OSwgMzEwMCwgMzEwMSwgMzEwMiwgMzEwMywgMzEwNCwgMzEwNSwgMzEwNiwgMzEwNywgMzEwOCwgMzEwOSwgMzExMCwgMzExMSwgMzExMiwgMzExMywgMzExNCwgMzExNSwgMzExNiwgMzExNywgMzExOCwgMzExOSwgMzEyMCwgMzEyMSwgMzEyMiwgMzEyMywgMzEyNCwgMzEyNSwgMzEyNiwgMzEyNywgMzEyOCwgMzEyOSwgMzEzMCwgMzEzMSwgMzEzMiwgMzEzMywgMzEzNCwgMzEzNCwgMzEzNSwgMzEzNiwgMzEzNywgMzEzOCwgMzEzOSwgMzE0MCwgMzE0MSwgMzE0MiwgMzE0MywgMzE0NCwgMzE0NSwgMzE0NiwgMzE0NywgMzE0OCwgMzE0OSwgMzE1MCwgMzE1MSwgMzE1MiwgMzE1MywgMzE1NCwgMzE1NSwgMzE1NiwgMzE1NywgMzE1OCwgMzE1OSwgMzE2MCwgMzE2MSwgMzE2MiwgMzE2MywgMzE2NCwgMzE2NSwgMzE2NiwgMzE2NywgMzE2OCwgMzE2OSwgMzE3MCwgMzE3MSwgMzE3MiwgMzE3MywgMzE3NCwgMzE3NSwgMzE3NiwgMzE3NywgMzE3OCwgMzE3OSwgMzE4MCwgMzE4MSwgMzE4MiwgMzE4MywgMzE4NCwgMzE4NSwgMzE4NiwgMzE4NywgMzE4OCwgMzE4OSwgMzE5MCwgMzE5MSwgMzE5MiwgMzE5MywgMzE5NCwgMzE5NSwgMzE5NiwgMzE5NywgMzE5OCwgMzE5OSwgMzIwMCwgMzIwMSwgMzIwMiwgMzIwMywgMzIwNCwgMzIwNSwgMzIwNiwgMzIwNywgMzIwOCwgMzIwOSwgMzIxMCwgMzIxMSwgMzIxMiwgMzIxMywgMzIxNCwgMzIxNSwgMzIxNiwgMzIxNywgMzIxOCwgMzIxOSwgMzIyMCwgMzIyMSwgMzIyMiwgMzIyMywgMzIyNCwgMzIyNSwgMzIyNiwgMzIyNywgMzIyOCwgMzIyOSwgMzIzMCwgMzIzMSwgMzIzMiwgMzIzMywgMzIzNCwgMzIzNSwgMzIzNiwgMzIzNywgMzIzOCwgMzIzOSwgMzI0MCwgMzI0MSwgMzI0MiwgMzI0MywgMzI0NCwgMzI0NSwgMzI0NiwgMzI0NywgMzI0OCwgMzI0OSwgMzI1MCwgMzI1MSwgMzI1MiwgMzI1MywgMzI1NCwgMzI1NSwgMzI1NiwgMzI1NywgMzI1OCwgMzI1OSwgMzI2MCwgMzI2MSwgMzI2MiwgMzI2MywgMzI2NCwgMzI2NSwgMzI2NiwgMzI2NywgMzI2OCwgMzI2OSwgMzI3MCwgMzI3MSwgMzI3MiwgMzI3MywgMzI3NCwgMzI3NSwgMzI3NiwgMzI3NywgMzI3OCwgMzI3OSwgMzI4MCwgMzI4MSwgMzI4MiwgMzI4MywgMzI4NCwgMzI4NSwgMzI4NiwgMzI4NywgMzI4OCwgMzI4OSwgMzI5MCwgMzI5MSwgMzI5MiwgMzI5MywgMzI5NCwgMzI5NSwgMzI5NiwgMzI5NywgMzI5OCwgMzI5OSwgMzMwMCwgMzMwMSwgMzMwMiwgMzMwMywgMzMwNCwgMzMwNSwgMzMwNiwgMzMwNywgMzMwOCwgMzMwOSwgMzMxMCwgMzMxMSwgMzMxMiwgMzMxMywgMzMxNCwgMzMxNSwgMzMxNiwgMzMxNywgMzMxOCwgMzMxOSwgMzMyMCwgMzMyMSwgMzMyMiwgMzMyMywgMzMyNCwgMzMyNSwgMzMyNiwgMzMyNywgMzMyOCwgMzMyOSwgMzMzMCwgMzMzMSwgMzMzMiwgMzMzMywgMzMzNCwgMzMzNSwgMzMzNiwgMzMzNywgMzMzOCwgMzMzOSwgMzM0MCwgMzM0MSwgMzM0MiwgMzM0MywgMzM0NCwgMzM0NSwgMzM0NiwgMzM0NywgMzM0OCwgMzM0OSwgMzM1MCwgMzM1MSwgMzM1MiwgMzM1MywgMzM1NCwgMzM1NSwgMzM1NiwgMzM1NywgMzM1OCwgMzM1OSwgMzM2MCwgMzM2MSwgMzM2MiwgMzM2MywgMzM2NCwgMzM2NSwgMzM2NiwgMzM2NywgMzM2OCwgMzM2OSwgMzM3MCwgMzM3MSwgMzM3MiwgMzM3MywgMzM3NCwgMzM3NSwgMzM3NiwgMzM3NywgMzM3OCwgMzM3OSwgMzM4MCwgMzM4MSwgMzM4MiwgMzM4MywgMzM4NCwgMzM4NSwgMzM4NiwgMzM4NywgMzM4OCwgMzM4OSwgMzM5MCwgMzM5MSwgMzM5MiwgMzM5MywgMzM5NCwgMzM5NSwgMzM5NiwgMzM5NywgMzM5OCwgMzM5OSwgMzQwMCwgMzQwMSwgMzQwMiwgMzQwMywgMzQwNCwgMzQwNSwgMzQwNiwgMzQwNywgMzQwOCwgMzQwOSwgMzQxMCwgMzQxMSwgMzQxMiwgMzQxMywgMzQxNCwgMzQxNSwgMzQxNiwgMzQxNywgMzQxOCwgMzQxOSwgMzQyMCwgMzQyMSwgMzQyMiwgMzQyMywgMzQyNCwgMzQyNSwgMzQyNiwgMzQyNywgMzQyOCwgMzQyOSwgMzQzMCwgMzQzMSwgMzQzMiwgMzQzMywgMzQzNCwgMzQzNSwgMzQzNiwgMzQzNywgMzQzOCwgMzQzOSwgMzQ0MCwgMzQ0MSwgMzQ0MiwgMzQ0MywgMzQ0NCwgMzQ0NSwgMzQ0NiwgMzQ0NywgMzQ0OCwgMzQ0OSwgMzQ1MCwgMzQ1MSwgMzQ1MiwgMzQ1MywgMzQ1NCwgMzQ1NSwgMzQ1NiwgMzQ1NywgMzQ1OCwgMzQ1OSwgMzQ2MCwgMzQ2MSwgMzQ2MiwgMzQ2MywgMzQ2NCwgMzQ2NSwgMzQ2NiwgMzQ2NywgMzQ2OCwgMzQ2OSwgMzQ3MCwgMzQ3MSwgMzQ3MiwgMzQ3MywgMzQ3NCwgMzQ3NSwgMzQ3NiwgMzQ3NywgMzQ3OCwgMzQ3OSwgMzQ4MCwgMzQ4MSwgMzQ4MiwgMzQ4MywgMzQ4NCwgMzQ4NSwgMzQ4NiwgMzQ4NywgMzQ4OCwgMzQ4OSwgMzQ5MCwgMzQ5MSwgMzQ5MiwgMzQ5MywgMzQ5NCwgMzQ5NSwgMzQ5NiwgMzQ5NywgMzQ5OCwgMzQ5OSwgMzUwMCwgMzUwMSwgMzUwMiwgMzUwMywgMzUwNCwgMzUwNSwgMzUwNiwgMzUwNywgMzUwOCwgMzUwOSwgMzUxMCwgMzUxMSwgMzUxMiwgMzUxMywgMzUxNCwgMzUxNSwgMzUxNiwgMzUxNywgMzUxOCwgMzUxOSwgMzUyMCwgMzUyMSwgMzUyMiwgMzUyMywgMzUyNCwgMzUyNSwgMzUyNiwgMzUyNywgMzUyOCwgMzUyOSwgMzUzMCwgMzUzMSwgMzUzMiwgMzUzMywgMzUzNCwgMzUzNSwgMzUzNiwgMzUzNywgMzUzOCwgMzUzOSwgMzU0MCwgMzU0MSwgMzU0MiwgMzU0MywgMzU0NCwgMzU0NSwgMzU0NiwgMzU0NywgMzU0OCwgMzU0OSwgMzU1MCwgMzU1MSwgMzU1MiwgMzU1MywgMzU1NCwgMzU1NSwgMzU1NiwgMzU1NywgMzU1OCwgMzU1OSwgMzU2MCwgMzU2MSwgMzU2MiwgMzU2MywgMzU2NCwgMzU2NSwgMzU2NiwgMzU2NywgMzU2OCwgMzU2OSwgMzU3MCwgMzU3MSwgMzU3MiwgMzU3MywgMzU3NCwgMzU3NSwgMzU3NiwgMzU3NywgMzU3OCwgMzU3OSwgMzU4MCwgMzU4MSwgMzU4MiwgMzU4MywgMzU4NCwgMzU4NSwgMzU4NiwgMzU4NywgMzU4OCwgMzU4OSwgMzU5MCwgMzU5MSwgMzU5MiwgMzU5MywgMzU5NCwgMzU5NSwgMzU5NiwgMzU5NywgMzU5OCwgMzU5OSwgMzYwMCwgMzYwMSwgMzYwMiwgMzYwMywgMzYwNCwgMzYwNSwgMzYwNiwgMzYwNywgMzYwOCwgMzYwOSwgMzYxMCwgMzYxMSwgMzYxMiwgMzYxMywgMzYxNCwgMzYxNSwgMzYxNiwgMzYxNywgMzYxOCwgMzYxOSwgMzYyMCwgMzYyMSwgMzYyMiwgMzYyMywgMzYyNCwgMzYyNSwgMzYyNiwgMzYyNywgMzYyOCwgMzYyOSwgMzYzMCwgMzYzMSwgMzYzMiwgMzYzMywgMzYzNCwgMzYzNSwgMzYzNiwgMzYzNywgMzYzOCwgMzYzOSwgMzY0MCwgMzY0MSwgMzY0MiwgMzY0MywgMzY0NCwgMzY0NSwgMzY0NiwgMzY0NywgMzY0OCwgMzY0OSwgMzY1MCwgMzY1MSwgMzY1MiwgMzY1MywgMzY1NCwgMzY1NSwgMzY1NiwgMzY1NywgMzY1OCwgMzY1OSwgMzY2MCwgMzY2MSwgMzY2MiwgMzY2MywgMzY2NCwgMzY2NSwgMzY2NiwgMzY2NywgMzY2OCwgMzY2OSwgMzY3MCwgMzY3MSwgMzY3MiwgMzY3MywgMzY3NCwgMzY3NSwgMzY3NiwgMzY3NywgMzY3OCwgMzY3OSwgMzY4MCwgMzY4MSwgMzY4MiwgMzY4MywgMzY4NCwgMzY4NSwgMzY4NiwgMzY4NywgMzY4OCwgMzY4OSwgMzY5MCwgMzY5MSwgMzY5MiwgMzY5MywgMzY5NCwgMzY5NSwgMzY5NiwgMzY5NywgMzY5OCwgMzY5OSwgMzcwMCwgMzcwMSwgMzcwMiwgMzcwMywgMzcwNCwgMzcwNSwgMzcwNiwgMzcwNywgMzcwOCwgMzcwOSwgMzcxMCwgMzcxMSwgMzcxMiwgMzcxMywgMzcxNCwgMzcxNSwgMzcxNiwgMzcxNywgMzcxOCwgMzcxOSwgMzcyMCwgMzcyMSwgMzcyMiwgMzcyMywgMzcyNCwgMzcyNSwgMzcyNiwgMzcyNywgMzcyOCwgMzcyOSwgMzczMCwgMzczMSwgMzczMiwgMzczMywgMzczNCwgMzczNSwgMzczNiwgMzczNywgMzczOF2UdWJzLg==",
+                            "widget data": "gASVqBQAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTScCjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUWDoUAABbMzAzNSwgMzAzNiwgMzAzNywgMzAzOCwgMzAzOSwgMzA0MCwgMzA0MSwgMzA0MiwgMzA0MywgMzA0NCwgMzA0NSwgMzA0NiwgMzA0NywgMzA0OCwgMzA0OSwgMzA1MCwgMzA1MSwgMzA1MiwgMzA1MywgMzA1NCwgMzA1NSwgMzA1NiwgMzA1NywgMzA1OCwgMzA1OSwgMzA2MCwgMzA2MSwgMzA2MiwgMzA2MywgMzA2NCwgMzA2NSwgMzA2NiwgMzA2NywgMzA2OCwgMzA2OSwgMzA3MCwgMzA3MSwgMzA3MiwgMzA3MywgMzA3NCwgMzA3NSwgMzA3NiwgMzA3NywgMzA3OCwgMzA3OSwgMzA4MCwgMzA4MSwgMzA4MiwgMzA4MywgMzA4NCwgMzA4NSwgMzA4NiwgMzA4NywgMzA4OCwgMzA4OSwgMzA5MCwgMzA5MSwgMzA5MiwgMzA5MywgMzA5NCwgMzA5NSwgMzA5NiwgMzA5NywgMzA5OCwgMzA5OSwgMzEwMCwgMzEwMSwgMzEwMiwgMzEwMywgMzEwNCwgMzEwNSwgMzEwNiwgMzEwNywgMzEwOCwgMzEwOSwgMzExMCwgMzExMSwgMzExMiwgMzExMywgMzExNCwgMzExNSwgMzExNiwgMzExNywgMzExOCwgMzExOSwgMzEyMCwgMzEyMSwgMzEyMiwgMzEyMywgMzEyNCwgMzEyNSwgMzEyNiwgMzEyNywgMzEyOCwgMzEyOSwgMzEzMCwgMzEzMSwgMzEzMiwgMzEzMywgMzEzNCwgMzEzNCwgMzEzNSwgMzEzNiwgMzEzNywgMzEzOCwgMzEzOSwgMzE0MCwgMzE0MSwgMzE0MiwgMzE0MywgMzE0NCwgMzE0NSwgMzE0NiwgMzE0NywgMzE0OCwgMzE0OSwgMzE1MCwgMzE1MSwgMzE1MiwgMzE1MywgMzE1NCwgMzE1NSwgMzE1NiwgMzE1NywgMzE1OCwgMzE1OSwgMzE2MCwgMzE2MSwgMzE2MiwgMzE2MywgMzE2NCwgMzE2NSwgMzE2NiwgMzE2NywgMzE2OCwgMzE2OSwgMzE3MCwgMzE3MSwgMzE3MiwgMzE3MywgMzE3NCwgMzE3NSwgMzE3NiwgMzE3NywgMzE3OCwgMzE3OSwgMzE4MCwgMzE4MSwgMzE4MiwgMzE4MywgMzE4NCwgMzE4NSwgMzE4NiwgMzE4NywgMzE4OCwgMzE4OSwgMzE5MCwgMzE5MSwgMzE5MiwgMzE5MywgMzE5NCwgMzE5NSwgMzE5NiwgMzE5NywgMzE5OCwgMzE5OSwgMzIwMCwgMzIwMSwgMzIwMiwgMzIwMywgMzIwNCwgMzIwNSwgMzIwNiwgMzIwNywgMzIwOCwgMzIwOSwgMzIxMCwgMzIxMSwgMzIxMiwgMzIxMywgMzIxNCwgMzIxNSwgMzIxNiwgMzIxNywgMzIxOCwgMzIxOSwgMzIyMCwgMzIyMSwgMzIyMiwgMzIyMywgMzIyNCwgMzIyNSwgMzIyNiwgMzIyNywgMzIyOCwgMzIyOSwgMzIzMCwgMzIzMSwgMzIzMiwgMzIzMywgMzIzNCwgMzIzNSwgMzIzNiwgMzIzNywgMzIzOCwgMzIzOSwgMzI0MCwgMzI0MSwgMzI0MiwgMzI0MywgMzI0NCwgMzI0NSwgMzI0NiwgMzI0NywgMzI0OCwgMzI0OSwgMzI1MCwgMzI1MSwgMzI1MiwgMzI1MywgMzI1NCwgMzI1NSwgMzI1NiwgMzI1NywgMzI1OCwgMzI1OSwgMzI2MCwgMzI2MSwgMzI2MiwgMzI2MywgMzI2NCwgMzI2NSwgMzI2NiwgMzI2NywgMzI2OCwgMzI2OSwgMzI3MCwgMzI3MSwgMzI3MiwgMzI3MywgMzI3NCwgMzI3NSwgMzI3NiwgMzI3NywgMzI3OCwgMzI3OSwgMzI4MCwgMzI4MSwgMzI4MiwgMzI4MywgMzI4NCwgMzI4NSwgMzI4NiwgMzI4NywgMzI4OCwgMzI4OSwgMzI5MCwgMzI5MSwgMzI5MiwgMzI5MywgMzI5NCwgMzI5NSwgMzI5NiwgMzI5NywgMzI5OCwgMzI5OSwgMzMwMCwgMzMwMSwgMzMwMiwgMzMwMywgMzMwNCwgMzMwNSwgMzMwNiwgMzMwNywgMzMwOCwgMzMwOSwgMzMxMCwgMzMxMSwgMzMxMiwgMzMxMywgMzMxNCwgMzMxNSwgMzMxNiwgMzMxNywgMzMxOCwgMzMxOSwgMzMyMCwgMzMyMSwgMzMyMiwgMzMyMywgMzMyNCwgMzMyNSwgMzMyNiwgMzMyNywgMzMyOCwgMzMyOSwgMzMzMCwgMzMzMSwgMzMzMiwgMzMzMywgMzMzNCwgMzMzNSwgMzMzNiwgMzMzNywgMzMzOCwgMzMzOSwgMzM0MCwgMzM0MSwgMzM0MiwgMzM0MywgMzM0NCwgMzM0NSwgMzM0NiwgMzM0NywgMzM0OCwgMzM0OSwgMzM1MCwgMzM1MSwgMzM1MiwgMzM1MywgMzM1NCwgMzM1NSwgMzM1NiwgMzM1NywgMzM1OCwgMzM1OSwgMzM2MCwgMzM2MSwgMzM2MiwgMzM2MywgMzM2NCwgMzM2NSwgMzM2NiwgMzM2NywgMzM2OCwgMzM2OSwgMzM3MCwgMzM3MSwgMzM3MiwgMzM3MywgMzM3NCwgMzM3NSwgMzM3NiwgMzM3NywgMzM3OCwgMzM3OSwgMzM4MCwgMzM4MSwgMzM4MiwgMzM4MywgMzM4NCwgMzM4NSwgMzM4NiwgMzM4NywgMzM4OCwgMzM4OSwgMzM5MCwgMzM5MSwgMzM5MiwgMzM5MywgMzM5NCwgMzM5NSwgMzM5NiwgMzM5NywgMzM5OCwgMzM5OSwgMzQwMCwgMzQwMSwgMzQwMiwgMzQwMywgMzQwNCwgMzQwNSwgMzQwNiwgMzQwNywgMzQwOCwgMzQwOSwgMzQxMCwgMzQxMSwgMzQxMiwgMzQxMywgMzQxNCwgMzQxNSwgMzQxNiwgMzQxNywgMzQxOCwgMzQxOSwgMzQyMCwgMzQyMSwgMzQyMiwgMzQyMywgMzQyNCwgMzQyNSwgMzQyNiwgMzQyNywgMzQyOCwgMzQyOSwgMzQzMCwgMzQzMSwgMzQzMiwgMzQzMywgMzQzNCwgMzQzNSwgMzQzNiwgMzQzNywgMzQzOCwgMzQzOSwgMzQ0MCwgMzQ0MSwgMzQ0MiwgMzQ0MywgMzQ0NCwgMzQ0NSwgMzQ0NiwgMzQ0NywgMzQ0OCwgMzQ0OSwgMzQ1MCwgMzQ1MSwgMzQ1MiwgMzQ1MywgMzQ1NCwgMzQ1NSwgMzQ1NiwgMzQ1NywgMzQ1OCwgMzQ1OSwgMzQ2MCwgMzQ2MSwgMzQ2MiwgMzQ2MywgMzQ2NCwgMzQ2NSwgMzQ2NiwgMzQ2NywgMzQ2OCwgMzQ2OSwgMzQ3MCwgMzQ3MSwgMzQ3MiwgMzQ3MywgMzQ3NCwgMzQ3NSwgMzQ3NiwgMzQ3NywgMzQ3OCwgMzQ3OSwgMzQ4MCwgMzQ4MSwgMzQ4MiwgMzQ4MywgMzQ4NCwgMzQ4NSwgMzQ4NiwgMzQ4NywgMzQ4OCwgMzQ4OSwgMzQ5MCwgMzQ5MSwgMzQ5MiwgMzQ5MywgMzQ5NCwgMzQ5NSwgMzQ5NiwgMzQ5NywgMzQ5OCwgMzQ5OSwgMzUwMCwgMzUwMSwgMzUwMiwgMzUwMywgMzUwNCwgMzUwNSwgMzUwNiwgMzUwNywgMzUwOCwgMzUwOSwgMzUxMCwgMzUxMSwgMzUxMiwgMzUxMywgMzUxNCwgMzUxNSwgMzUxNiwgMzUxNywgMzUxOCwgMzUxOSwgMzUyMCwgMzUyMSwgMzUyMiwgMzUyMywgMzUyNCwgMzUyNSwgMzUyNiwgMzUyNywgMzUyOCwgMzUyOSwgMzUzMCwgMzUzMSwgMzUzMiwgMzUzMywgMzUzNCwgMzUzNSwgMzUzNiwgMzUzNywgMzUzOCwgMzUzOSwgMzU0MCwgMzU0MSwgMzU0MiwgMzU0MywgMzU0NCwgMzU0NSwgMzU0NiwgMzU0NywgMzU0OCwgMzU0OSwgMzU1MCwgMzU1MSwgMzU1MiwgMzU1MywgMzU1NCwgMzU1NSwgMzU1NiwgMzU1NywgMzU1OCwgMzU1OSwgMzU2MCwgMzU2MSwgMzU2MiwgMzU2MywgMzU2NCwgMzU2NSwgMzU2NiwgMzU2NywgMzU2OCwgMzU2OSwgMzU3MCwgMzU3MSwgMzU3MiwgMzU3MywgMzU3NCwgMzU3NSwgMzU3NiwgMzU3NywgMzU3OCwgMzU3OSwgMzU4MCwgMzU4MSwgMzU4MiwgMzU4MywgMzU4NCwgMzU4NSwgMzU4NiwgMzU4NywgMzU4OCwgMzU4OSwgMzU5MCwgMzU5MSwgMzU5MiwgMzU5MywgMzU5NCwgMzU5NSwgMzU5NiwgMzU5NywgMzU5OCwgMzU5OSwgMzYwMCwgMzYwMSwgMzYwMiwgMzYwMywgMzYwNCwgMzYwNSwgMzYwNiwgMzYwNywgMzYwOCwgMzYwOSwgMzYxMCwgMzYxMSwgMzYxMiwgMzYxMywgMzYxNCwgMzYxNSwgMzYxNiwgMzYxNywgMzYxOCwgMzYxOSwgMzYyMCwgMzYyMSwgMzYyMiwgMzYyMywgMzYyNCwgMzYyNSwgMzYyNiwgMzYyNywgMzYyOCwgMzYyOSwgMzYzMCwgMzYzMSwgMzYzMiwgMzYzMywgMzYzNCwgMzYzNSwgMzYzNiwgMzYzNywgMzYzOCwgMzYzOSwgMzY0MCwgMzY0MSwgMzY0MiwgMzY0MywgMzY0NCwgMzY0NSwgMzY0NiwgMzY0NywgMzY0OCwgMzY0OSwgMzY1MCwgMzY1MSwgMzY1MiwgMzY1MywgMzY1NCwgMzY1NSwgMzY1NiwgMzY1NywgMzY1OCwgMzY1OSwgMzY2MCwgMzY2MSwgMzY2MiwgMzY2MywgMzY2NCwgMzY2NSwgMzY2NiwgMzY2NywgMzY2OCwgMzY2OSwgMzY3MCwgMzY3MSwgMzY3MiwgMzY3MywgMzY3NCwgMzY3NSwgMzY3NiwgMzY3NywgMzY3OCwgMzY3OSwgMzY4MCwgMzY4MSwgMzY4MiwgMzY4MywgMzY4NCwgMzY4NSwgMzY4NiwgMzY4NywgMzY4OCwgMzY4OSwgMzY5MCwgMzY5MSwgMzY5MiwgMzY5MywgMzY5NCwgMzY5NSwgMzY5NiwgMzY5NywgMzY5OCwgMzY5OSwgMzcwMCwgMzcwMSwgMzcwMiwgMzcwMywgMzcwNCwgMzcwNSwgMzcwNiwgMzcwNywgMzcwOCwgMzcwOSwgMzcxMCwgMzcxMSwgMzcxMiwgMzcxMywgMzcxNCwgMzcxNSwgMzcxNiwgMzcxNywgMzcxOCwgMzcxOSwgMzcyMCwgMzcyMSwgMzcyMiwgMzcyMywgMzcyNCwgMzcyNSwgMzcyNiwgMzcyNywgMzcyOCwgMzcyOSwgMzczMCwgMzczMSwgMzczMiwgMzczMywgMzczNCwgMzczNSwgMzczNiwgMzczNywgMzczOCwgMzczOSwgMzczOSwgMzc0MCwgMzc0MCwgMzc0MSwgMzc0MSwgMzc0MiwgMzc0MiwgMzc0MywgMzc0MywgMzc0NCwgMzc0NCwgMzc0NSwgMzc0NSwgMzc0NiwgMzc0NiwgMzc0NywgMzc0NywgMzc0OCwgMzc0OCwgMzc0OSwgMzc0OSwgMzc1MCwgMzc1MCwgMzc1MSwgMzc1MSwgMzc1MiwgMzc1MiwgMzc1MywgMzc1MywgMzc1NCwgMzc1NCwgMzc1NSwgMzc1NSwgMzc1NiwgMzc1NiwgMzc1NywgMzc1NywgMzc1OCwgMzc1OCwgMzc1OSwgMzc1OSwgMzc2MCwgMzc2MCwgMzc2MSwgMzc2MSwgMzc2MiwgMzc2MiwgMzc2MywgMzc2MywgMzc2NCwgMzc2NCwgMzc2NSwgMzc2NSwgMzc2NiwgMzc2NiwgMzc2NywgMzc2NywgMzc2OCwgMzc2OCwgMzc2OSwgMzc2OSwgMzc3MCwgMzc3MCwgMzc3MSwgMzc3MSwgMzc3MiwgMzc3MiwgMzc3MywgMzc3MywgMzc3NCwgMzc3NCwgMzc3NSwgMzc3NSwgMzc3NiwgMzc3NiwgMzc3NywgMzc3NywgMzc3OCwgMzc3OCwgMzc3OSwgMzc3OSwgMzc4MCwgMzc4MCwgMzc4MSwgMzc4MSwgMzc4MiwgMzc4MiwgMzc4MywgMzc4MywgMzc4NCwgMzc4NCwgMzc4NSwgMzc4NSwgMzc4NiwgMzc4NiwgMzc4NywgMzc4NywgMzc4OCwgMzc4OCwgMzc4OSwgMzc4OSwgMzc5MCwgMzc5MCwgMzc5MSwgMzc5MSwgMzc5MiwgMzc5MiwgMzc5MywgMzc5MywgMzc5NCwgMzc5NCwgMzc5NSwgMzc5NSwgMzc5NiwgMzc5NiwgMzc5NywgMzc5NywgMzc5OCwgMzc5OCwgMzc5OSwgMzc5OSwgMzgwMCwgMzgwMCwgMzgwMSwgMzgwMSwgMzgwMiwgMzgwMiwgMzgwMywgMzgwMywgMzgwNCwgMzgwNCwgMzgwNSwgMzgwNSwgMzgwNiwgMzgwNiwgMzgwNywgMzgwNywgMzgwOCwgMzgwOCwgMzgwOSwgMzgwOSwgMzgxMCwgMzgxMCwgMzgxMSwgMzgxMSwgMzgxMiwgMzgxMiwgMzgxMywgMzgxMywgMzgxNCwgMzgxNCwgMzgxNSwgMzgxNSwgMzgxNiwgMzgxNiwgMzgxNywgMzgxN12UdWJzLg==",
                             "widget name": "val",
                             "widget pos": "besides"
                         }
                     ],
+                    "inspector widget": {},
                     "outputs": [
                         {
-                            "GID": 40,
+                            "GID": 46,
                             "label": "val",
                             "type": "data"
                         }
                     ],
                     "pos x": 724.2936205842011,
                     "pos y": 249.9898748171978,
                     "state data": "gASVDgAAAAAAAAB9lIwGYWN0aXZllIlzLg==",
                     "unconnected ports hidden": false,
                     "version": "v0.1"
                 },
                 {
-                    "GID": 41,
+                    "GID": 49,
                     "Variables": {
                         "subscriptions": {
                             "a": "var_val_changed"
                         }
                     },
                     "actions": {
                         "change title": {
@@ -430,43 +472,44 @@
                     },
                     "additional data": {},
                     "collapsed": false,
                     "display title": "get var",
                     "identifier": "built_in.GetVar_Node",
                     "inputs": [
                         {
-                            "GID": 44,
+                            "GID": 52,
                             "default": {
-                                "GID": 120,
+                                "GID": 56,
                                 "identifier": "Data",
                                 "serialized": "gASVBQAAAAAAAACMAWGULg=="
                             },
                             "has widget": true,
                             "label": "",
                             "type": "data",
-                            "widget data": "gASVbAAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTR8SjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUjAFhlHVicy4=",
+                            "widget data": "gASVbAAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTSgCjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUjAFhlHVicy4=",
                             "widget name": "varname",
                             "widget pos": "besides"
                         }
                     ],
+                    "inspector widget": {},
                     "outputs": [
                         {
-                            "GID": 45,
+                            "GID": 54,
                             "label": "val",
                             "type": "data"
                         }
                     ],
                     "pos x": 164.80323966981427,
                     "pos y": 368.23084671814206,
                     "state data": "gAR9lC4=",
                     "unconnected ports hidden": false,
                     "version": "v0.2"
                 },
                 {
-                    "GID": 46,
+                    "GID": 57,
                     "Variables": {
                         "subscriptions": {}
                     },
                     "actions": {
                         "change title": {
                             "method": "change_title"
                         },
@@ -485,61 +528,62 @@
                         "update shape": {
                             "method": "update_shape"
                         }
                     },
                     "additional data": {},
                     "collapsed": false,
                     "display title": "clock",
-                    "identifier": "std.Clock_Node",
+                    "identifier": "examples.special_nodes.Clock_Node",
                     "inputs": [
                         {
-                            "GID": 50,
+                            "GID": 61,
                             "default": {
-                                "GID": 153,
+                                "GID": 67,
                                 "identifier": "Data",
                                 "serialized": "gARLAC4="
                             },
                             "has widget": true,
                             "label": "delay",
                             "type": "data",
-                            "widget data": "gASVagAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTSASjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUSwB1YnMu",
+                            "widget data": "gASVagAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTSkCjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUSwB1YnMu",
                             "widget name": "delay",
                             "widget pos": "besides"
                         },
                         {
-                            "GID": 51,
+                            "GID": 63,
                             "default": {
-                                "GID": 54,
+                                "GID": 68,
                                 "identifier": "Data",
                                 "serialized": "gASVBgAAAAAAAABK/////y4="
                             },
                             "has widget": true,
                             "label": "iterations",
                             "type": "data",
-                            "widget data": "gASVbQAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTSESjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUSv////91YnMu",
+                            "widget data": "gASVbQAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTSoCjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUSv////91YnMu",
                             "widget name": "iter",
                             "widget pos": "besides"
                         }
                     ],
+                    "inspector widget": {},
                     "main widget data": "gAR9lC4=",
                     "outputs": [
                         {
-                            "GID": 52,
+                            "GID": 65,
                             "label": "",
                             "type": "exec"
                         }
                     ],
                     "pos x": 230.23622828581165,
                     "pos y": 115.6139516414438,
                     "state data": "gAR9lC4=",
                     "unconnected ports hidden": false,
-                    "version": "v0.2"
+                    "version": "v0.3"
                 },
                 {
-                    "GID": 55,
+                    "GID": 69,
                     "Variables": {
                         "subscriptions": {}
                     },
                     "actions": {
                         "change title": {
                             "method": "change_title"
                         },
@@ -555,67 +599,68 @@
                     },
                     "additional data": {},
                     "collapsed": false,
                     "display title": "set var",
                     "identifier": "built_in.SetVar_Node",
                     "inputs": [
                         {
-                            "GID": 61,
+                            "GID": 75,
                             "label": "",
                             "type": "exec"
                         },
                         {
-                            "GID": 62,
+                            "GID": 76,
                             "default": {
-                                "GID": 109,
+                                "GID": 82,
                                 "identifier": "Data",
                                 "serialized": "gASVBwAAAAAAAACMA2N0cpQu"
                             },
                             "has widget": true,
                             "label": "var",
                             "type": "data",
-                            "widget data": "gASVbgAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTSISjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUjANjdHKUdWJzLg==",
+                            "widget data": "gASVbgAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTSsCjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUjANjdHKUdWJzLg==",
                             "widget name": "varname",
                             "widget pos": "besides"
                         },
                         {
-                            "GID": 63,
+                            "GID": 78,
                             "default": {
-                                "GID": 4634,
+                                "GID": 534,
                                 "identifier": "Data",
-                                "serialized": "gASVCAAAAAAAAACMBDM3MzmULg=="
+                                "serialized": "gASVCAAAAAAAAACMBDM4MTiULg=="
                             },
                             "has widget": true,
                             "label": "val",
                             "type": "data",
-                            "widget data": "gASVbwAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTSMSjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUjAQzNzM5lHVicy4=",
+                            "widget data": "gASVbwAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTSwCjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUjAQzODE4lHVicy4=",
                             "widget name": "val",
                             "widget pos": "besides"
                         }
                     ],
+                    "inspector widget": {},
                     "outputs": [
                         {
-                            "GID": 64,
+                            "GID": 80,
                             "label": "",
                             "type": "exec"
                         },
                         {
-                            "GID": 65,
+                            "GID": 81,
                             "label": "val",
                             "type": "data"
                         }
                     ],
                     "pos x": 846.1910218628586,
                     "pos y": 133.30644603168525,
                     "state data": "gASVDgAAAAAAAAB9lIwGYWN0aXZllIhzLg==",
                     "unconnected ports hidden": false,
                     "version": "v0.1"
                 },
                 {
-                    "GID": 66,
+                    "GID": 84,
                     "Variables": {
                         "subscriptions": {
                             "ctr": "var_val_changed"
                         }
                     },
                     "actions": {
                         "change title": {
@@ -633,43 +678,44 @@
                     },
                     "additional data": {},
                     "collapsed": false,
                     "display title": "get var",
                     "identifier": "built_in.GetVar_Node",
                     "inputs": [
                         {
-                            "GID": 69,
+                            "GID": 87,
                             "default": {
-                                "GID": 113,
+                                "GID": 91,
                                 "identifier": "Data",
                                 "serialized": "gASVBwAAAAAAAACMA2N0cpQu"
                             },
                             "has widget": true,
                             "label": "",
                             "type": "data",
-                            "widget data": "gASVbgAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTSQSjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUjANjdHKUdWJzLg==",
+                            "widget data": "gASVbgAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTS0CjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUjANjdHKUdWJzLg==",
                             "widget name": "varname",
                             "widget pos": "besides"
                         }
                     ],
+                    "inspector widget": {},
                     "outputs": [
                         {
-                            "GID": 70,
+                            "GID": 89,
                             "label": "val",
                             "type": "data"
                         }
                     ],
                     "pos x": 196.31117068512344,
                     "pos y": 265.7809649154535,
                     "state data": "gAR9lC4=",
                     "unconnected ports hidden": false,
                     "version": "v0.2"
                 },
                 {
-                    "GID": 71,
+                    "GID": 92,
                     "Variables": {
                         "subscriptions": {}
                     },
                     "actions": {
                         "add input": {
                             "method": "add_operand_input"
                         },
@@ -695,60 +741,61 @@
                         "update shape": {
                             "method": "update_shape"
                         }
                     },
                     "additional data": {},
                     "collapsed": false,
                     "display title": "+",
-                    "identifier": "std.Plus_Node",
+                    "identifier": "examples.basic_operators.Plus_Node",
                     "inputs": [
                         {
-                            "GID": 75,
+                            "GID": 96,
                             "default": {
-                                "GID": 4632,
+                                "GID": 532,
                                 "identifier": "Data",
-                                "serialized": "gASVBAAAAAAAAABNmg4u"
+                                "serialized": "gASVBAAAAAAAAABN6Q4u"
                             },
                             "has widget": true,
                             "label": "",
                             "type": "data",
-                            "widget data": "gASVawAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTSUSjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUTZoOdWJzLg==",
+                            "widget data": "gASVawAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTS4CjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUTekOdWJzLg==",
                             "widget name": "in",
                             "widget pos": "besides"
                         },
                         {
-                            "GID": 76,
+                            "GID": 98,
                             "default": {
-                                "GID": 110,
+                                "GID": 104,
                                 "identifier": "Data",
                                 "serialized": "gARLAS4="
                             },
                             "has widget": true,
                             "label": "",
                             "type": "data",
-                            "widget data": "gASVagAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTSYSjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUSwF1YnMu",
+                            "widget data": "gASVagAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTS8CjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUSwF1YnMu",
                             "widget name": "in",
                             "widget pos": "besides"
                         }
                     ],
+                    "inspector widget": {},
                     "outputs": [
                         {
-                            "GID": 77,
+                            "GID": 100,
                             "label": "",
                             "type": "data"
                         }
                     ],
                     "pos x": 478.68879139148794,
                     "pos y": 168.51150293252385,
                     "state data": "gAR9lC4=",
                     "unconnected ports hidden": false,
-                    "version": "v0.2"
+                    "version": "v0.3"
                 },
                 {
-                    "GID": 80,
+                    "GID": 105,
                     "Variables": {
                         "subscriptions": {}
                     },
                     "actions": {
                         "add input": {
                             "method": "add_inp"
                         },
@@ -768,32 +815,33 @@
                         "update shape": {
                             "method": "update_shape"
                         }
                     },
                     "additional data": {},
                     "collapsed": false,
                     "display title": "link IN",
-                    "identifier": "std.LinkIN_Node",
+                    "identifier": "examples.special_nodes.LinkIN_Node",
                     "inputs": [
                         {
-                            "GID": 82,
+                            "GID": 107,
                             "has widget": false,
                             "label": "",
                             "type": "data"
                         }
                     ],
+                    "inspector widget": {},
                     "outputs": [],
                     "pos x": 566.7044488232787,
                     "pos y": 478.94789784811906,
                     "state data": "gASVMAAAAAAAAAB9lIwCSUSUjCRjNWVmZjE5MC0yNzllLTQ3M2MtYTQ3Ny1iNjJmMjg0MGUzOTiUcy4=",
                     "unconnected ports hidden": false,
-                    "version": "v0.2"
+                    "version": "v0.3"
                 },
                 {
-                    "GID": 103,
+                    "GID": 108,
                     "Variables": {
                         "subscriptions": {}
                     },
                     "actions": {
                         "change title": {
                             "method": "change_title"
                         },
@@ -806,102 +854,103 @@
                         "update shape": {
                             "method": "update_shape"
                         }
                     },
                     "additional data": {},
                     "collapsed": false,
                     "display title": "Button",
-                    "identifier": "std.Button_Node",
+                    "identifier": "examples.special_nodes.Button_Node",
                     "inputs": [],
+                    "inspector widget": {},
                     "main widget data": "gAR9lC4=",
                     "outputs": [
                         {
-                            "GID": 104,
+                            "GID": 110,
                             "label": "",
                             "type": "exec"
                         }
                     ],
                     "pos x": 473.0,
                     "pos y": 51.0,
                     "state data": "gAR9lC4=",
                     "unconnected ports hidden": false,
-                    "version": "v0.2"
+                    "version": "v0.3"
                 }
             ],
             "output data": [
                 {
                     "data": {
-                        "GID": 4627,
+                        "GID": 536,
                         "identifier": "Data",
-                        "serialized": "gASVSAgAAAAAAABdlChN2wtN3AtN3QtN3gtN3wtN4AtN4QtN4gtN4wtN5AtN5QtN5gtN5wtN6AtN6QtN6gtN6wtN7AtN7QtN7gtN7wtN8AtN8QtN8gtN8wtN9AtN9QtN9gtN9wtN+AtN+QtN+gtN+wtN/AtN/QtN/gtN/wtNAAxNAQxNAgxNAwxNBAxNBQxNBgxNBwxNCAxNCQxNCgxNCwxNDAxNDQxNDgxNDwxNEAxNEQxNEgxNEwxNFAxNFQxNFgxNFwxNGAxNGQxNGgxNGwxNHAxNHQxNHgxNHwxNIAxNIQxNIgxNIwxNJAxNJQxNJgxNJwxNKAxNKQxNKgxNKwxNLAxNLQxNLgxNLwxNMAxNMQxNMgxNMwxNNAxNNQxNNgxNNwxNOAxNOQxNOgxNOwxNPAxNPQxNPgxNPgxNPwxNQAxNQQxNQgxNQwxNRAxNRQxNRgxNRwxNSAxNSQxNSgxNSwxNTAxNTQxNTgxNTwxNUAxNUQxNUgxNUwxNVAxNVQxNVgxNVwxNWAxNWQxNWgxNWwxNXAxNXQxNXgxNXwxNYAxNYQxNYgxNYwxNZAxNZQxNZgxNZwxNaAxNaQxNagxNawxNbAxNbQxNbgxNbwxNcAxNcQxNcgxNcwxNdAxNdQxNdgxNdwxNeAxNeQxNegxNewxNfAxNfQxNfgxNfwxNgAxNgQxNggxNgwxNhAxNhQxNhgxNhwxNiAxNiQxNigxNiwxNjAxNjQxNjgxNjwxNkAxNkQxNkgxNkwxNlAxNlQxNlgxNlwxNmAxNmQxNmgxNmwxNnAxNnQxNngxNnwxNoAxNoQxNogxNowxNpAxNpQxNpgxNpwxNqAxNqQxNqgxNqwxNrAxNrQxNrgxNrwxNsAxNsQxNsgxNswxNtAxNtQxNtgxNtwxNuAxNuQxNugxNuwxNvAxNvQxNvgxNvwxNwAxNwQxNwgxNwwxNxAxNxQxNxgxNxwxNyAxNyQxNygxNywxNzAxNzQxNzgxNzwxN0AxN0QxN0gxN0wxN1AxN1QxN1gxN1wxN2AxN2QxN2gxN2wxN3AxN3QxN3gxN3wxN4AxN4QxN4gxN4wxN5AxN5QxN5gxN5wxN6AxN6QxN6gxN6wxN7AxN7QxN7gxN7wxN8AxN8QxN8gxN8wxN9AxN9QxN9gxN9wxN+AxN+QxN+gxN+wxN/AxN/QxN/gxN/wxNAA1NAQ1NAg1NAw1NBA1NBQ1NBg1NBw1NCA1NCQ1NCg1NCw1NDA1NDQ1NDg1NDw1NEA1NEQ1NEg1NEw1NFA1NFQ1NFg1NFw1NGA1NGQ1NGg1NGw1NHA1NHQ1NHg1NHw1NIA1NIQ1NIg1NIw1NJA1NJQ1NJg1NJw1NKA1NKQ1NKg1NKw1NLA1NLQ1NLg1NLw1NMA1NMQ1NMg1NMw1NNA1NNQ1NNg1NNw1NOA1NOQ1NOg1NOw1NPA1NPQ1NPg1NPw1NQA1NQQ1NQg1NQw1NRA1NRQ1NRg1NRw1NSA1NSQ1NSg1NSw1NTA1NTQ1NTg1NTw1NUA1NUQ1NUg1NUw1NVA1NVQ1NVg1NVw1NWA1NWQ1NWg1NWw1NXA1NXQ1NXg1NXw1NYA1NYQ1NYg1NYw1NZA1NZQ1NZg1NZw1NaA1NaQ1Nag1Naw1NbA1NbQ1Nbg1Nbw1NcA1NcQ1Ncg1Ncw1NdA1NdQ1Ndg1Ndw1NeA1NeQ1Neg1New1NfA1NfQ1Nfg1Nfw1NgA1NgQ1Ngg1Ngw1NhA1NhQ1Nhg1Nhw1NiA1NiQ1Nig1Niw1NjA1NjQ1Njg1Njw1NkA1NkQ1Nkg1Nkw1NlA1NlQ1Nlg1Nlw1NmA1NmQ1Nmg1Nmw1NnA1NnQ1Nng1Nnw1NoA1NoQ1Nog1Now1NpA1NpQ1Npg1Npw1NqA1NqQ1Nqg1Nqw1NrA1NrQ1Nrg1Nrw1NsA1NsQ1Nsg1Nsw1NtA1NtQ1Ntg1Ntw1NuA1NuQ1Nug1Nuw1NvA1NvQ1Nvg1Nvw1NwA1NwQ1Nwg1Nww1NxA1NxQ1Nxg1Nxw1NyA1NyQ1Nyg1Nyw1NzA1NzQ1Nzg1Nzw1N0A1N0Q1N0g1N0w1N1A1N1Q1N1g1N1w1N2A1N2Q1N2g1N2w1N3A1N3Q1N3g1N3w1N4A1N4Q1N4g1N4w1N5A1N5Q1N5g1N5w1N6A1N6Q1N6g1N6w1N7A1N7Q1N7g1N7w1N8A1N8Q1N8g1N8w1N9A1N9Q1N9g1N9w1N+A1N+Q1N+g1N+w1N/A1N/Q1N/g1N/w1NAA5NAQ5NAg5NAw5NBA5NBQ5NBg5NBw5NCA5NCQ5NCg5NCw5NDA5NDQ5NDg5NDw5NEA5NEQ5NEg5NEw5NFA5NFQ5NFg5NFw5NGA5NGQ5NGg5NGw5NHA5NHQ5NHg5NHw5NIA5NIQ5NIg5NIw5NJA5NJQ5NJg5NJw5NKA5NKQ5NKg5NKw5NLA5NLQ5NLg5NLw5NMA5NMQ5NMg5NMw5NNA5NNQ5NNg5NNw5NOA5NOQ5NOg5NOw5NPA5NPQ5NPg5NPw5NQA5NQQ5NQg5NQw5NRA5NRQ5NRg5NRw5NSA5NSQ5NSg5NSw5NTA5NTQ5NTg5NTw5NUA5NUQ5NUg5NUw5NVA5NVQ5NVg5NVw5NWA5NWQ5NWg5NWw5NXA5NXQ5NXg5NXw5NYA5NYQ5NYg5NYw5NZA5NZQ5NZg5NZw5NaA5NaQ5Nag5Naw5NbA5NbQ5Nbg5Nbw5NcA5NcQ5Ncg5Ncw5NdA5NdQ5Ndg5Ndw5NeA5NeQ5Neg5New5NfA5NfQ5Nfg5Nfw5NgA5NgQ5Ngg5Ngw5NhA5NhQ5Nhg5Nhw5NiA5NiQ5Nig5Niw5NjA5NjQ5Njg5Njw5NkA5NkQ5Nkg5Nkw5NlA5NlQ5Nlg5Nlw5NmA5NmQ5Nmg5lLg=="
+                        "serialized": "gASVIgoAAAAAAABdlChN2wtN3AtN3QtN3gtN3wtN4AtN4QtN4gtN4wtN5AtN5QtN5gtN5wtN6AtN6QtN6gtN6wtN7AtN7QtN7gtN7wtN8AtN8QtN8gtN8wtN9AtN9QtN9gtN9wtN+AtN+QtN+gtN+wtN/AtN/QtN/gtN/wtNAAxNAQxNAgxNAwxNBAxNBQxNBgxNBwxNCAxNCQxNCgxNCwxNDAxNDQxNDgxNDwxNEAxNEQxNEgxNEwxNFAxNFQxNFgxNFwxNGAxNGQxNGgxNGwxNHAxNHQxNHgxNHwxNIAxNIQxNIgxNIwxNJAxNJQxNJgxNJwxNKAxNKQxNKgxNKwxNLAxNLQxNLgxNLwxNMAxNMQxNMgxNMwxNNAxNNQxNNgxNNwxNOAxNOQxNOgxNOwxNPAxNPQxNPgxNPgxNPwxNQAxNQQxNQgxNQwxNRAxNRQxNRgxNRwxNSAxNSQxNSgxNSwxNTAxNTQxNTgxNTwxNUAxNUQxNUgxNUwxNVAxNVQxNVgxNVwxNWAxNWQxNWgxNWwxNXAxNXQxNXgxNXwxNYAxNYQxNYgxNYwxNZAxNZQxNZgxNZwxNaAxNaQxNagxNawxNbAxNbQxNbgxNbwxNcAxNcQxNcgxNcwxNdAxNdQxNdgxNdwxNeAxNeQxNegxNewxNfAxNfQxNfgxNfwxNgAxNgQxNggxNgwxNhAxNhQxNhgxNhwxNiAxNiQxNigxNiwxNjAxNjQxNjgxNjwxNkAxNkQxNkgxNkwxNlAxNlQxNlgxNlwxNmAxNmQxNmgxNmwxNnAxNnQxNngxNnwxNoAxNoQxNogxNowxNpAxNpQxNpgxNpwxNqAxNqQxNqgxNqwxNrAxNrQxNrgxNrwxNsAxNsQxNsgxNswxNtAxNtQxNtgxNtwxNuAxNuQxNugxNuwxNvAxNvQxNvgxNvwxNwAxNwQxNwgxNwwxNxAxNxQxNxgxNxwxNyAxNyQxNygxNywxNzAxNzQxNzgxNzwxN0AxN0QxN0gxN0wxN1AxN1QxN1gxN1wxN2AxN2QxN2gxN2wxN3AxN3QxN3gxN3wxN4AxN4QxN4gxN4wxN5AxN5QxN5gxN5wxN6AxN6QxN6gxN6wxN7AxN7QxN7gxN7wxN8AxN8QxN8gxN8wxN9AxN9QxN9gxN9wxN+AxN+QxN+gxN+wxN/AxN/QxN/gxN/wxNAA1NAQ1NAg1NAw1NBA1NBQ1NBg1NBw1NCA1NCQ1NCg1NCw1NDA1NDQ1NDg1NDw1NEA1NEQ1NEg1NEw1NFA1NFQ1NFg1NFw1NGA1NGQ1NGg1NGw1NHA1NHQ1NHg1NHw1NIA1NIQ1NIg1NIw1NJA1NJQ1NJg1NJw1NKA1NKQ1NKg1NKw1NLA1NLQ1NLg1NLw1NMA1NMQ1NMg1NMw1NNA1NNQ1NNg1NNw1NOA1NOQ1NOg1NOw1NPA1NPQ1NPg1NPw1NQA1NQQ1NQg1NQw1NRA1NRQ1NRg1NRw1NSA1NSQ1NSg1NSw1NTA1NTQ1NTg1NTw1NUA1NUQ1NUg1NUw1NVA1NVQ1NVg1NVw1NWA1NWQ1NWg1NWw1NXA1NXQ1NXg1NXw1NYA1NYQ1NYg1NYw1NZA1NZQ1NZg1NZw1NaA1NaQ1Nag1Naw1NbA1NbQ1Nbg1Nbw1NcA1NcQ1Ncg1Ncw1NdA1NdQ1Ndg1Ndw1NeA1NeQ1Neg1New1NfA1NfQ1Nfg1Nfw1NgA1NgQ1Ngg1Ngw1NhA1NhQ1Nhg1Nhw1NiA1NiQ1Nig1Niw1NjA1NjQ1Njg1Njw1NkA1NkQ1Nkg1Nkw1NlA1NlQ1Nlg1Nlw1NmA1NmQ1Nmg1Nmw1NnA1NnQ1Nng1Nnw1NoA1NoQ1Nog1Now1NpA1NpQ1Npg1Npw1NqA1NqQ1Nqg1Nqw1NrA1NrQ1Nrg1Nrw1NsA1NsQ1Nsg1Nsw1NtA1NtQ1Ntg1Ntw1NuA1NuQ1Nug1Nuw1NvA1NvQ1Nvg1Nvw1NwA1NwQ1Nwg1Nww1NxA1NxQ1Nxg1Nxw1NyA1NyQ1Nyg1Nyw1NzA1NzQ1Nzg1Nzw1N0A1N0Q1N0g1N0w1N1A1N1Q1N1g1N1w1N2A1N2Q1N2g1N2w1N3A1N3Q1N3g1N3w1N4A1N4Q1N4g1N4w1N5A1N5Q1N5g1N5w1N6A1N6Q1N6g1N6w1N7A1N7Q1N7g1N7w1N8A1N8Q1N8g1N8w1N9A1N9Q1N9g1N9w1N+A1N+Q1N+g1N+w1N/A1N/Q1N/g1N/w1NAA5NAQ5NAg5NAw5NBA5NBQ5NBg5NBw5NCA5NCQ5NCg5NCw5NDA5NDQ5NDg5NDw5NEA5NEQ5NEg5NEw5NFA5NFQ5NFg5NFw5NGA5NGQ5NGg5NGw5NHA5NHQ5NHg5NHw5NIA5NIQ5NIg5NIw5NJA5NJQ5NJg5NJw5NKA5NKQ5NKg5NKw5NLA5NLQ5NLg5NLw5NMA5NMQ5NMg5NMw5NNA5NNQ5NNg5NNw5NOA5NOQ5NOg5NOw5NPA5NPQ5NPg5NPw5NQA5NQQ5NQg5NQw5NRA5NRQ5NRg5NRw5NSA5NSQ5NSg5NSw5NTA5NTQ5NTg5NTw5NUA5NUQ5NUg5NUw5NVA5NVQ5NVg5NVw5NWA5NWQ5NWg5NWw5NXA5NXQ5NXg5NXw5NYA5NYQ5NYg5NYw5NZA5NZQ5NZg5NZw5NaA5NaQ5Nag5Naw5NbA5NbQ5Nbg5Nbw5NcA5NcQ5Ncg5Ncw5NdA5NdQ5Ndg5Ndw5NeA5NeQ5Neg5New5NfA5NfQ5Nfg5Nfw5NgA5NgQ5Ngg5Ngw5NhA5NhQ5Nhg5Nhw5NiA5NiQ5Nig5Niw5NjA5NjQ5Njg5Njw5NkA5NkQ5Nkg5Nkw5NlA5NlQ5Nlg5Nlw5NmA5NmQ5Nmg5Nmw5Nmw5NnA5NnA5NnQ5NnQ5Nng5Nng5Nnw5Nnw5NoA5NoA5NoQ5NoQ5Nog5Nog5Now5Now5NpA5NpA5NpQ5NpQ5Npg5Npg5Npw5Npw5NqA5NqA5NqQ5NqQ5Nqg5Nqg5Nqw5Nqw5NrA5NrA5NrQ5NrQ5Nrg5Nrg5Nrw5Nrw5NsA5NsA5NsQ5NsQ5Nsg5Nsg5Nsw5Nsw5NtA5NtA5NtQ5NtQ5Ntg5Ntg5Ntw5Ntw5NuA5NuA5NuQ5NuQ5Nug5Nug5Nuw5Nuw5NvA5NvA5NvQ5NvQ5Nvg5Nvg5Nvw5Nvw5NwA5NwA5NwQ5NwQ5Nwg5Nwg5Nww5Nww5NxA5NxA5NxQ5NxQ5Nxg5Nxg5Nxw5Nxw5NyA5NyA5NyQ5NyQ5Nyg5Nyg5Nyw5Nyw5NzA5NzA5NzQ5NzQ5Nzg5Nzg5Nzw5Nzw5N0A5N0A5N0Q5N0Q5N0g5N0g5N0w5N0w5N1A5N1A5N1Q5N1Q5N1g5N1g5N1w5N1w5N2A5N2A5N2Q5N2Q5N2g5N2g5N2w5N2w5N3A5N3A5N3Q5N3Q5N3g5N3g5N3w5N3w5N4A5N4A5N4Q5N4Q5N4g5N4g5N4w5N4w5N5A5N5A5N5Q5N5Q5N5g5N5g5N5w5N5w5N6A5N6A5N6Q5N6Q5lLg=="
                     },
                     "dependent node outputs": [
                         0,
                         0
                     ]
                 },
                 {
                     "data": {
-                        "GID": 4631,
+                        "GID": 542,
                         "identifier": "Data",
-                        "serialized": "gASVBAAAAAAAAABNmg4u"
+                        "serialized": "gASVBAAAAAAAAABN6Q4u"
                     },
                     "dependent node outputs": [
                         1,
                         0
                     ]
                 },
                 {
                     "data": {
-                        "GID": 151,
+                        "GID": 547,
                         "identifier": "Data",
-                        "serialized": "gASVCgAAAAAAAABHP+haHKwIMScu"
+                        "serialized": "gASVCgAAAAAAAABHP+MzMzMzMzMu"
                     },
                     "dependent node outputs": [
                         3,
                         0
                     ]
                 },
                 {
                     "data": {
-                        "GID": 4630,
+                        "GID": 541,
                         "identifier": "Data",
-                        "serialized": "gASVSAgAAAAAAABdlChN2wtN3AtN3QtN3gtN3wtN4AtN4QtN4gtN4wtN5AtN5QtN5gtN5wtN6AtN6QtN6gtN6wtN7AtN7QtN7gtN7wtN8AtN8QtN8gtN8wtN9AtN9QtN9gtN9wtN+AtN+QtN+gtN+wtN/AtN/QtN/gtN/wtNAAxNAQxNAgxNAwxNBAxNBQxNBgxNBwxNCAxNCQxNCgxNCwxNDAxNDQxNDgxNDwxNEAxNEQxNEgxNEwxNFAxNFQxNFgxNFwxNGAxNGQxNGgxNGwxNHAxNHQxNHgxNHwxNIAxNIQxNIgxNIwxNJAxNJQxNJgxNJwxNKAxNKQxNKgxNKwxNLAxNLQxNLgxNLwxNMAxNMQxNMgxNMwxNNAxNNQxNNgxNNwxNOAxNOQxNOgxNOwxNPAxNPQxNPgxNPgxNPwxNQAxNQQxNQgxNQwxNRAxNRQxNRgxNRwxNSAxNSQxNSgxNSwxNTAxNTQxNTgxNTwxNUAxNUQxNUgxNUwxNVAxNVQxNVgxNVwxNWAxNWQxNWgxNWwxNXAxNXQxNXgxNXwxNYAxNYQxNYgxNYwxNZAxNZQxNZgxNZwxNaAxNaQxNagxNawxNbAxNbQxNbgxNbwxNcAxNcQxNcgxNcwxNdAxNdQxNdgxNdwxNeAxNeQxNegxNewxNfAxNfQxNfgxNfwxNgAxNgQxNggxNgwxNhAxNhQxNhgxNhwxNiAxNiQxNigxNiwxNjAxNjQxNjgxNjwxNkAxNkQxNkgxNkwxNlAxNlQxNlgxNlwxNmAxNmQxNmgxNmwxNnAxNnQxNngxNnwxNoAxNoQxNogxNowxNpAxNpQxNpgxNpwxNqAxNqQxNqgxNqwxNrAxNrQxNrgxNrwxNsAxNsQxNsgxNswxNtAxNtQxNtgxNtwxNuAxNuQxNugxNuwxNvAxNvQxNvgxNvwxNwAxNwQxNwgxNwwxNxAxNxQxNxgxNxwxNyAxNyQxNygxNywxNzAxNzQxNzgxNzwxN0AxN0QxN0gxN0wxN1AxN1QxN1gxN1wxN2AxN2QxN2gxN2wxN3AxN3QxN3gxN3wxN4AxN4QxN4gxN4wxN5AxN5QxN5gxN5wxN6AxN6QxN6gxN6wxN7AxN7QxN7gxN7wxN8AxN8QxN8gxN8wxN9AxN9QxN9gxN9wxN+AxN+QxN+gxN+wxN/AxN/QxN/gxN/wxNAA1NAQ1NAg1NAw1NBA1NBQ1NBg1NBw1NCA1NCQ1NCg1NCw1NDA1NDQ1NDg1NDw1NEA1NEQ1NEg1NEw1NFA1NFQ1NFg1NFw1NGA1NGQ1NGg1NGw1NHA1NHQ1NHg1NHw1NIA1NIQ1NIg1NIw1NJA1NJQ1NJg1NJw1NKA1NKQ1NKg1NKw1NLA1NLQ1NLg1NLw1NMA1NMQ1NMg1NMw1NNA1NNQ1NNg1NNw1NOA1NOQ1NOg1NOw1NPA1NPQ1NPg1NPw1NQA1NQQ1NQg1NQw1NRA1NRQ1NRg1NRw1NSA1NSQ1NSg1NSw1NTA1NTQ1NTg1NTw1NUA1NUQ1NUg1NUw1NVA1NVQ1NVg1NVw1NWA1NWQ1NWg1NWw1NXA1NXQ1NXg1NXw1NYA1NYQ1NYg1NYw1NZA1NZQ1NZg1NZw1NaA1NaQ1Nag1Naw1NbA1NbQ1Nbg1Nbw1NcA1NcQ1Ncg1Ncw1NdA1NdQ1Ndg1Ndw1NeA1NeQ1Neg1New1NfA1NfQ1Nfg1Nfw1NgA1NgQ1Ngg1Ngw1NhA1NhQ1Nhg1Nhw1NiA1NiQ1Nig1Niw1NjA1NjQ1Njg1Njw1NkA1NkQ1Nkg1Nkw1NlA1NlQ1Nlg1Nlw1NmA1NmQ1Nmg1Nmw1NnA1NnQ1Nng1Nnw1NoA1NoQ1Nog1Now1NpA1NpQ1Npg1Npw1NqA1NqQ1Nqg1Nqw1NrA1NrQ1Nrg1Nrw1NsA1NsQ1Nsg1Nsw1NtA1NtQ1Ntg1Ntw1NuA1NuQ1Nug1Nuw1NvA1NvQ1Nvg1Nvw1NwA1NwQ1Nwg1Nww1NxA1NxQ1Nxg1Nxw1NyA1NyQ1Nyg1Nyw1NzA1NzQ1Nzg1Nzw1N0A1N0Q1N0g1N0w1N1A1N1Q1N1g1N1w1N2A1N2Q1N2g1N2w1N3A1N3Q1N3g1N3w1N4A1N4Q1N4g1N4w1N5A1N5Q1N5g1N5w1N6A1N6Q1N6g1N6w1N7A1N7Q1N7g1N7w1N8A1N8Q1N8g1N8w1N9A1N9Q1N9g1N9w1N+A1N+Q1N+g1N+w1N/A1N/Q1N/g1N/w1NAA5NAQ5NAg5NAw5NBA5NBQ5NBg5NBw5NCA5NCQ5NCg5NCw5NDA5NDQ5NDg5NDw5NEA5NEQ5NEg5NEw5NFA5NFQ5NFg5NFw5NGA5NGQ5NGg5NGw5NHA5NHQ5NHg5NHw5NIA5NIQ5NIg5NIw5NJA5NJQ5NJg5NJw5NKA5NKQ5NKg5NKw5NLA5NLQ5NLg5NLw5NMA5NMQ5NMg5NMw5NNA5NNQ5NNg5NNw5NOA5NOQ5NOg5NOw5NPA5NPQ5NPg5NPw5NQA5NQQ5NQg5NQw5NRA5NRQ5NRg5NRw5NSA5NSQ5NSg5NSw5NTA5NTQ5NTg5NTw5NUA5NUQ5NUg5NUw5NVA5NVQ5NVg5NVw5NWA5NWQ5NWg5NWw5NXA5NXQ5NXg5NXw5NYA5NYQ5NYg5NYw5NZA5NZQ5NZg5NZw5NaA5NaQ5Nag5Naw5NbA5NbQ5Nbg5Nbw5NcA5NcQ5Ncg5Ncw5NdA5NdQ5Ndg5Ndw5NeA5NeQ5Neg5New5NfA5NfQ5Nfg5Nfw5NgA5NgQ5Ngg5Ngw5NhA5NhQ5Nhg5Nhw5NiA5NiQ5Nig5Niw5NjA5NjQ5Njg5Njw5NkA5NkQ5Nkg5Nkw5NlA5NlQ5Nlg5Nlw5NmA5NmQ5Nmg5lLg=="
+                        "serialized": "gASVIgoAAAAAAABdlChN2wtN3AtN3QtN3gtN3wtN4AtN4QtN4gtN4wtN5AtN5QtN5gtN5wtN6AtN6QtN6gtN6wtN7AtN7QtN7gtN7wtN8AtN8QtN8gtN8wtN9AtN9QtN9gtN9wtN+AtN+QtN+gtN+wtN/AtN/QtN/gtN/wtNAAxNAQxNAgxNAwxNBAxNBQxNBgxNBwxNCAxNCQxNCgxNCwxNDAxNDQxNDgxNDwxNEAxNEQxNEgxNEwxNFAxNFQxNFgxNFwxNGAxNGQxNGgxNGwxNHAxNHQxNHgxNHwxNIAxNIQxNIgxNIwxNJAxNJQxNJgxNJwxNKAxNKQxNKgxNKwxNLAxNLQxNLgxNLwxNMAxNMQxNMgxNMwxNNAxNNQxNNgxNNwxNOAxNOQxNOgxNOwxNPAxNPQxNPgxNPgxNPwxNQAxNQQxNQgxNQwxNRAxNRQxNRgxNRwxNSAxNSQxNSgxNSwxNTAxNTQxNTgxNTwxNUAxNUQxNUgxNUwxNVAxNVQxNVgxNVwxNWAxNWQxNWgxNWwxNXAxNXQxNXgxNXwxNYAxNYQxNYgxNYwxNZAxNZQxNZgxNZwxNaAxNaQxNagxNawxNbAxNbQxNbgxNbwxNcAxNcQxNcgxNcwxNdAxNdQxNdgxNdwxNeAxNeQxNegxNewxNfAxNfQxNfgxNfwxNgAxNgQxNggxNgwxNhAxNhQxNhgxNhwxNiAxNiQxNigxNiwxNjAxNjQxNjgxNjwxNkAxNkQxNkgxNkwxNlAxNlQxNlgxNlwxNmAxNmQxNmgxNmwxNnAxNnQxNngxNnwxNoAxNoQxNogxNowxNpAxNpQxNpgxNpwxNqAxNqQxNqgxNqwxNrAxNrQxNrgxNrwxNsAxNsQxNsgxNswxNtAxNtQxNtgxNtwxNuAxNuQxNugxNuwxNvAxNvQxNvgxNvwxNwAxNwQxNwgxNwwxNxAxNxQxNxgxNxwxNyAxNyQxNygxNywxNzAxNzQxNzgxNzwxN0AxN0QxN0gxN0wxN1AxN1QxN1gxN1wxN2AxN2QxN2gxN2wxN3AxN3QxN3gxN3wxN4AxN4QxN4gxN4wxN5AxN5QxN5gxN5wxN6AxN6QxN6gxN6wxN7AxN7QxN7gxN7wxN8AxN8QxN8gxN8wxN9AxN9QxN9gxN9wxN+AxN+QxN+gxN+wxN/AxN/QxN/gxN/wxNAA1NAQ1NAg1NAw1NBA1NBQ1NBg1NBw1NCA1NCQ1NCg1NCw1NDA1NDQ1NDg1NDw1NEA1NEQ1NEg1NEw1NFA1NFQ1NFg1NFw1NGA1NGQ1NGg1NGw1NHA1NHQ1NHg1NHw1NIA1NIQ1NIg1NIw1NJA1NJQ1NJg1NJw1NKA1NKQ1NKg1NKw1NLA1NLQ1NLg1NLw1NMA1NMQ1NMg1NMw1NNA1NNQ1NNg1NNw1NOA1NOQ1NOg1NOw1NPA1NPQ1NPg1NPw1NQA1NQQ1NQg1NQw1NRA1NRQ1NRg1NRw1NSA1NSQ1NSg1NSw1NTA1NTQ1NTg1NTw1NUA1NUQ1NUg1NUw1NVA1NVQ1NVg1NVw1NWA1NWQ1NWg1NWw1NXA1NXQ1NXg1NXw1NYA1NYQ1NYg1NYw1NZA1NZQ1NZg1NZw1NaA1NaQ1Nag1Naw1NbA1NbQ1Nbg1Nbw1NcA1NcQ1Ncg1Ncw1NdA1NdQ1Ndg1Ndw1NeA1NeQ1Neg1New1NfA1NfQ1Nfg1Nfw1NgA1NgQ1Ngg1Ngw1NhA1NhQ1Nhg1Nhw1NiA1NiQ1Nig1Niw1NjA1NjQ1Njg1Njw1NkA1NkQ1Nkg1Nkw1NlA1NlQ1Nlg1Nlw1NmA1NmQ1Nmg1Nmw1NnA1NnQ1Nng1Nnw1NoA1NoQ1Nog1Now1NpA1NpQ1Npg1Npw1NqA1NqQ1Nqg1Nqw1NrA1NrQ1Nrg1Nrw1NsA1NsQ1Nsg1Nsw1NtA1NtQ1Ntg1Ntw1NuA1NuQ1Nug1Nuw1NvA1NvQ1Nvg1Nvw1NwA1NwQ1Nwg1Nww1NxA1NxQ1Nxg1Nxw1NyA1NyQ1Nyg1Nyw1NzA1NzQ1Nzg1Nzw1N0A1N0Q1N0g1N0w1N1A1N1Q1N1g1N1w1N2A1N2Q1N2g1N2w1N3A1N3Q1N3g1N3w1N4A1N4Q1N4g1N4w1N5A1N5Q1N5g1N5w1N6A1N6Q1N6g1N6w1N7A1N7Q1N7g1N7w1N8A1N8Q1N8g1N8w1N9A1N9Q1N9g1N9w1N+A1N+Q1N+g1N+w1N/A1N/Q1N/g1N/w1NAA5NAQ5NAg5NAw5NBA5NBQ5NBg5NBw5NCA5NCQ5NCg5NCw5NDA5NDQ5NDg5NDw5NEA5NEQ5NEg5NEw5NFA5NFQ5NFg5NFw5NGA5NGQ5NGg5NGw5NHA5NHQ5NHg5NHw5NIA5NIQ5NIg5NIw5NJA5NJQ5NJg5NJw5NKA5NKQ5NKg5NKw5NLA5NLQ5NLg5NLw5NMA5NMQ5NMg5NMw5NNA5NNQ5NNg5NNw5NOA5NOQ5NOg5NOw5NPA5NPQ5NPg5NPw5NQA5NQQ5NQg5NQw5NRA5NRQ5NRg5NRw5NSA5NSQ5NSg5NSw5NTA5NTQ5NTg5NTw5NUA5NUQ5NUg5NUw5NVA5NVQ5NVg5NVw5NWA5NWQ5NWg5NWw5NXA5NXQ5NXg5NXw5NYA5NYQ5NYg5NYw5NZA5NZQ5NZg5NZw5NaA5NaQ5Nag5Naw5NbA5NbQ5Nbg5Nbw5NcA5NcQ5Ncg5Ncw5NdA5NdQ5Ndg5Ndw5NeA5NeQ5Neg5New5NfA5NfQ5Nfg5Nfw5NgA5NgQ5Ngg5Ngw5NhA5NhQ5Nhg5Nhw5NiA5NiQ5Nig5Niw5NjA5NjQ5Njg5Njw5NkA5NkQ5Nkg5Nkw5NlA5NlQ5Nlg5Nlw5NmA5NmQ5Nmg5Nmw5Nmw5NnA5NnA5NnQ5NnQ5Nng5Nng5Nnw5Nnw5NoA5NoA5NoQ5NoQ5Nog5Nog5Now5Now5NpA5NpA5NpQ5NpQ5Npg5Npg5Npw5Npw5NqA5NqA5NqQ5NqQ5Nqg5Nqg5Nqw5Nqw5NrA5NrA5NrQ5NrQ5Nrg5Nrg5Nrw5Nrw5NsA5NsA5NsQ5NsQ5Nsg5Nsg5Nsw5Nsw5NtA5NtA5NtQ5NtQ5Ntg5Ntg5Ntw5Ntw5NuA5NuA5NuQ5NuQ5Nug5Nug5Nuw5Nuw5NvA5NvA5NvQ5NvQ5Nvg5Nvg5Nvw5Nvw5NwA5NwA5NwQ5NwQ5Nwg5Nwg5Nww5Nww5NxA5NxA5NxQ5NxQ5Nxg5Nxg5Nxw5Nxw5NyA5NyA5NyQ5NyQ5Nyg5Nyg5Nyw5Nyw5NzA5NzA5NzQ5NzQ5Nzg5Nzg5Nzw5Nzw5N0A5N0A5N0Q5N0Q5N0g5N0g5N0w5N0w5N1A5N1A5N1Q5N1Q5N1g5N1g5N1w5N1w5N2A5N2A5N2Q5N2Q5N2g5N2g5N2w5N2w5N3A5N3A5N3Q5N3Q5N3g5N3g5N3w5N3w5N4A5N4A5N4Q5N4Q5N4g5N4g5N4w5N4w5N5A5N5A5N5Q5N5Q5N5g5N5g5N5w5N5w5N6A5N6A5N6Q5N6Q5lLg=="
                     },
                     "dependent node outputs": [
                         6,
                         0
                     ]
                 },
                 {
                     "data": {
-                        "GID": 4626,
+                        "GID": 535,
                         "identifier": "Data",
-                        "serialized": "gASVBAAAAAAAAABNmg4u"
+                        "serialized": "gASVBAAAAAAAAABN6Q4u"
                     },
                     "dependent node outputs": [
                         9,
                         0
                     ]
                 },
                 {
                     "data": {
-                        "GID": 4633,
+                        "GID": 543,
                         "identifier": "Data",
-                        "serialized": "gASVBAAAAAAAAABNmw4u"
+                        "serialized": "gASVBAAAAAAAAABN6g4u"
                     },
                     "dependent node outputs": [
                         10,
                         0
                     ]
                 }
             ]
         },
         "script 2": {
-            "GID": 83,
+            "GID": 117,
             "algorithm mode": "data",
             "connections": [
                 {
                     "connected input port index": 0,
                     "connected node": 1,
                     "output port index": 0,
                     "parent node index": 0
@@ -912,15 +961,15 @@
                 "view size": [
                     10000.0,
                     7000.0
                 ]
             },
             "nodes": [
                 {
-                    "GID": 84,
+                    "GID": 118,
                     "actions": {
                         "change title": {
                             "method": "change_title"
                         },
                         "console ref": {
                             "method": "console_ref_monkeypatch"
                         },
@@ -933,31 +982,32 @@
                         "update shape": {
                             "method": "update_shape"
                         }
                     },
                     "additional data": {},
                     "collapsed": false,
                     "display title": "link OUT",
-                    "identifier": "std.LinkOUT_Node",
+                    "identifier": "examples.special_nodes.LinkOUT_Node",
                     "inputs": [],
+                    "inspector widget": {},
                     "outputs": [
                         {
-                            "GID": 85,
+                            "GID": 119,
                             "label": "",
                             "type": "data"
                         }
                     ],
                     "pos x": 384.5648465384588,
                     "pos y": 259.39811467640766,
                     "state data": "gASVNwAAAAAAAAB9lIwJbGlua2VkIElElIwkYzVlZmYxOTAtMjc5ZS00NzNjLWE0NzctYjYyZjI4NDBlMzk4lHMu",
                     "unconnected ports hidden": false,
-                    "version": "v0.2"
+                    "version": "v0.3"
                 },
                 {
-                    "GID": 86,
+                    "GID": 120,
                     "actions": {
                         "change title": {
                             "method": "change_title"
                         },
                         "console ref": {
                             "method": "console_ref_monkeypatch"
                         },
@@ -970,49 +1020,52 @@
                     },
                     "additional data": {},
                     "collapsed": false,
                     "display title": "result",
                     "identifier": "built_in.Result_Node",
                     "inputs": [
                         {
-                            "GID": 88,
+                            "GID": 122,
                             "has widget": false,
                             "label": "",
                             "type": "data"
                         }
                     ],
+                    "inspector widget": {},
                     "main widget data": "gAR9lC4=",
                     "outputs": [],
                     "pos x": 642.5648465384588,
                     "pos y": 259.39811467640766,
                     "state data": "gAR9lC4=",
                     "unconnected ports hidden": false,
                     "version": "v0.2"
                 }
             ],
             "output data": [
                 {
                     "data": {
-                        "GID": 151,
+                        "GID": 547,
                         "identifier": "Data",
-                        "serialized": "gASVCgAAAAAAAABHP+haHKwIMScu"
+                        "serialized": "gASVCgAAAAAAAABHP+MzMzMzMzMu"
                     },
                     "dependent node outputs": [
                         0,
                         0
                     ]
                 }
             ]
         }
     },
     "general info": {
-        "ryven version": "3.3.0a1",
+        "ryven version": "3.4.3",
         "type": "Ryven project file"
     },
+    "geometry": "01d9d0cb0003000000000138000000960000071b000003d50000013c000000b200000717000003d1000000000000000008d00000013c000000b200000717000003d1",
     "required packages": [
         {
-            "dir": "/home/leon/projects/ryven_projects/Ryven/ryven/example_nodes/std",
-            "name": "std"
+            "dir": "/home/leon/projects/ryven_projects/Ryven/ryven-editor/ryven/example_nodes/examples",
+            "name": "examples"
         }
     ],
-    "version": "0.4.0a12"
+    "state": "000000ff00000000fd000000020000000000000124000001edfc0200000001fc0000001e000001ed0000014b0100001efa000000010200000002fb000000140066006c006f00770073005f0064006f0063006b0100000000ffffffff0000007f00fffffffb00000014006e006f006400650073005f0064006f0063006b0100000000ffffffff0000012c00ffffff00000003000005dc00000101fc0100000001fb000000160063006f006e0073006f006c00650044006f0063006b0100000000000005dc0000005d00ffffff000004a4000001ed00000004000000040000000800000008fc00000000",
+    "version": "0.4.0"
 }
```

### Comparing `ryven-3.4.3/ryven/examples_projects/matrices.json` & `ryven-3.5.0/ryven/example_projects/matrices.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5688288530166786%*

 * *Differences: {"'addons'": "{'Variables': {'custom state': {'5': {'a': {'GID': 772, 'serialized': "*

 * *             "'gASVCgAAAAAAAABHP+jlYEGJN0wu'}, 'mat': {'GID': 798, 'serialized': "*

 * *             "'gASVywAAAAAAAACMFW51bXB5LmNvcmUubXVsdGlhcnJheZSMDF9yZWNvbnN0cnVjdJSTlIwFbnVtcHmUjAduZGFycmF5lJOUSwCFlEMBYpSHlFKUKEsBSwJLAoaUaAOMBWR0eXBllJOUjANjMTaUiYiHlFKUKEsDjAE8lE5OTkr/////Sv////9LAHSUYolDQAAAAAAAAAAAAAAAAAAA8D8AAAAAAADwPwAAAAAAAAAAAAAAAAAAAAAAAAAAAADwv0w3iUFg5eg/AAAAAAAAAACUdJRiLg=='}}}}}",*

 * * "'flow_uis'": "OrderedDict([(' […]*

```diff
@@ -7,28 +7,47 @@
             "version": "0.0.1"
         },
         "Variables": {
             "GID": 3,
             "custom state": {
                 "5": {
                     "a": {
-                        "GID": 6432,
+                        "GID": 772,
                         "identifier": "Data",
-                        "serialized": "gASVCgAAAAAAAABHP+i0OVgQYk4u"
+                        "serialized": "gASVCgAAAAAAAABHP+jlYEGJN0wu"
                     },
                     "mat": {
-                        "GID": 6458,
+                        "GID": 798,
                         "identifier": "Data",
-                        "serialized": "gASVywAAAAAAAACMFW51bXB5LmNvcmUubXVsdGlhcnJheZSMDF9yZWNvbnN0cnVjdJSTlIwFbnVtcHmUjAduZGFycmF5lJOUSwCFlEMBYpSHlFKUKEsBSwJLAoaUaAOMBWR0eXBllJOUjANjMTaUiYiHlFKUKEsDjAE8lE5OTkr/////Sv////9LAHSUYolDQAAAAAAAAAAAAAAAAAAA8D8AAAAAAADwPwAAAAAAAAAAAAAAAAAAAAAAAAAAAADwv05iEFg5tOg/AAAAAAAAAACUdJRiLg=="
+                        "serialized": "gASVywAAAAAAAACMFW51bXB5LmNvcmUubXVsdGlhcnJheZSMDF9yZWNvbnN0cnVjdJSTlIwFbnVtcHmUjAduZGFycmF5lJOUSwCFlEMBYpSHlFKUKEsBSwJLAoaUaAOMBWR0eXBllJOUjANjMTaUiYiHlFKUKEsDjAE8lE5OTkr/////Sv////9LAHSUYolDQAAAAAAAAAAAAAAAAAAA8D8AAAAAAADwPwAAAAAAAAAAAAAAAAAAAAAAAAAAAADwv0w3iUFg5eg/AAAAAAAAAACUdJRiLg=="
                     }
                 }
             },
             "version": "0.4"
         }
     },
+    "flow_uis": {
+        "5": {
+            "geometry": "01d9d0cb000300000000000000000000000004dc000002810000000000000000ffffffffffffffff000000000000000008d00000000000000000000004dc00000281",
+            "state": "000000ff00000000fd0000000100000001000000d800000282fc0200000001fc0000000000000282000000d10000005bfa000000000200000006fb0000001c0069006e00730070006500630074006f0072005f0064006f0063006b0100000000ffffffff000000b200fffffffb000000220075006e0064006f005f0068006900730074006f00720079005f0064006f0063006b0100000000ffffffff0000005600fffffffb0000001a00730065007400740069006e00670073005f0064006f0063006b0100000000ffffffff0000003c0000003cfb0000001c007600610072006900610062006c00650073005f0064006f0063006b0100000000ffffffff0000007f00fffffffb00000016006c006f0067006700650072005f0064006f0063006b0100000000ffffffff0000004800fffffffb000000160073006f0075007200630065005f0064006f0063006b0100000000ffffffff0000009000ffffff000003f10000028200000004000000040000000800000008fc00000000",
+            "view": {
+                "h_scroll": 0,
+                "m11": 0.975210518583877,
+                "m12": 0.0,
+                "m13": 0.0,
+                "m21": 0.0,
+                "m22": 0.975210518583877,
+                "m23": 0.0,
+                "m31": 0.0,
+                "m32": 0.0,
+                "m33": 1.0,
+                "v_scroll": 51
+            }
+        }
+    },
     "flows": {
         "hello world": {
             "GID": 5,
             "algorithm mode": "data",
             "connections": [
                 {
                     "connected input port index": 0,
@@ -136,14 +155,15 @@
                         }
                     },
                     "additional data": {},
                     "collapsed": false,
                     "display title": "Matrix",
                     "identifier": "linalg.EditMatrix_Node",
                     "inputs": [],
+                    "inspector widget": {},
                     "main widget data": "gASVKwAAAAAAAAB9lCiMBHRleHSUjBMgIDFqICAgIDEKMC0xaiAgICBhlIwFc2hvd26UiHUu",
                     "outputs": [
                         {
                             "GID": 8,
                             "label": "",
                             "type": "data"
                         }
@@ -184,27 +204,28 @@
                         {
                             "GID": 15,
                             "has widget": false,
                             "label": "",
                             "type": "data"
                         }
                     ],
-                    "main widget data": "gASVQwAAAAAAAAB9lCiMBHRleHSUjCsgICAgICAgIDFqICAgICAoMSswaikKICAgICAgIC0xaiAoMC43NzIrMGoplIwFc2hvd26UiHUu",
+                    "inspector widget": {},
+                    "main widget data": "gASVQwAAAAAAAAB9lCiMBHRleHSUjCsgICAgICAgIDFqICAgICAoMSswaikKICAgICAgIC0xaiAoMC43NzgrMGoplIwFc2hvd26UiHUu",
                     "outputs": [
                         {
                             "GID": 16,
                             "label": "",
                             "type": "data"
                         }
                     ],
                     "pos x": 469.009788256565,
                     "pos y": 289.198189623965,
                     "state data": "gAR9lC4=",
                     "unconnected ports hidden": false,
-                    "version": "v0.2"
+                    "version": "v0.3"
                 },
                 {
                     "GID": 17,
                     "Variables": {
                         "subscriptions": {}
                     },
                     "actions": {
@@ -232,33 +253,34 @@
                                 "GID": 28,
                                 "identifier": "Data",
                                 "serialized": "gASVBQAAAAAAAACMAWGULg=="
                             },
                             "has widget": true,
                             "label": "var",
                             "type": "data",
-                            "widget data": "gASVbAAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTVAZjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUjAFhlHVicy4=",
+                            "widget data": "gASVbAAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTTIDjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUjAFhlHVicy4=",
                             "widget name": "varname",
                             "widget pos": "besides"
                         },
                         {
                             "GID": 25,
                             "default": {
-                                "GID": 6431,
+                                "GID": 771,
                                 "identifier": "Data",
-                                "serialized": "gASVCQAAAAAAAACMBTAuNzcylC4="
+                                "serialized": "gASVCQAAAAAAAACMBTAuNzc4lC4="
                             },
                             "has widget": true,
                             "label": "val",
                             "type": "data",
-                            "widget data": "gASVcAAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTVEZjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUjAUwLjc3MpR1YnMu",
+                            "widget data": "gASVcAAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTTMDjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUjAUwLjc3OJR1YnMu",
                             "widget name": "val",
                             "widget pos": "besides"
                         }
                     ],
+                    "inspector widget": {},
                     "outputs": [
                         {
                             "GID": 27,
                             "label": "val",
                             "type": "data"
                         }
                     ],
@@ -286,58 +308,59 @@
                         "update shape": {
                             "method": "update_shape"
                         }
                     },
                     "additional data": {},
                     "collapsed": false,
                     "display title": "slider",
-                    "identifier": "std.Slider_Node",
+                    "identifier": "examples.special_nodes.Slider_Node",
                     "inputs": [
                         {
                             "GID": 34,
                             "default": {
                                 "GID": 40,
                                 "identifier": "Data",
                                 "serialized": "gARLAS4="
                             },
                             "has widget": true,
                             "label": "scl",
                             "type": "data",
-                            "widget data": "gASVagAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTVIZjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUSwF1YnMu",
+                            "widget data": "gASVagAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTTQDjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUSwF1YnMu",
                             "widget name": "scale",
                             "widget pos": "besides"
                         },
                         {
                             "GID": 36,
                             "default": {
                                 "GID": 42,
                                 "identifier": "Data",
                                 "serialized": "gASJLg=="
                             },
                             "has widget": true,
                             "label": "round",
                             "type": "data",
-                            "widget data": "gASVaQAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTVMZjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUiXVicy4=",
+                            "widget data": "gASVaQAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTTUDjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUiXVicy4=",
                             "widget name": "round",
                             "widget pos": "besides"
                         }
                     ],
+                    "inspector widget": {},
                     "main widget data": "gAR9lC4=",
                     "outputs": [
                         {
                             "GID": 38,
                             "label": "",
                             "type": "data"
                         }
                     ],
                     "pos x": 210.009788256565,
                     "pos y": 95.19818962396499,
-                    "state data": "gASVEwAAAAAAAAB9lIwDdmFslEc/6LQ5WBBiTnMu",
+                    "state data": "gASVEwAAAAAAAAB9lIwDdmFslEc/6OVgQYk3THMu",
                     "unconnected ports hidden": false,
-                    "version": "v0.2"
+                    "version": "v0.3"
                 },
                 {
                     "GID": 43,
                     "Variables": {
                         "subscriptions": {}
                     },
                     "actions": {
@@ -366,57 +389,58 @@
                         "update shape": {
                             "method": "update_shape"
                         }
                     },
                     "additional data": {},
                     "collapsed": false,
                     "display title": "*",
-                    "identifier": "std.Multiply_Node",
+                    "identifier": "examples.basic_operators.Multiply_Node",
                     "inputs": [
                         {
                             "GID": 47,
                             "default": {
-                                "GID": 6429,
+                                "GID": 769,
                                 "identifier": "Data",
-                                "serialized": "gASVCgAAAAAAAABHP+i0OVgQYk4u"
+                                "serialized": "gASVCgAAAAAAAABHP+jlYEGJN0wu"
                             },
                             "has widget": true,
                             "label": "",
                             "type": "data",
-                            "widget data": "gASVcQAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTVQZjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSURz/otDlYEGJOdWJzLg==",
+                            "widget data": "gASVcQAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTTYDjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSURz/o5WBBiTdMdWJzLg==",
                             "widget name": "in",
                             "widget pos": "besides"
                         },
                         {
                             "GID": 49,
                             "default": {
                                 "GID": 55,
                                 "identifier": "Data",
                                 "serialized": "gARLAS4="
                             },
                             "has widget": true,
                             "label": "",
                             "type": "data",
-                            "widget data": "gASVagAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTVUZjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUSwF1YnMu",
+                            "widget data": "gASVagAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTTcDjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUSwF1YnMu",
                             "widget name": "in",
                             "widget pos": "besides"
                         }
                     ],
+                    "inspector widget": {},
                     "outputs": [
                         {
                             "GID": 51,
                             "label": "",
                             "type": "data"
                         }
                     ],
                     "pos x": 381.009788256565,
                     "pos y": 122.19818962396499,
                     "state data": "gAR9lC4=",
                     "unconnected ports hidden": false,
-                    "version": "v0.2"
+                    "version": "v0.3"
                 },
                 {
                     "GID": 56,
                     "Variables": {
                         "subscriptions": {}
                     },
                     "actions": {
@@ -444,33 +468,34 @@
                                 "GID": 67,
                                 "identifier": "Data",
                                 "serialized": "gASVBwAAAAAAAACMA21hdJQu"
                             },
                             "has widget": true,
                             "label": "var",
                             "type": "data",
-                            "widget data": "gASVbgAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTVYZjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUjANtYXSUdWJzLg==",
+                            "widget data": "gASVbgAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTTgDjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUjANtYXSUdWJzLg==",
                             "widget name": "varname",
                             "widget pos": "besides"
                         },
                         {
                             "GID": 64,
                             "default": {
-                                "GID": 6435,
+                                "GID": 775,
                                 "identifier": "Data",
-                                "serialized": "gASVMgAAAAAAAACMLltbMC4gICArMS5qIDEuICAgKzAual0KIFswLiAgIC0xLmogMC43NzIrMC5qXV2ULg=="
+                                "serialized": "gASVMgAAAAAAAACMLltbMC4gICArMS5qIDEuICAgKzAual0KIFswLiAgIC0xLmogMC43NzgrMC5qXV2ULg=="
                             },
                             "has widget": true,
                             "label": "val",
                             "type": "data",
-                            "widget data": "gASVmQAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTVcZjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUjC5bWzAuICAgKzEuaiAxLiAgICswLmpdCiBbMC4gICAtMS5qIDAuNzcyKzAual1dlHVicy4=",
+                            "widget data": "gASVmQAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTTkDjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUjC5bWzAuICAgKzEuaiAxLiAgICswLmpdCiBbMC4gICAtMS5qIDAuNzc4KzAual1dlHVicy4=",
                             "widget name": "val",
                             "widget pos": "besides"
                         }
                     ],
+                    "inspector widget": {},
                     "outputs": [
                         {
                             "GID": 66,
                             "label": "val",
                             "type": "data"
                         }
                     ],
@@ -512,19 +537,20 @@
                                 "GID": 76,
                                 "identifier": "Data",
                                 "serialized": "gASVBwAAAAAAAACMA21hdJQu"
                             },
                             "has widget": true,
                             "label": "",
                             "type": "data",
-                            "widget data": "gASVbgAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTVgZjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUjANtYXSUdWJzLg==",
+                            "widget data": "gASVbgAAAAAAAAB9lIwDdmFslIwOcnl2ZW5jb3JlLkRhdGGUjAREYXRhlJOUKYGUfZQojAlnbG9iYWxfaWSUTToDjA5wcmV2X2dsb2JhbF9pZJROjAxwcmV2X3ZlcnNpb26UTowIX3BheWxvYWSUjANtYXSUdWJzLg==",
                             "widget name": "varname",
                             "widget pos": "besides"
                         }
                     ],
+                    "inspector widget": {},
                     "outputs": [
                         {
                             "GID": 74,
                             "label": "val",
                             "type": "data"
                         }
                     ],
@@ -564,27 +590,28 @@
                         {
                             "GID": 80,
                             "has widget": false,
                             "label": "",
                             "type": "data"
                         }
                     ],
-                    "main widget data": "gASVRwAAAAAAAAB9lCiMBHRleHSUjC8gICAtMC40MzU3aiAgICAgMC41NjQzagooMC41NjQzKzBqKSAoMC41NjQzKzBqKZSMBXNob3dulIh1Lg==",
+                    "inspector widget": {},
+                    "main widget data": "gASVRwAAAAAAAAB9lCiMBHRleHSUjC8gICAtMC40Mzc2aiAgICAgMC41NjI0agooMC41NjI0KzBqKSAoMC41NjI0KzBqKZSMBXNob3dulIh1Lg==",
                     "outputs": [
                         {
                             "GID": 81,
                             "label": "",
                             "type": "data"
                         }
                     ],
                     "pos x": 175.96624820900752,
                     "pos y": 548.4374023593136,
                     "state data": "gAR9lC4=",
                     "unconnected ports hidden": false,
-                    "version": "v0.2"
+                    "version": "v0.3"
                 },
                 {
                     "GID": 82,
                     "Variables": {
                         "subscriptions": {}
                     },
                     "actions": {
@@ -612,27 +639,28 @@
                         {
                             "GID": 85,
                             "has widget": false,
                             "label": "",
                             "type": "data"
                         }
                     ],
-                    "main widget data": "gASVLAAAAAAAAAB9lCiMBHRleHSUjBQtMC41NjQzMzQwODU3Nzg3ODExapSMBXNob3dulIh1Lg==",
+                    "inspector widget": {},
+                    "main widget data": "gASVKwAAAAAAAAB9lCiMBHRleHSUjBMtMC41NjI0Mjk2OTYyODc5NjRqlIwFc2hvd26UiHUu",
                     "outputs": [
                         {
                             "GID": 86,
                             "label": "",
                             "type": "data"
                         }
                     ],
                     "pos x": 611.0383971650748,
                     "pos y": 548.1962980663284,
                     "state data": "gAR9lC4=",
                     "unconnected ports hidden": false,
-                    "version": "v0.2"
+                    "version": "v0.3"
                 },
                 {
                     "GID": 87,
                     "Variables": {
                         "subscriptions": {}
                     },
                     "actions": {
@@ -666,27 +694,28 @@
                         {
                             "GID": 92,
                             "has widget": false,
                             "label": "",
                             "type": "data"
                         }
                     ],
-                    "main widget data": "gASVLwAAAAAAAAB9lCiMBHRleHSUjBcgICAtMC40MzU3aiAoMC41NjQzKzBqKZSMBXNob3dulIh1Lg==",
+                    "inspector widget": {},
+                    "main widget data": "gASVLwAAAAAAAAB9lCiMBHRleHSUjBcgICAtMC40Mzc2aiAoMC41NjI0KzBqKZSMBXNob3dulIh1Lg==",
                     "outputs": [
                         {
                             "GID": 93,
                             "label": "",
                             "type": "data"
                         }
                     ],
                     "pos x": 885.1839459089059,
                     "pos y": 322.570155217133,
                     "state data": "gAR9lC4=",
                     "unconnected ports hidden": false,
-                    "version": "v0.2"
+                    "version": "v0.3"
                 },
                 {
                     "GID": 94,
                     "Variables": {
                         "subscriptions": {}
                     },
                     "actions": {
@@ -720,27 +749,28 @@
                         {
                             "GID": 99,
                             "has widget": false,
                             "label": "",
                             "type": "data"
                         }
                     ],
+                    "inspector widget": {},
                     "main widget data": "gASVMwAAAAAAAAB9lCiMBHRleHSUjBsoMSswaikgICAgIDBqCiAgICAwaiAoMSswaimUjAVzaG93bpSIdS4=",
                     "outputs": [
                         {
                             "GID": 100,
                             "label": "",
                             "type": "data"
                         }
                     ],
                     "pos x": 361.26934314274683,
                     "pos y": 439.43716494485284,
                     "state data": "gAR9lC4=",
                     "unconnected ports hidden": false,
-                    "version": "v0.2"
+                    "version": "v0.3"
                 },
                 {
                     "GID": 101,
                     "Variables": {
                         "subscriptions": {}
                     },
                     "actions": {
@@ -760,36 +790,37 @@
                         "update shape": {
                             "method": "update_shape"
                         }
                     },
                     "additional data": {},
                     "collapsed": false,
                     "display title": "eval",
-                    "identifier": "std.Eval_Node",
+                    "identifier": "examples.special_nodes.Eval_Node",
                     "inputs": [
                         {
                             "GID": 103,
                             "has widget": false,
                             "label": "",
                             "type": "data"
                         }
                     ],
+                    "inspector widget": {},
                     "main widget data": "gASVHAAAAAAAAAB9lIwEdGV4dJSMDihpbnBbMF0pWzBdWzpdlHMu",
                     "outputs": [
                         {
                             "GID": 104,
                             "label": "",
                             "type": "data"
                         }
                     ],
                     "pos x": 598.3422117376416,
                     "pos y": 418.5614824529824,
                     "state data": "gASVPQAAAAAAAAB9lCiMEG51bSBwYXJhbSBpbnB1dHOUSwGMD2V4cHJlc3Npb24gY29kZZSMDihpbnBbMF0pWzBdWzpdlHUu",
                     "unconnected ports hidden": false,
-                    "version": "v0.2"
+                    "version": "v0.3"
                 },
                 {
                     "GID": 105,
                     "Variables": {
                         "subscriptions": {}
                     },
                     "actions": {
@@ -814,146 +845,149 @@
                         {
                             "GID": 107,
                             "has widget": false,
                             "label": "",
                             "type": "data"
                         }
                     ],
+                    "inspector widget": {},
                     "main widget data": "gAR9lC4=",
                     "outputs": [],
                     "pos x": 882.6120564064703,
                     "pos y": 429.0070935431757,
                     "state data": "gAR9lC4=",
                     "unconnected ports hidden": false,
                     "version": "v0.2"
                 }
             ],
             "output data": [
                 {
                     "data": {
-                        "GID": 6456,
+                        "GID": 796,
                         "identifier": "MatrixData",
-                        "serialized": "gASVywAAAAAAAACMFW51bXB5LmNvcmUubXVsdGlhcnJheZSMDF9yZWNvbnN0cnVjdJSTlIwFbnVtcHmUjAduZGFycmF5lJOUSwCFlEMBYpSHlFKUKEsBSwJLAoaUaAOMBWR0eXBllJOUjANjMTaUiYiHlFKUKEsDjAE8lE5OTkr/////Sv////9LAHSUYolDQAAAAAAAAAAAAAAAAAAA8D8AAAAAAADwPwAAAAAAAAAAAAAAAAAAAAAAAAAAAADwv05iEFg5tOg/AAAAAAAAAACUdJRiLg=="
+                        "serialized": "gASVywAAAAAAAACMFW51bXB5LmNvcmUubXVsdGlhcnJheZSMDF9yZWNvbnN0cnVjdJSTlIwFbnVtcHmUjAduZGFycmF5lJOUSwCFlEMBYpSHlFKUKEsBSwJLAoaUaAOMBWR0eXBllJOUjANjMTaUiYiHlFKUKEsDjAE8lE5OTkr/////Sv////9LAHSUYolDQAAAAAAAAAAAAAAAAAAA8D8AAAAAAADwPwAAAAAAAAAAAAAAAAAAAAAAAAAAAADwv0w3iUFg5eg/AAAAAAAAAACUdJRiLg=="
                     },
                     "dependent node outputs": [
                         0,
                         0
                     ]
                 },
                 {
                     "data": {
-                        "GID": 6457,
+                        "GID": 797,
                         "identifier": "MatrixData",
-                        "serialized": "gASVywAAAAAAAACMFW51bXB5LmNvcmUubXVsdGlhcnJheZSMDF9yZWNvbnN0cnVjdJSTlIwFbnVtcHmUjAduZGFycmF5lJOUSwCFlEMBYpSHlFKUKEsBSwJLAoaUaAOMBWR0eXBllJOUjANjMTaUiYiHlFKUKEsDjAE8lE5OTkr/////Sv////9LAHSUYolDQAAAAAAAAAAAAAAAAAAA8D8AAAAAAADwPwAAAAAAAAAAAAAAAAAAAAAAAAAAAADwv05iEFg5tOg/AAAAAAAAAACUdJRiLg=="
+                        "serialized": "gASVywAAAAAAAACMFW51bXB5LmNvcmUubXVsdGlhcnJheZSMDF9yZWNvbnN0cnVjdJSTlIwFbnVtcHmUjAduZGFycmF5lJOUSwCFlEMBYpSHlFKUKEsBSwJLAoaUaAOMBWR0eXBllJOUjANjMTaUiYiHlFKUKEsDjAE8lE5OTkr/////Sv////9LAHSUYolDQAAAAAAAAAAAAAAAAAAA8D8AAAAAAADwPwAAAAAAAAAAAAAAAAAAAAAAAAAAAADwv0w3iUFg5eg/AAAAAAAAAACUdJRiLg=="
                     },
                     "dependent node outputs": [
                         1,
                         0
                     ]
                 },
                 {
                     "data": {
-                        "GID": 6428,
+                        "GID": 768,
                         "identifier": "Data",
-                        "serialized": "gASVCgAAAAAAAABHP+i0OVgQYk4u"
+                        "serialized": "gASVCgAAAAAAAABHP+jlYEGJN0wu"
                     },
                     "dependent node outputs": [
                         3,
                         0
                     ]
                 },
                 {
                     "data": {
-                        "GID": 6430,
+                        "GID": 770,
                         "identifier": "Data",
-                        "serialized": "gASVCgAAAAAAAABHP+i0OVgQYk4u"
+                        "serialized": "gASVCgAAAAAAAABHP+jlYEGJN0wu"
                     },
                     "dependent node outputs": [
                         4,
                         0
                     ]
                 },
                 {
                     "data": {
-                        "GID": 6468,
+                        "GID": 808,
                         "identifier": "Data",
-                        "serialized": "gASVywAAAAAAAACMFW51bXB5LmNvcmUubXVsdGlhcnJheZSMDF9yZWNvbnN0cnVjdJSTlIwFbnVtcHmUjAduZGFycmF5lJOUSwCFlEMBYpSHlFKUKEsBSwJLAoaUaAOMBWR0eXBllJOUjANjMTaUiYiHlFKUKEsDjAE8lE5OTkr/////Sv////9LAHSUYolDQAAAAAAAAAAAAAAAAAAA8D8AAAAAAADwPwAAAAAAAAAAAAAAAAAAAAAAAAAAAADwv05iEFg5tOg/AAAAAAAAAACUdJRiLg=="
+                        "serialized": "gASVywAAAAAAAACMFW51bXB5LmNvcmUubXVsdGlhcnJheZSMDF9yZWNvbnN0cnVjdJSTlIwFbnVtcHmUjAduZGFycmF5lJOUSwCFlEMBYpSHlFKUKEsBSwJLAoaUaAOMBWR0eXBllJOUjANjMTaUiYiHlFKUKEsDjAE8lE5OTkr/////Sv////9LAHSUYolDQAAAAAAAAAAAAAAAAAAA8D8AAAAAAADwPwAAAAAAAAAAAAAAAAAAAAAAAAAAAADwv0w3iUFg5eg/AAAAAAAAAACUdJRiLg=="
                     },
                     "dependent node outputs": [
                         6,
                         0
                     ]
                 },
                 {
                     "data": {
-                        "GID": 6472,
+                        "GID": 812,
                         "identifier": "MatrixData",
-                        "serialized": "gASVywAAAAAAAACMFW51bXB5LmNvcmUubXVsdGlhcnJheZSMDF9yZWNvbnN0cnVjdJSTlIwFbnVtcHmUjAduZGFycmF5lJOUSwCFlEMBYpSHlFKUKEsBSwJLAoaUaAOMBWR0eXBllJOUjANjMTaUiYiHlFKUKEsDjAE8lE5OTkr/////Sv////9LAHSUYolDQAAAAAAAAAAAEPljSfPh278AAAAAAAAAAHgDTlsGD+I/eANOWwYP4j8AAAAAAAAAAHgDTlsGD+I/AAAAAAAAAACUdJRiLg=="
+                        "serialized": "gASVywAAAAAAAACMFW51bXB5LmNvcmUubXVsdGlhcnJheZSMDF9yZWNvbnN0cnVjdJSTlIwFbnVtcHmUjAduZGFycmF5lJOUSwCFlEMBYpSHlFKUKEsBSwJLAoaUaAOMBWR0eXBllJOUjANjMTaUiYiHlFKUKEsDjAE8lE5OTkr/////Sv////9LAHSUYolDQAAAAAAAAAAAADcJ4CYB3L8AAAAAAAAAAIBk+49s/+E/gGT7j2z/4T8AAAAAAAAAAIBk+49s/+E/AAAAAAAAAACUdJRiLg=="
                     },
                     "dependent node outputs": [
                         7,
                         0
                     ]
                 },
                 {
                     "data": {
-                        "GID": 6473,
+                        "GID": 813,
                         "identifier": "MatrixData",
-                        "serialized": "gASVcgAAAAAAAACMFW51bXB5LmNvcmUubXVsdGlhcnJheZSMBnNjYWxhcpSTlIwFbnVtcHmUjAVkdHlwZZSTlIwDYzE2lImIh5RSlChLA4wBPJROTk5K/////0r/////SwB0lGJDEAAAAAAAAAAAeANOWwYP4r+UhpRSlC4="
+                        "serialized": "gASVcgAAAAAAAACMFW51bXB5LmNvcmUubXVsdGlhcnJheZSMBnNjYWxhcpSTlIwFbnVtcHmUjAVkdHlwZZSTlIwDYzE2lImIh5RSlChLA4wBPJROTk5K/////0r/////SwB0lGJDEAAAAAAAAAAAgGT7j2z/4b+UhpRSlC4="
                     },
                     "dependent node outputs": [
                         8,
                         0
                     ]
                 },
                 {
                     "data": {
-                        "GID": 6479,
+                        "GID": 817,
                         "identifier": "MatrixData",
-                        "serialized": "gASVqQAAAAAAAACMFW51bXB5LmNvcmUubXVsdGlhcnJheZSMDF9yZWNvbnN0cnVjdJSTlIwFbnVtcHmUjAduZGFycmF5lJOUSwCFlEMBYpSHlFKUKEsBSwKFlGgDjAVkdHlwZZSTlIwDYzE2lImIh5RSlChLA4wBPJROTk5K/////0r/////SwB0lGKJQyAAAAAAAAAAABD5Y0nz4du/eANOWwYP4j8AAAAAAAAAAJR0lGIu"
+                        "serialized": "gASVqQAAAAAAAACMFW51bXB5LmNvcmUubXVsdGlhcnJheZSMDF9yZWNvbnN0cnVjdJSTlIwFbnVtcHmUjAduZGFycmF5lJOUSwCFlEMBYpSHlFKUKEsBSwKFlGgDjAVkdHlwZZSTlIwDYzE2lImIh5RSlChLA4wBPJROTk5K/////0r/////SwB0lGKJQyAAAAAAAAAAAAA3CeAmAdy/gGT7j2z/4T8AAAAAAAAAAJR0lGIu"
                     },
                     "dependent node outputs": [
                         9,
                         0
                     ]
                 },
                 {
                     "data": {
-                        "GID": 6474,
+                        "GID": 814,
                         "identifier": "MatrixData",
-                        "serialized": "gASVywAAAAAAAACMFW51bXB5LmNvcmUubXVsdGlhcnJheZSMDF9yZWNvbnN0cnVjdJSTlIwFbnVtcHmUjAduZGFycmF5lJOUSwCFlEMBYpSHlFKUKEsBSwJLAoaUaAOMBWR0eXBllJOUjANjMTaUiYiHlFKUKEsDjAE8lE5OTkr/////Sv////9LAHSUYolDQAAAAAAAAPA/AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAkP6YJq2umDwAAAAAAAAAAAAAAAAAAPA/AAAAAAAAAACUdJRiLg=="
+                        "serialized": "gASVywAAAAAAAACMFW51bXB5LmNvcmUubXVsdGlhcnJheZSMDF9yZWNvbnN0cnVjdJSTlIwFbnVtcHmUjAduZGFycmF5lJOUSwCFlEMBYpSHlFKUKEsBSwJLAoaUaAOMBWR0eXBllJOUjANjMTaUiYiHlFKUKEsDjAE8lE5OTkr/////Sv////9LAHSUYolDQAAAAAAAAPA/AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAKxyE25yiDwAAAAAAAAAAAAAAAAAAPA/AAAAAAAAAACUdJRiLg=="
                     },
                     "dependent node outputs": [
                         10,
                         0
                     ]
                 },
                 {
                     "data": {
-                        "GID": 6478,
+                        "GID": 815,
                         "identifier": "Data",
                         "serialized": "gASVqQAAAAAAAACMFW51bXB5LmNvcmUubXVsdGlhcnJheZSMDF9yZWNvbnN0cnVjdJSTlIwFbnVtcHmUjAduZGFycmF5lJOUSwCFlEMBYpSHlFKUKEsBSwKFlGgDjAVkdHlwZZSTlIwDYzE2lImIh5RSlChLA4wBPJROTk5K/////0r/////SwB0lGKJQyAAAAAAAADwPwAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAJR0lGIu"
                     },
                     "dependent node outputs": [
                         11,
                         0
                     ]
                 }
             ]
         }
     },
     "general info": {
-        "ryven version": "3.3.0a1",
+        "ryven version": "3.4.3",
         "type": "Ryven project file"
     },
+    "geometry": "01d9d0cb00030000000001270000009b000007590000047f0000012b000000b7000007550000047b000000000000000008d00000012b000000b7000007550000047b",
     "required packages": [
         {
-            "dir": "/home/leon/projects/ryven_projects/Ryven/ryven/example_nodes/linalg",
-            "name": "linalg"
+            "dir": "/home/leon/projects/ryven_projects/Ryven/ryven-editor/ryven/example_nodes/examples",
+            "name": "examples"
         },
         {
-            "dir": "/home/leon/projects/ryven_projects/Ryven/ryven/example_nodes/std",
-            "name": "std"
+            "dir": "/home/leon/projects/ryven_projects/Ryven/ryven-editor/ryven/example_nodes/linalg",
+            "name": "linalg"
         }
     ],
-    "version": "0.4.0a12"
+    "state": "000000ff00000000fd000000020000000000000124000002b7fc0200000001fc0000001e000002b70000014b0100001efa000000010200000002fb000000140066006c006f00770073005f0064006f0063006b0100000000ffffffff0000007f00fffffffb00000014006e006f006400650073005f0064006f0063006b0100000000ffffffff0000012c00ffffff000000030000062b000000dcfc0100000001fb000000160063006f006e0073006f006c00650044006f0063006b01000000000000062b0000005d00ffffff000004f3000002b700000004000000040000000800000008fc00000000",
+    "version": "0.4.0"
 }
```

### Comparing `ryven-3.4.3/ryven/gui/code_editor/CodeEditorWidget.py` & `ryven-3.5.0/ryven/gui/code_editor/CodeEditorWidget.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/gui/code_editor/CodePreviewWidget.py` & `ryven-3.5.0/ryven/gui/code_editor/CodePreviewWidget.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,95 @@
+# prevent circular imports
+from __future__ import annotations
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from ryven.gui.main_window import MainWindow
+
 from dataclasses import dataclass
-from typing import Type, Optional
+from typing import Type, Optional, List
 
 from qtpy.QtCore import Qt
-from qtpy.QtWidgets import QWidget, QHBoxLayout, QVBoxLayout, QRadioButton, QLabel, QCheckBox, QGridLayout, \
+from qtpy.QtWidgets import (
+    QWidget, 
+    QHBoxLayout, 
+    QVBoxLayout, 
+    QRadioButton, 
+    QLabel, 
+    QCheckBox, 
+    QGridLayout,
     QPushButton
-from ryvencore import Node
+)
 
 from ryven.gui.code_editor.EditSrcCodeInfoDialog import EditSrcCodeInfoDialog
 from ryven.gui.code_editor.CodeEditorWidget import CodeEditorWidget
 from ryven.gui.code_editor.SourceCodeUpdater import SrcCodeUpdater
-from ryven.gui.code_editor.codes_storage import class_codes, mod_codes, modif_codes, NodeTypeCodes, \
-    Inspectable, NodeInspectable, MainWidgetInspectable, CustomInputWidgetInspectable
+from ryven.gui.code_editor.codes_storage import (
+    class_codes, 
+    mod_codes, 
+    modif_codes, 
+    NodeTypeCodes,
+    Inspectable, 
+    NodeInspectable, 
+    MainWidgetInspectable, 
+    CustomInputWidgetInspectable,
+    load_src_code,
+)
+
+from ryvencore import Node
+from ryvencore_qt.src.flows.FlowView import FlowView
+
+
+class LoadSrcCodeButton(QPushButton):
+    def __init__(self):
+        super().__init__('load source code')
+        self._node = None
+    
+    @property
+    def node(self):
+        return self._node
+    
+    @node.setter
+    def node(self, node):
+        self._node = node
 
 
 class LinkedRadioButton(QRadioButton):
     """Represents a button linked to one particular inspectable object."""
 
     def __init__(self, name, obj: Inspectable):
         super().__init__(name)
         self.representing: Inspectable = obj
 
 
 class CodePreviewWidget(QWidget):
-    def __init__(self, main_window, flow_view):
+    def __init__(self, main_window: MainWindow, flow_view: FlowView):
         super().__init__()
 
         self.edits_enabled = main_window.config.src_code_edits_enabled
         self.current_insp: Optional[Inspectable] = None
 
         # widgets
-        self.radio_buttons = []
+        self.radio_buttons: List[QRadioButton] = []
         self.text_edit = CodeEditorWidget(main_window.theme)
 
         self.setup_ui()
         self._set_node(None)
         flow_view.nodes_selection_changed.connect(self.set_selected_nodes)
 
     def setup_ui(self):
 
         secondary_layout = QHBoxLayout()
 
+        # load source code button
+        self.load_code_button = LoadSrcCodeButton()
+        self.load_code_button.setProperty('class', 'small_button')
+        secondary_layout.addWidget(self.load_code_button)
+        self.load_code_button.hide()
+        self.load_code_button.clicked.connect(self._load_code_button_clicked)
+
         # class radio buttons widget
         self.class_selection_layout = QHBoxLayout()  # QGridLayout()
 
         secondary_layout.addLayout(self.class_selection_layout)
         self.class_selection_layout.setAlignment(Qt.AlignLeft)
         # secondary_layout.setAlignment(self.class_selection_layout, Qt.AlignLeft)
 
@@ -92,44 +138,55 @@
             # clear view
             if self.edits_enabled:
                 self.edit_code_button.setEnabled(False)
                 self.override_code_button.setEnabled(False)
                 self.reset_code_button.setEnabled(False)
             self.text_edit.set_code('')
             self._clear_class_layout()
-            return
+        else:
+            if class_codes.get(node.__class__) is None:
+                # source code not loaded yet
+                self.load_code_button.node = node
+                self.load_code_button.show()
+                self._clear_class_layout()
+                self._update_code(NodeInspectable(node, 'source not loaded'))
+            else:
+                self._process_node_src(node)
 
+    def _process_node_src(self, node: Node):
         self._rebuild_class_selection(node)
-
-        code = class_codes[node.__class__].node_cls
-
+        codes = class_codes[node.__class__]
+        assert codes is not None
+        code = codes.node_cls
         if self.edits_enabled and node in modif_codes:
             code = modif_codes[node]
-
         self._update_code(NodeInspectable(node, code))
 
-
     def _update_code(self, insp: Inspectable):
         if self.edits_enabled:
             self._disable_editing()
             self._update_radio_buttons_edit_status()
             self.edit_code_button.setEnabled(True)
             self.reset_code_button.setEnabled(insp.obj in modif_codes)
 
         self.text_edit.disable_highlighting()
 
         self.current_insp = insp
         self.text_edit.set_code(insp.code)
 
 
     def _rebuild_class_selection(self, node: Node):
+        assert hasattr(node, 'gui')
+
+        self.load_code_button.hide()
         self._clear_class_layout()
         self.radio_buttons.clear()
 
-        codes: NodeTypeCodes = class_codes[node.__class__]
+        codes = class_codes[node.__class__]
+        assert codes is not None
 
         def register_rb(rb: QRadioButton):
            rb.toggled.connect(self._class_rb_toggled)
            self.class_selection_layout.addWidget(rb)
            self.radio_buttons.append(rb)
 
         # node radio button
@@ -164,14 +221,20 @@
     def _clear_class_layout(self):
         # clear layout
         for i in range(self.class_selection_layout.count()):
             item = self.class_selection_layout.itemAt(0)
             widget = item.widget()
             widget.hide()
             self.class_selection_layout.removeItem(item)
+    
+    def _load_code_button_clicked(self) -> None:
+        node: Node = self.sender().node
+        load_src_code(node.__class__)
+        self.load_code_button.hide()
+        self._process_node_src(node)
 
     def _update_radio_buttons_edit_status(self):
         """Draws radio buttons referring to modified objects bold."""
 
         for br in self.radio_buttons:
             if modif_codes.get(br.representing.obj) is not None:
                 # o.setStyleSheet('color: #3B9CD9;')
@@ -180,15 +243,15 @@
                 br.setFont(f)
             else:
                 # o.setStyleSheet('color: white;')
                 f = br.font()
                 f.setBold(False)
                 br.setFont(f)
 
-    def _class_rb_toggled(self, checked):
+    def _class_rb_toggled(self, checked: bool) -> None:
         if checked:
             rb: LinkedRadioButton = self.sender()
             self._update_code(rb.representing)
 
     def _edit_code_button_clicked(self):
         if not EditSrcCodeInfoDialog.dont_show_again:
             info_dialog = EditSrcCodeInfoDialog(self)
```

### Comparing `ryven-3.4.3/ryven/gui/code_editor/EditSrcCodeInfoDialog.py` & `ryven-3.5.0/ryven/gui/code_editor/EditSrcCodeInfoDialog.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/gui/code_editor/SourceCodeUpdater.py` & `ryven-3.5.0/ryven/gui/code_editor/SourceCodeUpdater.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import types
-from typing import Union
+from typing import Union, List
 
 
 def get_method_funcs(cls_def_str: str, obj):
     """
     Parses the class definition string and returns a dict with python functions under their names,
     parsed from the methods in the class definition string using the ast module.
     """
@@ -12,23 +12,23 @@
     if sys.version_info < (3, 9):
         raise Exception('src code modifications are only supported on Python >=3.9')
 
     # requires Python >= 3.9 for ast.unparse()
     import ast
 
     # extract functions
-    ast_funcs: [ast.FunctionDef] = [
+    ast_funcs: List[ast.FunctionDef] = [
         f
-        for f in ast.parse(cls_def_str).body[0].body
+        for f in ast.parse(cls_def_str).body[0].body  # type: ignore
         if type(f) == ast.FunctionDef
     ]
 
     funcs = {}
     for astf in ast_funcs:
-        d = __builtins__.copy()  # important: provide builtins when parsing the function
+        d = __builtins__.__dict__.copy()  # important: provide builtins when parsing the function
         exec(ast.unparse(astf), d)
         f = d[astf.name]
         # # add locals scope of the object to the function
         # f.__dict__ = obj.
 
         funcs[astf.name] = f
 
@@ -43,14 +43,15 @@
     @staticmethod
     def override_code(obj: object, new_class_src) -> Union[None, Exception]:
         try:
             funcs = get_method_funcs(new_class_src, obj)
             for name, f in funcs.items():  # override all methods
                 setattr(obj, name, types.MethodType(f, obj))
                 # types.MethodType() creates a method bound to obj, from the function f
+            return None
         except Exception as e:
             return e
 
 
     # below is the old implementation, for documentation purposes only; see discussion below
```

### Comparing `ryven-3.4.3/ryven/gui/code_editor/codes_storage.py` & `ryven-3.5.0/ryven/gui/code_editor/codes_storage.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,36 @@
 # statically stores source codes of nodes and their widgets
 from dataclasses import dataclass
-from typing import Type, Optional
+from typing import Type, Optional, Dict, no_type_check
 import inspect
 
 from ryvencore import Node
 from ryven.main.config import instance
 
 
 def register_node_type(n: Type[Node]):
     """
-    Inspects and stores source code of a node type.
+    Registers a node type and loads its source code directly if deferred 
+    source code loading is disabled.
     """
 
-    has_gui = hasattr(n, 'GUI')  # check if node type has custom gui
-    has_mw = has_gui and n.GUI.main_widget_class is not None
+    assert instance is not None, 'Ryven instance not initialized.'
+
+    if not instance.defer_code_loading:
+        load_src_code(n)
+    else:
+        class_codes[n] = None
 
+
+@no_type_check
+def load_src_code(n: Type[Node]):
+    # check for custom GUI and main widget
+    has_gui = hasattr(n, 'GUI')
+    has_mw = has_gui and n.GUI.main_widget_class is not None
+    
     src = inspect.getsource(n)
     mw_src = inspect.getsource(n.GUI.main_widget_class) if has_mw else None
     inp_src = {
         name: inspect.getsource(cls)
         for name, cls in n.GUI.input_widget_classes.items()
     } if has_gui else None
 
@@ -38,15 +50,15 @@
                 mod_codes[inp_cls] = inspect.getsource(inspect.getmodule(inp_cls))
 
 
 @dataclass
 class NodeTypeCodes:
     node_cls: str
     main_widget_cls: Optional[str]
-    custom_input_widget_clss: {str: str}
+    custom_input_widget_clss: Dict[str, str]
 
 
 class Inspectable:
     """
     Represents an object whose source code can be inspected.
     This is either a node or some node widget.
     Used by the code editor to store polymorphic references to
@@ -67,23 +79,23 @@
     pass
 
 
 class CustomInputWidgetInspectable(Inspectable):
     pass
 
 
-class_codes: {Type[Node]: {}} = {}
+class_codes: Dict[Type[Node], Optional[NodeTypeCodes]] = {}
 # {
 #     Type[Node]: NodeTypeCodeInfo
 # }
 
 
 #
 # below fields are only used when src code edits are enabled
 #
 
 
 # maps node- or widget classes to their full module source code
-mod_codes: {Type: str} = {}
+mod_codes: Dict[Type, str] = {}
 
 # maps node- or widget objects to their modified source code
-modif_codes: {object: str} = {}
+modif_codes: Dict[object, str] = {}
```

### Comparing `ryven-3.4.3/ryven/gui/code_editor/pygments/dracula.py` & `ryven-3.5.0/ryven/gui/code_editor/pygments/dracula.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/gui/dialogs.py` & `ryven-3.5.0/ryven/gui/dialogs.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/gui/main_console.py` & `ryven-3.5.0/ryven/gui/main_console.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Optional, List
 import code
 import re
 import os
 
 from ryven.gui.code_editor.CodeEditorWidget import CodeEditorWidget
 
 from qtpy.QtWidgets import QWidget, QLineEdit, QGridLayout, QPlainTextEdit, QLabel, QPushButton, QGroupBox, \
@@ -147,15 +148,17 @@
 
             if more:
                 # self.setprompt('> ')
                 if self.prompt_label.isHidden():
                     self.prompt_label.show()
 
                 # add leading space for next input
-                leading_space = re.match(r"\s*", self.buffer[-1]).group()
+                m = re.match(r"\s*", self.buffer[-1])
+                assert m is not None
+                leading_space = m.group()
                 self.inpedit.next_line = leading_space
 
             else:   # no more input required
                 self.prompt_label.hide()
                 self.buffer = []  # reset buffer
 
     def write(self, line: str) -> None:
@@ -163,17 +166,17 @@
         if len(line) != 1 or ord(line[0]) != 10:
             self.writeoutput(line.rstrip())  # , self.outfmt)
 
     def errorwrite(self, line: str) -> None:
         """capture stderr and print to outdisplay"""
         self.writeoutput(line, self.errfmt)
 
-    def writeoutput(self, line: str, fmt: QTextCharFormat = None) -> None:
+    def writeoutput(self, line: str, fmt: Optional[QTextCharFormat] = None) -> None:
         """prints to outdisplay"""
-        if fmt:
+        if fmt is not None:
             self.out_display.setCurrentCharFormat(fmt)
         self.out_display.appendPlainText(line.rstrip())
         self.out_display.setCurrentCharFormat(self.outfmt)
 
 
 class ConsoleInputLineEdit(QLineEdit):
     """Input line edit with a history buffer for recalling previous lines."""
@@ -184,15 +187,15 @@
         super().__init__()
 
         self.setObjectName('ConsoleInputLineEdit')
         self.code_text_edit = code_text_edit
         self.code_text_edit.returned.connect(self.code_text_edit_returned)
         self.max_hist = max_history
         self.hist_index = 0
-        self.hist_list = []
+        self.hist_list: List[str] = []
         self.next_line = ''  # can be set by console
         self.prompt_pattern = re.compile('^[>\.]')
 
     def event(self, ev: QEvent) -> bool:
 
         #   Tab: Insert 4 spaces
         #   Arrow Up/Down: select a line from the history buffer
```

### Comparing `ryven-3.4.3/ryven/gui/main_window.py` & `ryven-3.5.0/ryven/gui/main_window.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,71 @@
+from typing import Set, Dict, List, Optional, Type, Union
+
 import sys
 import os
 import os.path
 
 from qtpy.QtGui import QIcon, QKeySequence
-from qtpy.QtWidgets import QMainWindow, QFileDialog, QShortcut, QAction, QActionGroup, QMenu, QMessageBox
+from qtpy.QtWidgets import (
+    QMainWindow,
+    QFileDialog,
+    QShortcut,
+    QAction,
+    QActionGroup,
+    QMenu,
+    QMessageBox,
+    QTabWidget,
+    QDockWidget,
+)
 from ryvencore_qt import NodeGUI
+from qtpy.QtCore import Qt, QByteArray
 
 from ryven.gui.main_console import MainConsole
 from ryven.gui.flow_ui import FlowUI
 from ryven.main.config import Config
 from ryven.main.packages.nodes_package import NodesPackage
 from ryven.gui.uic.ui_main_window import Ui_MainWindow
-from ryven.main.utils import \
-    abs_path_from_package_dir, \
-    abs_path_from_ryven_dir, \
-    ryven_version
+from ryven.main.utils import (
+    abs_path_from_package_dir,
+    abs_path_from_ryven_dir,
+    ryven_version,
+)
 from ryven import import_nodes_package
 from ryven.gui.dialogs import GetTextDialog, ChooseFlowDialog
 
 # ryvencore_qt
 import ryvencore_qt as rc
 import ryvencore_qt.src.widgets as rc_GUI
 
-from ryvencore import InfoMsgs
+from ryvencore import InfoMsgs, Flow, Session as CoreSession
 
 
 class MainWindow(QMainWindow):
 
     def __init__(
-            self,
-
-            config: Config,
-            requested_packages: set = (),
-            required_packages: set = None,  # only valid when project_content is provided
-            project_content: dict = None,
-
-            parent=None,
+        self,
+        config: Config,
+        requested_packages: Optional[Set] = None,
+        required_packages: Optional[Set] = None,  # only valid when project_content is provided
+        project_content: Optional[Dict] = None,
+        parent=None,
     ):
         super().__init__(parent)
 
         self.config = config
-        self.session_gui, self.core_session = None, None
+        self.session_gui: rc.SessionGUI
+        self.core_session: CoreSession
         self.theme = config.window_theme
-        self.node_packages = {}  # {Node: str}
-        self.flow_UIs = {}
+        self.node_packages: Dict[Type[rc.Node], NodesPackage] = {}
+        self.flow_UIs: Dict[Flow, FlowUI] = {}
+        self.flow_ui_template: Optional[Dict[str, Union[QByteArray, Dict]]] = None
+        self._project_content: Optional[Dict] = None
 
         # Init Session GUI
-        
+
         self.session_gui = rc.SessionGUI(self)
         self.core_session = self.session_gui.core_session
         if self.config.verbose:
             self.core_session._info_messenger().enable(traceback=True)
         else:
             self.core_session._info_messenger().disable()
 
@@ -58,108 +73,183 @@
         self.session_gui.flow_renamed.connect(self.flow_renamed)
         self.session_gui.flow_deleted.connect(self.flow_deleted)
 
         # unused; default flow theme etc. are defined by Config
         # self.session_gui.design.load_from_config(abs_path_from_package_dir('gui/styling/design_config.json'))
 
         self.session_gui.design.set_flow_theme(name=self.config.flow_theme)
-        self.session_gui.design.set_performance_mode(self.config.performance_mode)
         self.session_gui.design.set_animations_enabled(self.config.animations)
 
         # Assemble Window UI
-        
+
         self.setup_ui()
 
-        self.flow_view_theme_actions = []
+        self.flow_view_theme_actions: List[QAction] = []
         self.setup_menu_actions()
 
         self.setWindowTitle(self.config.window_title)
         self.setWindowIcon(QIcon(abs_path_from_package_dir('resources/pics/Ryven_icon.png')))
         self.ui.flows_tab_widget.removeTab(0)  # remove placeholder tab
 
         # Configure window-wide Shortcuts
-        
+
         save_shortcut = QShortcut(QKeySequence.Save, self)
         save_shortcut.activated.connect(self.on_save_project_triggered)
         import_nodes_shortcut = QShortcut(QKeySequence('Ctrl+i'), self)
         import_nodes_shortcut.activated.connect(self.on_import_nodes_triggered)
 
         # Setup Main Console
-
+        assert MainConsole.instance is not None, 'MainConsole not initialized'
         MainConsole.instance.session = self.session_gui
         MainConsole.instance.reset_interpreter()
 
         # very dirty hack to access nodes from the console
         def console_ref_monkeypatch(self):
             MainConsole.instance.add_obj_context(self.node)
+
         NodeGUI.console_ref_monkeypatch = console_ref_monkeypatch
         old_ac_init = NodeGUI._init_default_actions
-        NodeGUI._init_default_actions = lambda self: {
+        NodeGUI._init_default_actions = lambda self: {  # type: ignore
             **old_ac_init(self),
-            'console ref': {'method': self.console_ref_monkeypatch}
+            'console ref': {'method': self.console_ref_monkeypatch},
         }
 
+        if config.verbose and MainConsole.instance:
+            MainConsole.instance.writeoutput(
+                '''Editor is in Verbose mode. 
+All output will be printed in the terminal, not the editor console.
+The editor console can still be used for commands.
+              '''
+            )
+            # hide the console in verbose mode
+            self.ui.consoleDock.hide()
+
         # Setup ryvencore Session and load project
 
         self.import_nodes(path=abs_path_from_package_dir('main/packages/built_in/'))
 
         # Requested packages take precedence over other packages
         print('importing requested packages...')
+        if requested_packages is None:
+            requested_packages = set()
         self.import_packages(requested_packages)
         if project_content is not None:
+            assert required_packages is not None, 'required_packages must be provided when loading a project'
+            self._project_content = project_content
             print('importing required packages...')
             self.import_packages(required_packages)
             print('loading project...')
             self.core_session.load(project_content)
+            # load the flow_ui_template if it exists
+            self.set_flow_ui_template(project_content.get('flow_ui_template'))
+            # After everything has loaded, load previous UI geometry and state
+            self.load_qt_window(project_content)
+            for flow_ui in self.flow_UIs.values():
+                self.load_flow_ui(flow_ui)
             print('done')
         else:
             self.core_session.create_flow(title='hello world')
 
         self.resize(1500, 800)  # FIXME: this renders the --geometry argument useless, no?
         # self.showMaximized()
-
+    
+    def closeEvent(self, event):
+        for flow_ui in self.flow_UIs.values():
+            flow_ui.unload()
+        
     def print_info(self):
         print('''
 CONTROLS
     nodes dialog: right mouse in scene
     place nodes: drag and drop from left
         or hit enter in scene dialog
     select: left mouse
     pan / navigating scene: right mouse
     save: ctrl+s
     import: ctrl+i
         ''')
 
     # UI
 
-    def setup_ui(self):
+    def setup_ui(self) -> None:
         self.ui = Ui_MainWindow()
         self.ui.setupUi(self)
         self.ui.statusBar.hide()
 
+        def unset_flow_template():
+            self.set_flow_ui_template(None)
+
+        def set_flow_template():
+            flow_ui = self.flow_UIs.get(self.get_current_flow())
+            if not flow_ui:
+                return
+            template = {
+                'geometry': flow_ui.saveGeometry().toHex().data().decode(),
+                'state': flow_ui.saveState().toHex().data().decode(),
+                'view': flow_ui.flow_view.save_state()
+            }
+            self.set_flow_ui_template(template)
+
+        self.flow_ui_template_menu = QMenu()
+        self.flow_ui_template_menu.setTitle('Flow Template')
+
+        restore_default = QAction('Restore Default', self)
+        restore_default.triggered.connect(unset_flow_template)
+        save_current = QAction('Save Current', self)
+        save_current.triggered.connect(set_flow_template)
+
+        self.flow_ui_template_menu.addAction(save_current)
+        self.flow_ui_template_menu.addAction(restore_default)
+
+        # set tabs to be on top
+        self.setTabPosition(Qt.AllDockWidgetAreas, QTabWidget.North)
+
         # main console
         if MainConsole.instance is not None:
-            self.ui.main_vertical_splitter.addWidget(MainConsole.instance)
+            self.ui.consoleDock.setWidget(MainConsole.instance)
             self.ui.console_placeholder_widget.setParent(None)
         # self.ui.right_vertical_splitter.setSizes([600, 0])
 
         # splitter sizes
         # self.ui.left_vertical_splitter.setSizes([350, 350])
         self.ui.main_vertical_splitter.setSizes([700, 0])
 
         self.flows_list_widget = rc_GUI.FlowsList(self.session_gui)
-        self.ui.flows_groupBox.layout().addWidget(self.flows_list_widget)
+        self.ui.flows_dock.setWidget(self.flows_list_widget)
 
-        self.nodes_list_widget = rc_GUI.NodeListWidget(self.session_gui)
-        self.ui.nodes_groupBox.layout().addWidget(self.nodes_list_widget)
+        self.nodes_list_widget = rc_GUI.NodeListWidget(self.session_gui, True)
+        self.ui.nodes_dock.setWidget(self.nodes_list_widget)
 
-        self.ui.main_horizontal_splitter.setSizes([120, 800-120])
+        self.ui.main_horizontal_splitter.setSizes([120, 800 - 120])
 
+        # add widget actions to menu
+        all_dock_widgets: list[QDockWidget] = [d for d in self.findChildren(QDockWidget)]
+        open_all_docks = QAction('Open All', self)
+        open_all_docks.triggered.connect(self.open_docks)
+        close_all_docks = QAction('Close All Tabs', self)
+        close_all_docks.triggered.connect(self.close_docks)
+        self.ui.menuDocks.addActions([open_all_docks, close_all_docks])
+        self.ui.menuDocks.addActions([w.toggleViewAction() for w in all_dock_widgets])
+        # tabify all left tabs at a fresh project
+        left_widgets = [
+            d for d in all_dock_widgets if self.dockWidgetArea(d) == Qt.LeftDockWidgetArea
+        ]
+        for i in range(1, len(left_widgets)):
+            self.tabifyDockWidget(left_widgets[i - 1], left_widgets[i])
+
+    def open_docks(self):
+        for dock in self.findChildren(QDockWidget):
+            dock.show()
+    
+    def close_docks(self):
+        for dock in self.findChildren(QDockWidget):
+            if not dock.isFloating():
+                dock.close()
+            
     def setup_menu_actions(self):
-
         # flow designs
         light_themes_menu = QMenu('light')
         for d in self.session_gui.design.flow_themes:
             design_action = QAction(d.name, self)
             if d.type_ == 'dark':
                 self.ui.menuFlow_Design_Style.addAction(design_action)
             else:
@@ -176,37 +266,44 @@
         # TODO: rename occurences of "Script" to "Flow" in the UI
         self.ui.actionNew_Flow.triggered.connect(self.on_new_flow_triggered)
         self.ui.actionRename_Flow.triggered.connect(self.on_rename_flow_triggered)
         self.ui.actionDelete_Flow.triggered.connect(self.on_delete_flow_triggered)
         self.ui.actionEnableInfoMessages.triggered.connect(self.on_enable_info_msgs_triggered)
         self.ui.actionDisableInfoMessages.triggered.connect(self.on_disable_info_msgs_triggered)
         self.ui.actionSave_Pic_Viewport.triggered.connect(self.on_save_scene_pic_viewport_triggered)
-        self.ui.actionSave_Pic_Whole_Scene_scaled.triggered.connect(self.on_save_scene_pic_whole_triggered)
+        self.ui.actionSave_Pic_Whole_Scene_scaled.triggered.connect(
+            self.on_save_scene_pic_whole_triggered
+        )
 
         # performance mode
+        self.session_gui.design.performance_mode_changed.connect(
+            self.on_performance_mode_value_changed
+        )
+
         self.ac_perf_mode_fast = QAction('Fast', self)
         self.ac_perf_mode_fast.setCheckable(True)
 
         self.ac_perf_mode_pretty = QAction('Pretty', self)
         self.ac_perf_mode_pretty.setCheckable(True)
 
         perf_mode_ag = QActionGroup(self)
         perf_mode_ag.addAction(self.ac_perf_mode_fast)
         perf_mode_ag.addAction(self.ac_perf_mode_pretty)
 
-        self.ac_perf_mode_fast.setChecked(self.session_gui.design.performance_mode == 'fast')
-        self.ac_perf_mode_pretty.setChecked(self.session_gui.design.performance_mode == 'pretty')
+        self.ac_perf_mode_fast.setChecked(self.config.performance_mode == 'fast')
+        self.ac_perf_mode_pretty.setChecked(self.config.performance_mode == 'pretty')
 
         perf_mode_ag.triggered.connect(self.on_performance_mode_changed)
 
         perf_menu = QMenu('Performance Mode', self)
         perf_menu.addAction(self.ac_perf_mode_fast)
         perf_menu.addAction(self.ac_perf_mode_pretty)
 
         self.ui.menuView.addMenu(perf_menu)
+        self.session_gui.design.set_performance_mode(self.config.performance_mode)
 
         # animations
         self.ac_anims_active = QAction('Enabled', self)
         self.ac_anims_active.setCheckable(True)
 
         self.ac_anims_inactive = QAction('Disabled', self)
         self.ac_anims_inactive.setCheckable(True)
@@ -232,23 +329,46 @@
             f = open(abs_path_from_package_dir('resources/stylesheets/' + ss + '.txt'))
             ss_content = f.read()
             f.close()
         finally:
             self.session_gui.set_stylesheet(ss_content)
             self.setStyleSheet(ss_content)
 
+    # necessary for proper flow view loading
+    def showEvent(self, event):
+        for flow_ui in self.flow_UIs.values():
+            flow_ui.flow_view.reload()
+        
+    # events
+    
+    def on_performance_mode_value_changed(self, mode: str):
+        if mode == 'fast':
+            self.setDockOptions(self.dockOptions() & ~QMainWindow.AnimatedDocks)
+        else:
+            self.setDockOptions(self.dockOptions() | QMainWindow.AnimatedDocks)
+
     # slots
 
     def on_import_nodes_triggered(self):
-        file_path = QFileDialog.getOpenFileName(self, 'select nodes file', abs_path_from_ryven_dir('nodes'), 'Python File (*.py)')[0]
+        file_path = QFileDialog.getOpenFileName(
+            self,
+            'select nodes file',
+            abs_path_from_ryven_dir('nodes'),
+            'Python File (*.py)',
+        )[0]
         if file_path != '':
             self.import_nodes(path=os.path.dirname(file_path))
 
     def on_import_example_nodes_triggered(self):
-        file_path = QFileDialog.getOpenFileName(self, 'select nodes file', abs_path_from_package_dir('example_nodes'), 'Python File (*.py)')[0]
+        file_path = QFileDialog.getOpenFileName(
+            self,
+            'select nodes file',
+            abs_path_from_package_dir('example_nodes'),
+            'Python File (*.py)',
+        )[0]
         if file_path != '':
             self.import_nodes(path=os.path.dirname(file_path))
 
     def on_performance_mode_changed(self, action):
         if action == self.ac_perf_mode_fast:
             self.session_gui.design.set_performance_mode('fast')
         else:
@@ -279,26 +399,30 @@
         flow = self.ui.flows_tab_widget.currentWidget().flow
         view = self.session_gui.flow_views[flow]
         img = view.get_viewport_img()
         img.save(file_path)
 
     def on_save_scene_pic_whole_triggered(self):
         """Saves a picture of the whole currently visible scene."""
-        if len(self.session_gui.flows) == 0:
+        if len(self.core_session.flows) == 0:
             return
 
         file_path = QFileDialog.getSaveFileName(self, 'select file', '', 'PNG(*.png)')[0]
         flow = self.ui.flows_tab_widget.currentWidget().flow
         view = self.session_gui.flow_views[flow]
         img = view.get_whole_scene_img()
         img.save(file_path)
 
     def on_save_project_triggered(self):
-        file_name = QFileDialog.getSaveFileName(self, 'select location and give file name',
-                                                abs_path_from_ryven_dir('saves'), 'JSON(*.json)')[0]
+        file_name = QFileDialog.getSaveFileName(
+            self,
+            'select location and give file name',
+            abs_path_from_ryven_dir('saves'),
+            'JSON(*.json)',
+        )[0]
         if not file_name.endswith('.json'):
             file_name += '.json'
 
         if file_name != '':
             self.save_project(file_name)
 
     def on_new_flow_triggered(self):
@@ -316,108 +440,187 @@
 
         if self.core_session.flow_title_valid(new_title):
             self.core_session.rename_flow(flow, new_title)
 
     def on_delete_flow_triggered(self):
         flow = ChooseFlowDialog('choose flow', self.core_session.flows, self).get_flow()
 
-        msg_box = QMessageBox(QMessageBox.Warning, 'sure about deleting flow?',
-                              'You are about to delete a flow. This cannot be undone, all content will be gone. '
-                              'Do you want to continue?', QMessageBox.Cancel | QMessageBox.Yes, self)
+        msg_box = QMessageBox(
+            QMessageBox.Warning,
+            'sure about deleting flow?',
+            'You are about to delete a flow. This cannot be undone, all content will be gone. '
+            'Do you want to continue?',
+            QMessageBox.Cancel | QMessageBox.Yes,
+            self,
+        )
         msg_box.setDefaultButton(QMessageBox.Cancel)
         ret = msg_box.exec_()
         if ret != QMessageBox.Yes:
             return
 
         self.core_session.delete_flow(flow)
 
     # session
 
-    def flow_created(self, flow, flow_view):
+    def flow_created(self, flow: Flow, flow_view):
         flow_widget = FlowUI(self, flow, flow_view)
         self.flow_UIs[flow] = flow_widget
         self.ui.flows_tab_widget.addTab(flow_widget, flow.title)
+        flow_view.menu().addMenu(self.flow_ui_template_menu)
+        if self.flow_ui_template:
+            flow_widget.load_directly(self.flow_ui_template)
+
         self.focus_on_flow(flow)
 
     def flow_renamed(self, flow):
         self.ui.flows_tab_widget.setTabText(
-            self.session_gui.core_session.flows.index(flow),
-            flow.title
+            self.session_gui.core_session.flows.index(flow), flow.title
         )
 
     def flow_deleted(self, flow):
         self.ui.flows_tab_widget.removeTab(self.ui.flows_tab_widget.indexOf(self.flow_UIs[flow]))
+        self.flow_UIs[flow].unload()
         del self.flow_UIs[flow]
 
     def get_current_flow(self):
         return self.core_session.flows[self.ui.flows_tab_widget.currentIndex()]
 
     def focus_on_flow(self, flow):
         self.ui.flows_tab_widget.setCurrentWidget(self.flow_UIs[flow])
 
-    def import_packages(self, packages_list: [NodesPackage]):
+    def import_packages(self, packages_list: List[NodesPackage]):
         for p in packages_list:
             self.import_nodes(p)
 
-    def import_nodes(self, package: NodesPackage = None, path: str = None):
-
+    def import_nodes(self, package: Optional[NodesPackage] = None, path: Optional[str] = None):
         if package is not None:
             p = package
         else:
+            assert path is not None, 'either package or path must be provided'
             p = NodesPackage(path)
 
         if p in self.node_packages.values():
             # never import package twice!
             # different packages with same name are forbidden
             print('package with this name already exists')
             return
 
         try:
             nodes, data_types = import_nodes_package(p)
         except ModuleNotFoundError as e:
-            msg_box = QMessageBox(QMessageBox.Warning, 'Missing Python module', str(e), QMessageBox.Ok, self)
+            msg_box = QMessageBox(
+                QMessageBox.Warning,
+                'Missing Python module',
+                str(e),
+                QMessageBox.Ok,
+                self,
+            )
             msg_box.exec_()
-            sys.exit(e)
+            sys.exit(str(e))
 
         self.core_session.register_data_types(data_types)
         self.core_session.register_node_types(nodes)
 
         for n in nodes:
             self.node_packages[n] = p
 
         self.nodes_list_widget.update_list(self.core_session.nodes)
+        self.nodes_list_widget.make_pack_hier()
+
+    # should be dict[str, str] | dict[str, QByteArray | dict] | None in 3.9+
+    def set_flow_ui_template(self, template):
+        if template is None:
+            self.flow_ui_template = None
+            return
+        save = (
+            lambda key: template[key]
+            if type(template[key]) is QByteArray
+            else bytes.fromhex(template[key])
+        )
+        self.flow_ui_template = {
+            'geometry': save('geometry'), 
+            'state': save('state'),
+            'view': template['view']
+        }
+
+    def load_qt_window(self, project_dict):
+        """
+        Loads the main windows previous geometry and state, if they were saved.
+        """
+        if 'geometry' in project_dict:
+            self.restoreGeometry(bytes.fromhex(project_dict['geometry']))
+        if 'state' in project_dict:
+            self.restoreState(bytes.fromhex(project_dict['state']))
+
+    def load_flow_ui(self, flow_ui: FlowUI):
+        """
+        Loads a flow uis previous geometry and state based on the previous flow id.
+        """
+        if self._project_content is None:
+            return
+        try:
+            flow_ui.load(self._project_content['flow_uis'])
+        except Exception as e:
+            # print(f'Could not load previous UI state for flow with previous id: {flow_ui.flow.prev_global_id}')
+            pass
 
-    def save_project(self, file_name):
+    def save_project(self, file_name: str) -> None:
         import json
 
         file = None
         try:
             if os.path.exists(file_name):
                 os.remove(file_name)
             file = open(file_name, 'w')
         except FileNotFoundError:
             InfoMsgs.write('couldn\'t open file')
             return
 
-        general_project_info_dict = {'type': 'Ryven project file', 'ryven version': str(ryven_version())}
+        general_project_info_dict = {
+            'type': 'Ryven project file',
+            'ryven version': str(ryven_version()),
+        }
 
         flows_data = self.core_session.serialize()
 
         required_packages = set()
         for node in self.core_session.all_node_objects():
-            if node.__class__ not in self.node_packages.keys() or \
-                    self.node_packages[node.__class__] is None or \
-                    self.node_packages[node.__class__].name == 'built_in':
+            if (
+                node.__class__ not in self.node_packages.keys()
+                or self.node_packages[node.__class__] is None
+                or self.node_packages[node.__class__].name == 'built_in'
+            ):
                 continue
-            required_packages.add(
-                self.node_packages[node.__class__]
-            )
+            required_packages.add(self.node_packages[node.__class__])
+
+        # Serialization of the main window
+        geometry = self.saveGeometry().toHex().data().decode()
+        state = self.saveState().toHex().data().decode()
+
+        # Serialization of the flow views
+        # should be dict[str, dict[str, str | dict]] in 3.9+
+        flow_uis_ser: Dict[str, Dict] = {}
+        for flow, flow_ui in self.flow_UIs.items():
+            flow_uis_ser[str(flow.global_id)] = flow_ui.save_state()
+
+        whole_project_dict = {
+            'general info': general_project_info_dict,
+            'required packages': [p.config_data() for p in required_packages],
+            **flows_data,
+            'geometry': geometry,
+            'state': state,
+            'flow_uis': flow_uis_ser,
+        }
 
-        whole_project_dict = {'general info': general_project_info_dict,
-                              'required packages': [p.config_data() for p in required_packages],
-                              **flows_data}
+        # flow ui template
+        if self.flow_ui_template:
+            whole_project_dict['flow_ui_template'] = {
+                'geometry': QByteArray(self.flow_ui_template['geometry']).toHex().data().decode(),  # type: ignore
+                'state': QByteArray(self.flow_ui_template['state']).toHex().data().decode(),  # type: ignore
+                'view': self.flow_ui_template['view']
+            }
 
         data = json.dumps(whole_project_dict, indent=4)
         InfoMsgs.write(data)
 
         file.write(data)
         file.close()
```

### Comparing `ryven-3.4.3/ryven/gui/startup_dialog/StartupDialog.py` & `ryven-3.5.0/ryven/gui/startup_dialog/StartupDialog.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,42 @@
 import os
 import pathlib
 from typing import Optional
 
 from qtpy.QtWidgets import (
-    QDialog, QVBoxLayout, QHBoxLayout, QPushButton, QTextEdit, QFileDialog,
-    QRadioButton, QButtonGroup, QLabel, QFormLayout, QComboBox, QDialogButtonBox,
-    QCheckBox, QListWidget, QListWidgetItem, QMessageBox,
-    QStyleOptionFrame, QStyle, QLineEdit)
+    QDialog,
+    QVBoxLayout,
+    QHBoxLayout,
+    QPushButton,
+    QTextEdit,
+    QFileDialog,
+    QRadioButton,
+    QButtonGroup,
+    QLabel,
+    QFormLayout,
+    QComboBox,
+    QDialogButtonBox,
+    QCheckBox,
+    QListWidget,
+    QListWidgetItem,
+    QMessageBox,
+    QStyleOptionFrame,
+    QStyle,
+    QLineEdit,
+)
 from qtpy.QtCore import Qt, QSize
 from qtpy.QtGui import QIcon, QPainter
 
 from ryven.main.args_parser import unparse_sys_args
 from ryven.main.config import Config
 from ryven.main.utils import (
-    abs_path_from_package_dir, abs_path_from_ryven_dir, ryven_dir_path)
+    abs_path_from_package_dir,
+    abs_path_from_ryven_dir,
+    ryven_dir_path,
+)
 from ryven.main.packages.nodes_package import process_nodes_packages
 from ryven.gui.styling.window_theme import apply_stylesheet
 
 
 LBL_CREATE_PROJECT = '<create new project>'
 LBL_DEFAULT_FLOW_THEME = '<default>'
 
@@ -26,14 +45,15 @@
     """A QLabel with ellipsis, if the text is too long to be fully displayed.
 
     See:
         https://stackoverflow.com/questions/68092087/one-line-elideable-qlabel#answer-68092991
 
     Copyright (C) 2021  https://github.com/MaurizioB/
     """
+
     _elideMode = Qt.ElideMiddle
 
     def setText(self, label, *args, **kwargs):
         """Sets text and tooltip."""
         s = str(label)
         super().setText(s, *args, **kwargs)
         self.setToolTip(s)
@@ -47,39 +67,41 @@
             self.updateGeometry()
 
     def minimumSizeHint(self):
         return self.sizeHint()
 
     def sizeHint(self):
         hint = self.fontMetrics().boundingRect(self.text()).size()
-        l, t, r, b = self.getContentsMargins()
+        c_margins = self.contentsMargins()
+        l, t, r, b = c_margins.left(), c_margins.top(), c_margins.right(), c_margins.bottom()
         margin = self.margin() * 2
         return QSize(
             min(100, hint.width()) + l + r + margin,
-            min(self.fontMetrics().height(), hint.height()) + t + b + margin
+            min(self.fontMetrics().height(), hint.height()) + t + b + margin,
         )
 
     def paintEvent(self, event):
         qp = QPainter(self)
         opt = QStyleOptionFrame()
         self.initStyleOption(opt)
-        self.style().drawControl(
-            QStyle.CE_ShapedFrame, opt, qp, self)
-        l, t, r, b = self.getContentsMargins()
+        self.style().drawControl(QStyle.CE_ShapedFrame, opt, qp, self)
+        c_margins = self.contentsMargins()
+        l, t, r, b = c_margins.left(), c_margins.top(), c_margins.right(), c_margins.bottom()
         margin = self.margin()
         try:
             # since Qt >= 5.11
             m = self.fontMetrics().horizontalAdvance('x') / 2 - margin
         except:
             m = self.fontMetrics().width('x') / 2 - margin
-        r = self.contentsRect().adjusted(
-            margin + m,  margin, -(margin + m), -margin)
-        qp.drawText(r, self.alignment(),
-            self.fontMetrics().elidedText(
-                self.text(), self.elideMode(), r.width()))
+        r = self.contentsRect().adjusted(margin + m, margin, -(margin + m), -margin)
+        qp.drawText(
+            r,
+            self.alignment(),
+            self.fontMetrics().elidedText(self.text(), self.elideMode(), r.width()),
+        )
 
 
 class ShowCommandDialog(QDialog):
     def __init__(self, command, config, parent=None):
         super().__init__(parent)
 
         layout = QVBoxLayout()
@@ -183,95 +205,118 @@
         # The form with the configuration options
         fbox = QFormLayout()
 
         # Project
         project_label = QLabel('Project:')
 
         project_layout = QVBoxLayout()
+
         self.project_name = ElideLabel()
         if self.conf.project is not None:
             self.project_name.setText(str(config.project))
         else:
             self.project_name.setText(LBL_CREATE_PROJECT)
         project_layout.addWidget(self.project_name)
 
         project_buttons_widget = QDialogButtonBox()
+
         self.create_project_button = QPushButton('New')
         self.create_project_button.setToolTip('Create a new project')
         self.create_project_button.setDefault(True)
         self.create_project_button.clicked.connect(self.on_create_project_button_clicked)
         project_buttons_widget.addButton(self.create_project_button, QDialogButtonBox.ActionRole)
+
         load_project_button = QPushButton('Load')
         load_project_button.setToolTip('Load an existing project')
         load_project_button.clicked.connect(self.on_load_project_button_clicked)
         project_buttons_widget.addButton(load_project_button, QDialogButtonBox.ActionRole)
+
         load_example_project_button = QPushButton('Example')
         load_example_project_button.setToolTip('Load a Ryven example')
         load_example_project_button.clicked.connect(self.on_load_example_project_button_clicked)
         project_buttons_widget.addButton(load_example_project_button, QDialogButtonBox.ActionRole)
+
         project_layout.addWidget(project_buttons_widget)
 
         fbox.addRow(project_label, project_layout)
 
         # Nodes packages
         packages_label = QLabel('Nodes packages:')
 
         packages_layout = QVBoxLayout()
         packages_sublayout = QHBoxLayout()
 
         # FIXME: The three following columns should have half their default size!
         # ???: How is that achieved?
         packages_imported_layout = QVBoxLayout()
         label_imported = QLabel('Imported:')
-        label_imported.setToolTip('Nodes packages which are required by the project and are found')
+        label_imported.setToolTip(
+            'Nodes packages which are required by the project and are found'
+        )
         label_imported.setAlignment(Qt.AlignCenter)
         packages_imported_layout.addWidget(label_imported)
         self.imported_list_widget = QListWidget()
         packages_imported_layout.addWidget(self.imported_list_widget)
         packages_sublayout.addLayout(packages_imported_layout)
 
         packages_missing_layout = QVBoxLayout()
         label_missing = QLabel('Missing:')
-        label_missing.setToolTip('Nodes packages which are required by the project but could not be found')
+        label_missing.setToolTip(
+            'Nodes packages which are required by the project but could not be found'
+        )
         label_missing.setAlignment(Qt.AlignCenter)
         packages_missing_layout.addWidget(label_missing)
         self.missing_list_widget = QListWidget()
         packages_missing_layout.addWidget(self.missing_list_widget)
         packages_sublayout.addLayout(packages_missing_layout)
 
         packages_manually_layout = QVBoxLayout()
         label_manually = QLabel('Manually imported:')
-        label_manually.setToolTip('Nodes packages which are manually imported\nThey will override the packages required by the project\nAdditional packages can be imported later …')
+        label_manually.setToolTip(
+            '''Nodes packages which are manually imported
+            They will override the packages required by the project
+            Additional packages can be imported later.'''
+        )
         label_manually.setAlignment(Qt.AlignCenter)
         packages_manually_layout.addWidget(label_manually)
+
         self.manually_list_widget = QListWidget()
         self.manually_list_widget.setSelectionMode(QListWidget.MultiSelection)
         self.manually_list_widget.itemSelectionChanged.connect(self.on_packages_manually_selection)
         packages_manually_layout.addWidget(self.manually_list_widget)
         packages_sublayout.addLayout(packages_manually_layout)
 
         packages_layout.addLayout(packages_sublayout)
 
         packages_buttons_widget = QDialogButtonBox()
         self.autodiscover_packages_button = QPushButton('Find')
-        self.autodiscover_packages_button.setToolTip('Automatically find and import missing packages')
+        self.autodiscover_packages_button.setToolTip(
+            'Automatically find and import missing packages'
+        )
         self.autodiscover_packages_button.clicked.connect(self.on_autodiscover_package_clicked)
         packages_buttons_widget.addButton(self.autodiscover_packages_button, QDialogButtonBox.ActionRole)
         self.autodiscover_packages_button.setEnabled(False)
+        
         import_package_button = QPushButton('Import')
         import_package_button.setToolTip('Manually load a nodes package')
         import_package_button.clicked.connect(self.on_import_package_clicked)
         packages_buttons_widget.addButton(import_package_button, QDialogButtonBox.ActionRole)
+
         self.remove_packages_button = QPushButton('Remove')
-        self.remove_packages_button.setToolTip('Remove manually imported nodes packages')
+        self.remove_packages_button.setToolTip(
+            'Remove manually imported nodes packages'
+        )
         self.remove_packages_button.clicked.connect(self.on_remove_packages_clicked)
         self.remove_packages_button.setEnabled(False)
         packages_buttons_widget.addButton(self.remove_packages_button, QDialogButtonBox.ActionRole)
+
         self.clear_packages_button = QPushButton('Clear')
-        self.clear_packages_button.setToolTip('Clear the list of manually imported nodes packages ')
+        self.clear_packages_button.setToolTip(
+            'Clear the list of manually imported nodes packages '
+        )
         self.clear_packages_button.clicked.connect(self.on_clear_packages_clicked)
         self.clear_packages_button.setEnabled(False)
         packages_buttons_widget.addButton(self.clear_packages_button, QDialogButtonBox.ActionRole)
         packages_layout.addWidget(packages_buttons_widget)
 
         fbox.addRow(packages_label, packages_layout)
 
@@ -288,16 +333,20 @@
             windowtheme_layout.addWidget(rb)
         windowtheme_button_group.buttonToggled.connect(self.on_window_theme_toggled)
         fbox.addRow(windowtheme_label, windowtheme_layout)
 
         # Flow theme
         flowtheme_label = QLabel('Flow theme:')
         flowtheme_widget = QComboBox()
-        flowtheme_widget.setToolTip('Select the theme of the flow display\nCan also be changed later …')
-        flowtheme_widget.addItems([LBL_DEFAULT_FLOW_THEME] + list(self.conf.get_available_flow_themes()))
+        flowtheme_widget.setToolTip(
+            'Select the theme of the flow display\nCan also be changed later …'
+        )
+        flowtheme_widget.addItems(
+            [LBL_DEFAULT_FLOW_THEME] + list(self.conf.get_available_flow_themes())
+        )
         flowtheme_widget.insertSeparator(1)
         flowtheme_widget.currentTextChanged.connect(self.on_flow_theme_selected)
         fbox.addRow(flowtheme_label, flowtheme_widget)
 
         # Performance mode
         performance_label = QLabel('Performance mode:')
         performance_layout = QHBoxLayout()
@@ -334,22 +383,36 @@
             all output goes to the terminal from which Ryven was
             launched. Also, it causes lots of debug info to be 
             printed.'''
         )
         verbose_output_cb.toggled.connect(self.on_verbose_toggled)
         fbox.addRow(verbose_output_label, verbose_output_cb)
 
+        # Defer source code loading
+        defer_code_label = QLabel('Defer SCL:')
+        defer_code_cb = QCheckBox('Enable defer source code loading')
+        defer_code_cb.setToolTip(
+            f'''Choose whether source code will be loaded on package
+            import or when the user manually attempt to inspect the
+            source on a specific node. Helps reduce package import
+            time.'''
+        )
+        defer_code_cb.toggled.connect(self.on_defer_toggled)
+        fbox.addRow(defer_code_label, defer_code_cb)
+        
         layout.addLayout(fbox)
 
         # Buttons
         buttons_layout = QHBoxLayout()
         gen_config_button = QPushButton('generate / save config')
         gen_config_button.clicked.connect(self.gen_config_clicked)
         buttons_layout.addWidget(gen_config_button)
-        buttons = QDialogButtonBox(QDialogButtonBox.Ok | QDialogButtonBox.Cancel)   # this crashes with Python 3.11
+        buttons = QDialogButtonBox(
+            QDialogButtonBox.Ok | QDialogButtonBox.Cancel
+        )  # this crashes with Python 3.11
         self.ok_button = buttons.button(QDialogButtonBox.Ok)
         buttons.accepted.connect(self.accept)
         buttons.rejected.connect(self.reject)
         buttons_layout.addWidget(buttons)
         layout.addLayout(buttons_layout)
 
         self.setLayout(layout)
@@ -384,17 +447,22 @@
         else:
             idx = flowtheme_widget.findText(LBL_DEFAULT_FLOW_THEME)
         flowtheme_widget.setCurrentIndex(idx)
 
         # Set verbose output
         verbose_output_cb.setChecked(self.conf.verbose)
 
+        # Set defer code loading
+        defer_code_cb.setChecked(self.conf.defer_code_loading)
+        
         # Set window title and icon
         self.setWindowTitle('Ryven')
-        self.setWindowIcon(QIcon(abs_path_from_package_dir('resources/pics/Ryven_icon.png')))
+        self.setWindowIcon(
+            QIcon(abs_path_from_package_dir('resources/pics/Ryven_icon.png'))
+        )
 
     #
     # Call-back methods
     #
 
     # Project
 
@@ -411,16 +479,16 @@
         if project_path is not None:
             self.load_project(project_path)
 
     def on_load_example_project_button_clicked(self):
         """Call-back method, whenever the 'Example' button was clicked."""
         # Load an example project, starting in the ryven's example directory
         project_path = self.get_project(
-            abs_path_from_package_dir('examples_projects'),
-            title='Select Ryven example')
+            abs_path_from_package_dir('example_projects'), title='Select Ryven example'
+        )
 
         if project_path is not None:
             self.load_project(project_path)
 
     # Nodes packages
 
     def on_packages_manually_selection(self):
@@ -441,17 +509,19 @@
         self.auto_discover(pathlib.Path(abs_path_from_package_dir('example_nodes')))
         self.update_packages_lists()
 
     def on_import_package_clicked(self):
         """Call-back method, whenever the 'Import' button was clicked."""
         # Import a nodes package, starting in the user's ryven directory
         file_name = QFileDialog.getOpenFileName(
-            self, 'Select',
+            self,
+            'Select',
             abs_path_from_ryven_dir('packages'),
-            'ryven nodes package (nodes.py)')[0]
+            'ryven nodes package (nodes.py)',
+        )[0]
 
         if file_name:
             file_path = pathlib.Path(file_name)
             if file_path.exists():
                 self.conf.nodes.add(file_path.parent)
                 self.update_packages_lists()
 
@@ -521,19 +591,25 @@
     # Verbose output
 
     def on_verbose_toggled(self, check):
         """Call-back method, whenever the verbose checkbox was toggled."""
         # "Apply" the verbose option
         self.conf.verbose = check
 
+    # Defer Source Code Loading
+    def on_defer_toggled(self, check):
+        """Call-back method, whenever the defer source code loading checkbox was toggled"""
+        self.conf.defer_code_loading = check
     #
     # Helper/Working methods
     #
 
-    def get_project(self, base_dir: str, title='Select project file') -> Optional[pathlib.Path]:
+    def get_project(
+        self, base_dir: str, title='Select project file'
+    ) -> Optional[pathlib.Path]:
         """Get a project file from the user.
 
         Parameters
         ----------
         base_dir : str|pathlib.Path
             The initial directory shown in the file dialog.
         title : str, optional
@@ -544,17 +620,16 @@
         -------
         file_path : pathlib.Path|None
             The path of the selected file.
 
         """
         # Get the file from the user
         file_name = QFileDialog.getOpenFileName(
-            self, title,
-            str(base_dir), 'JSON (*.json)'
-            )[0]
+            self, title, str(base_dir), 'JSON (*.json)'
+        )[0]
 
         if file_name:
             file_path = pathlib.Path(file_name)
             if file_path.exists():
                 return file_path
 
         return None
@@ -583,15 +658,15 @@
         if project_path is None:
             self.conf.project = None
             self.project_name.setText(LBL_CREATE_PROJECT)
             self.create_project_button.setEnabled(False)
 
         else:
             self.conf.project = project_path
-            self.project_name.setText(project_path)
+            self.project_name.setText(str(project_path))
             self.create_project_button.setEnabled(True)
 
             required_nodes, missing_nodes, _ = process_nodes_packages(project_path)
             item_flags = ~Qt.ItemIsSelectable & ~Qt.ItemIsEditable
             for node in sorted(required_nodes, key=lambda n: n.name):
                 node_item = QListWidgetItem(node.name)
                 node_item.setToolTip(node.directory)
@@ -617,19 +692,20 @@
         -------
         None.
 
         """
         # List of packages which are missing
         missing_packages = [
             self.missing_list_widget.item(i).text()
-            for i in range(self.missing_list_widget.count())]
+            for i in range(self.missing_list_widget.count())
+        ]
 
         # Search for missing packages under `package_dir`
-        for top, dirs, files in os.walk(packages_dir):
-            path = pathlib.Path(top)
+        for entry in filter(lambda e: e.is_dir(), os.scandir(packages_dir)):
+            path = pathlib.Path(entry.path)
             if path.name in missing_packages:
                 node_path = path.joinpath('nodes.py')
                 if node_path.exists():
                     self.conf.nodes.add(path)
 
     def update_packages_lists(self):
         """Update the packages lists and buttons.
@@ -649,15 +725,15 @@
                     font.setStrikeOut(True)
                     break
             else:
                 font.setStrikeOut(False)
             node_item.setFont(font)
 
         # Mark all missing packages, if they were manually imported
-        missing_packages = False         # Track, if we have to enable the 'Find' button
+        missing_packages = False  # Track, if we have to enable the 'Find' button
         for i in range(self.missing_list_widget.count()):
             node_item = self.missing_list_widget.item(i)
             font = node_item.font()
             for pkg_path in self.conf.nodes:
                 if node_item.text() == pkg_path.stem:
                     # Missing package is provided by manually imported package
                     font.setStrikeOut(True)
```

### Comparing `ryven-3.4.3/ryven/gui/std_input_widgets.py` & `ryven-3.5.0/ryven/gui/std_input_widgets.py`

 * *Files 6% similar despite different names*

```diff
@@ -114,15 +114,15 @@
                         max(new_width, self.base_width),
                         self.max_width
                     ))
                     self.node_gui.update_shape()
                 self.on_widget_val_changed(self.val)
 
             @property
-            def val(self) -> data_type:
+            def val(self) -> Data:
                 try:
                     return data_type(eval(self.text()))
                 except:
                     return data_type(self.text())
 
             def load_from(self, val: Data):
                 with self._prevent_update:
@@ -193,15 +193,15 @@
                         max(new_width, self.base_width),
                         self.max_width
                     ))
                     self.node_gui.update_shape()
                 self.on_widget_val_changed(self.val)
 
             @property
-            def val(self) -> data_type:
+            def val(self) -> Data:
                 return data_type(self.text())
 
             def load_from(self, val: Data):
                 with self._prevent_update:
                     self.setText(str(val.payload))
 
             def val_update_event(self, val: Data):
@@ -244,15 +244,15 @@
                 # initial value and rage
                 with self._prevent_update:
                     self.setRange(*range)
                     self.setValue(init)
 
 
             @property
-            def val(self) -> data_type:
+            def val(self) -> Data:
                 return data_type(self.value())
 
             def load_from(self, val: Data):
                 with self._prevent_update:
                     self.setValue(val.payload)
 
             def value_changed(self, _):
@@ -288,15 +288,15 @@
 
                 # initial value and rage
                 with self._prevent_update:
                     self.setRange(*range)
                     self.setValue(init)
 
             @property
-            def val(self) -> data_type:
+            def val(self) -> Data:
                 return data_type(self.value())
 
             def load_from(self, val: Data):
                 with self._prevent_update:
                     self.setValue(val.payload)
 
             def value_changed(self, _):
@@ -329,15 +329,15 @@
                 self.stateChanged.connect(self.state_changed)
 
                 # initial value
                 with self._prevent_update:
                     self.setChecked(init)
 
             @property
-            def val(self) -> data_type:
+            def val(self) -> Data:
                 return data_type(self.isChecked())
 
             def load_from(self, val: Data):
                 with self._prevent_update:
                     self.setChecked(val.payload)
 
             def state_changed(self, _):
```

### Comparing `ryven-3.4.3/ryven/gui/styling/design_config.json` & `ryven-3.5.0/ryven/gui/styling/design_config.json`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/gui/styling/window_theme.py` & `ryven-3.5.0/ryven/gui/styling/window_theme.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+from typing import Dict, Optional
+
 from ryven.main.utils import abs_path_from_package_dir
 
 
 def hex_to_rgb(hex: str):
     if hex is None:
         return None
     else:
         return tuple(int(hex[i:i + 2], 16) for i in (1, 3, 5))
 
 
 class WindowTheme:
 
     name = ''
-    colors = {}
-    rules = {}
+    colors: Dict[str, Optional[str]] = {}
+    rules: Dict[str, Optional[str]] = {}
 
     def __init__(self):
         self.init_rules()
 
     def init_rules(self):
         self.rules = {
             # colors
@@ -77,24 +79,27 @@
         'secondaryTextColor': None,
         'danger': None,
         'warning': None,
         'success': None,
     }
 
 
-def apply_stylesheet(style: str):
+def apply_stylesheet(style: str) -> WindowTheme:
+
     from qtpy.QtWidgets import QApplication
 
     # set to None if not used
     icons_dir = abs_path_from_package_dir('resources/stylesheets/icons')
     if icons_dir is not None:
         from qtpy.QtCore import QDir
         d = QDir()
         d.setSearchPaths('icon', [icons_dir])
 
+    window_theme: WindowTheme
+
     if style in (None, 'plain'):
         window_theme = WindowTheme_Plain()
         stylesheet = None
     else:
         if style == 'dark':
             window_theme = WindowTheme_Dark()
         elif style == 'light':
```

### Comparing `ryven-3.4.3/ryven/gui/uic/flow.ui` & `ryven-3.5.0/ryven/gui/uic/flow.ui`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/gui/uic/main_window.ui` & `ryven-3.5.0/ryven/gui/uic/main_window.ui`

 * *Files 16% similar despite different names*

#### Comparing `ryven-3.4.3/ryven/gui/uic/main_window.ui` & `ryven-3.5.0/ryven/gui/uic/main_window.ui`

```diff
@@ -15,42 +15,28 @@
         <horstretch>0</horstretch>
         <verstretch>0</verstretch>
       </sizepolicy>
     </property>
     <property name="windowTitle">
       <string>MainWindow</string>
     </property>
+    <property name="dockOptions">
+      <set>QMainWindow::AllowTabbedDocks|QMainWindow::AnimatedDocks</set>
+    </property>
     <widget class="QWidget" name="centralWidget">
       <layout class="QGridLayout" name="gridLayout">
         <item row="0" column="0">
           <widget class="QSplitter" name="main_vertical_splitter">
             <property name="orientation">
               <enum>Qt::Vertical</enum>
             </property>
             <widget class="QSplitter" name="main_horizontal_splitter">
               <property name="orientation">
                 <enum>Qt::Horizontal</enum>
               </property>
-              <widget class="QSplitter" name="splitter">
-                <property name="orientation">
-                  <enum>Qt::Vertical</enum>
-                </property>
-                <widget class="QGroupBox" name="flows_groupBox">
-                  <property name="title">
-                    <string>Flows</string>
-                  </property>
-                  <layout class="QVBoxLayout" name="verticalLayout_2"/>
-                </widget>
-                <widget class="QGroupBox" name="nodes_groupBox">
-                  <property name="title">
-                    <string>Nodes</string>
-                  </property>
-                  <layout class="QVBoxLayout" name="verticalLayout"/>
-                </widget>
-              </widget>
               <widget class="QTabWidget" name="flows_tab_widget">
                 <property name="sizePolicy">
                   <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
                     <horstretch>0</horstretch>
                     <verstretch>0</verstretch>
                   </sizepolicy>
                 </property>
@@ -60,26 +46,25 @@
                 <widget class="QWidget" name="tab">
                   <attribute name="title">
                     <string>Main</string>
                   </attribute>
                 </widget>
               </widget>
             </widget>
-            <widget class="QWidget" name="console_placeholder_widget" native="true"/>
           </widget>
         </item>
       </layout>
     </widget>
     <widget class="QMenuBar" name="menuBar">
       <property name="geometry">
         <rect>
           <x>0</x>
           <y>0</y>
           <width>1368</width>
-          <height>30</height>
+          <height>22</height>
         </rect>
       </property>
       <widget class="QMenu" name="menuFile">
         <property name="title">
           <string>File</string>
         </property>
         <widget class="QMenu" name="menuScripts">
@@ -107,15 +92,21 @@
         <widget class="QMenu" name="menuSave_Picture">
           <property name="title">
             <string>Save Picture</string>
           </property>
           <addaction name="actionSave_Pic_Viewport"/>
           <addaction name="actionSave_Pic_Whole_Scene_scaled"/>
         </widget>
+        <widget class="QMenu" name="menuDocks">
+          <property name="title">
+            <string>Windows</string>
+          </property>
+        </widget>
         <addaction name="separator"/>
+        <addaction name="menuDocks"/>
         <addaction name="menuFlow_Design_Style"/>
         <addaction name="menuSave_Picture"/>
       </widget>
       <widget class="QMenu" name="menuDebugging">
         <property name="title">
           <string>Options</string>
         </property>
@@ -129,14 +120,78 @@
         <addaction name="menuInfo_Messages"/>
       </widget>
       <addaction name="menuFile"/>
       <addaction name="menuView"/>
       <addaction name="menuDebugging"/>
     </widget>
     <widget class="QStatusBar" name="statusBar"/>
+    <widget class="QDockWidget" name="flows_dock">
+      <property name="features">
+        <set>QDockWidget::DockWidgetClosable|QDockWidget::DockWidgetFloatable|QDockWidget::DockWidgetMovable</set>
+      </property>
+      <property name="windowTitle">
+        <string>Flows</string>
+      </property>
+      <attribute name="dockWidgetArea">
+        <number>1</number>
+      </attribute>
+      <widget class="QWidget" name="flowsWidgetContents">
+        <property name="sizePolicy">
+          <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
+            <horstretch>0</horstretch>
+            <verstretch>0</verstretch>
+          </sizepolicy>
+        </property>
+      </widget>
+    </widget>
+    <widget class="QDockWidget" name="nodes_dock">
+      <property name="features">
+        <set>QDockWidget::DockWidgetClosable|QDockWidget::DockWidgetFloatable|QDockWidget::DockWidgetMovable</set>
+      </property>
+      <property name="windowTitle">
+        <string>Nodes</string>
+      </property>
+      <attribute name="dockWidgetArea">
+        <number>1</number>
+      </attribute>
+      <widget class="QWidget" name="nodesWidgetContents">
+        <property name="sizePolicy">
+          <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
+            <horstretch>0</horstretch>
+            <verstretch>0</verstretch>
+          </sizepolicy>
+        </property>
+      </widget>
+    </widget>
+    <widget class="QDockWidget" name="consoleDock">
+      <property name="features">
+        <set>QDockWidget::DockWidgetClosable|QDockWidget::DockWidgetFloatable|QDockWidget::DockWidgetMovable</set>
+      </property>
+      <property name="allowedAreas">
+        <set>Qt::BottomDockWidgetArea</set>
+      </property>
+      <property name="windowTitle">
+        <string>CONSOLE</string>
+      </property>
+      <attribute name="dockWidgetArea">
+        <number>8</number>
+      </attribute>
+      <widget class="QWidget" name="consoleDockContents">
+        <widget class="QWidget" name="console_placeholder_widget" native="true">
+          <property name="geometry">
+            <rect>
+              <x>0</x>
+              <y>0</y>
+              <width>976</width>
+              <height>407</height>
+            </rect>
+          </property>
+        </widget>
+      </widget>
+    </widget>
     <action name="actionImport_Nodes">
       <property name="text">
         <string>Import Nodes</string>
       </property>
     </action>
     <action name="actionSave_Project">
       <property name="text">
@@ -198,12 +253,17 @@
       </property>
     </action>
     <action name="actionImport_Example_Nodes">
       <property name="text">
         <string>Import Example Nodes</string>
       </property>
     </action>
+    <action name="action">
+      <property name="text">
+        <string>sd</string>
+      </property>
+    </action>
   </widget>
   <layoutdefault spacing="6" margin="11"/>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `ryven-3.4.3/ryven/gui/uic/ui_flow.py` & `ryven-3.5.0/ryven/gui/uic/ui_flow.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/main/Ryven.py` & `ryven-3.5.0/ryven/main/Ryven.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,16 +3,47 @@
 
 import ryven.main.packages.nodes_package
 from ryven.main import utils
 from ryven.main.config import Config
 from ryven.main.args_parser import process_args
 
 
+def check_pyside_available(qt_api: str):
+    if qt_api == 'pyside2':
+        if sys.version_info >= (3, 11):
+            sys.exit(
+                'You are trying to use PySide2 as the Qt API, but it is not available for Python 3.11 and later. '
+                'Please use PySide6 instead (run `ryven -q pyside6`), or use Python 3.10 or earlier. '
+            )
+        try:
+            import PySide2
+        except ImportError:
+            sys.exit(
+                'You are trying to use PySide2 as the Qt API, but it is not available. '
+                'Please install it, or use pyside6 as the Qt API. Either of those can '
+                'installed through pip, e.g. `pip install pyside2` or `pip install \'pyside6<6.7\'`. '
+            )
+    elif qt_api == 'pyside6':
+        try:
+            import PySide6
+        except ImportError:
+            sys.exit(
+                'You are trying to use PySide6 as the Qt API, but it is not available. '
+                'please install it, or use pyside2 as the Qt API. Either of those can '
+                'installed through pip, e.g. `pip install pyside2` or `pip install \'pyside6<6.7\'`. '
+            )
+    else:
+        sys.exit(
+            f'Error: Illegal Qt API: "{qt_api}". '
+            f'Use either "pyside2" or "pyside6". '
+        )
+
+
 def run(*args_,
-        qt_app=None, gui_parent=None, use_sysargs=True,
+        qt_app=None, gui_parent=None, use_sysargs: bool = True,
         **kwargs):
     """Start the Ryven window.
 
     The `*args_` and `**kwargs` arguments correspond to their positional and
     optional command line equivalents, respectively (see `parse_args()`).
     Optional keyword arguments are specified without the leading double hyphens
     '--'. As a name, the corresponding 'dest' value of `add_argument` has to
@@ -68,14 +99,15 @@
     conf: Config = process_args(use_sysargs, *args_, **kwargs)
 
     #
     # Qt application setup
     #
 
     # Init environment
+    check_pyside_available(conf.qt_api)
     os.environ['RYVEN_MODE'] = 'gui'
     os.environ['QT_API'] = conf.qt_api
     from ryven.node_env import init_node_env
     from ryven.gui_env import init_node_guis_env  # Qt dependency
     init_node_env()
     init_node_guis_env()
 
@@ -120,23 +152,24 @@
 
         sw = StartupDialog(config=conf, parent=gui_parent)
         # Exit if dialog couldn't initialize or is exited
         if sw.exec_() <= 0:
             sys.exit('Start-up screen dismissed')
 
     # Replace node directories with `NodePackage` instances
-    if conf.nodes:
+    if len(conf.nodes) > 0:
         conf.nodes, pkgs_not_found, _ = ryven.main.packages.nodes_package.process_nodes_packages(list(conf.nodes))
         if pkgs_not_found:
             sys.exit(
                 f'Error: Nodes packages not found: {", ".join([str(p) for p in pkgs_not_found])}')
 
         # editor_config['requested packages'] = conf.nodes
 
     # Store WindowTheme object
+    assert isinstance(conf.window_theme, str)
     conf.window_theme = apply_stylesheet(conf.window_theme)
 
     # Adjust flow theme if not set
     if conf.flow_theme is None:
         if conf.window_theme.name == 'dark':
             conf.flow_theme = 'pure dark'
         else:
@@ -146,21 +179,23 @@
     #   At this point, the Config is fully populated with exact types
     #   (e.g. `conf.nodes` is a list of `NodePackage` instances, and
     #   not a list of `str` anymore).
 
     # Get packages required by the project
     if conf.project:
         pkgs, pkgs_not_found, project_dict = ryven.main.packages.nodes_package.process_nodes_packages(
-            conf.project, requested_packages=list(conf.nodes))
+            conf.project,
+            requested_packages=list(conf.nodes)  # type: ignore
+        )
 
         if pkgs_not_found:
             str_missing_pkgs = ', '.join([str(p.name) for p in pkgs_not_found])
             plural = len(pkgs_not_found) > 1
             sys.exit(
-                f'The package{"s" if plural else ""} {str_missing_pkgs}'
+                f'The package{"s" if plural else ""} {str_missing_pkgs} '
                 f'{"were" if plural else "was"} requested, '
                 f'but {"they are" if plural else "it is"} not available.\n'
                 f'Update the project file or supply the missing package{"s" if plural else ""} '
                 f'{str_missing_pkgs} on the command line with the "-n" switch.')
 
         requested_packages = conf.nodes
         required_packages = pkgs
```

### Comparing `ryven-3.4.3/ryven/main/RyvenConsole.py` & `ryven-3.5.0/ryven/main/RyvenConsole.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# TODO this could be improved
+
 """
 This module includes the whole Ryven Console application.
 It simply deploys a session with the project provided and implements a REPL.
 This is supposed to be used in an interactive way. For scripting and deploying
 projects without GUI programmatically, the ryvencore lib should be used directly.
 """
 import argparse
```

### Comparing `ryven-3.4.3/ryven/main/args_parser.py` & `ryven-3.5.0/ryven/main/args_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     -------
     args : argparse.Namespace
         The parsed command line arguments or the default values.
 
     """
 
     # Get available examples
-    exampledir = utils.abs_path_from_package_dir('examples_projects')
+    exampledir = utils.abs_path_from_package_dir('example_projects')
     examples = [e.stem for e in pathlib.Path(exampledir).glob('*.json')]
 
     #
     # The parser
     #
 
     parser = CustomArgumentParser(
@@ -204,14 +204,24 @@
         help=f'''
             • Enables a (highly unstable and hacky) feature that allows temporary\\ 
             editing of the source code of nodes in the source code preview panel\\
             (useful for debugging)\\
             • When enabled, Ryven might consume much more memory than usual
             ''')
 
+    parser.add_argument(
+        '--defer-code-loading',
+        action='store_true',
+        dest='defer_code_loading',
+        help=f'''
+            • When using deferred code loading, Ryven will load the source code of\\
+            nodes only once the user wants to inspect it.\\
+            • Deferred code loading decreases package loading time.\\
+            ''')
+
     # Project configuration
 
     group = parser.add_argument_group('project configuration')
 
     group.add_argument(
         '-n', '--nodes',
         action='append',
@@ -351,24 +361,23 @@
         args = parser.parse_args([], namespace=Config())
     else:
         args = parser.parse_args(namespace=Config())
 
     # Check, if project file exists
     if args.project:
         if args.project == '-':
-            args.project = sys.stdin
-        else:
-            project = utils.find_project(args.project)
-            if project is None:
-                parser.error(
-                    'project file does not exist')
-            args.project = project
+            args.project = pathlib.Path(str(sys.stdin))
+        project = utils.find_project(args.project)
+        if project is None:
+            parser.error(
+                'project file does not exist')
+        args.project = project
 
     # Make a `set` of paths to node packages
-    args.nodes = set([pathlib.Path(nodes_pkg) for nodes_pkg in args.nodes])
+    args.nodes = set([pathlib.Path(nodes_pkg) for nodes_pkg in args.nodes])  # type: ignore
 
     # Put example into 'project' argument
     if args.example:
         if args.project:
             parser.error(
                 'when loading an example, no argument PROJECT is allowed')
```

### Comparing `ryven-3.4.3/ryven/main/config.py` & `ryven-3.5.0/ryven/main/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,24 +25,25 @@
     # initially, but will be converted to actual types
     # by the args parser.
     #
 
     project: Optional[pathlib.Path] = None
     show_dialog: bool = True
     verbose: bool = False
-    nodes: Union[Set[pathlib.Path], Set[NodesPackage]] = []
+    nodes: Union[Set[pathlib.Path], Set[NodesPackage]] = set()
     example: Optional[str] = None
     window_theme: Union[str, WindowTheme] = 'dark'
     flow_theme: Optional[str] = None  # None means it depends on window_theme
     performance_mode: str = 'pretty'
     animations: bool = True
     window_geometry: Optional[str] = None
     window_title: str = 'Ryven'
     qt_api: str = 'pyside2'
     src_code_edits_enabled: bool = False
+    defer_code_loading: bool = False
 
     @staticmethod
     def get_available_window_themes() -> Set[str]:
         return {'dark', 'light', 'plain'}
 
     @staticmethod
     def get_available_flow_themes() -> Set[str]:
```

### Comparing `ryven-3.4.3/ryven/main/packages/built_in/gui.py` & `ryven-3.5.0/ryven/main/packages/built_in/gui.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ryvencore import Data
 
 from ryven.gui_env import *
-
+from .nodes import *
 from qtpy.QtGui import QKeySequence
 from qtpy.QtCore import Signal
 from qtpy.QtWidgets import QLineEdit, QDialog, QDialogButtonBox, QMessageBox, QPlainTextEdit, QShortcut, QVBoxLayout
 
 
 class Result_Node_MainWidget(NodeMainWidget, QLineEdit):
     def __init__(self, params):
@@ -16,15 +16,15 @@
         self.setFixedWidth(120)
 
 
     def show_val(self, new_val):
         self.setText(str(new_val))
         self.setCursorPosition(0)
 
-
+@node_gui(Result_Node)
 class ResultGui(NodeGUI):
     main_widget_class = Result_Node_MainWidget
     main_widget_pos = 'between ports'
     color = '#c69a15'
 
 
 class ValNode_MainWidget(NodeMainWidget, QLineEdit):
@@ -104,15 +104,15 @@
         val = self.val_text_edit.toPlainText()
         try:
             val = eval(val)
         except Exception as e:
             pass
         return val
 
-
+@node_gui(Val_Node)
 class ValGui(NodeGUI):
     main_widget_class = ValNode_MainWidget
     style = 'small'
     color = '#c69a15'
 
     def initialized(self):
         self.main_widget().value_changed.connect(self.widget_val_updated)
@@ -125,15 +125,15 @@
     def action_edit_via_dialog(self):
         val_dialog = EditVal_Dialog(parent=None, init_val=self.node.val)
         accepted = val_dialog.exec_()
         if accepted:
             self.main_widget().setText(str(val_dialog.get_val()))
             self.update()
 
-
+@node_gui(SetVarsPassive_Node)
 class SetVarsGui(NodeGUI):
     style = 'normal'
     color = '#c69a15'
 
     def initialized(self):
         self.actions['add var input'] = {'method': self.add_var}
         self.actions['remove var input'] = {}
@@ -158,15 +158,15 @@
         for i in range(self.node.num_vars):
             self.actions[f'remove var input'][f'{i+1}'] = {
                 'method': self.remove_var,
                 'data': i+1
             }
 
 
-
+@node_gui(SetVar_Node)
 class SetVarGui(NodeGUI):
     input_widget_classes = {
         'varname': inp_widgets.Builder.str_line_edit(),
         'val': inp_widgets.Builder.str_line_edit(),
     }
     # init_input_widgets = {
     #     1: {'name': 'varname', 'pos': 'besides'},
@@ -177,25 +177,16 @@
 
     def __init__(self, params):
         super().__init__(params)
 
         self.input_widgets[self.node.inputs[-2]] = {'name': 'varname', 'pos': 'besides'}
         self.input_widgets[self.node.inputs[-1]] = {'name': 'val', 'pos': 'besides'}
 
-
+@node_gui(GetVar_Node)
 class GetVarGui(NodeGUI):
     input_widget_classes = {
         'varname': inp_widgets.Builder.str_line_edit(),
     }
     init_input_widgets = {
         0: {'name': 'varname', 'pos': 'besides'}
     }
     color = '#c69a15'
-
-
-export_guis([
-    GetVarGui,
-    ResultGui,
-    ValGui,
-    SetVarGui,
-    SetVarsGui,
-])
```

### Comparing `ryven-3.4.3/ryven/main/packages/built_in/nodes.py` & `ryven-3.5.0/ryven/main/packages/built_in/nodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-from ryven.node_env import *
-guis = import_guis(__file__)
-import ryvencore as rc
-
+from ryvencore import Node, NodeInputType, NodeOutputType, Data
+from ryven.node_env import export_nodes, on_gui_load
 
 class NodeBase(Node):
     def have_gui(self):
         return hasattr(self, 'gui')
 
     def vars_addon(self):
         return self.get_addon('Variables')
@@ -13,43 +11,38 @@
     def get_var_val(self, var_name):
         return self.vars_addon().var(self.flow, var_name).get()
 
     def set_var_val(self, var_name, val):
         return self.vars_addon().var(self.flow, var_name).set(val)
 
 
-
 class GetVar_Node(NodeBase):
     """Gets the value of a script variable"""
 
     version = 'v0.2'
 
     title = 'get var'
     init_inputs = [
         NodeInputType(),
     ]
-    init_outputs = [
-        NodeOutputType(label='val')
-    ]
-    GUI = guis.GetVarGui
+    init_outputs = [NodeOutputType(label='val')]
 
     def __init__(self, params):
         super().__init__(params)
 
         self.var_name = ''
         self.temp_var_val = None
 
     def place_event(self):
         self.update()
         if self.input(0) is not None:
             self.var_name = self.input(0).payload
 
     def update_event(self, input_called=-1):
         if self.input(0).payload != self.var_name:
-
             if self.var_name != '':  # disconnect old var val update connection
                 self.vars_addon().unsubscribe(self, self.var_name, self.var_val_changed)
 
             self.var_name = self.input(0).payload
 
             # create new var update connection
             self.vars_addon().subscribe(self, self.var_name, self.var_val_changed)
@@ -65,15 +58,14 @@
 
     version = 'v0.2'
 
     title = 'result'
     init_inputs = [
         NodeInputType(type_='data'),
     ]
-    GUI = guis.ResultGui
 
     def __init__(self, params):
         super().__init__(params)
         self.val = None
 
     def rebuilt(self):
         self.update()
@@ -90,38 +82,34 @@
     version = 'v0.2'
 
     title = 'val'
     init_inputs = [
         # NodeInputType(default=Data()),
     ]
     init_outputs = [
-        NodeInputType(type_='data'),
+        NodeOutputType(type_='data'),
     ]
-    GUI = guis.ValGui
 
     def __init__(self, params):
         super().__init__(params)
 
         self.display_title = ''
         self.val = Data()
 
-
     def place_event(self):
         self.update()
 
     def update_event(self, input_called=-1):
         self.set_output_val(0, self.val)
 
     def get_current_var_name(self):
         return self.input(0).payload if self.input(0) is not None else None
 
     def get_state(self):
-        return {
-            'val': self.val  # self.main_widget().get_val()
-        }
+        return {'val': self.val}  # self.main_widget().get_val()
 
     def set_state(self, data, version):
         self.val = data['val']
 
 
 class SetVar_Node(NodeBase):
     """Sets the value of a script variable"""
@@ -135,38 +123,33 @@
         NodeInputType(label='val'),
     ]
     init_outputs = [
         NodeOutputType(type_='exec'),
         NodeOutputType(type_='data', label='val'),
     ]
 
-    GUI = guis.SetVarGui
-
     def __init__(self, params):
         super().__init__(params)
 
         self.active = True
 
         self.var_name = ''
         self.num_vars = 1
 
     def place_event(self):
         if self.have_gui():
             self.gui.actions['make passive'] = {'method': self.action_make_passive}
 
     def update_event(self, input_called=-1):
-
         if self.active and input_called == 0:
-
             if self.set_var_val(self.input(1).payload, self.input(2).payload):
                 self.set_output_val(1, self.input(2))
             self.exec_output(0)
 
         elif not self.active:
-
             self.var_name = self.input(0).payload
             if self.set_var_val(self.input(0).payload, self.input(1).payload):
                 self.set_output_val(0, Data(self.get_var_val(self.var_name)))
 
     def action_make_passive(self):
         self.active = False
         self.delete_input(0)
@@ -196,15 +179,14 @@
     """Sets the values of multiple script variables"""
 
     version = 'v0.1'
 
     title = 'set vars passive'
     init_inputs = []
     init_outputs = []
-    GUI = guis.SetVarsGui
 
     def __init__(self, params):
         super().__init__(params)
 
         self.num_vars = 0
 
     def add_var_input(self):
@@ -215,16 +197,16 @@
 
         self.num_vars += 1
 
         if self.have_gui():
             self.gui.rebuild_remove_actions()
 
     def remove_var_input(self, number):
-        self.delete_input((number-1)*2)
-        self.delete_input((number-1)*2)
+        self.delete_input((number - 1) * 2)
+        self.delete_input((number - 1) * 2)
         self.num_vars -= 1
         # self.rebuild_remove_actions()
 
         if self.have_gui():
             self.gui.rebuild_remove_actions()
 
     # def rebuild_remove_actions(self):
@@ -242,28 +224,30 @@
     #     for i in range(self.num_vars):
     #         self.gui.actions[f'remove var {i+1}'] = {
     #             'method': self.remove_var_input,
     #             'data': i+1
     #         }
 
     def update_event(self, input_called=-1):
-
         var_names = [self.input(i).payload for i in range(0, len(self.inputs), 2)]
         values = [self.input(i).payload for i in range(1, len(self.inputs), 2)]
 
         for i in range(len(var_names)):
             self.set_var_val(var_names[i], values[i])
 
     def get_state(self):
         return {'num vars': self.num_vars}
 
     def set_state(self, data, version):
         self.num_vars = data['num vars']
 
-
 export_nodes([
     SetVar_Node,
     GetVar_Node,
     Val_Node,
     Result_Node,
     SetVarsPassive_Node
 ])
+
+@on_gui_load
+def load_gui():
+    from . import gui
```

### Comparing `ryven-3.4.3/ryven/main/packages/nodes_package.py` & `ryven-3.5.0/ryven/main/packages/nodes_package.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 """
 This module, together with the node_env and gui_env defines Ryven's nodes
 package system. It can be used outside of Ryven as well.
 """
 
 import importlib.util
-import os
+import os, sys
 import pathlib
 from os.path import basename, dirname, splitext, normpath, join
-from typing import Tuple, List, Type, Union, Set, Optional
+from typing import Tuple, List, Type, Union, Set, Optional, Dict
+import pkgutil
 
 from ryvencore import Node, Data
 
-from ryven.main.utils import read_project, ryven_dir_path, abs_path_from_package_dir
-
+from ryven.main.utils import (
+    read_project, 
+    ryven_dir_path, 
+    abs_path_from_package_dir, 
+    in_gui_mode,
+    load_from_file,
+)
+from ryven.main.packages.node_env import load_current_guis
 
 class NodesPackage:
     """
     A small container to store meta data about imported node packages.
     """
 
     def __init__(self, directory: str):
-
         self.name = basename(normpath(directory))
         self.directory = directory
 
         self.file_path = normpath(join(directory, 'nodes.py'))
 
     def __str__(self):
         return f'{self.__class__.__name__}({self.name})'
@@ -44,74 +50,66 @@
     def config_data(self):
         return {
             'name': self.name,
             'dir': self.directory,
         }
 
 
-def load_from_file(file: str = None, components_list: [str] = None) -> tuple:
-    """
-    Imports specified components from a python module with given file path.
-    """
-    if components_list is None:
-        components_list = []
-
-    name = basename(file).split('.')[0]
-    spec = importlib.util.spec_from_file_location(name, file)
-
-    importlib.util.module_from_spec(spec)
-
-    mod = spec.loader.load_module(name)
-    # using load_module(name) instead of exec_module(mod) here,
-    # because exec_module() somehow then registers it as "built-in"
-    # which is wrong and prevents inspect from parsing the source
-
-    comps = tuple([getattr(mod, c) for c in components_list])
-
-    return comps
-
-
-def import_nodes_package(package: NodesPackage = None, directory: str = None) -> \
-        Tuple[List[Type[Node]], List[Type[Data]]]:
+# should be Tuple[list[Type[Node]], list[Type[Data]] in 3.9+
+def import_nodes_package(
+    package: Optional[NodesPackage] = None, directory: Optional[str] = None
+) -> Tuple[List[Type[Node]], List[Type[Data]]]:
     """Loads node and data classes from a Ryven nodes package and returns both in separate lists.
 
     Can be used without a running Ryven instance, but you need to specify in which mode nodes should be loaded
     by setting the environment variable RYVEN_MODE to either 'gui' (gui imports enabled) or 'no-gui'.
 
     :param package: The NodesPackage object.
     :param directory: The path to the directory where the nodes.py file is located, used if package is None.
     :return: A tuple containing node types (classes) first, and the data types exported by the package second.
     """
 
     if package is None:
+        assert directory is not None, 'Either package or directory must be specified.'
         package = NodesPackage(directory)
 
     if 'RYVEN_MODE' not in os.environ:
         raise Exception(
-            "Please specify the environment variable RYVEN_MODE ('gui' or 'no-gui') before loading any packages. "
-            "For example set os.environ['RYVEN_MODE'] = 'no-gui' for gui-less deployment."
+            """Please specify the environment variable RYVEN_MODE ('gui' or 'no-gui') before loading any packages. 
+            For example, set os.environ['RYVEN_MODE'] = 'no-gui' for gui-less deployment.
+            Ryven and RyvenConsole should do this automatically.
+            """
         )
 
     from ryven import node_env
+
     node_env.NodesEnvRegistry.current_package = package
     load_from_file(package.file_path)
 
-    node_types = node_env.NodesEnvRegistry.exported_nodes[-1]
-    data_types = node_env.NodesEnvRegistry.exported_data_types[-1]
-
+    # load guis
+    if in_gui_mode():
+        load_current_guis()
+    
+    node_types, data_types = node_env.NodesEnvRegistry.consume_last_exported_package()
+    
+    # load source codes
+    if in_gui_mode():
+        from ryven.gui.code_editor.codes_storage import register_node_type
+        for node_type in node_types:
+            register_node_type(node_type)
+    
     return node_types, data_types
 
-
 def process_nodes_packages(
     project_or_nodes: Union[
-        Union[str, pathlib.Path],                       # path to Ryven project
-        List[Union[str, pathlib.Path, NodesPackage]]    # list of node packages
+        Union[str, pathlib.Path],  # path to Ryven project
+        List[Union[str, pathlib.Path, NodesPackage]],  # list of node packages
     ],
-    requested_packages: List[NodesPackage] = None
-) -> Tuple[Set[NodesPackage], List[pathlib.Path], Optional[dict]]:
+    requested_packages: Optional[List[NodesPackage]] = None,
+) -> Tuple[Set[NodesPackage], Set[pathlib.Path], Optional[Dict]]:
     """Takes a project or list of node packages and additionally requested node
     packages and checks whether the node packages are valid.
 
     It also removes duplicates based on the name (and not the contents!).
 
     :param project_or_nodes:
         Either a path to a Ryven project or a list of node packages.
@@ -136,28 +134,26 @@
             - Dictionary with the contents of the project or `None`.
     """
     # from ryven.main.packages.nodes_package import NodesPackage
 
     if requested_packages is None:
         requested_packages = []
 
+    pkgs: Set[NodesPackage] = set()
+    pkgs_not_found: Set[pathlib.Path] = set()
+    project_dict: Optional[Dict]
+
     # Find nodes in the project file
-    try:
+    if isinstance(project_or_nodes, (str, pathlib.Path)):
         project_dict = read_project(project_or_nodes)
         node_pkg_paths = [p['dir'] for p in project_dict['required packages']]
-    except TypeError:
+    else:
         project_dict = None
         node_pkg_paths = project_or_nodes
-    except KeyError:
-        # No required packages found
-        project_dict = None
-        node_pkg_paths = []
 
-    pkgs = set()
-    pkgs_not_found = set()
     for pkg in node_pkg_paths:
         if isinstance(pkg, NodesPackage):
             pkgs.add(pkg)
         else:
             # For backward compatibility we have to deal with Windows and Posix
             # paths in the project's file
             pkg_windows_path = pathlib.PureWindowsPath(pkg)
@@ -185,13 +181,12 @@
             # Package could not be found
             pkgs_not_found.add(pkg_path)
 
     # Check, if nodes which could not be found are already available in
     # `requested_nodes`.
     # This check is done by comparing the path name to the nodes' names
     args_pkgs_names = [pkg.name for pkg in requested_packages]
-    pkgs_not_found = [
-        pkg_path
-        for pkg_path in pkgs_not_found
-        if pkg_path.name not in args_pkgs_names]
+    pkgs_not_found = set(
+        pkg_path for pkg_path in pkgs_not_found if pkg_path.name not in args_pkgs_names
+    )
 
     return pkgs, pkgs_not_found, project_dict
```

### Comparing `ryven-3.4.3/ryven/main/utils.py` & `ryven-3.5.0/ryven/main/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,62 @@
 """
 Core utilities for handling Ryven projects and nodes packages, and
 resolving paths. Deos not depend on any Qt modules.
 """
-
+import sys
+import os
+from os import environ
 from os.path import normpath, join, dirname, abspath, expanduser
 import pathlib
-from typing import Union, Optional
+import importlib
+from typing import Union, Optional, Tuple, List, Dict
 from packaging.version import Version
 
+from ryvencore import InfoMsgs
+
+def in_gui_mode() -> bool:
+    return environ['RYVEN_MODE'] == 'gui'
+
+
+def load_from_file(file: str, components_list: Optional[List[str]] = None) -> Optional[Tuple]:
+    """
+    Imports specified components from a python module with given file path.
+    The directory of the file is added to sys.path if not already present.
+    """
+    if components_list is None:
+        components_list = []
+
+    dirpath, filename = os.path.split(file)
+    parent_dirpath, pkg_name = os.path.split(dirpath)
+    mod_name = filename.split('.')[0]
+    name = f"{pkg_name}.{mod_name}"  # e.g. built_in.nodes
+
+    # protection from re-loading for no reason
+    if name in sys.modules:
+        return None
+    
+    if parent_dirpath not in sys.path:
+        sys.path.append(parent_dirpath)
+    
+    # import the corresponding module
+    try:
+        mod = importlib.import_module(name, pkg_name)
+        comps = tuple([getattr(mod, c) for c in components_list])
+        return comps
+    except ModuleNotFoundError as e:
+        InfoMsgs.write_err(
+            f'\n\nCould not import {name}: {e}\n'
+            f'This could be due to a missing __init__.py file in the nodes package, '
+            f'or your package name conflicts with another python package name '
+            f'that the interpreter knows about (e.g. math).\n\n'
+        )
+        raise e
+
 
-def read_project(project_path: Union[str, pathlib.Path]) -> dict:
+def read_project(project_path: Union[str, pathlib.Path]) -> Dict:
     """Read the project file and return its dictionary.
 
     :param project_path: The path to the project file.
     :return: The contents of the project file.
     """
     import io
     import json
@@ -32,42 +75,43 @@
             Version(project_dict['general info']['ryven version']) <= Version('3.2'):
         print(
             'WARNING: project was created with an older version of Ryven.',
             'Attempting to translate project to current version.'
         )
         project_dict = translate_project_v3_2_0(project_dict)
 
+    assert isinstance(project_dict, Dict), 'Project file seems corrupted.'
     return project_dict
 
 
-def translate_project_v3_2_0(p: dict):
-    def max_gid(d: dict) -> int:
+def translate_project_v3_2_0(p: Dict):
+    def max_gid(d: Dict) -> int:
         """Recursively find the maximum GID used in the project.."""
         n = 0
         for k, v in d.items():
-            if isinstance(v, dict):
+            if isinstance(v, Dict):
                 n = max(n, max_gid(v))
             elif isinstance(v, list):
                 for e in v:
-                    if isinstance(e, dict):
+                    if isinstance(e, Dict):
                         n = max(n, max_gid(e))
             elif k == 'GID':
                 n = max(n, v)
         return n
 
     gid_ctr = max_gid(p) + 1
     def get_gid():
         nonlocal gid_ctr
         gid_ctr += 1
         return gid_ctr
 
     def replace_item(obj, key, replace_value):
         # https://stackoverflow.com/questions/45335445/how-to-recursively-replace-dictionary-values-with-a-matching-key
         for k, v in obj.items():
-            if isinstance(v, dict):
+            if isinstance(v, Dict):
                 obj[k] = replace_item(v, key, replace_value)
         if key in obj:
             obj[key] = replace_value
         return obj
 
     proj = {
         'general info': p['general info'],
```

### Comparing `ryven-3.4.3/ryven/resources/fonts/asap/Asap-Bold.ttf` & `ryven-3.5.0/ryven/resources/fonts/asap/Asap-Bold.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/asap/Asap-BoldItalic.ttf` & `ryven-3.5.0/ryven/resources/fonts/asap/Asap-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/asap/Asap-Italic.ttf` & `ryven-3.5.0/ryven/resources/fonts/asap/Asap-Italic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/asap/Asap-Medium.ttf` & `ryven-3.5.0/ryven/resources/fonts/asap/Asap-Medium.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/asap/Asap-MediumItalic.ttf` & `ryven-3.5.0/ryven/resources/fonts/asap/Asap-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/asap/Asap-Regular.ttf` & `ryven-3.5.0/ryven/resources/fonts/asap/Asap-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/asap/Asap-SemiBold.ttf` & `ryven-3.5.0/ryven/resources/fonts/asap/Asap-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/asap/Asap-SemiBoldItalic.ttf` & `ryven-3.5.0/ryven/resources/fonts/asap/Asap-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/asap/OFL.txt` & `ryven-3.5.0/ryven/resources/fonts/asap/OFL.txt`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/poppins/OFL.txt` & `ryven-3.5.0/ryven/resources/fonts/poppins/OFL.txt`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-Black.ttf` & `ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-Black.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-BlackItalic.ttf` & `ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-Bold.ttf` & `ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-Bold.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-BoldItalic.ttf` & `ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-ExtraBold.ttf` & `ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-ExtraBold.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-ExtraBoldItalic.ttf` & `ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-ExtraBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-ExtraLight.ttf` & `ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-ExtraLightItalic.ttf` & `ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-Italic.ttf` & `ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-Italic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-Light.ttf` & `ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-Light.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-LightItalic.ttf` & `ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-Medium.ttf` & `ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-Medium.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-MediumItalic.ttf` & `ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-Regular.ttf` & `ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-SemiBold.ttf` & `ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-SemiBoldItalic.ttf` & `ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-Thin.ttf` & `ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-Thin.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/poppins/Poppins-ThinItalic.ttf` & `ryven-3.5.0/ryven/resources/fonts/poppins/Poppins-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/source_code_pro/OFL.txt` & `ryven-3.5.0/ryven/resources/fonts/source_code_pro/OFL.txt`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/source_code_pro/SourceCodePro-Black.ttf` & `ryven-3.5.0/ryven/resources/fonts/source_code_pro/SourceCodePro-Black.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/source_code_pro/SourceCodePro-BlackItalic.ttf` & `ryven-3.5.0/ryven/resources/fonts/source_code_pro/SourceCodePro-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/source_code_pro/SourceCodePro-Bold.ttf` & `ryven-3.5.0/ryven/resources/fonts/source_code_pro/SourceCodePro-Bold.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/source_code_pro/SourceCodePro-BoldItalic.ttf` & `ryven-3.5.0/ryven/resources/fonts/source_code_pro/SourceCodePro-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/source_code_pro/SourceCodePro-ExtraLight.ttf` & `ryven-3.5.0/ryven/resources/fonts/source_code_pro/SourceCodePro-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/source_code_pro/SourceCodePro-ExtraLightItalic.ttf` & `ryven-3.5.0/ryven/resources/fonts/source_code_pro/SourceCodePro-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/source_code_pro/SourceCodePro-Italic.ttf` & `ryven-3.5.0/ryven/resources/fonts/source_code_pro/SourceCodePro-Italic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/source_code_pro/SourceCodePro-Light.ttf` & `ryven-3.5.0/ryven/resources/fonts/source_code_pro/SourceCodePro-Light.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/source_code_pro/SourceCodePro-LightItalic.ttf` & `ryven-3.5.0/ryven/resources/fonts/source_code_pro/SourceCodePro-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/source_code_pro/SourceCodePro-Medium.ttf` & `ryven-3.5.0/ryven/resources/fonts/source_code_pro/SourceCodePro-Medium.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/source_code_pro/SourceCodePro-MediumItalic.ttf` & `ryven-3.5.0/ryven/resources/fonts/source_code_pro/SourceCodePro-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/source_code_pro/SourceCodePro-Regular.ttf` & `ryven-3.5.0/ryven/resources/fonts/source_code_pro/SourceCodePro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/source_code_pro/SourceCodePro-SemiBold.ttf` & `ryven-3.5.0/ryven/resources/fonts/source_code_pro/SourceCodePro-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/fonts/source_code_pro/SourceCodePro-SemiBoldItalic.ttf` & `ryven-3.5.0/ryven/resources/fonts/source_code_pro/SourceCodePro-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/pics/Ryven_icon.jpg` & `ryven-3.5.0/ryven/resources/pics/Ryven_icon.jpg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/pics/Ryven_icon.png` & `ryven-3.5.0/ryven/resources/pics/Ryven_icon.png`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/pics/Ryven_icon_blurred.png` & `ryven-3.5.0/ryven/resources/pics/Ryven_icon_blurred.png`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/pics/logo.png` & `ryven-3.5.0/ryven/resources/pics/logo.png`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/branch-closed.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/branch-closed.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/branch-end.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/branch-end.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/branch-more.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/branch-more.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/branch-open.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/branch-open.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/checkbox_checked.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/checkbox_checked.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/checkbox_indeterminate.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/checkbox_indeterminate.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/checkbox_unchecked.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/checkbox_unchecked.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/close.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/close.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/downarrow.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/downarrow.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/downarrow2.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/downarrow2.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/float.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/float.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/leftarrow.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/leftarrow.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/leftarrow2.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/leftarrow2.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/orig/base.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/orig/base.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/orig/branch-closed.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/orig/branch-closed.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/orig/branch-end.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/orig/branch-end.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/orig/branch-more.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/orig/branch-more.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/orig/branch-open.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/orig/branch-open.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/orig/checkbox_checked.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/orig/checkbox_checked.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/orig/checkbox_indeterminate.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/orig/checkbox_indeterminate.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/orig/checkbox_unchecked.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/orig/checkbox_unchecked.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/orig/close.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/orig/close.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/orig/downarrow.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/orig/downarrow.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/orig/downarrow2.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/orig/downarrow2.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/orig/float.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/orig/float.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/orig/leftarrow.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/orig/leftarrow.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/orig/leftarrow2.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/orig/leftarrow2.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/orig/radiobutton_checked.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/orig/radiobutton_checked.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/orig/radiobutton_unchecked.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/orig/radiobutton_unchecked.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/orig/rightarrow.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/orig/rightarrow.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/orig/rightarrow2.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/orig/rightarrow2.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/orig/sizegrip.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/orig/sizegrip.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/orig/slider.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/orig/slider.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/orig/splitter-horizontal.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/orig/splitter-horizontal.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/orig/splitter-vertical.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/orig/splitter-vertical.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/orig/tab_close.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/orig/tab_close.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/orig/toolbar-handle-horizontal.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/orig/toolbar-handle-horizontal.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/orig/toolbar-handle-vertical.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/orig/toolbar-handle-vertical.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/orig/uparrow.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/orig/uparrow.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/orig/uparrow2.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/orig/uparrow2.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/orig/vline.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/orig/vline.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/radiobutton_checked.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/radiobutton_checked.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/radiobutton_unchecked.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/radiobutton_unchecked.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/rightarrow.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/rightarrow.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/rightarrow2.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/rightarrow2.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/sizegrip.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/sizegrip.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/slider.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/slider.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/splitter-horizontal.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/splitter-horizontal.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/splitter-vertical.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/splitter-vertical.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/tab_close.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/tab_close.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/toolbar-handle-horizontal.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/toolbar-handle-horizontal.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/toolbar-handle-vertical.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/toolbar-handle-vertical.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/uparrow.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/uparrow.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/uparrow2.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/uparrow2.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/icons/vline.svg` & `ryven-3.5.0/ryven/resources/stylesheets/icons/vline.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/resources/stylesheets/style_template.css` & `ryven-3.5.0/ryven/resources/stylesheets/style_template.css`

 * *Files 0% similar despite different names*

```diff
@@ -320,14 +320,15 @@
   text-transform: uppercase;
   font-weight: bold;
 }
 
 QTabBar::tab {
   color: {{secondaryTextColor}};
   border: 0px;
+  min-width: 65px;
 }
 
 QTabBar::tab:bottom,
 QTabBar::tab:top{
   padding: 0 15px;
   height: 30px;
 }
```

### Comparing `ryven-3.4.3/ryven/unused/EditVal_Dialog.py` & `ryven-3.5.0/ryven/unused/EditVal_Dialog.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/unused/NodeDetailsWidget.py` & `ryven-3.5.0/ryven/unused/NodeDetailsWidget.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/unused/NodesTreeListWidget.py` & `ryven-3.5.0/ryven/unused/NodesTreeListWidget.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven/unused/test.stl` & `ryven-3.5.0/ryven/unused/test.stl`

 * *Files identical despite different names*

### Comparing `ryven-3.4.3/ryven.egg-info/PKG-INFO` & `ryven-3.5.0/ryven.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: ryven
-Version: 3.4.3
+Version: 3.5.0
 Summary: Flow-based visual scripting for Python
 Home-page: https://github.com/leon-thomm/Ryven
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
-Requires-Dist: ryvencore-qt==0.4.*
-Requires-Dist: ryvencore==0.4.*
+Requires-Dist: ryvencore-qt==0.5.*
+Requires-Dist: ryvencore==0.5.*
 Requires-Dist: Jinja2
 Requires-Dist: Pygments
 Requires-Dist: textdistance
 Requires-Dist: packaging
```

### Comparing `ryven-3.4.3/ryven.egg-info/SOURCES.txt` & `ryven-3.5.0/ryven.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 LICENSE
 MANIFEST.in
-pyproject.toml
 setup.cfg
 setup.py
 ryven/__init__.py
 ryven/gui_env.py
 ryven/node_env.py
 ryven.egg-info/PKG-INFO
 ryven.egg-info/SOURCES.txt
 ryven.egg-info/dependency_links.txt
 ryven.egg-info/entry_points.txt
 ryven.egg-info/requires.txt
 ryven.egg-info/top_level.txt
 ryven/example_nodes/OpenCV/README.md
 ryven/example_nodes/OpenCV/nodes.py
 ryven/example_nodes/OpenCV/widgets.py
+ryven/example_nodes/examples/README.md
+ryven/example_nodes/examples/__init__.py
+ryven/example_nodes/examples/basic_operators.py
+ryven/example_nodes/examples/control_structures.py
+ryven/example_nodes/examples/gui.py
+ryven/example_nodes/examples/nodes.py
+ryven/example_nodes/examples/special_nodes.py
+ryven/example_nodes/inspector_example/__init__.py
+ryven/example_nodes/inspector_example/gui.py
+ryven/example_nodes/inspector_example/nodes.py
 ryven/example_nodes/linalg/README.md
+ryven/example_nodes/linalg/__init__.py
 ryven/example_nodes/linalg/gui.py
+ryven/example_nodes/linalg/matrices.py
 ryven/example_nodes/linalg/nodes.py
-ryven/example_nodes/std/README.md
-ryven/example_nodes/std/basic_operators.py
-ryven/example_nodes/std/control_structures.py
-ryven/example_nodes/std/gui.py
-ryven/example_nodes/std/nodes.py
-ryven/example_nodes/std/special_nodes.py
-ryven/examples_projects/basics.json
-ryven/examples_projects/matrices.json
+ryven/example_projects/basics.json
+ryven/example_projects/matrices.json
 ryven/gui/__init__.py
 ryven/gui/dialogs.py
 ryven/gui/flow_ui.py
 ryven/gui/main_console.py
 ryven/gui/main_window.py
 ryven/gui/std_input_widgets.py
 ryven/gui/code_editor/CodeEditorWidget.py
@@ -44,16 +49,18 @@
 ryven/gui/startup_dialog/StartupDialog.py
 ryven/gui/startup_dialog/__init__.py
 ryven/gui/styling/__init__.py
 ryven/gui/styling/design_config.json
 ryven/gui/styling/window_theme.py
 ryven/gui/uic/__init__.py
 ryven/gui/uic/flow.ui
+ryven/gui/uic/flow_window.ui
 ryven/gui/uic/main_window.ui
 ryven/gui/uic/ui_flow.py
+ryven/gui/uic/ui_flow_window.py
 ryven/gui/uic/ui_main_window.py
 ryven/main/Ryven.py
 ryven/main/RyvenConsole.py
 ryven/main/__init__.py
 ryven/main/args_parser.py
 ryven/main/config.py
 ryven/main/utils.py
```

### Comparing `ryven-3.4.3/setup.cfg` & `ryven-3.5.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ryven
-version = 3.4.3
+version = 3.5.0
 author = Leon Thomm
 author_email = l.thomm@mailbox.org
 description = Flow-based visual scripting for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_files = 
 	LICENSE
@@ -15,23 +15,29 @@
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 include_package_data = True
-python_requires = >=3.6, <3.11
+python_requires = >=3.6, <3.13
 install_requires = 
-	ryvencore-qt ==0.4.*
-	ryvencore ==0.4.*
+	ryvencore-qt ==0.5.*
+	ryvencore ==0.5.*
 	Jinja2
 	Pygments
 	textdistance
 	packaging
 
+[optionas.extras_require]
+PySide2 = 
+	PySide2
+PySide6 = 
+	PySide6 = <6.7
+
 [options.entry_points]
 console_scripts = 
 	ryven = ryven:run_ryven
 	ryven-console = ryven:run_ryven_console
 
 [egg_info]
 tag_build =
```

### Comparing `ryven-3.4.3/setup.py` & `ryven-3.5.0/setup.py`

 * *Files identical despite different names*

