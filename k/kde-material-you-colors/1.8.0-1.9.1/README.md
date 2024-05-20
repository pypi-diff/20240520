# Comparing `tmp/kde-material-you-colors-1.8.0.tar.gz` & `tmp/kde_material_you_colors-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kde-material-you-colors-1.8.0.tar", last modified: Tue Mar 12 11:12:55 2024, max compression
+gzip compressed data, was "kde_material_you_colors-1.9.1.tar", last modified: Mon May 20 13:30:32 2024, max compression
```

## Comparing `kde-material-you-colors-1.8.0.tar` & `kde_material_you_colors-1.9.1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-03-12 11:12:55.947680 kde-material-you-colors-1.8.0/
--rw-r--r--   0 luis      (1000) luis      (1000)     6073 2024-02-14 22:52:49.000000 kde-material-you-colors-1.8.0/.clang-format
--rw-r--r--   0 luis      (1000) luis      (1000)      348 2023-07-30 22:23:15.000000 kde-material-you-colors-1.8.0/.editorconfig
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-03-12 11:12:55.934347 kde-material-you-colors-1.8.0/.github/
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-03-12 11:12:55.937680 kde-material-you-colors-1.8.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 luis      (1000) luis      (1000)      895 2022-08-21 04:50:25.000000 kde-material-you-colors-1.8.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 luis      (1000) luis      (1000)      595 2022-08-21 04:50:25.000000 kde-material-you-colors-1.8.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 luis      (1000) luis      (1000)     2164 2024-02-14 22:52:49.000000 kde-material-you-colors-1.8.0/.gitignore
--rw-r--r--   0 luis      (1000) luis      (1000)     1933 2023-07-30 22:23:15.000000 kde-material-you-colors-1.8.0/.pylintrc
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-03-12 11:12:55.937680 kde-material-you-colors-1.8.0/.vscode/
--rw-r--r--   0 luis      (1000) luis      (1000)      318 2024-02-14 22:52:49.000000 kde-material-you-colors-1.8.0/.vscode/c_cpp_properties.json
--rw-r--r--   0 luis      (1000) luis      (1000)      168 2024-02-14 22:52:49.000000 kde-material-you-colors-1.8.0/.vscode/extensions.json
--rw-r--r--   0 luis      (1000) luis      (1000)      612 2024-02-14 22:52:49.000000 kde-material-you-colors-1.8.0/.vscode/settings.json
--rw-r--r--   0 luis      (1000) luis      (1000)      697 2024-03-12 00:08:30.000000 kde-material-you-colors-1.8.0/CMakeLists.txt
--rw-r--r--   0 luis      (1000) luis      (1000)      841 2023-12-11 20:10:40.000000 kde-material-you-colors-1.8.0/CONTRIBUTING.md
--rw-r--r--   0 luis      (1000) luis      (1000)    35149 2022-08-21 04:50:25.000000 kde-material-you-colors-1.8.0/LICENSE
--rw-r--r--   0 luis      (1000) luis      (1000)       99 2024-02-14 22:52:49.000000 kde-material-you-colors-1.8.0/MANIFEST.in
--rw-r--r--   0 luis      (1000) luis      (1000)     9594 2024-03-12 11:12:55.944347 kde-material-you-colors-1.8.0/PKG-INFO
--rw-r--r--   0 luis      (1000) luis      (1000)     8555 2024-03-11 22:59:10.000000 kde-material-you-colors-1.8.0/README.md
--rw-r--r--   0 luis      (1000) luis      (1000)     1265 2024-02-14 22:52:49.000000 kde-material-you-colors-1.8.0/pyproject.toml
--rw-r--r--   0 luis      (1000) luis      (1000)       38 2024-03-12 11:12:55.947680 kde-material-you-colors-1.8.0/setup.cfg
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-03-12 11:12:55.934347 kde-material-you-colors-1.8.0/src/
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-03-12 11:12:55.937680 kde-material-you-colors-1.8.0/src/kde_material_you_colors/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-12-17 07:46:06.000000 kde-material-you-colors-1.8.0/src/kde_material_you_colors/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)     3048 2024-02-14 22:52:49.000000 kde-material-you-colors-1.8.0/src/kde_material_you_colors/apply_themes.py
--rw-r--r--   0 luis      (1000) luis      (1000)     8639 2024-03-12 06:45:58.000000 kde-material-you-colors-1.8.0/src/kde_material_you_colors/config.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-03-12 11:12:55.941014 kde-material-you-colors-1.8.0/src/kde_material_you_colors/data/
--rw-r--r--   0 luis      (1000) luis      (1000)      233 2023-08-17 21:29:39.000000 kde-material-you-colors-1.8.0/src/kde_material_you_colors/data/kde-material-you-colors-stop.desktop
--rw-r--r--   0 luis      (1000) luis      (1000)      183 2024-02-14 22:52:49.000000 kde-material-you-colors-1.8.0/src/kde_material_you_colors/data/kde-material-you-colors.desktop
--rw-r--r--   0 luis      (1000) luis      (1000)     6242 2024-02-14 22:52:49.000000 kde-material-you-colors-1.8.0/src/kde_material_you_colors/data/sample_config.conf
--rw-r--r--   0 luis      (1000) luis      (1000)     3724 2024-02-14 22:49:41.000000 kde-material-you-colors-1.8.0/src/kde_material_you_colors/logging_config.py
--rwxr-xr-x   0 luis      (1000) luis      (1000)    14882 2024-03-12 00:38:31.000000 kde-material-you-colors-1.8.0/src/kde_material_you_colors/main.py
--rw-r--r--   0 luis      (1000) luis      (1000)    45901 2024-02-14 22:52:49.000000 kde-material-you-colors-1.8.0/src/kde_material_you_colors/schemeconfigs.py
--rw-r--r--   0 luis      (1000) luis      (1000)     3591 2024-03-12 10:46:09.000000 kde-material-you-colors-1.8.0/src/kde_material_you_colors/settings.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-03-12 11:12:55.944347 kde-material-you-colors-1.8.0/src/kde_material_you_colors/utils/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-08-13 17:02:44.000000 kde-material-you-colors-1.8.0/src/kde_material_you_colors/utils/__init.py__
--rw-r--r--   0 luis      (1000) luis      (1000)    10370 2024-02-14 22:52:49.000000 kde-material-you-colors-1.8.0/src/kde_material_you_colors/utils/color_utils.py
--rw-r--r--   0 luis      (1000) luis      (1000)      144 2023-08-13 17:02:44.000000 kde-material-you-colors-1.8.0/src/kde_material_you_colors/utils/config_utils.py
--rw-r--r--   0 luis      (1000) luis      (1000)     2344 2024-02-14 22:52:49.000000 kde-material-you-colors-1.8.0/src/kde_material_you_colors/utils/extra_image_utils.py
--rw-r--r--   0 luis      (1000) luis      (1000)     1705 2023-12-22 22:41:33.000000 kde-material-you-colors-1.8.0/src/kde_material_you_colors/utils/file_utils.py
--rw-r--r--   0 luis      (1000) luis      (1000)    11338 2024-02-14 22:49:41.000000 kde-material-you-colors-1.8.0/src/kde_material_you_colors/utils/konsole_utils.py
--rw-r--r--   0 luis      (1000) luis      (1000)      831 2023-12-13 11:12:48.000000 kde-material-you-colors-1.8.0/src/kde_material_you_colors/utils/ksyntax_utils.py
--rw-r--r--   0 luis      (1000) luis      (1000)     7017 2024-03-12 00:08:30.000000 kde-material-you-colors-1.8.0/src/kde_material_you_colors/utils/kwin_utils.py
--rw-r--r--   0 luis      (1000) luis      (1000)     7935 2024-02-14 22:52:49.000000 kde-material-you-colors-1.8.0/src/kde_material_you_colors/utils/m3_scheme_utils.py
--rw-r--r--   0 luis      (1000) luis      (1000)      171 2023-12-22 22:41:33.000000 kde-material-you-colors-1.8.0/src/kde_material_you_colors/utils/math_utils.py
--rw-r--r--   0 luis      (1000) luis      (1000)      668 2023-12-08 09:15:58.000000 kde-material-you-colors-1.8.0/src/kde_material_you_colors/utils/notify.py
--rw-r--r--   0 luis      (1000) luis      (1000)     8823 2023-12-22 22:41:33.000000 kde-material-you-colors-1.8.0/src/kde_material_you_colors/utils/plasma_utils.py
--rw-r--r--   0 luis      (1000) luis      (1000)     3960 2023-08-13 17:02:44.000000 kde-material-you-colors-1.8.0/src/kde_material_you_colors/utils/pywal_sequences_timeout.py
--rw-r--r--   0 luis      (1000) luis      (1000)     2256 2023-12-22 22:41:33.000000 kde-material-you-colors-1.8.0/src/kde_material_you_colors/utils/pywal_utils.py
--rw-r--r--   0 luis      (1000) luis      (1000)       53 2023-08-13 17:02:44.000000 kde-material-you-colors-1.8.0/src/kde_material_you_colors/utils/string_utils.py
--rw-r--r--   0 luis      (1000) luis      (1000)      777 2023-08-13 17:02:44.000000 kde-material-you-colors-1.8.0/src/kde_material_you_colors/utils/timeout_utils.py
--rw-r--r--   0 luis      (1000) luis      (1000)     9549 2023-12-22 22:41:33.000000 kde-material-you-colors-1.8.0/src/kde_material_you_colors/utils/titlebar_utils.py
--rw-r--r--   0 luis      (1000) luis      (1000)    11902 2024-02-14 22:52:49.000000 kde-material-you-colors-1.8.0/src/kde_material_you_colors/utils/utils.py
--rw-r--r--   0 luis      (1000) luis      (1000)    10763 2024-03-12 07:56:18.000000 kde-material-you-colors-1.8.0/src/kde_material_you_colors/utils/wallpaper_utils.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-03-12 11:12:55.944347 kde-material-you-colors-1.8.0/src/kde_material_you_colors.egg-info/
--rw-r--r--   0 luis      (1000) luis      (1000)     9594 2024-03-12 11:12:55.000000 kde-material-you-colors-1.8.0/src/kde_material_you_colors.egg-info/PKG-INFO
--rw-r--r--   0 luis      (1000) luis      (1000)     2804 2024-03-12 11:12:55.000000 kde-material-you-colors-1.8.0/src/kde_material_you_colors.egg-info/SOURCES.txt
--rw-r--r--   0 luis      (1000) luis      (1000)        1 2024-03-12 11:12:55.000000 kde-material-you-colors-1.8.0/src/kde_material_you_colors.egg-info/dependency_links.txt
--rw-r--r--   0 luis      (1000) luis      (1000)       78 2024-03-12 11:12:55.000000 kde-material-you-colors-1.8.0/src/kde_material_you_colors.egg-info/entry_points.txt
--rw-r--r--   0 luis      (1000) luis      (1000)       90 2024-03-12 11:12:55.000000 kde-material-you-colors-1.8.0/src/kde_material_you_colors.egg-info/requires.txt
--rw-r--r--   0 luis      (1000) luis      (1000)       51 2024-03-12 11:12:55.000000 kde-material-you-colors-1.8.0/src/kde_material_you_colors.egg-info/top_level.txt
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-03-12 11:12:55.944347 kde-material-you-colors-1.8.0/src/plasmoid/
--rw-r--r--   0 luis      (1000) luis      (1000)      872 2024-03-12 00:08:30.000000 kde-material-you-colors-1.8.0/src/plasmoid/CMakeLists.txt
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-03-12 11:12:55.944347 kde-material-you-colors-1.8.0/src/plasmoid/package/
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-03-12 11:12:55.934347 kde-material-you-colors-1.8.0/src/plasmoid/package/contents/
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-03-12 11:12:55.944347 kde-material-you-colors-1.8.0/src/plasmoid/package/contents/config/
--rw-r--r--   0 luis      (1000) luis      (1000)      205 2024-02-14 22:52:49.000000 kde-material-you-colors-1.8.0/src/plasmoid/package/contents/config/config.qml
--rw-r--r--   0 luis      (1000) luis      (1000)      412 2024-02-14 22:52:49.000000 kde-material-you-colors-1.8.0/src/plasmoid/package/contents/config/main.xml
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-03-12 11:12:55.944347 kde-material-you-colors-1.8.0/src/plasmoid/package/contents/icons/
--rw-r--r--   0 luis      (1000) luis      (1000)     3727 2024-02-14 22:52:49.000000 kde-material-you-colors-1.8.0/src/plasmoid/package/contents/icons/icon.svg
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-03-12 11:12:55.944347 kde-material-you-colors-1.8.0/src/plasmoid/package/contents/ui/
--rw-r--r--   0 luis      (1000) luis      (1000)      817 2024-03-12 10:27:25.000000 kde-material-you-colors-1.8.0/src/plasmoid/package/contents/ui/CompactRepresentation.qml
--rw-r--r--   0 luis      (1000) luis      (1000)    98067 2024-03-12 10:46:28.000000 kde-material-you-colors-1.8.0/src/plasmoid/package/contents/ui/FullRepresentation.qml
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-03-12 11:12:55.944347 kde-material-you-colors-1.8.0/src/plasmoid/package/contents/ui/components/
--rw-r--r--   0 luis      (1000) luis      (1000)     1955 2024-03-12 00:08:30.000000 kde-material-you-colors-1.8.0/src/plasmoid/package/contents/ui/components/CustomColorButton.qml
--rw-r--r--   0 luis      (1000) luis      (1000)      725 2024-02-14 22:52:49.000000 kde-material-you-colors-1.8.0/src/plasmoid/package/contents/ui/components/FadeBehavior.qml
--rw-r--r--   0 luis      (1000) luis      (1000)      541 2024-03-12 07:18:03.000000 kde-material-you-colors-1.8.0/src/plasmoid/package/contents/ui/components/PlasmoidIcon.qml
--rw-r--r--   0 luis      (1000) luis      (1000)     3083 2024-03-12 00:08:30.000000 kde-material-you-colors-1.8.0/src/plasmoid/package/contents/ui/configGeneral.qml
--rw-r--r--   0 luis      (1000) luis      (1000)     2186 2024-03-12 00:08:30.000000 kde-material-you-colors-1.8.0/src/plasmoid/package/contents/ui/main.qml
--rw-r--r--   0 luis      (1000) luis      (1000)      856 2024-03-12 10:46:54.000000 kde-material-you-colors-1.8.0/src/plasmoid/package/metadata.json
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-03-12 11:12:55.944347 kde-material-you-colors-1.8.0/src/screenshot_helper/
--rw-r--r--   0 luis      (1000) luis      (1000)      797 2024-03-12 00:08:30.000000 kde-material-you-colors-1.8.0/src/screenshot_helper/CMakeLists.txt
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-03-12 11:12:55.944347 kde-material-you-colors-1.8.0/src/screenshot_helper/desktop/
--rw-r--r--   0 luis      (1000) luis      (1000)      319 2024-02-14 22:52:49.000000 kde-material-you-colors-1.8.0/src/screenshot_helper/desktop/CMakeLists.txt
--rw-r--r--   0 luis      (1000) luis      (1000)      336 2024-02-14 22:52:49.000000 kde-material-you-colors-1.8.0/src/screenshot_helper/desktop/kde-material-you-colors-screenshot-helper.cmake
--rw-r--r--   0 luis      (1000) luis      (1000)     4834 2024-03-12 06:48:49.000000 kde-material-you-colors-1.8.0/src/screenshot_helper/main.cpp
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-05-20 13:30:32.547781 kde_material_you_colors-1.9.1/
+-rw-r--r--   0 luis      (1000) luis      (1000)     6073 2024-02-14 22:52:49.000000 kde_material_you_colors-1.9.1/.clang-format
+-rw-r--r--   0 luis      (1000) luis      (1000)      348 2023-07-30 22:23:15.000000 kde_material_you_colors-1.9.1/.editorconfig
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-05-20 13:30:32.524447 kde_material_you_colors-1.9.1/.github/
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-05-20 13:30:32.531114 kde_material_you_colors-1.9.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 luis      (1000) luis      (1000)      895 2022-08-21 04:50:25.000000 kde_material_you_colors-1.9.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 luis      (1000) luis      (1000)      595 2022-08-21 04:50:25.000000 kde_material_you_colors-1.9.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 luis      (1000) luis      (1000)     2176 2024-05-17 08:31:16.000000 kde_material_you_colors-1.9.1/.gitignore
+-rw-r--r--   0 luis      (1000) luis      (1000)     1933 2023-07-30 22:23:15.000000 kde_material_you_colors-1.9.1/.pylintrc
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-05-20 13:30:32.534448 kde_material_you_colors-1.9.1/.vscode/
+-rw-r--r--   0 luis      (1000) luis      (1000)      318 2024-02-14 22:52:49.000000 kde_material_you_colors-1.9.1/.vscode/c_cpp_properties.json
+-rw-r--r--   0 luis      (1000) luis      (1000)      168 2024-02-14 22:52:49.000000 kde_material_you_colors-1.9.1/.vscode/extensions.json
+-rw-r--r--   0 luis      (1000) luis      (1000)      612 2024-02-14 22:52:49.000000 kde_material_you_colors-1.9.1/.vscode/settings.json
+-rw-r--r--   0 luis      (1000) luis      (1000)      655 2024-05-17 01:20:58.000000 kde_material_you_colors-1.9.1/CMakeLists.txt
+-rw-r--r--   0 luis      (1000) luis      (1000)      841 2023-12-11 20:10:40.000000 kde_material_you_colors-1.9.1/CONTRIBUTING.md
+-rw-r--r--   0 luis      (1000) luis      (1000)    35149 2022-08-21 04:50:25.000000 kde_material_you_colors-1.9.1/LICENSE
+-rw-r--r--   0 luis      (1000) luis      (1000)       99 2024-02-14 22:52:49.000000 kde_material_you_colors-1.9.1/MANIFEST.in
+-rw-r--r--   0 luis      (1000) luis      (1000)    11290 2024-05-20 13:30:32.547781 kde_material_you_colors-1.9.1/PKG-INFO
+-rw-r--r--   0 luis      (1000) luis      (1000)    10237 2024-05-20 09:32:12.000000 kde_material_you_colors-1.9.1/README.md
+-rw-r--r--   0 luis      (1000) luis      (1000)     1271 2024-05-17 01:20:58.000000 kde_material_you_colors-1.9.1/pyproject.toml
+-rw-r--r--   0 luis      (1000) luis      (1000)       38 2024-05-20 13:30:32.547781 kde_material_you_colors-1.9.1/setup.cfg
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-05-20 13:30:32.527781 kde_material_you_colors-1.9.1/src/
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-05-20 13:30:32.534448 kde_material_you_colors-1.9.1/src/kde_material_you_colors/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-12-17 07:46:06.000000 kde_material_you_colors-1.9.1/src/kde_material_you_colors/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     3699 2024-05-20 08:41:35.000000 kde_material_you_colors-1.9.1/src/kde_material_you_colors/apply_themes.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     8932 2024-05-20 08:37:26.000000 kde_material_you_colors-1.9.1/src/kde_material_you_colors/config.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-05-20 13:30:32.537781 kde_material_you_colors-1.9.1/src/kde_material_you_colors/data/
+-rw-r--r--   0 luis      (1000) luis      (1000)      233 2023-08-17 21:29:39.000000 kde_material_you_colors-1.9.1/src/kde_material_you_colors/data/kde-material-you-colors-stop.desktop
+-rw-r--r--   0 luis      (1000) luis      (1000)      183 2024-02-14 22:52:49.000000 kde_material_you_colors-1.9.1/src/kde_material_you_colors/data/kde-material-you-colors.desktop
+-rw-r--r--   0 luis      (1000) luis      (1000)     6865 2024-05-20 09:04:09.000000 kde_material_you_colors-1.9.1/src/kde_material_you_colors/data/sample_config.conf
+-rw-r--r--   0 luis      (1000) luis      (1000)     3746 2024-05-17 08:51:59.000000 kde_material_you_colors-1.9.1/src/kde_material_you_colors/logging_config.py
+-rwxr-xr-x   0 luis      (1000) luis      (1000)    15909 2024-05-20 08:00:13.000000 kde_material_you_colors-1.9.1/src/kde_material_you_colors/main.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    41111 2024-05-18 10:05:19.000000 kde_material_you_colors-1.9.1/src/kde_material_you_colors/schemeconfigs.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     3591 2024-05-20 10:35:26.000000 kde_material_you_colors-1.9.1/src/kde_material_you_colors/settings.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-05-20 13:30:32.541114 kde_material_you_colors-1.9.1/src/kde_material_you_colors/utils/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-08-13 17:02:44.000000 kde_material_you_colors-1.9.1/src/kde_material_you_colors/utils/__init.py__
+-rw-r--r--   0 luis      (1000) luis      (1000)    11876 2024-05-18 11:47:37.000000 kde_material_you_colors-1.9.1/src/kde_material_you_colors/utils/color_utils.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      144 2023-08-13 17:02:44.000000 kde_material_you_colors-1.9.1/src/kde_material_you_colors/utils/config_utils.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     1021 2024-05-17 01:20:58.000000 kde_material_you_colors-1.9.1/src/kde_material_you_colors/utils/extra_image_utils.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     1705 2023-12-22 22:41:33.000000 kde_material_you_colors-1.9.1/src/kde_material_you_colors/utils/file_utils.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    11510 2024-05-20 08:29:12.000000 kde_material_you_colors-1.9.1/src/kde_material_you_colors/utils/konsole_utils.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      922 2024-05-18 10:05:19.000000 kde_material_you_colors-1.9.1/src/kde_material_you_colors/utils/ksyntax_utils.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     7213 2024-05-20 09:17:30.000000 kde_material_you_colors-1.9.1/src/kde_material_you_colors/utils/kwin_utils.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    11313 2024-05-18 12:32:20.000000 kde_material_you_colors-1.9.1/src/kde_material_you_colors/utils/m3_scheme_utils.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      171 2024-05-18 11:47:39.000000 kde_material_you_colors-1.9.1/src/kde_material_you_colors/utils/math_utils.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      668 2024-05-17 23:16:45.000000 kde_material_you_colors-1.9.1/src/kde_material_you_colors/utils/notify.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     8847 2024-05-17 08:58:32.000000 kde_material_you_colors-1.9.1/src/kde_material_you_colors/utils/plasma_utils.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     3960 2024-05-17 12:15:20.000000 kde_material_you_colors-1.9.1/src/kde_material_you_colors/utils/pywal_sequences_timeout.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     2356 2024-05-18 10:05:19.000000 kde_material_you_colors-1.9.1/src/kde_material_you_colors/utils/pywal_utils.py
+-rw-r--r--   0 luis      (1000) luis      (1000)       53 2023-08-13 17:02:44.000000 kde_material_you_colors-1.9.1/src/kde_material_you_colors/utils/string_utils.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      777 2023-08-13 17:02:44.000000 kde_material_you_colors-1.9.1/src/kde_material_you_colors/utils/timeout_utils.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     9710 2024-05-19 00:22:18.000000 kde_material_you_colors-1.9.1/src/kde_material_you_colors/utils/titlebar_utils.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    12312 2024-05-20 08:12:45.000000 kde_material_you_colors-1.9.1/src/kde_material_you_colors/utils/utils.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    11309 2024-05-20 09:21:27.000000 kde_material_you_colors-1.9.1/src/kde_material_you_colors/utils/wallpaper_utils.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-05-20 13:30:32.547781 kde_material_you_colors-1.9.1/src/kde_material_you_colors.egg-info/
+-rw-r--r--   0 luis      (1000) luis      (1000)    11290 2024-05-20 13:30:32.000000 kde_material_you_colors-1.9.1/src/kde_material_you_colors.egg-info/PKG-INFO
+-rw-r--r--   0 luis      (1000) luis      (1000)     2804 2024-05-20 13:30:32.000000 kde_material_you_colors-1.9.1/src/kde_material_you_colors.egg-info/SOURCES.txt
+-rw-r--r--   0 luis      (1000) luis      (1000)        1 2024-05-20 13:30:32.000000 kde_material_you_colors-1.9.1/src/kde_material_you_colors.egg-info/dependency_links.txt
+-rw-r--r--   0 luis      (1000) luis      (1000)       78 2024-05-20 13:30:32.000000 kde_material_you_colors-1.9.1/src/kde_material_you_colors.egg-info/entry_points.txt
+-rw-r--r--   0 luis      (1000) luis      (1000)       89 2024-05-20 13:30:32.000000 kde_material_you_colors-1.9.1/src/kde_material_you_colors.egg-info/requires.txt
+-rw-r--r--   0 luis      (1000) luis      (1000)       51 2024-05-20 13:30:32.000000 kde_material_you_colors-1.9.1/src/kde_material_you_colors.egg-info/top_level.txt
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-05-20 13:30:32.541114 kde_material_you_colors-1.9.1/src/plasmoid/
+-rw-r--r--   0 luis      (1000) luis      (1000)      872 2024-05-17 01:20:58.000000 kde_material_you_colors-1.9.1/src/plasmoid/CMakeLists.txt
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-05-20 13:30:32.544448 kde_material_you_colors-1.9.1/src/plasmoid/package/
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-05-20 13:30:32.524447 kde_material_you_colors-1.9.1/src/plasmoid/package/contents/
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-05-20 13:30:32.544448 kde_material_you_colors-1.9.1/src/plasmoid/package/contents/config/
+-rw-r--r--   0 luis      (1000) luis      (1000)      205 2024-02-14 22:52:49.000000 kde_material_you_colors-1.9.1/src/plasmoid/package/contents/config/config.qml
+-rw-r--r--   0 luis      (1000) luis      (1000)      412 2024-02-14 22:52:49.000000 kde_material_you_colors-1.9.1/src/plasmoid/package/contents/config/main.xml
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-05-20 13:30:32.544448 kde_material_you_colors-1.9.1/src/plasmoid/package/contents/icons/
+-rw-r--r--   0 luis      (1000) luis      (1000)     3727 2024-02-14 22:52:49.000000 kde_material_you_colors-1.9.1/src/plasmoid/package/contents/icons/icon.svg
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-05-20 13:30:32.544448 kde_material_you_colors-1.9.1/src/plasmoid/package/contents/ui/
+-rw-r--r--   0 luis      (1000) luis      (1000)      817 2024-05-17 01:20:58.000000 kde_material_you_colors-1.9.1/src/plasmoid/package/contents/ui/CompactRepresentation.qml
+-rw-r--r--   0 luis      (1000) luis      (1000)   104273 2024-05-20 10:37:08.000000 kde_material_you_colors-1.9.1/src/plasmoid/package/contents/ui/FullRepresentation.qml
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-05-20 13:30:32.544448 kde_material_you_colors-1.9.1/src/plasmoid/package/contents/ui/components/
+-rw-r--r--   0 luis      (1000) luis      (1000)     1955 2024-05-17 01:20:58.000000 kde_material_you_colors-1.9.1/src/plasmoid/package/contents/ui/components/CustomColorButton.qml
+-rw-r--r--   0 luis      (1000) luis      (1000)      725 2024-02-14 22:52:49.000000 kde_material_you_colors-1.9.1/src/plasmoid/package/contents/ui/components/FadeBehavior.qml
+-rw-r--r--   0 luis      (1000) luis      (1000)      541 2024-05-17 01:20:58.000000 kde_material_you_colors-1.9.1/src/plasmoid/package/contents/ui/components/PlasmoidIcon.qml
+-rw-r--r--   0 luis      (1000) luis      (1000)     3083 2024-05-17 01:20:58.000000 kde_material_you_colors-1.9.1/src/plasmoid/package/contents/ui/configGeneral.qml
+-rw-r--r--   0 luis      (1000) luis      (1000)     2186 2024-05-17 01:20:58.000000 kde_material_you_colors-1.9.1/src/plasmoid/package/contents/ui/main.qml
+-rw-r--r--   0 luis      (1000) luis      (1000)      856 2024-05-20 10:36:45.000000 kde_material_you_colors-1.9.1/src/plasmoid/package/metadata.json
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-05-20 13:30:32.544448 kde_material_you_colors-1.9.1/src/screenshot_helper/
+-rw-r--r--   0 luis      (1000) luis      (1000)      995 2024-05-17 01:20:58.000000 kde_material_you_colors-1.9.1/src/screenshot_helper/CMakeLists.txt
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2024-05-20 13:30:32.547781 kde_material_you_colors-1.9.1/src/screenshot_helper/desktop/
+-rw-r--r--   0 luis      (1000) luis      (1000)      319 2024-02-14 22:52:49.000000 kde_material_you_colors-1.9.1/src/screenshot_helper/desktop/CMakeLists.txt
+-rw-r--r--   0 luis      (1000) luis      (1000)      336 2024-02-14 22:52:49.000000 kde_material_you_colors-1.9.1/src/screenshot_helper/desktop/kde-material-you-colors-screenshot-helper.cmake
+-rw-r--r--   0 luis      (1000) luis      (1000)     4834 2024-03-22 08:24:36.000000 kde_material_you_colors-1.9.1/src/screenshot_helper/main.cpp
```

### Comparing `kde-material-you-colors-1.8.0/.clang-format` & `kde_material_you_colors-1.9.1/.clang-format`

 * *Files identical despite different names*

### Comparing `kde-material-you-colors-1.8.0/.github/ISSUE_TEMPLATE/bug_report.md` & `kde_material_you_colors-1.9.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kde-material-you-colors-1.8.0/.github/ISSUE_TEMPLATE/feature_request.md` & `kde_material_you_colors-1.9.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `kde-material-you-colors-1.8.0/.gitignore` & `kde_material_you_colors-1.9.1/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -165,7 +165,8 @@
 # Executables
 *.exe
 *.out
 *.app
 
 compile_commands.json
 CMakeUserPresets.json
+playground/
```

### Comparing `kde-material-you-colors-1.8.0/.pylintrc` & `kde_material_you_colors-1.9.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `kde-material-you-colors-1.8.0/.vscode/settings.json` & `kde_material_you_colors-1.9.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `kde-material-you-colors-1.8.0/CMakeLists.txt` & `kde_material_you_colors-1.9.1/CMakeLists.txt`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 set(PROJECT_DEP_VERSION "6.0.0")
 set(QT_MIN_VERSION "6.6.0")
 set(KF6_MIN_VERSION "6.0.0")
 set(KDE_COMPILERSETTINGS_LEVEL "5.85")
 
 find_package(ECM ${KF6_MIN_VERSION} REQUIRED NO_MODULE)
-set(CMAKE_MODULE_PATH ${ECM_MODULE_PATH} ${CMAKE_CURRENT_SOURCE_DIR}/cmake/modules)
+set(CMAKE_MODULE_PATH ${ECM_MODULE_PATH})
 
 if(INSTALL_PLASMOID)
     find_package(Plasma5Support ${PROJECT_DEP_VERSION} REQUIRED)
     find_package(Plasma ${PROJECT_DEP_VERSION} REQUIRED)
 endif()
 
 add_subdirectory(src/screenshot_helper)
```

### Comparing `kde-material-you-colors-1.8.0/CONTRIBUTING.md` & `kde_material_you_colors-1.9.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `kde-material-you-colors-1.8.0/LICENSE` & `kde_material_you_colors-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kde-material-you-colors-1.8.0/PKG-INFO` & `kde_material_you_colors-1.9.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,195 +1,203 @@
-Metadata-Version: 2.1
-Name: kde-material-you-colors
-Version: 1.8.0
-Summary: Automatic Material You Colors Generator from your wallpaper for the Plasma Desktop
-Author-email: Luis Bocanegra <luisbocanegra17b@gmail.com>
-Project-URL: Homepage, https://github.com/luisbocanegra/kde-material-you-colors
-Project-URL: Repository, https://github.com/luisbocanegra/kde-material-you-colors
-Project-URL: Bug Tracker, https://github.com/luisbocanegra/kde-material-you-colors/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Topic :: Desktop Environment :: K Desktop Environment (KDE) :: Themes
-Classifier: Environment :: X11 Applications :: KDE
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: dbus-python>=1.3.2
-Requires-Dist: numpy>=1.20
-Requires-Dist: material-color-utilities-python>=0.1.5
-Provides-Extra: cli
-Requires-Dist: pywal>=3.3.0; extra == "cli"
-
 <div align="center">
 
 # 🎨 KDE Material You Colors
 
 <img src="https://github.com/luisbocanegra/kde-material-you-colors/assets/15076387/6bd4e04a-48a7-48bc-8dd1-3a75524cd10e" alt="Screenshot" height="250px">
 
-Automatically generate Light/Dark Color Themes for KDE (and pywal if installed) from your current wallpaper, using [Python implementation](https://github.com/avanishsubbiah/material-color-utilities-python) of Google's [Material Color Utilities](https://github.com/material-foundation/material-color-utilities)
+Automatically generate light/dark color themes for KDE (and pywal if installed) from your current wallpaper, using [@T-Dynamos Python implementation](https://github.com/T-Dynamos/materialyoucolor-python) of Google's [Material Color Utilities](https://github.com/material-foundation/material-color-utilities)
 
 [![AUR version](https://img.shields.io/aur/version/kde-material-you-colors?style=for-the-badge&logo=archlinux&labelColor=2d333b&color=1f425f)](https://aur.archlinux.org/packages/kde-material-you-colors)
 [![PyPI - Version](https://img.shields.io/pypi/v/kde-material-you-colors?style=for-the-badge&logo=python&labelColor=2d333b&color=1f425f)](https://pypi.org/project/kde-material-you-colors/)
-[![Dynamic JSON Badge](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fraw.githubusercontent.com%2Fluisbocanegra%2Fkde-material-you-colors%2Fmain%2Fsrc%2Fplasmoid%2Fpackage%2Fmetadata.json&query=KPlugin.Version&style=for-the-badge&color=1f425f&labelColor=2d333b&logo=kde&label=Plasmoid)](https://store.kde.org/p/2073783)
+[![Dynamic JSON Badge](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fraw.githubusercontent.com%2Fluisbocanegra%2Fkde-material-you-colors%2Fmain%2Fsrc%2Fplasmoid%2Fpackage%2Fmetadata.json&query=KPlugin.Version&style=for-the-badge&color=1f425f&labelColor=2d333b&logo=kde&label=Plasmoid)](https://store.kde.org/p/2136963)
 
 </div>
 
 [![Screenshots](https://user-images.githubusercontent.com/15076387/188578458-8171e42b-f36c-44c1-9eb0-506c301d4f16.gif)](https://user-images.githubusercontent.com/15076387/188578458-8171e42b-f36c-44c1-9eb0-506c301d4f16.gif)
 
-# Features
+## Features
 
-## Plasma specific
+### Plasma specific
 
-- [Plasma Widget](https://store.kde.org/p/2073783)
+- [Plasma Widget](https://store.kde.org/p/2136963) (Plasma 6 version)
 - Support for all Wallpaper plugins (color, image, slideshows, animated, Plasma 5.26+ dark wallpaper variants)
 - Update automatically on wallpaper change
 - Change icon themes
 - Start automatically on login
 - Make titlebar darker to match specified applications like terminals, code editors and other programs themed by pywal
 - Follow Plasma Material You Dark/Light change to work with theme schedulers like [Koi](https://github.com/baduhai/Koi)
 - **Plasma addons**
   - Tint [SierraBreeze](https://github.com/kay0u/SierraBreeze) window decoration buttons
   - TitleBar opacity control for [Klassy](https://github.com/paulmcauley/klassy) and [SierraBreezeEnhanced](https://github.com/kupiqu/SierraBreezeEnhanced) window decorations
   - ToolBar opacity control for [Lightly](https://github.com/Luwx/Lightly) Application style
   - Tint [Klassy](https://github.com/paulmcauley/klassy) window decoration outline
 
-## Themeable programs
+### Themeable programs
 
 - Konsole color scheme
   - opacity control
 - **[Pywal](https://github.com/dylanaraps/pywal) support to theme other programs using Material You Colors**
 - Basic KSyntaxHighlighting support (Kate, KWrite, KDevelop...)
 
-## Theming options
+### Theming options
 
 - Alternative Material You color selection if the wallpaper provides more than one
 - Use your favorite color to generate Material You color schemes
 - Custom colors list used for konsole/pywal
-- Custom amount for background color tint
+- Custom amount for colorfulness and brightness of theme
+- Color scheme variants from Material You (Vibrant, Monochrome, Neutral...)
 - Dark/light Color schemes (Plasma and pywal/konsole independently)
 - Set a script that will be executed on start or wallpaper/dark/light/settings change
 - Configuration file
 
-# Installing
+## Installing
 
-## 1. Backend
+1. Install `pipx` system packages from your distribution packages.
 
-Using pypi with `pipx` (recommended) using this command,
-```sh
-pipx install kde-material-you-colors
-# Optional
-# pywal to theme other programs using Material You Colors
-pipx inject kde-material-you-colors pywal
-```
+2. Install the backend
 
-or `pip` using this command
-```sh
-pip install kde-material-you-colors
-# Optional
-# pywal to theme other programs using Material You Colors
-pip install pywal
-```
+    **For Plasma 5** this is the last version, development has switched to plasma 6
+
+    ```sh
+    pipx install kde-material-you-colors==1.7.1
+    pipx inject kde-material-you-colors pywal
+    ```
+
+    **For Plasma 6**
+
+    ```sh
+    pipx install kde-material-you-colors
+    pipx inject kde-material-you-colors pywal
+    # to upgrade to newer version
+    pipx upgrade kde-material-you-colors
+    ```
+
+    **Note:** You may need to install `gcc python-dbus-dev libglib2.0-dev` system packages or their equivalent for your distribution. Additionally, installing some libraries for Pillow may be necessary, see [Pillow docs](https://pillow.readthedocs.io/en/latest/installation.html#external-libraries)
+
+3. Install the widget from the KDE Store [Plasma 6 version](https://store.kde.org/p/2136963) | [Plasma 5 version](https://www.pling.com/p/2073783/)
+
+   1. **Right click on the Panel** > **Add Widgets** > **Get New Widgets** > **Download New Plasma Widgets**
+   2. **Search** for "**KDE Material You Colors**", install & add it to your Panel/Desktop.
+
+4. Install the screenshot helper. **Optional but recommended if you use other than default Image wallpaper plugin**
+
+    **Plasma 6**
+
+    Install `git extra-cmake-modules` system packages or their equivalent for your distribution.
 
-> [!IMPORTANT]
-> You may need to install `gcc python-dbus-dev libglib2.0-dev` system packages or their equivalent for your distribution. Additionally, installing some libraries for Pillow may be necessary, see [Pillow docs](https://pillow.readthedocs.io/en/latest/installation.html#external-libraries)
+    ```sh
+    git clone https://github.com/luisbocanegra/kde-material-you-colors
+    ./install-screenshot-helper.sh
+    ```
 
-## 2. Plasma widget and desktop screenshot helper (support for all wallpaper plugins)
+    **Plasma 5**
 
-Install `extra-cmake-modules qt5-qttools-devel kf5-plasma-devel` system packages or their equivalent for your distribution.
+    Install `git extra-cmake-modules` system packages or their equivalent for your distribution.
 
-### User install
+    ```sh
+    git clone https://github.com/luisbocanegra/kde-material-you-colors -b plasma5
+    ./install-screenshot-helper.sh
+    ```
+
+To upgrade to a new version repeat these steps.
+
+**Note:** When you upgrade te widget to a newer version it will inform you if it requires a new version of the backend.
+
+### Arch Linux
+
+- [AUR](https://aur.archlinux.org/packages/kde-material-you-colors) use your preferred AUR helper e.g:
 
 ```sh
-cmake -B build -S . -DCMAKE_INSTALL_PREFIX=~/.local -DINSTALL_PLASMOID=ON
-cmake --build build
-cmake --install build
+yay -S kde-material-you-colors
 ```
 
-### System-wide install
+## Running
+
+You can Start and change the configuration from the widget.
+
+### From terminal
 
 ```sh
-cmake -B build -S . -DCMAKE_INSTALL_PREFIX=/usr -DINSTALL_PLASMOID=ON
-cmake --build build
-sudo cmake --install build
+kde-material-you-colors
 ```
 
-> [!NOTE]
-> You can also install the widget from the [KDE Store](https://store.kde.org/p/2073783) and set `-DINSTALL_PLASMOID=OFF` in the command above
->
-> 1. Right click on panel > Add Widgets > Get New Widgets > Download New Plasma Widgets
-> 2. Search for "KDE Material You Colors"
+Run `kde-material-you-colors -h` to see the list of available options (Flags take precedence over configuration file)
 
-### Arch Linux
+### Starting/Stopping Desktop entries
 
-- [AUR](https://aur.archlinux.org/packages/kde-material-you-colors) use your preferred AUR helper
+**If not installed by your package manager**, run `kde-material-you-colors -cl`
 
-### Optional features
+- To start the program launch **KDE Material You Colors** from your applications list
+- To stop, launch **Stop KDE Material You Colors** from your applications list
 
-- Install the [pywal](https://pypi.org/project/pywal/) python module to theme other programs using Material You Colors
-  - Check [pywal Customization Wiki](https://github.com/dylanaraps/pywal/wiki/Customization) to theme supported programs
+### Running on Startup
 
-# Running from terminal to debug your configuration
+```sh
+kde-material-you-colors -a
+```
 
-- Run `kde-material-you-colors`
+#### Removing from autostart
 
-- Flags take precedence over configuration file, run `kde-material-you-colors -h` to see the list of available options
+1. Open **System Settings** > **Autostart**
+2. Remove **kde-material-you-colors** by clicking on the **Trash** button.
 
-## Starting/Stopping Desktop entries
+## Configuration file
 
-> [!NOTE]
-> **If not installed by your package manager**, run `kde-material-you-colors -cl` to copy desktop entries to ~/.local/share/applications/
+The preferred way to change the configuration is from the widget. If the configuration doesn't exist, it will be automatically created by the widget.
 
-- To start the program launch **KDE Material You Colors** from your applications list
-- To stop it launch **Stop KDE Material You Colors** from your applications list
+**Editing manually**
+
+The default configuration file can be created by running `kde-material-you-colors -c` the location is `~/.config/kde-material-you-colors/config.conf`
+
+Run `kde-material-you-colors` with no arguments from terminal to test your changes in real time.
 
-# Running on Startup
+Due to Qt limitations, comments are removed from the configuration file by the widget. **You can view the sample configuration file with comments [here](https://github.com/luisbocanegra/kde-material-you-colors/blob/main/src/kde_material_you_colors/data/sample_config.conf)**.
 
-After finishing the setup, you can make it run automatically on boot
+## FAQ
 
-1. Copy the default configuration to ~/.config/kde-material-you-colors/config.conf:
+**Q.** How does this different from Plasma's "**Accent Color From Wallpaper**" and "**Tint all colors with accent color**"?
 
-    `kde-material-you-colors -c`
+There are some key differences:
 
-2. Set the program to automatically start with Plasma:
+- Brighter accent/buttons colors
+- Option to choose another color if the wallpaper returns more than one
+- Can also apply colors to Konsole and pywal (both from wallpaper and custom ones)
+- Colors comparison https://imgur.com/a/a28uZka (kde-material-you-colors top, default tint option bottom)
 
-    `kde-material-you-colors -a`
+**Q.** Why there are duplicated color schemes in **System Settings**
 
-3. Reboot or logout/login and test the changes
+To update color with `plasma-apply-colorscheme` (utility provided by KDE developers), the file containing the new color scheme must have a different name than the current one, to workaround that, this program creates two color scheme files with different names, then applies one after the other. As a result you end up with duplicated color schemes and maybe some lag while updating schemes.
 
-## Removing from autostart
+**Q.** Can't get wallpaper colors of the default wallpaper
 
-1. Open `System Settings` > `Startup and Shutdown`
-2. Remove `kde-material-you-colors` by clicking on the `-` button.
+If you are using the default Image wallpaper plugin try changing the image to something else at least once first.
 
-# Configuration file
+**Q.** Slideshow wallpaper (or any other Plugin) doesn't update colors correctly
 
-- Copy default configuration: run `kde-material-you-colors -c`
-- Edit ~/.config/kde-material-you-colors/config.conf
-- Run `kde-material-you-colors` with no arguments from terminal to test it.
-- **You can view the sample configuration file [here](https://github.com/luisbocanegra/kde-material-you-colors/blob/main/src/kde_material_you_colors/data/sample_config.conf)**
+Try enabling **Only use screenshot method** from the widget **Advanced settings**
 
-# Notes
+**Q.** How does wallpaper detection work and why it fails sometimes?
 
-- To update color with `plasma-apply-colorscheme` (utility provided by plasma developers), the file containing the new color scheme must have a different name than the current one, to workaround this the program creates two scheme files with different names, then applies one after the other. As a result you end up with duplicated color schemes and maybe some lag while updating schemes.
+The wallpaper is obtained in the following order:
 
-- The wallpaper is obtained in the following order:
+- First, uses the [Plasma Desktop Scripting API](https://develop.kde.org/docs/plasma/scripting/api/) to read Wallpaper plugin configuration.
+- If the previous fails, the screenshot helper (if installed) is used
 
-  - First, uses the [Plasma Desktop Scripting API](https://develop.kde.org/docs/plasma/scripting/api/) to read Wallpaper plugin configuration.
-  - If the previous fails, the screenshot helper (if installed) is used
+The backend uses the [KWin Scripting API](https://develop.kde.org/docs/plasma/kwin/api/) and calls the screenshot helper to take a Screenshot of the Desktop view using the [KWin's Screenshot plugin](https://github.com/KDE/kwin/tree/master/src/plugins/screenshot)
 
-    The backend uses the [KWin Scripting API](https://develop.kde.org/docs/plasma/kwin/api/) and calls the screenshot helper to take a Screenshot of the Desktop view using the [KWin's Screenshot plugin](https://github.com/KDE/kwin/tree/master/src/plugins/screenshot)
+Both methods are somewhat robust but there are edge cases when detection will fail, which are [explained here](https://github.com/luisbocanegra/kde-material-you-colors/issues/187)
 
 ## Bug reporting / Feature requests / Contributing
 
-Please read the [Contributing guidelines in this repository](CONTRIBUTING.md)
+Please read the [Contributing guidelines in this repository](https://github.com/luisbocanegra/kde-material-you-colors/blob/main/CONTRIBUTING.md)
 
-# Credits
+## Credits
 
-- [Python Implementation](https://github.com/avanishsubbiah/material-color-utilities-python) of Material Color Utilities used by this project.
+- [@T-Dynamos Python Implementation](https://github.com/T-Dynamos/materialyoucolor-python) of Material Color Utilities used by this project.
+- [@avanisubbiah Python Implementation](https://github.com/avanishsubbiah/material-color-utilities-python) of Material Color Utilities (used until v1.8.0).
 - [Material Color Utilities](https://github.com/material-foundation/material-color-utilities)
 - [Pywal](https://github.com/dylanaraps/pywal) used to apply material colors to pywal supported software
 - [MaterialColorUtilities (C#)](https://github.com/albi005/MaterialColorUtilities) (used until v0.8.0).
 - [xdg-desktop-portal-kde](https://invent.kde.org/plasma/xdg-desktop-portal-kde) base for desktop screenshot helper.
 - [kdotool](https://github.com/jinliu/kdotool) base for getting desktop window id.
-- [Google LLC. / Pictogrammers](https://pictogrammers.com/library/mdi/) for the widget icon.
+- [Google LLC. / Pictogrammers](https://pictogrammers.com/library/mdi/) for the widget icon assets.
 - [This comment on Reddit](https://www.reddit.com/r/kde/comments/mg6wr4/comment/gssbtqe/?utm_source=share&utm_medium=web2x&context=3) and [ksetwallpaper](https://github.com/pashazz/ksetwallpaper) for the code to get the current Wallpaper that served me as inspiration.
```

### Comparing `kde-material-you-colors-1.8.0/README.md` & `kde_material_you_colors-1.9.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,173 +1,226 @@
+Metadata-Version: 2.1
+Name: kde-material-you-colors
+Version: 1.9.1
+Summary: Automatic Material You Colors Generator from your wallpaper for the Plasma Desktop
+Author-email: Luis Bocanegra <luisbocanegra17b@gmail.com>
+Project-URL: Homepage, https://github.com/luisbocanegra/kde-material-you-colors
+Project-URL: Repository, https://github.com/luisbocanegra/kde-material-you-colors
+Project-URL: Bug Tracker, https://github.com/luisbocanegra/kde-material-you-colors/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Topic :: Desktop Environment :: K Desktop Environment (KDE) :: Themes
+Classifier: Environment :: X11 Applications :: KDE
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: dbus-python>=1.3.2
+Requires-Dist: numpy>=1.20
+Requires-Dist: pillow>=9.2.0
+Requires-Dist: materialyoucolor>=2.0.8
+Provides-Extra: cli
+Requires-Dist: pywal>=3.3.0; extra == "cli"
+
 <div align="center">
 
 # 🎨 KDE Material You Colors
 
 <img src="https://github.com/luisbocanegra/kde-material-you-colors/assets/15076387/6bd4e04a-48a7-48bc-8dd1-3a75524cd10e" alt="Screenshot" height="250px">
 
-Automatically generate Light/Dark Color Themes for KDE (and pywal if installed) from your current wallpaper, using [Python implementation](https://github.com/avanishsubbiah/material-color-utilities-python) of Google's [Material Color Utilities](https://github.com/material-foundation/material-color-utilities)
+Automatically generate light/dark color themes for KDE (and pywal if installed) from your current wallpaper, using [@T-Dynamos Python implementation](https://github.com/T-Dynamos/materialyoucolor-python) of Google's [Material Color Utilities](https://github.com/material-foundation/material-color-utilities)
 
 [![AUR version](https://img.shields.io/aur/version/kde-material-you-colors?style=for-the-badge&logo=archlinux&labelColor=2d333b&color=1f425f)](https://aur.archlinux.org/packages/kde-material-you-colors)
 [![PyPI - Version](https://img.shields.io/pypi/v/kde-material-you-colors?style=for-the-badge&logo=python&labelColor=2d333b&color=1f425f)](https://pypi.org/project/kde-material-you-colors/)
-[![Dynamic JSON Badge](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fraw.githubusercontent.com%2Fluisbocanegra%2Fkde-material-you-colors%2Fmain%2Fsrc%2Fplasmoid%2Fpackage%2Fmetadata.json&query=KPlugin.Version&style=for-the-badge&color=1f425f&labelColor=2d333b&logo=kde&label=Plasmoid)](https://store.kde.org/p/2073783)
+[![Dynamic JSON Badge](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fraw.githubusercontent.com%2Fluisbocanegra%2Fkde-material-you-colors%2Fmain%2Fsrc%2Fplasmoid%2Fpackage%2Fmetadata.json&query=KPlugin.Version&style=for-the-badge&color=1f425f&labelColor=2d333b&logo=kde&label=Plasmoid)](https://store.kde.org/p/2136963)
 
 </div>
 
 [![Screenshots](https://user-images.githubusercontent.com/15076387/188578458-8171e42b-f36c-44c1-9eb0-506c301d4f16.gif)](https://user-images.githubusercontent.com/15076387/188578458-8171e42b-f36c-44c1-9eb0-506c301d4f16.gif)
 
-# Features
+## Features
 
-## Plasma specific
+### Plasma specific
 
-- [Plasma Widget](https://store.kde.org/p/2073783)
+- [Plasma Widget](https://store.kde.org/p/2136963) (Plasma 6 version)
 - Support for all Wallpaper plugins (color, image, slideshows, animated, Plasma 5.26+ dark wallpaper variants)
 - Update automatically on wallpaper change
 - Change icon themes
 - Start automatically on login
 - Make titlebar darker to match specified applications like terminals, code editors and other programs themed by pywal
 - Follow Plasma Material You Dark/Light change to work with theme schedulers like [Koi](https://github.com/baduhai/Koi)
 - **Plasma addons**
   - Tint [SierraBreeze](https://github.com/kay0u/SierraBreeze) window decoration buttons
   - TitleBar opacity control for [Klassy](https://github.com/paulmcauley/klassy) and [SierraBreezeEnhanced](https://github.com/kupiqu/SierraBreezeEnhanced) window decorations
   - ToolBar opacity control for [Lightly](https://github.com/Luwx/Lightly) Application style
   - Tint [Klassy](https://github.com/paulmcauley/klassy) window decoration outline
 
-## Themeable programs
+### Themeable programs
 
 - Konsole color scheme
   - opacity control
 - **[Pywal](https://github.com/dylanaraps/pywal) support to theme other programs using Material You Colors**
 - Basic KSyntaxHighlighting support (Kate, KWrite, KDevelop...)
 
-## Theming options
+### Theming options
 
 - Alternative Material You color selection if the wallpaper provides more than one
 - Use your favorite color to generate Material You color schemes
 - Custom colors list used for konsole/pywal
-- Custom amount for background color tint
+- Custom amount for colorfulness and brightness of theme
+- Color scheme variants from Material You (Vibrant, Monochrome, Neutral...)
 - Dark/light Color schemes (Plasma and pywal/konsole independently)
 - Set a script that will be executed on start or wallpaper/dark/light/settings change
 - Configuration file
 
-# Installing
+## Installing
 
-## 1. Backend
+1. Install `pipx` system packages from your distribution packages.
 
-Using pypi with `pipx` (recommended) using this command,
-```sh
-pipx install kde-material-you-colors
-# Optional
-# pywal to theme other programs using Material You Colors
-pipx inject kde-material-you-colors pywal
-```
+2. Install the backend
 
-or `pip` using this command
-```sh
-pip install kde-material-you-colors
-# Optional
-# pywal to theme other programs using Material You Colors
-pip install pywal
-```
+    **For Plasma 5** this is the last version, development has switched to plasma 6
+
+    ```sh
+    pipx install kde-material-you-colors==1.7.1
+    pipx inject kde-material-you-colors pywal
+    ```
+
+    **For Plasma 6**
+
+    ```sh
+    pipx install kde-material-you-colors
+    pipx inject kde-material-you-colors pywal
+    # to upgrade to newer version
+    pipx upgrade kde-material-you-colors
+    ```
+
+    **Note:** You may need to install `gcc python-dbus-dev libglib2.0-dev` system packages or their equivalent for your distribution. Additionally, installing some libraries for Pillow may be necessary, see [Pillow docs](https://pillow.readthedocs.io/en/latest/installation.html#external-libraries)
+
+3. Install the widget from the KDE Store [Plasma 6 version](https://store.kde.org/p/2136963) | [Plasma 5 version](https://www.pling.com/p/2073783/)
+
+   1. **Right click on the Panel** > **Add Widgets** > **Get New Widgets** > **Download New Plasma Widgets**
+   2. **Search** for "**KDE Material You Colors**", install & add it to your Panel/Desktop.
+
+4. Install the screenshot helper. **Optional but recommended if you use other than default Image wallpaper plugin**
+
+    **Plasma 6**
+
+    Install `git extra-cmake-modules` system packages or their equivalent for your distribution.
 
-> [!IMPORTANT]
-> You may need to install `gcc python-dbus-dev libglib2.0-dev` system packages or their equivalent for your distribution. Additionally, installing some libraries for Pillow may be necessary, see [Pillow docs](https://pillow.readthedocs.io/en/latest/installation.html#external-libraries)
+    ```sh
+    git clone https://github.com/luisbocanegra/kde-material-you-colors
+    ./install-screenshot-helper.sh
+    ```
 
-## 2. Plasma widget and desktop screenshot helper (support for all wallpaper plugins)
+    **Plasma 5**
 
-Install `extra-cmake-modules qt5-qttools-devel kf5-plasma-devel` system packages or their equivalent for your distribution.
+    Install `git extra-cmake-modules` system packages or their equivalent for your distribution.
 
-### User install
+    ```sh
+    git clone https://github.com/luisbocanegra/kde-material-you-colors -b plasma5
+    ./install-screenshot-helper.sh
+    ```
+
+To upgrade to a new version repeat these steps.
+
+**Note:** When you upgrade te widget to a newer version it will inform you if it requires a new version of the backend.
+
+### Arch Linux
+
+- [AUR](https://aur.archlinux.org/packages/kde-material-you-colors) use your preferred AUR helper e.g:
 
 ```sh
-cmake -B build -S . -DCMAKE_INSTALL_PREFIX=~/.local -DINSTALL_PLASMOID=ON
-cmake --build build
-cmake --install build
+yay -S kde-material-you-colors
 ```
 
-### System-wide install
+## Running
+
+You can Start and change the configuration from the widget.
+
+### From terminal
 
 ```sh
-cmake -B build -S . -DCMAKE_INSTALL_PREFIX=/usr -DINSTALL_PLASMOID=ON
-cmake --build build
-sudo cmake --install build
+kde-material-you-colors
 ```
 
-> [!NOTE]
-> You can also install the widget from the [KDE Store](https://store.kde.org/p/2073783) and set `-DINSTALL_PLASMOID=OFF` in the command above
->
-> 1. Right click on panel > Add Widgets > Get New Widgets > Download New Plasma Widgets
-> 2. Search for "KDE Material You Colors"
+Run `kde-material-you-colors -h` to see the list of available options (Flags take precedence over configuration file)
 
-### Arch Linux
+### Starting/Stopping Desktop entries
 
-- [AUR](https://aur.archlinux.org/packages/kde-material-you-colors) use your preferred AUR helper
+**If not installed by your package manager**, run `kde-material-you-colors -cl`
 
-### Optional features
+- To start the program launch **KDE Material You Colors** from your applications list
+- To stop, launch **Stop KDE Material You Colors** from your applications list
 
-- Install the [pywal](https://pypi.org/project/pywal/) python module to theme other programs using Material You Colors
-  - Check [pywal Customization Wiki](https://github.com/dylanaraps/pywal/wiki/Customization) to theme supported programs
+### Running on Startup
 
-# Running from terminal to debug your configuration
+```sh
+kde-material-you-colors -a
+```
 
-- Run `kde-material-you-colors`
+#### Removing from autostart
 
-- Flags take precedence over configuration file, run `kde-material-you-colors -h` to see the list of available options
+1. Open **System Settings** > **Autostart**
+2. Remove **kde-material-you-colors** by clicking on the **Trash** button.
 
-## Starting/Stopping Desktop entries
+## Configuration file
 
-> [!NOTE]
-> **If not installed by your package manager**, run `kde-material-you-colors -cl` to copy desktop entries to ~/.local/share/applications/
+The preferred way to change the configuration is from the widget. If the configuration doesn't exist, it will be automatically created by the widget.
 
-- To start the program launch **KDE Material You Colors** from your applications list
-- To stop it launch **Stop KDE Material You Colors** from your applications list
+**Editing manually**
+
+The default configuration file can be created by running `kde-material-you-colors -c` the location is `~/.config/kde-material-you-colors/config.conf`
+
+Run `kde-material-you-colors` with no arguments from terminal to test your changes in real time.
 
-# Running on Startup
+Due to Qt limitations, comments are removed from the configuration file by the widget. **You can view the sample configuration file with comments [here](https://github.com/luisbocanegra/kde-material-you-colors/blob/main/src/kde_material_you_colors/data/sample_config.conf)**.
 
-After finishing the setup, you can make it run automatically on boot
+## FAQ
 
-1. Copy the default configuration to ~/.config/kde-material-you-colors/config.conf:
+**Q.** How does this different from Plasma's "**Accent Color From Wallpaper**" and "**Tint all colors with accent color**"?
 
-    `kde-material-you-colors -c`
+There are some key differences:
 
-2. Set the program to automatically start with Plasma:
+- Brighter accent/buttons colors
+- Option to choose another color if the wallpaper returns more than one
+- Can also apply colors to Konsole and pywal (both from wallpaper and custom ones)
+- Colors comparison https://imgur.com/a/a28uZka (kde-material-you-colors top, default tint option bottom)
 
-    `kde-material-you-colors -a`
+**Q.** Why there are duplicated color schemes in **System Settings**
 
-3. Reboot or logout/login and test the changes
+To update color with `plasma-apply-colorscheme` (utility provided by KDE developers), the file containing the new color scheme must have a different name than the current one, to workaround that, this program creates two color scheme files with different names, then applies one after the other. As a result you end up with duplicated color schemes and maybe some lag while updating schemes.
 
-## Removing from autostart
+**Q.** Can't get wallpaper colors of the default wallpaper
 
-1. Open `System Settings` > `Startup and Shutdown`
-2. Remove `kde-material-you-colors` by clicking on the `-` button.
+If you are using the default Image wallpaper plugin try changing the image to something else at least once first.
 
-# Configuration file
+**Q.** Slideshow wallpaper (or any other Plugin) doesn't update colors correctly
 
-- Copy default configuration: run `kde-material-you-colors -c`
-- Edit ~/.config/kde-material-you-colors/config.conf
-- Run `kde-material-you-colors` with no arguments from terminal to test it.
-- **You can view the sample configuration file [here](https://github.com/luisbocanegra/kde-material-you-colors/blob/main/src/kde_material_you_colors/data/sample_config.conf)**
+Try enabling **Only use screenshot method** from the widget **Advanced settings**
 
-# Notes
+**Q.** How does wallpaper detection work and why it fails sometimes?
 
-- To update color with `plasma-apply-colorscheme` (utility provided by plasma developers), the file containing the new color scheme must have a different name than the current one, to workaround this the program creates two scheme files with different names, then applies one after the other. As a result you end up with duplicated color schemes and maybe some lag while updating schemes.
+The wallpaper is obtained in the following order:
 
-- The wallpaper is obtained in the following order:
+- First, uses the [Plasma Desktop Scripting API](https://develop.kde.org/docs/plasma/scripting/api/) to read Wallpaper plugin configuration.
+- If the previous fails, the screenshot helper (if installed) is used
 
-  - First, uses the [Plasma Desktop Scripting API](https://develop.kde.org/docs/plasma/scripting/api/) to read Wallpaper plugin configuration.
-  - If the previous fails, the screenshot helper (if installed) is used
+The backend uses the [KWin Scripting API](https://develop.kde.org/docs/plasma/kwin/api/) and calls the screenshot helper to take a Screenshot of the Desktop view using the [KWin's Screenshot plugin](https://github.com/KDE/kwin/tree/master/src/plugins/screenshot)
 
-    The backend uses the [KWin Scripting API](https://develop.kde.org/docs/plasma/kwin/api/) and calls the screenshot helper to take a Screenshot of the Desktop view using the [KWin's Screenshot plugin](https://github.com/KDE/kwin/tree/master/src/plugins/screenshot)
+Both methods are somewhat robust but there are edge cases when detection will fail, which are [explained here](https://github.com/luisbocanegra/kde-material-you-colors/issues/187)
 
 ## Bug reporting / Feature requests / Contributing
 
-Please read the [Contributing guidelines in this repository](CONTRIBUTING.md)
+Please read the [Contributing guidelines in this repository](https://github.com/luisbocanegra/kde-material-you-colors/blob/main/CONTRIBUTING.md)
 
-# Credits
+## Credits
 
-- [Python Implementation](https://github.com/avanishsubbiah/material-color-utilities-python) of Material Color Utilities used by this project.
+- [@T-Dynamos Python Implementation](https://github.com/T-Dynamos/materialyoucolor-python) of Material Color Utilities used by this project.
+- [@avanisubbiah Python Implementation](https://github.com/avanishsubbiah/material-color-utilities-python) of Material Color Utilities (used until v1.8.0).
 - [Material Color Utilities](https://github.com/material-foundation/material-color-utilities)
 - [Pywal](https://github.com/dylanaraps/pywal) used to apply material colors to pywal supported software
 - [MaterialColorUtilities (C#)](https://github.com/albi005/MaterialColorUtilities) (used until v0.8.0).
 - [xdg-desktop-portal-kde](https://invent.kde.org/plasma/xdg-desktop-portal-kde) base for desktop screenshot helper.
 - [kdotool](https://github.com/jinliu/kdotool) base for getting desktop window id.
-- [Google LLC. / Pictogrammers](https://pictogrammers.com/library/mdi/) for the widget icon.
+- [Google LLC. / Pictogrammers](https://pictogrammers.com/library/mdi/) for the widget icon assets.
 - [This comment on Reddit](https://www.reddit.com/r/kde/comments/mg6wr4/comment/gssbtqe/?utm_source=share&utm_medium=web2x&context=3) and [ksetwallpaper](https://github.com/pashazz/ksetwallpaper) for the code to get the current Wallpaper that served me as inspiration.
```

### Comparing `kde-material-you-colors-1.8.0/pyproject.toml` & `kde_material_you_colors-1.9.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,16 @@
     "Operating System :: POSIX :: Linux",
 ]
 requires-python = ">=3.8"
 
 dependencies = [
     "dbus-python>=1.3.2",
     "numpy>=1.20",
-    "material-color-utilities-python>=0.1.5",
+    "pillow>=9.2.0",
+    "materialyoucolor>=2.0.8",
 ]
 
 [tool.setuptools.dynamic]
 version = {attr = "kde_material_you_colors.settings.__version__"}
 
 [project.scripts]
 kde-material-you-colors = "kde_material_you_colors.main:main"
```

### Comparing `kde-material-you-colors-1.8.0/src/kde_material_you_colors/apply_themes.py` & `kde_material_you_colors-1.9.1/src/kde_material_you_colors/apply_themes.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,41 @@
-from . import schemeconfigs
-from .config import Configs
-from .utils.wallpaper_utils import WallpaperReader
-from .utils import (
+import logging
+from kde_material_you_colors import schemeconfigs
+from kde_material_you_colors.config import Configs
+from kde_material_you_colors.utils.wallpaper_utils import WallpaperReader
+from kde_material_you_colors.utils import (
     utils,
     m3_scheme_utils,
     pywal_utils,
     plasma_utils,
     konsole_utils,
     titlebar_utils,
     kwin_utils,
     ksyntax_utils,
 )
 
 
 def apply(config: Configs, wallpaper: WallpaperReader, dark_light):
     needs_kwin_reload = False
+    qdbus_executable = config.read("qdbus_executable")
+    if qdbus_executable is None:
+        qdbus_executable = "qdbus6"
+    if utils.find_executable(qdbus_executable) is None:
+        logging.error(
+            f"QDbus executable '{qdbus_executable}' wasn't found, there will be errors. Please set the correct one in the configuration"
+        )
+
     material_colors = m3_scheme_utils.get_color_schemes(
         wallpaper,
         config.read("ncolor"),
+        config.read("scheme_variant"),
+        config.read("chroma_multiplier"),
+        config.read("tone_multiplier"),
     )
+
     if material_colors is None:
         return
     schemes = schemeconfigs.ThemeConfig(
         material_colors,
         wallpaper.source,
         config.read("light_blend_multiplier"),
         config.read("dark_blend_multiplier"),
@@ -61,32 +74,34 @@
         pywal_light=config.read("pywal_light"),
         schemes=schemes,
         konsole_opacity=config.read("konsole_opacity"),
         konsole_opacity_dark=config.read("konsole_opacity_dark"),
         dark_light=dark_light,
     )
     if config.read("disable_konsole") is not True:
-        konsole_utils.apply_color_scheme()
+        konsole_utils.apply_color_scheme(qdbus_executable)
     if config.read("darker_window_list"):
         titlebar_utils.kwin_rule_darker_titlebar(
-            dark_light
-            if config.read("pywal_light") is None
-            else config.read("pywal_light"),
+            (
+                dark_light
+                if config.read("pywal_light") is None
+                else config.read("pywal_light")
+            ),
             config.read("darker_window_list"),
         )
     if config.read("pywal"):
         pywal_utils.apply_schemes(
             light=config.read("light"),
             use_pywal=config.read("pywal"),
             pywal_light=config.read("pywal_light"),
             schemes=schemes,
             dark_light=dark_light,
         )
     if needs_kwin_reload is True:
-        kwin_utils.reload()
+        kwin_utils.reload(qdbus_executable)
     pywal_utils.print_color_palette(
         light=config.read("light"),
         pywal_light=config.read("pywal_light"),
         schemes=schemes,
         dark_light=dark_light,
     )
     utils.run_hook(config.read("on_change_hook"))
```

### Comparing `kde-material-you-colors-1.8.0/src/kde_material_you_colors/config.py` & `kde_material_you_colors-1.9.1/src/kde_material_you_colors/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import configparser
 import logging
 import os
-from .utils import color_utils
-from .utils import math_utils
+from kde_material_you_colors.utils import color_utils
+from kde_material_you_colors.utils import math_utils
 
 
 class Configs:
     """Create configuration based on arguments and config file"""
 
     def __init__(self, args, config_file):
         self._args = args
@@ -128,15 +128,15 @@
     def read(self, key: str):
         if key in self._options:
             return self._options[key]
 
     @property
     def defaults(self):
         # property : [value, fallback, type]
-        # Types: 0 = bool, 1 = int, 2 = float, 3 = str
+        # Types: bool(0), int(1), float(2), str(3)
         args = self._args
         return {
             "light": [self._light, None, 0],
             "file": [args.file, None, 3],
             "monitor": [args.monitor, 0, 1],
             "ncolor": [args.ncolor, 0, 1],
             "iconslight": [args.iconslight, None, 3],
@@ -163,14 +163,18 @@
             "plasma_follows_scheme": [None, None, 0],
             "pywal_follows_scheme": [None, None, 0],
             "main_loop_delay": [args.main_loop_delay, 1, 2],
             "screenshot_delay": [args.screenshot_delay, 900, 2],
             "once_after_change": [args.once_after_change, False, 0],
             "pause_mode": [None, False, 0],
             "screenshot_only_mode": [args.screenshot_only_mode, False, 0],
+            "scheme_variant": [args.scheme_variant, 5, 1],
+            "chroma_multiplier": [args.chroma_multiplier, 1, 2],
+            "tone_multiplier": [args.tone_multiplier, 1, 2],
+            "qdbus_executable": [args.qdbus_executable, None, 3],
         }
 
     def parse_conf(self):
         """Create options dictionary from configuration or arguments/defaults"""
         for key, val in self.defaults.items():
             self._options[key] = self.eval_conf(
                 key=key,
```

### Comparing `kde-material-you-colors-1.8.0/src/kde_material_you_colors/data/sample_config.conf` & `kde_material_you_colors-1.9.1/src/kde_material_you_colors/data/sample_config.conf`

 * *Files 6% similar despite different names*

```diff
@@ -160,7 +160,38 @@
 # Commented by default
 #once_after_change = False
 
 # Pause mode
 # Disables wallpaper detection and automatic theming
 # Default is False
 #pause_mode = False
+
+# Scheme Variant
+# Changes between Material You scheme variants (0-8)
+# 0 = Content
+# 1 = Expressive
+# 2 = Fidelity
+# 3 = Monochrome
+# 4 = Neutral
+# 5 = TonalSpot
+# 6 = Vibrant
+# 7 = Rainbow
+# 8 = FruitSalad
+# Default is 5
+scheme_variant = 5
+
+# Colorfulness
+# Changes chroma (colorfulness) of theme
+# An integer between 0.5 and 10
+# Default is 1
+chroma_multiplier = 1
+
+# Brightness
+# Changes tone (brightness) of theme
+# An integer between 0.5 and 1.5
+# Default is 1
+tone_multiplier = 1
+
+# QDbus executable
+# Name or location of the QDbus executable e.g qdbus6, qdbus-qt6...
+# Default is qdbus6
+#qdbus_executable = qdbus6
```

### Comparing `kde-material-you-colors-1.8.0/src/kde_material_you_colors/logging_config.py` & `kde_material_you_colors-1.9.1/src/kde_material_you_colors/logging_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from logging.handlers import RotatingFileHandler
 import logging
 import sys
 import os
 import re
-from . import settings
+from kde_material_you_colors import settings
 
 # Set logging level for pillow
 logging.getLogger("PIL").setLevel(logging.WARNING)
 
 # Custom logging format (adapted from https://stackoverflow.com/a/14859558)
```

### Comparing `kde-material-you-colors-1.8.0/src/kde_material_you_colors/main.py` & `kde_material_you_colors-1.9.1/src/kde_material_you_colors/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -305,14 +305,47 @@
     parser.add_argument(
         "--version",
         "-v",
         action="store_true",
         help="Print version information",
     )
 
+    parser.add_argument(
+        "--scheme-variant",
+        "-sv",
+        type=int,
+        help="Changes between Material You scheme variants 0 = Content, 1 = Expressive, 2 = Fidelity, 3 = Monochrome, 4 = Neutral, 5 = TonalSpot, 6 = Vibrant, 7 = Rainbow, 8 = FruitSalad (default is 5)",
+        default=None,
+        metavar="<integer>",
+    )
+
+    parser.add_argument(
+        "--chroma-multiplier",
+        type=float,
+        help="Colorfulness of the theme (value from 0.5 to 10, default is 1)",
+        default=None,
+        metavar="<float>",
+    )
+
+    parser.add_argument(
+        "--tone-multiplier",
+        type=float,
+        help="Brightness of the theme (value from 0 to 1.5, default is 1)",
+        default=None,
+        metavar="<float>",
+    )
+
+    parser.add_argument(
+        "--qdbus-executable",
+        type=str,
+        help="Name or location of the QDbus executable e.g qdbus6, qdbus-qt6... (default is qdbus6)",
+        default=None,
+        metavar="<string>",
+    )
+
     # Get commandline arguments
     args = parser.parse_args()
     # Check for one shot arguments
     utils.one_shot_actions(args)
     # Kill existing instance if found
     utils.kill_existing()
 
@@ -394,15 +427,15 @@
             continue
 
         #
         #
         #
         #
         # update wallpaper
-        wallpaper.update(config)
+        wallpaper.update(config, skip_screenshot=counter != 0)
         wallpaper_watcher.set_value(wallpaper.current)
 
         target_cycles = config.read("screenshot_delay") / (
             config.read("main_loop_delay") or 1
         )
 
         # Monitor file for changes (image and screenshot only)
```

### Comparing `kde-material-you-colors-1.8.0/src/kde_material_you_colors/schemeconfigs.py` & `kde_material_you_colors-1.9.1/src/kde_material_you_colors/schemeconfigs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import logging
-from .utils.color_utils import (
+from kde_material_you_colors.utils.color_utils import (
     blendColors,
     lighteen_color,
     scale_saturation,
     blend2contrast,
     sort_colors_luminance,
     hex2alpha,
     hex2rgb,
 )
-from .utils import math_utils
-from .utils import string_utils
-from .utils import color_utils
+from kde_material_you_colors.utils import string_utils
 
 
 class ThemeConfig:
     def __init__(
         self,
         colors,
         wallpaper_data,
@@ -24,167 +22,38 @@
         toolbar_opacity_dark=None,
         custom_colors_list=None,
     ):
         if custom_colors_list is not None:
             colors_best = custom_colors_list
             colors_str = ""
             for color in custom_colors_list:
-                rgb = color_utils.hex2rgb(color)
+                rgb = hex2rgb(color)
                 colors_str += f"\033[38;2;{rgb[0]};{rgb[1]};{rgb[2]};1m{color} \033[0m"
             logging.info(f"Using custom colors: {colors_str[:-5]}")
         else:
-            colors_best = list(colors["best"].values())
-        # colors_best = list(colors['best'].values())
+            colors_best = colors["best"]
         tones_primary = colors["palettes"]["primary"]
         tones_secondary = colors["palettes"]["secondary"]
         tones_neutral = colors["palettes"]["neutral"]
         tones_neutral_variant = colors["palettes"]["neutralVariant"]
         tones_tertiary = colors["palettes"]["tertiary"]
         tones_error = colors["palettes"]["error"]
+
         colors_light = colors["schemes"]["light"]
         colors_dark = colors["schemes"]["dark"]
 
-        lbm = math_utils.clip(light_blend_multiplier, 0, 4, 1.0)
-        dbm = math_utils.clip(dark_blend_multiplier, 0, 4, 1.0)
-
-        # Base text states taken from Breeze Color Scheme
-        base_text_states = {
-            "Link": "#2980b9",
-            "Visited": "#9b59b6",
-            "Negative": "#da4453",
-            "Neutral": "#f67400",
-            "Positive": "#27ae60",
-        }
-
         self._material_you_schemes = colors
 
-        # Blend some extra colors by factor left(0.0) to right(1.0)
-        self._extras = {
-            "dark": {
-                "surface": blendColors(tones_neutral[5], tones_primary[40], 0.08 * dbm),
-                "surface1": blendColors(
-                    colors_dark["background"], tones_primary[40], 0.05 * dbm
-                ),
-                "surface2": blendColors(
-                    colors_dark["background"], tones_primary[40], 0.08 * dbm
-                ),
-                "surface3": blendColors(
-                    colors_dark["background"], tones_primary[40], 0.18 * dbm
-                ),
-                "linkOnPrimary": blendColors(
-                    colors_dark["onPrimary"], base_text_states["Link"], 0.5
-                ),
-                "linkVisitedOnPrimary": blendColors(
-                    colors_dark["onPrimary"], base_text_states["Visited"], 0.8
-                ),
-                "negativeOnPrimary": blendColors(
-                    colors_dark["onPrimary"], base_text_states["Negative"], 0.8
-                ),
-                "positiveOnPrimary": blendColors(
-                    colors_dark["onPrimary"], base_text_states["Positive"], 0.8
-                ),
-                "neutralOnPrimary": blendColors(
-                    colors_dark["onPrimary"], base_text_states["Neutral"], 0.8
-                ),
-                # view
-                "linkOnSurface": blendColors(
-                    colors_dark["onSurface"], base_text_states["Link"], 0.8
-                ),
-                "linkVisitedOnSurface": blendColors(
-                    colors_dark["onSurface"], base_text_states["Visited"], 0.8
-                ),
-                "negativeOnSurface": blendColors(
-                    colors_dark["onSurface"], base_text_states["Negative"], 0.8
-                ),
-                "positiveOnSurface": blendColors(
-                    colors_dark["onSurface"], base_text_states["Positive"], 0.8
-                ),
-                "neutralOnSurface": blendColors(
-                    colors_dark["onSurface"], base_text_states["Neutral"], 0.8
-                ),
-                "selectionAltActive": blendColors(
-                    colors_dark["background"], colors_dark["secondary"], 0.5
-                ),
-            },
-            "light": {
-                "surface": blendColors(
-                    colors_light["background"], tones_primary[70], 0.08 * lbm
-                ),
-                "surface1": blendColors(
-                    colors_light["background"], tones_primary[70], 0.18 * lbm
-                ),
-                "surface2": blendColors(
-                    colors_light["background"], tones_primary[70], 0.23 * lbm
-                ),
-                "surface3": blendColors(
-                    colors_light["background"], tones_primary[70], 0.20 * lbm
-                ),
-                "linkOnPrimary": blendColors(
-                    colors_light["onPrimary"], base_text_states["Link"], 0.5
-                ),
-                "linkVisitedOnPrimary": blendColors(
-                    colors_light["onPrimary"], base_text_states["Visited"], 0.8
-                ),
-                "negativeOnPrimary": blendColors(
-                    colors_light["onPrimary"], base_text_states["Negative"], 0.8
-                ),
-                "positiveOnPrimary": blendColors(
-                    colors_light["onPrimary"], base_text_states["Positive"], 0.8
-                ),
-                "neutralOnPrimary": blendColors(
-                    colors_light["onPrimary"], base_text_states["Neutral"], 0.8
-                ),
-                # view
-                "linkOnSurface": blendColors(
-                    colors_light["onSurface"], base_text_states["Link"], 0.5
-                ),
-                "linkVisitedOnSurface": blendColors(
-                    colors_light["onSurface"], base_text_states["Visited"], 0.8
-                ),
-                "negativeOnSurface": blendColors(
-                    colors_light["onSurface"], base_text_states["Negative"], 0.8
-                ),
-                "positiveOnSurface": blendColors(
-                    colors_light["onSurface"], base_text_states["Positive"], 0.8
-                ),
-                "neutralOnSurface": blendColors(
-                    colors_light["onSurface"], base_text_states["Neutral"], 0.8
-                ),
-                "selectionAltActive": blendColors(
-                    colors_light["background"], colors_light["secondary"], 0.5
-                ),
-            },
-        }
-        self._extras["dark"].update(
-            {
-                "selectionAlt": blendColors(
-                    tones_secondary[30], self._extras["dark"]["surface3"], 0.05 * dbm
-                ),
-                "selectionHover": blendColors(
-                    tones_secondary[50], self._extras["dark"]["surface3"], 0.1 * dbm
-                ),
-            }
-        )
-
-        self._extras["light"].update(
-            {
-                "selectionAlt": blendColors(
-                    self._extras["light"]["surface3"], tones_primary[30], 0.05 * lbm
-                ),
-                "selectionHover": blendColors(
-                    self._extras["light"]["surface3"], tones_primary[50], 0.1 * lbm
-                ),
-            }
-        )
+        self._extras = colors["custom"]
 
         extras = self._extras
 
         best_colors_count = len(colors_best)
         # bg , ansi 30
-        pywal_colors_dark = (extras["dark"]["surface"],)
+        pywal_colors_dark = (colors_dark["surface"],)
         # gray? bold, ansi 30
         pywal_colors_dark_intense = (
             blendColors(pywal_colors_dark[0], tones_secondary[90], 0.8),
         )
         # dark gray? faint ansi 30
         pywal_colors_dark_faint = (
             blendColors(pywal_colors_dark[0], tones_secondary[90], 0.7),
@@ -193,38 +62,38 @@
 
         for x in range(7):
             if len(pywal_colors_dark) <= 7:
                 if x < best_colors_count:
                     c = lighteen_color(colors_best[x], 0.2, tones_neutral[99])
                     pywal_colors_dark += (
                         blend2contrast(
-                            c, pywal_colors_dark[0], tones_neutral[99], 4.5, 0.01, True
+                            c, pywal_colors_dark[0], tones_neutral[99], 2.5, 0.01, True
                         ),
                     )
                 else:
                     if len(pywal_colors_dark) <= 7:
                         c = lighteen_color(tones_primary[tone], 0.2, tones_neutral[99])
                         pywal_colors_dark += (
                             blend2contrast(
                                 c,
                                 pywal_colors_dark[0],
                                 tones_neutral[99],
-                                4.5,
+                                2.5,
                                 0.01,
                                 True,
                             ),
                         )
                     if len(pywal_colors_dark) <= 7:
                         c = lighteen_color(tones_tertiary[tone], 0.2, tones_neutral[99])
                         pywal_colors_dark += (
                             blend2contrast(
                                 c,
                                 pywal_colors_dark[0],
                                 tones_neutral[99],
-                                4.5,
+                                2.5,
                                 0.01,
                                 True,
                             ),
                         )
                     if tone < 91:
                         tone += 8
             else:
@@ -247,15 +116,15 @@
 
             pywal_colors_dark_faint += (
                 blendColors(pywal_colors_dark[0], all_colors[n], 0.7),
             )
 
         tone = 50
         # ansi 30
-        pywal_colors_light = (extras["light"]["surface"],)
+        pywal_colors_light = (colors_light["surface"],)
         pywal_colors_light_intense = (
             blendColors(pywal_colors_light[0], tones_secondary[25], 0.8),
         )
         pywal_colors_light_faint = (
             blendColors(pywal_colors_light[0], tones_secondary[25], 0.7),
         )
 
@@ -265,40 +134,40 @@
                     c = scale_saturation(colors_best[x], 1)
                     c = lighteen_color(c, 0.2, tones_neutral[99])
                     pywal_colors_light += (
                         blend2contrast(
                             c,
                             pywal_colors_light[0],
                             tones_neutral[10],
-                            4.5,
+                            2,
                             0.01,
                             False,
                         ),
                     )
                 else:
                     if len(pywal_colors_light) <= 7:
                         c = scale_saturation(tones_primary[tone], 1)
                         pywal_colors_light += (
                             blend2contrast(
                                 c,
                                 pywal_colors_light[0],
                                 tones_neutral[10],
-                                4.5,
+                                2,
                                 0.01,
                                 False,
                             ),
                         )
                     if len(pywal_colors_light) <= 7:
                         c = scale_saturation(tones_tertiary[tone], 1)
                         pywal_colors_light += (
                             blend2contrast(
                                 c,
                                 pywal_colors_light[0],
                                 tones_neutral[10],
-                                4.5,
+                                2,
                                 0.01,
                                 False,
                             ),
                         )
                     if tone < 91:
                         tone += 8
             else:
@@ -355,310 +224,308 @@
         # print("CONTRAST CHECK LIGHT - FAINT")
         # for color in pywal_colors_light_faint:
         #     c = contrast_ratio(pywal_colors_light[0], color)
         #     print(f"{color}  {'{0:.2g}'.format(c)} |", end=" ")
         # print()
 
         self._light_scheme = f"""[ColorEffects:Disabled]
-Color={extras['light']['surface1']}
-ColorAmount=0.55
-ColorEffect=0
-ContrastAmount=0.65
-ContrastEffect=1
-IntensityAmount=0.1
-IntensityEffect=2
+Color={colors_light["surfaceContainer"]}
+ColorAmount=0.5
+ColorEffect=3
+ContrastAmount=0
+ContrastEffect=0
+IntensityAmount=0
+IntensityEffect=0
 
 [ColorEffects:Inactive]
 ChangeSelectionColor=true
-Color={colors_light['surfaceVariant']}
+Color={colors_light['surfaceContainerLowest']}
 ColorAmount=0.025
-ColorEffect=2
+ColorEffect=0
 ContrastAmount=0.1
-ContrastEffect=2
+ContrastEffect=0
 Enable=false
 IntensityAmount=0
 IntensityEffect=0
 
 [Colors:Button]
 BackgroundAlternate={colors_light['surfaceVariant']}
-BackgroundNormal={extras['light']['selectionAlt']}
+BackgroundNormal={colors_light['surfaceContainerHigh']}
 DecorationFocus={colors_light['primary']}
 DecorationHover={colors_light['primary']}
 ForegroundActive={colors_light['onSurface']}
 ForegroundInactive={colors_light['outline']}
-ForegroundLink={base_text_states['Link']}
-ForegroundNegative={base_text_states['Negative']}
-ForegroundNeutral={base_text_states['Neutral']}
+ForegroundLink={extras['link']['light']['primary']}
+ForegroundNegative={extras['negative']['light']['primary']}
+ForegroundNeutral={extras['neutral']['light']['primary']}
 ForegroundNormal={colors_light['onSurface']}
-ForegroundPositive={base_text_states['Positive']}
-ForegroundVisited={base_text_states['Visited']}
+ForegroundPositive={extras['positive']['light']['primary']}
+ForegroundVisited={extras['visited']['light']['primary']}
 
 [Colors:Complementary]
-BackgroundAlternate={extras['light']['surface']}
-BackgroundNormal={extras['light']['surface3']}
+BackgroundAlternate={colors_light['surface']}
+BackgroundNormal={colors_light['surfaceContainer']}
 DecorationFocus={colors_light['primary']}
 DecorationHover={colors_light['primary']}
 ForegroundActive={colors_light['inverseSurface']}
 ForegroundInactive={colors_light['outline']}
-ForegroundLink={base_text_states['Link']}
-ForegroundNegative={colors_light['error']}
-ForegroundNeutral={base_text_states['Neutral']}
+ForegroundLink={extras['link']['light']['primary']}
+ForegroundNegative={extras['negative']['light']['primary']}
+ForegroundNeutral={extras['neutral']['light']['primary']}
 ForegroundNormal={colors_light['onSurfaceVariant']}
-ForegroundPositive={base_text_states['Positive']}
-ForegroundVisited={base_text_states['Visited']}
+ForegroundPositive={extras['positive']['light']['primary']}
+ForegroundVisited={extras['visited']['light']['primary']}
 
 [Colors:Header]
-BackgroundAlternate={extras['light']['surface']}
-BackgroundNormal={extras['light']['surface3']}
+BackgroundAlternate={colors_light['surface']}
+BackgroundNormal={colors_light['surface']}
 DecorationFocus={colors_light['primary']}
 DecorationHover={colors_light['primary']}
 ForegroundActive={colors_light['inverseSurface']}
 ForegroundInactive={colors_light['outline']}
-ForegroundLink={base_text_states['Link']}
-ForegroundNegative={colors_light['error']}
-ForegroundNeutral={base_text_states['Neutral']}
-ForegroundNormal={colors_light['onSurfaceVariant']}
-ForegroundPositive={base_text_states['Positive']}
-ForegroundVisited={base_text_states['Visited']}
+ForegroundLink={extras['link']['light']['primary']}
+ForegroundNegative={extras['negative']['light']['primary']}
+ForegroundNeutral={extras['neutral']['light']['primary']}
+ForegroundNormal={colors_light['onSurface']}
+ForegroundPositive={extras['positive']['light']['primary']}
+ForegroundVisited={extras['visited']['light']['primary']}
 
 [Colors:Header][Inactive]
-BackgroundAlternate={extras['light']['surface']}
-BackgroundNormal={extras['light']['surface3']}
+BackgroundAlternate={colors_light['surface']}
+BackgroundNormal={colors_light['surface']}
 DecorationFocus={colors_light['primary']}
 DecorationHover={colors_light['primary']}
 ForegroundActive={colors_light['inverseSurface']}
 ForegroundInactive={colors_light['outline']}
-ForegroundLink={base_text_states['Link']}
-ForegroundNegative={colors_light['error']}
-ForegroundNeutral={base_text_states['Neutral']}
+ForegroundLink={extras['link']['light']['primary']}
+ForegroundNegative={extras['negative']['light']['primary']}
+ForegroundNeutral={extras['neutral']['light']['primary']}
 ForegroundNormal={colors_light['onSurfaceVariant']}
-ForegroundPositive={base_text_states['Positive']}
-ForegroundVisited={base_text_states['Visited']}
+ForegroundPositive={extras['positive']['light']['primary']}
+ForegroundVisited={extras['visited']['light']['primary']}
 
 [Colors:Selection]
 BackgroundAlternate={colors_light['primary']}
 BackgroundNormal={colors_light['primary']}
 DecorationFocus={colors_light['primary']}
-DecorationHover={colors_light['primary']}
+DecorationHover={colors_light['secondary']}
 ForegroundActive={colors_light['onPrimary']}
 ForegroundInactive={colors_light['onPrimary']}
-ForegroundLink={extras['light']['linkOnPrimary']}
-ForegroundNegative={extras['light']['negativeOnPrimary']}
-ForegroundNeutral={extras['light']['neutralOnPrimary']}
+ForegroundLink={extras['link']['light']['onPrimaryFixedVariant']}
+ForegroundNegative={extras['negative']['light']['onPrimaryFixedVariant']}
+ForegroundNeutral={extras['neutral']['light']['onPrimaryFixedVariant']}
 ForegroundNormal={colors_light['onPrimary']}
-ForegroundPositive={extras['light']['positiveOnPrimary']}
-ForegroundVisited={extras['light']['linkVisitedOnPrimary']}
+ForegroundPositive={extras['positive']['light']['onPrimaryFixedVariant']}
+ForegroundVisited={extras['visited']['light']['onPrimaryFixedVariant']}
 
 [Colors:Tooltip]
 BackgroundAlternate={colors_light['surfaceVariant']}
-BackgroundNormal={extras['light']['surface']}
+BackgroundNormal={colors_light['surfaceContainer']}
 DecorationFocus={colors_light['primary']}
 DecorationHover={colors_light['primary']}
 ForegroundActive={colors_light['onSurface']}
 ForegroundInactive={colors_light['outline']}
-ForegroundLink={base_text_states['Link']}
-ForegroundNegative={colors_light['error']}
-ForegroundNeutral={base_text_states['Neutral']}
+ForegroundLink={extras['link']['light']['primary']}
+ForegroundNegative={extras['negative']['light']['primary']}
+ForegroundNeutral={extras['neutral']['light']['primary']}
 ForegroundNormal={colors_light['onSurface']}
-ForegroundPositive={base_text_states['Positive']}
-ForegroundVisited={base_text_states['Visited']}
+ForegroundPositive={extras['positive']['light']['primary']}
+ForegroundVisited={extras['visited']['light']['primary']}
 
 [Colors:View]
-BackgroundAlternate={extras['light']['surface2']}
-BackgroundNormal={extras['light']['surface']}
+BackgroundAlternate={colors_light['surfaceContainer']}
+BackgroundNormal={colors_light['surfaceBright']}
 DecorationFocus={colors_light['primary']}
 #-----------------------------------------------
-DecorationHover={extras['light']['selectionHover']}
+DecorationHover={colors_light['secondaryFixed']}
 ForegroundActive={colors_light['inverseSurface']}
 ForegroundInactive={colors_light['outline']}
-ForegroundLink={extras['light']['linkOnSurface']}
-ForegroundNegative={colors_light['error']}
-ForegroundNeutral={extras['light']['neutralOnSurface']}
-ForegroundNormal={colors_light['onSurfaceVariant']}
-ForegroundPositive={extras['light']['positiveOnSurface']}
-ForegroundVisited={extras['light']['linkVisitedOnSurface']}
+ForegroundLink={extras['link']['light']['primary']}
+ForegroundNegative={extras['negative']['light']['primary']}
+ForegroundNeutral={extras['neutral']['light']['primary']}
+ForegroundNormal={colors_light['onSurface']}
+ForegroundPositive={extras['positive']['light']['primary']}
+ForegroundVisited={extras['visited']['light']['primary']}
 
 [Colors:Window]
-BackgroundAlternate={extras['light']['surface']}
-BackgroundNormal={extras['light']['surface3']}
+BackgroundAlternate={colors_light['surfaceVariant']}
+BackgroundNormal={colors_light['surfaceContainer']}
 DecorationFocus={colors_light['primary']}
 DecorationHover={colors_light['primary']}
-ForegroundActive={colors_light['inverseSurface']}
+ForegroundActive={extras['link']['light']['primary']}
 ForegroundInactive={colors_light['outline']}
-ForegroundLink={base_text_states['Link']}
-ForegroundNegative={colors_light['error']}
-ForegroundNeutral={base_text_states['Neutral']}
+ForegroundLink={extras['link']['light']['primary']}
+ForegroundNegative={extras['negative']['light']['primary']}
+ForegroundNeutral={extras['neutral']['light']['primary']}
 #--- Window titles, context icons
 ForegroundNormal={colors_light['onSurfaceVariant']}
-ForegroundPositive={base_text_states['Positive']}
-ForegroundVisited={base_text_states['Visited']}
+ForegroundPositive={extras['positive']['light']['primary']}
+ForegroundVisited={extras['visited']['light']['primary']}
 
 [General]
 ColorScheme=MaterialYouLight
 Name=Material You Light
 shadeSortColumn=true
 
 [KDE]
 contrast=4
 
 [WM]
-activeBackground={hex2alpha(extras['light']['surface3'],toolbar_opacity)}
+activeBackground={hex2alpha(colors_light["surfaceContainerHighest"],toolbar_opacity)}
 activeBlend=227,229,231
 activeForeground={colors_light['onSurface']}
 inactiveBackground={hex2alpha(colors_light['secondaryContainer'],toolbar_opacity)}
 inactiveBlend=239,240,241
 inactiveForeground={colors_light['onSurfaceVariant']}
         """
 
         self._dark_scheme = f"""[ColorEffects:Disabled]
-Color={extras['dark']['surface1']}
-ColorAmount=0
-ColorEffect=0
-ContrastAmount=0.65
-ContrastEffect=1
-IntensityAmount=0.1
-IntensityEffect=2
+Color={colors_dark["surfaceContainer"]}
+ColorAmount=0.5
+ColorEffect=3
+ContrastAmount=0
+ContrastEffect=0
+IntensityAmount=0
+IntensityEffect=0
 
 [ColorEffects:Inactive]
 ChangeSelectionColor=true
-Color=Color={colors_dark['surfaceVariant']}
+Color={colors_dark['surfaceContainerLowest']}
 ColorAmount=0.025
-ColorEffect=2
+ColorEffect=0
 ContrastAmount=0.1
-ContrastEffect=2
-Enable=false
+ContrastEffect=0
+Enable=true
 IntensityAmount=0
 IntensityEffect=0
 
 [Colors:Button]
 BackgroundAlternate={colors_dark['surfaceVariant']}
-BackgroundNormal={extras['dark']['selectionAlt']}
+BackgroundNormal={colors_dark['surfaceContainerHigh']}
 DecorationFocus={colors_dark['primary']}
 DecorationHover={colors_dark['primary']}
 ForegroundActive={colors_dark['onSurface']}
 ForegroundInactive={colors_dark['outline']}
-ForegroundLink={base_text_states['Link']}
-ForegroundNegative={tones_error[50]}
-ForegroundNeutral={base_text_states['Neutral']}
+ForegroundLink={extras['link']['dark']['primary']}
+ForegroundNegative={extras['negative']['dark']['primary']}
+ForegroundNeutral={extras['neutral']['dark']['primary']}
 ForegroundNormal={colors_dark['onSurface']}
-ForegroundPositive={base_text_states['Positive']}
-ForegroundVisited={base_text_states['Visited']}
+ForegroundPositive={extras['positive']['dark']['primary']}
+ForegroundVisited={extras['visited']['dark']['primary']}
 
 [Colors:Complementary]
-BackgroundAlternate={extras['dark']['surface']}
-BackgroundNormal={extras['dark']['surface3']}
+BackgroundAlternate={colors_dark['surface']}
+BackgroundNormal={colors_dark['surfaceContainer']}
 DecorationFocus={colors_dark['primary']}
 DecorationHover={colors_dark['primary']}
 ForegroundActive={colors_dark['inverseSurface']}
 ForegroundInactive={colors_dark['outline']}
-ForegroundLink={base_text_states['Link']}
-ForegroundNegative={tones_error[50]}
-ForegroundNeutral={base_text_states['Neutral']}
+ForegroundLink={extras['link']['dark']['primary']}
+ForegroundNegative={extras['negative']['dark']['primary']}
+ForegroundNeutral={extras['neutral']['dark']['primary']}
 ForegroundNormal={colors_dark['onSurfaceVariant']}
-ForegroundPositive={base_text_states['Positive']}
-ForegroundVisited={base_text_states['Visited']}
+ForegroundPositive={extras['positive']['dark']['primary']}
+ForegroundVisited={extras['visited']['dark']['primary']}
 
 [Colors:Header]
-BackgroundAlternate={extras['dark']['surface']}
-BackgroundNormal={extras['dark']['surface3']}
+BackgroundAlternate={colors_dark['surface']}
+BackgroundNormal={colors_dark['surface']}
 DecorationFocus={colors_dark['primary']}
 DecorationHover={colors_dark['primary']}
 ForegroundActive={colors_dark['inverseSurface']}
 ForegroundInactive={colors_dark['outline']}
-ForegroundLink={base_text_states['Link']}
-ForegroundNegative={tones_error[50]}
-ForegroundNeutral={base_text_states['Neutral']}
+ForegroundLink={extras['link']['dark']['primary']}
+ForegroundNegative={extras['negative']['dark']['primary']}
+ForegroundNeutral={extras['neutral']['dark']['primary']}
 ForegroundNormal={colors_dark['onSurfaceVariant']}
-ForegroundPositive={base_text_states['Positive']}
-ForegroundVisited={base_text_states['Visited']}
+ForegroundPositive={extras['positive']['dark']['primary']}
+ForegroundVisited={extras['visited']['dark']['primary']}
 
 [Colors:Header][Inactive]
-BackgroundAlternate={extras['dark']['surface']}
-BackgroundNormal={extras['dark']['surface3']}
+BackgroundAlternate={colors_dark['surface']}
+BackgroundNormal={colors_dark['surface']}
 DecorationFocus={colors_dark['primary']}
 DecorationHover={colors_dark['primary']}
 ForegroundActive={colors_dark['inverseSurface']}
 ForegroundInactive={colors_dark['outline']}
-ForegroundLink={base_text_states['Link']}
-ForegroundNegative={tones_error[50]}
-ForegroundNeutral={base_text_states['Neutral']}
+ForegroundLink={extras['link']['dark']['primary']}
+ForegroundNegative={extras['negative']['dark']['primary']}
+ForegroundNeutral={extras['neutral']['dark']['primary']}
 ForegroundNormal={colors_dark['onSurfaceVariant']}
-ForegroundPositive={base_text_states['Positive']}
-ForegroundVisited={base_text_states['Visited']}
+ForegroundPositive={extras['positive']['dark']['primary']}
+ForegroundVisited={extras['visited']['dark']['primary']}
 
 [Colors:Selection]
 BackgroundAlternate={colors_dark['primary']}
 BackgroundNormal={colors_dark['primary']}
 DecorationFocus={colors_dark['primary']}
-DecorationHover={colors_dark['primary']}
+DecorationHover={colors_dark['secondary']}
 ForegroundActive={colors_dark['onPrimary']}
 ForegroundInactive={colors_dark['onPrimary']}
-ForegroundLink={extras['dark']['linkOnPrimary']}
-ForegroundNegative={extras['dark']['negativeOnPrimary']}
-ForegroundNeutral={extras['dark']['neutralOnPrimary']}
+ForegroundLink={extras['link']['dark']['onPrimaryFixedVariant']}
+ForegroundNegative={extras['negative']['dark']['onPrimaryFixedVariant']}
+ForegroundNeutral={extras['neutral']['dark']['onPrimaryFixedVariant']}
 ForegroundNormal={colors_dark['onPrimary']}
-ForegroundPositive={extras['dark']['positiveOnPrimary']}
-ForegroundVisited={extras['dark']['linkVisitedOnPrimary']}
-
-
+ForegroundPositive={extras['positive']['dark']['onPrimaryFixedVariant']}
+ForegroundVisited={extras['visited']['dark']['onPrimaryFixedVariant']}
 
 [Colors:Tooltip]
 BackgroundAlternate={colors_dark['surfaceVariant']}
-BackgroundNormal={extras['dark']['surface']}
+BackgroundNormal={colors_dark['surfaceContainer']}
 DecorationFocus={colors_dark['primary']}
 DecorationHover={colors_dark['primary']}
 ForegroundActive={colors_dark['onSurface']}
 ForegroundInactive={colors_dark['outline']}
-ForegroundLink={base_text_states['Link']}
-ForegroundNegative={tones_error[50]}
-ForegroundNeutral={base_text_states['Neutral']}
+ForegroundLink={extras['link']['dark']['primary']}
+ForegroundNegative={extras['negative']['dark']['primary']}
+ForegroundNeutral={extras['neutral']['dark']['primary']}
 ForegroundNormal={colors_dark['onSurface']}
-ForegroundPositive={base_text_states['Positive']}
-ForegroundVisited={base_text_states['Visited']}
+ForegroundPositive={extras['positive']['dark']['primary']}
+ForegroundVisited={extras['visited']['dark']['primary']}
 
 [Colors:View]
-BackgroundAlternate={extras['dark']['surface2']}
-BackgroundNormal={extras['dark']['surface']}
+BackgroundAlternate={colors_dark['surfaceContainer']}
+BackgroundNormal={colors_dark['surfaceDim']}
 DecorationFocus={colors_dark['primary']}
 #-----------------------------------------------
 DecorationHover={colors_dark['inversePrimary']}
 ForegroundActive={colors_dark['inverseSurface']}
 ForegroundInactive={colors_dark['outline']}
-ForegroundLink={extras['dark']['linkOnSurface']}
-ForegroundNegative={extras['dark']['negativeOnSurface']}
-ForegroundNeutral={extras['dark']['neutralOnSurface']}
-ForegroundNormal={colors_dark['onSurfaceVariant']}
-ForegroundPositive={extras['dark']['positiveOnSurface']}
-ForegroundVisited={extras['dark']['linkVisitedOnSurface']}
+ForegroundLink={extras['link']['dark']['primary']}
+ForegroundNegative={extras['negative']['dark']['primary']}
+ForegroundNeutral={extras['neutral']['dark']['primary']}
+ForegroundNormal={colors_dark['onSurface']}
+ForegroundPositive={extras['positive']['dark']['primary']}
+ForegroundVisited={extras['visited']['dark']['primary']}
 
 [Colors:Window]
-BackgroundAlternate={extras['dark']['surface']}
-BackgroundNormal={extras['dark']['surface3']}
+BackgroundAlternate={colors_dark['surfaceVariant']}
+BackgroundNormal={colors_dark['surfaceContainer']}
 DecorationFocus={colors_dark['primary']}
 DecorationHover={colors_dark['primary']}
-ForegroundActive={colors_dark['inverseSurface']}
+ForegroundActive={extras['link']['dark']['primary']}
 ForegroundInactive={colors_dark['outline']}
-ForegroundLink={base_text_states['Link']}
-ForegroundNegative={tones_error[50]}
-ForegroundNeutral={base_text_states['Neutral']}
+ForegroundLink={extras['link']['dark']['primary']}
+ForegroundNegative={extras['negative']['dark']['primary']}
+ForegroundNeutral={extras['neutral']['dark']['primary']}
 #--- Window titles, context icons
 ForegroundNormal={colors_dark['onSurfaceVariant']}
-ForegroundPositive={base_text_states['Positive']}
-ForegroundVisited={base_text_states['Visited']}
+ForegroundPositive={extras['positive']['dark']['primary']}
+ForegroundVisited={extras['visited']['dark']['primary']}
 
 [General]
 ColorScheme=MaterialYouDark
 Name=Material You dark
 shadeSortColumn=true
 
 [KDE]
 contrast=4
 
 [WM]
-activeBackground={hex2alpha(extras['dark']['surface3'],toolbar_opacity_dark)}
+activeBackground={hex2alpha(colors_dark['surfaceContainerHighest'],toolbar_opacity_dark)}
 activeBlend=252,252,252
 activeForeground={colors_dark['onSurface']}
 inactiveBackground={hex2alpha(colors_dark['secondaryContainer'],toolbar_opacity_dark)}
 inactiveBlend=161,169,177
 inactiveForeground={colors_dark['onSecondaryContainer']}
         """
 
@@ -757,18 +624,18 @@
                 "color20": pywal_colors_dark_faint[4],
                 "color21": pywal_colors_dark_faint[5],
                 "color22": pywal_colors_dark_faint[6],
                 "color23": pywal_colors_dark_faint[7],
             },
         }
         dark_active = colors_dark["onBackground"]
-        dark_inactive = extras["dark"]["surface3"]
+        dark_inactive = colors_dark["surfaceContainerHighest"]
 
         light_active = colors_light["onBackground"]
-        light_inactive = extras["light"]["surface3"]
+        light_inactive = colors_light["surfaceContainerHighest"]
 
         self._sierra_breeze_dark_colors = {
             "btn_close_active_color": string_utils.tup2str(
                 hex2rgb(blendColors(dark_active, tones_primary[80], 0.7))
             ),
             "btn_minimize_active_color": string_utils.tup2str(
                 hex2rgb(blendColors(dark_active, tones_primary[70], 0.7))
@@ -791,33 +658,33 @@
             "btn_inactive_color": string_utils.tup2str(
                 hex2rgb(blendColors(dark_inactive, colors_dark["secondary"], 0.32))
             ),
         }
 
         self._sierra_breeze_light_colors = {
             "btn_close_active_color": string_utils.tup2str(
-                hex2rgb(blendColors(tones_primary[50], light_active, 0.05 * lbm))
+                hex2rgb(blendColors(tones_primary[50], light_active, 0.05))
             ),
             "btn_minimize_active_color": string_utils.tup2str(
-                hex2rgb(blendColors(tones_primary[60], light_active, 0.05 * lbm))
+                hex2rgb(blendColors(tones_primary[60], light_active, 0.05))
             ),
             "btn_maximize_active_color": string_utils.tup2str(
-                hex2rgb(blendColors(tones_primary[70], light_active, 0.05 * lbm))
+                hex2rgb(blendColors(tones_primary[70], light_active, 0.05))
             ),
             "btn_keep_above_active_color": string_utils.tup2str(
-                hex2rgb(blendColors("#118cff", light_active, 0.05 * lbm))
+                hex2rgb(blendColors("#118cff", light_active, 0.05))
             ),
             "btn_keep_below_active_color": string_utils.tup2str(
-                hex2rgb(blendColors("#5d00b9", light_active, 0.05 * lbm))
+                hex2rgb(blendColors("#5d00b9", light_active, 0.05))
             ),
             "btn_on_all_desktops_active_color": string_utils.tup2str(
-                hex2rgb(blendColors("#00b9b9", light_active, 0.05 * lbm))
+                hex2rgb(blendColors("#00b9b9", light_active, 0.05))
             ),
             "btn_shade_active_color": string_utils.tup2str(
-                hex2rgb(blendColors("#b900b6", light_active, 0.05 * lbm))
+                hex2rgb(blendColors("#b900b6", light_active, 0.05))
             ),
             "btn_inactive_color": string_utils.tup2str(
                 hex2rgb(blendColors(light_inactive, colors_light["secondary"], 0.32))
             ),
         }
 
         self._ksyntax_highlighting_dark = {
@@ -839,17 +706,17 @@
                 "IconBorder": pywal_colors_dark[0],
                 "IndentationLine": tones_secondary[20],
                 "LineNumbers": tones_neutral[45],
                 "MarkBookmark": "#0404bf",
                 "MarkBreakpointActive": "#8b0607",
                 "MarkBreakpointDisabled": "#820683",
                 "MarkBreakpointReached": "#6d6e07",
-                "MarkError": extras["dark"]["negativeOnSurface"],
+                "MarkError": extras["negative"]["dark"]["onPrimaryFixedVariant"],
                 "MarkExecution": "#4d4e50",
-                "MarkWarning": extras["dark"]["neutralOnSurface"],
+                "MarkWarning": extras["neutral"]["dark"]["onPrimaryFixedVariant"],
                 "ModifiedLines": "#c04900",
                 "ReplaceHighlight": "#808021",
                 "SavedLines": "#1c8042",
                 "SearchHighlight": "#218058",
                 "Separator": "#3f4347",
                 "SpellChecking": "#c0392b",
                 "TabMarker": "#4d4d4d",
@@ -975,16 +842,16 @@
                 "LineNumbers": tones_neutral[55],
                 "CurrentLineNumber": colors_light["onSurface"],
                 "MarkBookmark": "#0000ff",
                 "MarkBreakpointActive": "#ff0000",
                 "MarkBreakpointReached": "#ffff00",
                 "MarkBreakpointDisabled": "#ff00ff",
                 "MarkExecution": "#a0a0a4",
-                "MarkWarning": extras["light"]["neutralOnSurface"],
-                "MarkError": extras["light"]["negativeOnSurface"],
+                "MarkWarning": extras["neutral"]["dark"]["onPrimaryFixedVariant"],
+                "MarkError": extras["negative"]["dark"]["onPrimaryFixedVariant"],
                 "ModifiedLines": "#fdbc4b",
                 "ReplaceHighlight": "#00ff00",
                 "SavedLines": "#2ecc71",
                 "SearchHighlight": "#ffff00",
                 "TextSelection": tones_secondary[80],
                 "Separator": "#d5d5d5",
                 "SpellChecking": "#bf0303",
```

### Comparing `kde-material-you-colors-1.8.0/src/kde_material_you_colors/settings.py` & `kde_material_you_colors-1.9.1/src/kde_material_you_colors/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import tempfile
 from pathlib import Path
 import importlib.util
 import shutil
 import sysconfig
 from kde_material_you_colors.utils.utils import find_executable
 
-__version__ = "1.8.0"
+__version__ = "1.9.1"
 USERNAME = getpass.getuser()
 USER_HAS_PYWAL = importlib.util.find_spec("pywal") is not None
 HOME = str(Path.home())
 TEMPDIR = tempfile.gettempdir()
 PKG_INSTALL_DIR = os.path.dirname(__file__)
 PKG_BIN = sysconfig.get_path("scripts") + "/kde-material-you-colors"
```

### Comparing `kde-material-you-colors-1.8.0/src/kde_material_you_colors/utils/color_utils.py` & `kde_material_you_colors-1.9.1/src/kde_material_you_colors/utils/color_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,35 @@
-import operator
-import numpy
 import colorsys
 import re
-from . import math_utils
-from material_color_utilities_python.utils.theme_utils import *
+import operator
+import numpy
+from materialyoucolor.blend import Blend
+from materialyoucolor.utils.color_utils import red_from_argb
+from materialyoucolor.utils.color_utils import green_from_argb
+from materialyoucolor.utils.color_utils import blue_from_argb
+from kde_material_you_colors.utils import math_utils
 
 
 def hex2rgb(hex):
     hex = hex.lstrip("#")
     rgb = tuple(int(hex[i : i + 2], 16) for i in (0, 2, 4))
     # print(f'{rgb} {type(rgb)}')
     return rgb
 
 
 def rgb2hex(r, g, b):
     hex = "#{:02x}{:02x}{:02x}".format(r, g, b)
     return hex
 
 
+def rgba_to_opaque_hex(r, g, b, a):
+    hex = "#{:02x}{:02x}{:02x}".format(r, g, b)
+    return hex
+
+
 # Blend RGB colors using Oklab
 # Adapted from https://github.com/ProtonAOSP/android_frameworks_base/commit/28cc1ae1b1436120f111f1e21ca62e1fc9e0a7df
 
 
 def cube(x):
     x = float(x)
     return x * x * x
@@ -293,14 +301,63 @@
     if format == 1:
         r, g, b = [int(c) for c in color.split(",")]
         return rgb2hex(r, g, b)
     elif format == 2:
         return color
 
 
+def hexFromArgb(argb):
+    r = red_from_argb(argb)
+    g = green_from_argb(argb)
+    b = blue_from_argb(argb)
+    outParts = [f"{r:x}", f"{g:x}", f"{b:x}"]
+    # Pad single-digit output values
+    for i, part in enumerate(outParts):
+        if len(part) == 1:
+            outParts[i] = "0" + part
+    return "#" + "".join(outParts)
+
+
+def parseIntHex(value):
+    return int(value, 16)
+
+
+def rshift(val, n):
+    return val >> n if val >= 0 else (val + 0x100000000) >> n
+
+
+def argbFromHex(hex):
+    hex = hex.replace("#", "")
+    isThree = len(hex) == 3
+    isSix = len(hex) == 6
+    isEight = len(hex) == 8
+    if not isThree and not isSix and not isEight:
+        raise Exception("unexpected hex " + hex)
+
+    r = 0
+    g = 0
+    b = 0
+    if isThree:
+        r = parseIntHex(hex[0:1] * 2)
+        g = parseIntHex(hex[1:2] * 2)
+        b = parseIntHex(hex[2:3] * 2)
+    elif isSix:
+        r = parseIntHex(hex[0:2])
+        g = parseIntHex(hex[2:4])
+        b = parseIntHex(hex[4:6])
+    elif isEight:
+        r = parseIntHex(hex[2:4])
+        g = parseIntHex(hex[4:6])
+        b = parseIntHex(hex[6:8])
+
+    return rshift(
+        ((255 << 24) | ((r & 0x0FF) << 16) | ((g & 0x0FF) << 8) | (b & 0x0FF)), 0
+    )
+
+
 # Tests
 if __name__ == "__main__":
     # Test color blend
     print("> Test color blend #ff0000 , #00ff00")
     print(blendColors("#ff0000", "#00ff00", 0.01))
     print(blendColors("#ff0000", "#00ff00", 0.25))
     print(blendColors("#ff0000", "#00ff00", 0.5))
@@ -343,15 +400,15 @@
     print(blend2contrast("#475AC6", "#1A1A22", "#c1f7fb", 4.5, 0.1, True))
     print("> Test blend2contrast '#e1ffb4','#FEFCF5','#060605', 4.5, 0.01, False")
     print(blend2contrast("#e1ffb4", "#FEFCF5", "#060605", 4.5, 0.01, False))
 
     print("> Oklab vs cam16 blend '#ff0000', '#0000ff', .5")
     print(f"oklab: {blendColors('#ff0000', '#0000ff', .5)}")
     print(
-        f"cam16: {hexFromArgb(Blend.cam16Ucs(argbFromHex('#ff0000'),argbFromHex('#0000ff'),0.5))}"
+        f"cam16: {hexFromArgb(Blend.cam16_ucs(argbFromHex('#ff0000'),argbFromHex('#0000ff'),0.5))}"
     )
 
     print("> lighteen_color '#b70708',.15,'#ffffff'")
     print(lighteen_color("#b70708", 0.15, "#ffffff"))
 
     test_colors = [
         "#000000",
```

### Comparing `kde-material-you-colors-1.8.0/src/kde_material_you_colors/utils/file_utils.py` & `kde_material_you_colors-1.9.1/src/kde_material_you_colors/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `kde-material-you-colors-1.8.0/src/kde_material_you_colors/utils/konsole_utils.py` & `kde_material_you_colors-1.9.1/src/kde_material_you_colors/utils/konsole_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import subprocess
 import configparser
 import logging
 import dbus
-from .color_utils import hex2rgb
-from .string_utils import tup2str
-from .. import settings
-from ..schemeconfigs import ThemeConfig
+from kde_material_you_colors.utils.color_utils import hex2rgb
+from kde_material_you_colors.utils.string_utils import tup2str
+from kde_material_you_colors import settings
+from kde_material_you_colors.schemeconfigs import ThemeConfig
 
 
 def export_scheme(
     light=None,
     pywal_light=None,
     schemes: ThemeConfig = None,
     konsole_opacity=100,
@@ -117,15 +117,15 @@
 
     with open(
         settings.KONSOLE_COLOR_SCHEME_ALT_PATH, "w", encoding="utf-8"
     ) as configfile:
         config.write(configfile, space_around_delimiters=False)
 
 
-def apply_color_scheme():
+def apply_color_scheme(qdbus_executable: str):
     """Applies the color scheme to the existing default profile or a new one"""
     profile_name = set_default_profile(settings.KONSOLE_DEFAULT_THEMED_PROFILE)
     profile_path = settings.KONSOLE_DIR + profile_name + ".profile"
     create_profile(profile_path, profile_name)
 
     profile = configparser.ConfigParser()
     # preserve case
@@ -153,18 +153,18 @@
         profile["General"]["Parent"] = profile_name
         with open(settings.KONSOLE_TEMP_PROFILE, "w", encoding="utf-8") as configfile:
             profile.write(configfile, space_around_delimiters=False)
 
     except Exception as e:
         logging.exception(f"Error applying Konsole profile:\n{e}")
 
-    reload_profile(profile_name)
+    reload_profile(profile_name, qdbus_executable)
 
 
-def reload_profile(profile: str):
+def reload_profile(profile: str, qdbus_executable: str):
     """Reload the konsole profile for all running konsole sessions
 
     Args:
         profile (str): Konsole profile
     """
     bus = dbus.SessionBus()
     konsole_dbus_services = bus.list_names() or []
@@ -176,15 +176,15 @@
     if konsole_dbus_services:
         logging.debug(
             f"Konsole services (windows) running ({len(konsole_dbus_services)}):"
         )
         for service in konsole_dbus_services:
             try:
                 # get open sessions (tabs and splits)
-                cmd = ["qdbus", service]
+                cmd = [qdbus_executable, service]
                 result = subprocess.run(
                     cmd,
                     stdout=subprocess.PIPE,
                     stderr=subprocess.STDOUT,
                     text=True,
                     check=True,
                 )
```

### Comparing `kde-material-you-colors-1.8.0/src/kde_material_you_colors/utils/ksyntax_utils.py` & `kde_material_you_colors-1.9.1/src/kde_material_you_colors/utils/ksyntax_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 import os
-from .. import settings
+from kde_material_you_colors import settings
+from kde_material_you_colors.schemeconfigs import ThemeConfig
 
 
-def export_schemes(schemes=None):
+def export_schemes(schemes: ThemeConfig):
     # Make sure the schemes path exists
     if not os.path.exists(settings.KSYNTAX_THEMES_DIR):
         os.makedirs(settings.KSYNTAX_THEMES_DIR)
     light_scheme = schemes.get_ksyntax_highlighting_light()
     dark_scheme = schemes.get_ksyntax_highlighting_dark()
 
     with open(
```

### Comparing `kde-material-you-colors-1.8.0/src/kde_material_you_colors/utils/kwin_utils.py` & `kde_material_you_colors-1.9.1/src/kde_material_you_colors/utils/kwin_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import logging
 import subprocess
 import dbus
 import time
-from .. import settings
+from kde_material_you_colors import settings
 
 
-def reload():
+def reload(qdbus_executable: str):
     logging.info(f"Reloading KWin")
     subprocess.Popen(
-        "qdbus org.kde.KWin /KWin reconfigure",
+        qdbus_executable + " org.kde.KWin /KWin reconfigure",
         shell=True,
         stderr=subprocess.DEVNULL,
         stdout=subprocess.DEVNULL,
     )
 
 
 def blend_changes():
@@ -25,15 +25,15 @@
         kwin.start()
     except Exception as e:
         logging.warning(
             f"Could not start blend effect (requires Plasma 5.25 or later):\n{e}"
         )
 
 
-def load_desktop_window_id_script():
+def load_desktop_window_id_script(qdbus_executable: str):
     # based on https://github.com/jinliu/kdotool/blob/master/src/main.rs 7eebebe
     is_loaded = False
     try:
         bus = dbus.SessionBus()
         kwin = bus.get_object("org.kde.KWin", "/Scripting")
         kwin_iface = dbus.Interface(kwin, dbus_interface="org.kde.kwin.Scripting")
         is_loaded = bool(
@@ -61,15 +61,15 @@
 
     # Calling this overloaded method raises TypeError:
     # Fewer items found in D-Bus signature than in Python arguments
     # So have use subprocess with qdbus instead :(
     try:
         # Construct the command with the necessary arguments
         command = [
-            "qdbus",
+            qdbus_executable,
             "org.kde.KWin",
             "/Scripting",
             "org.kde.kwin.Scripting.loadScript",
             settings.KWIN_DESKTOP_ID_JSCRIPT,
             "kde_material_you_get_desktop_view_id",
         ]
 
@@ -89,15 +89,17 @@
         logging.exception(f"An error occurred while loading the script: {e}")
         raise
     except ValueError as e:
         logging.exception(f"An error occurred: {e}")
         raise
 
 
-def get_desktop_window_id(screen: int = 0) -> str | None:
+def get_desktop_window_id(
+    screen: int = 0, qdbus_executable: str = "qdbus6"
+) -> str | None:
     # based on https://github.com/jinliu/kdotool/blob/master/src/main.rs 7eebebe
     """_summary_
 
     Args:
         screen (int): Screen number
 
     Returns:
@@ -120,22 +122,23 @@
     }}
 }}
 // TODO: Make sure this is reliable for more than two monitors,
 // Looks like KWin already returns the windows in a predictable way,
 // it seems the list of windows is sorted by the screens positions(?)
 // and (at least on my machine) this works for any arrangement
 //desktopWindows.sort((b,a) => (a.pos.x - b.pos.x))
-print("KMYC-desktop-window-id:", desktopWindows[{screen}].id)
+// FIXME: Use callDBus + dbus service instead
+console.error("KMYC-desktop-window-id:", desktopWindows[{screen}].id)
 """
     with open(settings.KWIN_DESKTOP_ID_JSCRIPT, "w", encoding="utf-8") as js:
         js.write(script_str)
 
     # Load the script using qdbus
     try:
-        script_id = load_desktop_window_id_script()
+        script_id = load_desktop_window_id_script(qdbus_executable)
     except Exception as error:
         logging.error(error)
         raise
 
     try:
         # run the script
         bus = dbus.SessionBus()
```

### Comparing `kde-material-you-colors-1.8.0/src/kde_material_you_colors/utils/m3_scheme_utils.py` & `kde_material_you_colors-1.9.1/src/kde_material_you_colors/utils/plasma_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,217 +1,232 @@
+import configparser
 import logging
 import os
-from .. import settings
-from . import color_utils
-from . import math_utils
-from . import notify
-from .wallpaper_utils import WallpaperReader
-from .extra_image_utils import sourceColorsFromImage
-from material_color_utilities_python.utils.theme_utils import *
-
-
-def dict_to_rgb(dark_scheme):
-    out = {}
-    for key, color in dark_scheme.items():
-        out.update({key: hexFromArgb(color)})
-    return out
-
-
-def tones_from_palette(palette):
-    tones = {}
-    for x in range(100):
-        tones.update({x: palette.tone(x)})
-    return tones
-
-
-def get_custom_colors(custom_colors):
-    colors = {}
-    for custom_color in custom_colors:
-        value = hexFromArgb(custom_color["color"]["value"])
-        colors.update(
-            {
-                value: {
-                    "color": dict_to_rgb(custom_color["color"]),
-                    "value": hexFromArgb(custom_color["value"]),
-                    "light": dict_to_rgb(custom_color["light"]),
-                    "dark": dict_to_rgb(custom_color["dark"]),
-                }
-            },
-        )
-    return colors
+import subprocess
+from kde_material_you_colors import settings
+from kde_material_you_colors.utils import file_utils
+from kde_material_you_colors.schemeconfigs import ThemeConfig
+from kde_material_you_colors.config import Configs
+from kde_material_you_colors.utils.utils import Watcher
+from kde_material_you_colors.utils import plasma_utils
+
+
+def make_scheme(schemes: ThemeConfig):
+    # Make sure the schemes path exists
+    if not os.path.exists(settings.USER_SCHEMES_PATH):
+        os.makedirs(settings.USER_SCHEMES_PATH)
+    light_scheme = schemes.get_light_scheme()
+    dark_scheme = schemes.get_dark_scheme()
+    # plasma-apply-colorscheme doesnt allow to apply the same theme twice to reload
+    # since I don't know how to reaload it with code lets make a copy and switch between them
+    # sadly color settings will show copies too
+
+    with open(
+        settings.THEME_LIGHT_PATH + "2.colors", "w", encoding="utf8"
+    ) as light_scheme_file:
+        light_scheme_file.write(light_scheme)
+    with open(
+        settings.THEME_LIGHT_PATH + ".colors", "w", encoding="utf8"
+    ) as light_scheme_file:
+        light_scheme_file.write(light_scheme)
+    with open(
+        settings.THEME_DARK_PATH + "2.colors", "w", encoding="utf8"
+    ) as dark_scheme_file:
+        dark_scheme_file.write(dark_scheme)
+    with open(
+        settings.THEME_DARK_PATH + ".colors", "w", encoding="utf8"
+    ) as dark_scheme_file:
+        dark_scheme_file.write(dark_scheme)
+
+    plasma_darker_header(schemes)
 
 
-def get_material_you_colors(wallpaper_data, ncolor, source_type):
-    """Get material you colors from wallpaper or hex color using material-color-utility
+def apply_color_schemes(light=False):
+    color_scheme = settings.THEME_LIGHT_PATH if light else settings.THEME_DARK_PATH
+    subprocess.run(
+        "plasma-apply-colorscheme " + color_scheme + "2.colors",
+        shell=True,
+        stderr=subprocess.DEVNULL,
+        stdout=subprocess.DEVNULL,
+        check=False,
+    )
+    colorscheme_out = subprocess.check_output(
+        "plasma-apply-colorscheme " + color_scheme + ".colors",
+        shell=True,
+        stderr=subprocess.PIPE,
+        universal_newlines=True,
+    ).strip()
+    logging.info(colorscheme_out)
+    # Get hash of the updated theme
+    colors_hash = file_utils.get_file_sha1(color_scheme + ".colors")
+    # Update ColorScheme hash in kdeglobals file
+    if os.path.exists(settings.KDE_GLOBALS) and colors_hash is not None:
+        kdeglobals = configparser.ConfigParser()
+        kdeglobals.optionxform = str
+        try:
+            kdeglobals.read(settings.KDE_GLOBALS)
+            if "General" not in kdeglobals:
+                kdeglobals.add_section("General")
+
+            general = kdeglobals["General"]
+            general["ColorSchemeHash"] = colors_hash
+
+            with open(settings.KDE_GLOBALS, "w", encoding="utf-8") as configfile:
+                kdeglobals.write(configfile, space_around_delimiters=False)
+        except Exception as e:
+            logging.error(f"Error:\n{e}")
+
+
+def set_icons(icons_light, icons_dark, light=False):
+    """Set icon theme with plasma-changeicons for light and dark schemes
 
     Args:
-        wallpaper_data (tuple): wallpaper (type and data)
-        ncolor (int): Alternative color number flag passed to material-color-utility
-        source_type (str): image or color string passed to material-color-utility
+        icons_light (str): Light mode icon theme
+        icons_dark (str): Dark mode icon theme
+        light (bool): wether using light or dark mode
+    """
+
+    icons = icons_light if light else icons_dark
+
+    if icons and settings.PLASMA_CHANGEICONS_PATH:
+        try:
+            # Execute the command to change icons.
+            changeicons_output = subprocess.check_output(
+                [settings.PLASMA_CHANGEICONS_PATH, icons],
+                stderr=subprocess.STDOUT,
+                universal_newlines=True,
+            ).strip()
+            logging.info(f"Icon theme changed to {icons}: {changeicons_output}")
+        except subprocess.CalledProcessError as e:
+            logging.error(f"Error changing icon theme to {icons}: {e.output}")
+    else:
+        if not icons:
+            logging.debug("No icon theme specified.")
+        if not settings.PLASMA_CHANGEICONS_PATH:
+            logging.warning(
+                f"{settings.CHANGE_ICONS_PROGRAM} wasn't found, can't apply icon themes."
+            )
+
+
+def kde_globals_light():
+    kdeglobals = configparser.ConfigParser()
+    if os.path.exists(settings.KDE_GLOBALS):
+        try:
+            kdeglobals.read(settings.KDE_GLOBALS)
+            if "General" in kdeglobals:
+                general = kdeglobals["General"]
+                if "ColorScheme" in general:
+                    if "MaterialYouLight" in general["ColorScheme"]:
+                        return True
+        except Exception as e:
+            logging.error(f"Error:\n{e}")
+
+    return False
+
+
+def get_initial_mode():
+    """Try to get the initial theme mode based based on the theme name,
+    if failed try to get it from the stored hash and the current
+    generated schemes.
 
     Returns:
-        str: string data from python-material-color-utilities
+        bool: Current mode light=True, dark=False
     """
 
-    try:
-        seedColor = 0
-        if source_type == "image":
-            # open image file
-            img = Image.open(wallpaper_data)
-            # resize image proportionally
-            basewidth = 128
-            wpercent = basewidth / float(img.size[0])
-            hsize = int((float(img.size[1]) * float(wpercent)))
-            img = img.resize((basewidth, hsize), Image.Resampling.LANCZOS)
-            # get best colors
-            source_colors = sourceColorsFromImage(img, top=False)
-            # close image file
-            img.close()
-            seed_color = source_colors[0]
-        else:
-            seed_color = argbFromHex(wallpaper_data)
-            source_colors = [seed_color]
-
-        # best colors
-        best_colors = {}
-        for i, color in enumerate(source_colors):
-            best_colors.update({str(i): hexFromArgb(color)})
-        # generate theme from seed color
-        theme = themeFromSourceColor(seed_color)
-
-        # Given a image, the alt color and hex color
-        # return a selected color or a single color for hex code
-        totalColors = len(best_colors)
-        if ncolor and ncolor != None:
-            ncolor = math_utils.clip(ncolor, 0, totalColors, 0)
-        else:
-            ncolor = 0
-
-        if totalColors > ncolor:
-            seedColor = hexFromArgb(source_colors[ncolor])
-            seedNo = ncolor
-        else:
-            seedColor = hexFromArgb(source_colors[-1])
-            seedNo = totalColors - 1
-        if seedColor != 0:
-            theme = themeFromSourceColor(argbFromHex(seedColor))
-
-        dark_scheme = json.loads(theme["schemes"]["dark"].toJSON())
-        light_scheme = json.loads(theme["schemes"]["light"].toJSON())
-        primary_palete = theme["palettes"]["primary"]
-        secondary_palete = theme["palettes"]["secondary"]
-        tertiary_palete = theme["palettes"]["tertiary"]
-        neutral_palete = theme["palettes"]["neutral"]
-        neutral_variant_palete = theme["palettes"]["neutralVariant"]
-        error_palette = theme["palettes"]["error"]
-        custom_colors = theme["customColors"]
-
-        materialYouColors = {
-            "best": best_colors,
-            "seed": {
-                seedNo: hexFromArgb(theme["source"]),
-            },
-            "schemes": {
-                "light": dict_to_rgb(light_scheme),
-                "dark": dict_to_rgb(dark_scheme),
-            },
-            "palettes": {
-                "primary": dict_to_rgb(tones_from_palette(primary_palete)),
-                "secondary": dict_to_rgb(tones_from_palette(secondary_palete)),
-                "tertiary": dict_to_rgb(tones_from_palette(tertiary_palete)),
-                "neutral": dict_to_rgb(tones_from_palette(neutral_palete)),
-                "neutralVariant": dict_to_rgb(
-                    tones_from_palette(neutral_variant_palete)
-                ),
-                "error": dict_to_rgb(tones_from_palette(error_palette)),
-            },
-            "custom": [get_custom_colors(custom_colors)],
-        }
-        return materialYouColors
-
-    except Exception as e:
-        error = f"Error trying to get colors from {wallpaper_data}: {e}"
-        logging.error(error)
-        notify.send_notification("Could not get colors", error)
-        return None
+    theme_from_name = kde_globals_light()
 
+    if theme_from_name is not None:
+        logging.info("Using theme from stored name")
+        return theme_from_name
 
-def get_color_schemes(wallpaper: WallpaperReader, ncolor=None):
-    """Display best colors, allow to select alternative color,
-    and make and apply color schemes for dark and light mode
+    logging.info(
+        "Couldn't find theme by name, trying to resolve theme from last stored hash..."
+    )
 
-    Args:
-        wallpaper (tuple): wallpaper (type and data)
-        ncolor (int): Alternative color number flag passed to material-color-utility
+    current_theme_hash = None
+    kdeglobals = configparser.ConfigParser()
+    kdeglobals.optionxform = str
+    try:
+        kdeglobals.read(settings.KDE_GLOBALS)
+        if "General" in kdeglobals and "ColorSchemeHash" in kdeglobals["General"]:
+            current_theme_hash = kdeglobals["General"]["ColorSchemeHash"]
+    except Exception as e:
+        logging.error(f"Error:\n{e}")
 
-    Returns:
+    if current_theme_hash is not None:
+        logging.debug(f"Config file hash: {current_theme_hash}")
+        dark_scheme_hash = file_utils.get_file_sha1(
+            settings.THEME_DARK_PATH + ".colors"
+        )
+        logging.debug(f"Dark scheme hash: {dark_scheme_hash}")
+        light_scheme_hash = file_utils.get_file_sha1(
+            settings.THEME_LIGHT_PATH + ".colors"
+        )
+        logging.debug(f"Light scheme hash: {light_scheme_hash}")
+        if current_theme_hash == dark_scheme_hash:
+            return False
+        if current_theme_hash == light_scheme_hash:
+            return True
 
-    """
-    if wallpaper is not None:
-        materialYouColors = None
-        wallpaper_type = wallpaper.type
-        wallpaper_data = wallpaper.source
-        if wallpaper_type in ["image", "screenshot"]:
-            if wallpaper_data and os.path.exists(wallpaper_data):
-                if not os.path.isdir(wallpaper_data):
-                    materialYouColors = get_material_you_colors(
-                        wallpaper_data, ncolor=ncolor, source_type="image"
-                    )
-                else:
-                    logging.error(f'"{wallpaper_data}" is a directory, aborting')
-
-        elif wallpaper_type == "color":
-            if wallpaper_data:
-                wallpaper_data = color_utils.color2hex(wallpaper_data)
-                materialYouColors = get_material_you_colors(
-                    wallpaper_data, ncolor=ncolor, source_type=wallpaper_type
-                )
-
-        if materialYouColors is not None:
-            try:
-                if len(materialYouColors["best"]) > 1:
-                    best_colors = f"Best colors: {settings.TERM_STY_BOLD}"
-
-                    for i, color in materialYouColors["best"].items():
-                        rgb = color_utils.hex2rgb(color)
-                        preview = (
-                            f"\033[38;2;{rgb[0]};{rgb[1]};{rgb[2]};1m{color} \033[0m"
-                        )
-                        best_colors += f"{settings.TERM_COLOR_DEF+settings.TERM_STY_BOLD}{i}:{preview}"
-                    logging.info(best_colors[:-5])
-
-                seed = materialYouColors["seed"]
-                sedColor = list(seed.values())[0]
-                seedNo = list(seed.keys())[0]
-                rgb = color_utils.hex2rgb(sedColor)
-                preview = f"\033[38;2;{rgb[0]};{rgb[1]};{rgb[2]};1m{sedColor}\033[0m"
-                logging.info(
-                    f"Using seed: {settings.TERM_COLOR_DEF+settings.TERM_STY_BOLD}{seedNo}:{preview}"
-                )
-                return materialYouColors
-
-            except Exception as e:
-                logging.exception(f"Error:\n{e}")
-                return None
+    logging.warning("Couldn't find previus theme, falling back to dark mode...")
+    return False
 
 
-def export_schemes(schemes):
-    """Export generated schemes to MATERIAL_YOU_COLORS_JSON
+def plasma_darker_header(schemes):
+    """Make a copy of the generated plasma themes but with darker headers
 
     Args:
         schemes (ThemeConfig): generated color schemes
     """
-    colors = schemes.get_material_schemes()
-    colors.update(
-        {
-            "extras": schemes.get_extras(),
-            "pywal": {
-                "light": schemes.get_wal_light_scheme(),
-                "dark": schemes.get_wal_dark_scheme(),
-            },
-        }
-    )
+    light_color = schemes.get_wal_light_scheme()["special"]["background"]
+    dark_color = schemes.get_wal_dark_scheme()["special"]["background"]
+    color_scheme = configparser.ConfigParser()
+    color_scheme.optionxform = str
+    try:
+        # Edit titlebar of dark scheme
+        color_scheme.read(settings.THEME_DARK_PATH + ".colors")
+        color_scheme["Colors:Header][Inactive"]["BackgroundNormal"] = dark_color
+        color_scheme["Colors:Header"]["BackgroundNormal"] = dark_color
+        color_scheme["General"]["Name"] = "Material You Dark (darker titlebar)"
+
+        with open(
+            settings.THEME_DARK_PATH + "_darker_titlebar.colors", "w", encoding="utf-8"
+        ) as configfile:
+            color_scheme.write(configfile, space_around_delimiters=False)
+        color_scheme["General"]["Name"] = "Material You Dark (darker titlebar2)"
+        with open(
+            settings.THEME_DARK_PATH + "_darker_titlebar2.colors", "w", encoding="utf-8"
+        ) as configfile:
+            color_scheme.write(configfile, space_around_delimiters=False)
+
+        # Edit titlebar of light scheme
+        color_scheme.read(settings.THEME_LIGHT_PATH + ".colors")
+        color_scheme["Colors:Header][Inactive"]["BackgroundNormal"] = light_color
+        color_scheme["Colors:Header"]["BackgroundNormal"] = light_color
+        color_scheme["General"]["Name"] = "Material You Light (darker titlebar)"
+
+        with open(
+            settings.THEME_LIGHT_PATH + "_darker_titlebar.colors", "w", encoding="utf-8"
+        ) as configfile:
+            color_scheme.write(configfile, space_around_delimiters=False)
+        color_scheme["General"]["Name"] = "Material You Light (darker titlebar2)"
+        with open(
+            settings.THEME_LIGHT_PATH + "_darker_titlebar2.colors",
+            "w",
+            encoding="utf-8",
+        ) as configfile:
+            color_scheme.write(configfile, space_around_delimiters=False)
 
-    with open(
-        settings.MATERIAL_YOU_COLORS_JSON, "w", encoding="utf8"
-    ) as material_you_colors:
-        json.dump(colors, material_you_colors, indent=4, ensure_ascii=False)
+    except Exception as e:
+        logging.error(f"Error:\n{e}")
+
+
+def update_light_mode(config: Configs, light_mode_watcher: Watcher, first_run: bool):
+    if config.read("light") is not None:
+        light_mode_watcher.set_value(config.read("light"))
+    # try to get the initial theme with from hash
+    elif first_run is True:
+        light_mode_watcher.set_value(plasma_utils.get_initial_mode())
+    else:
+        light_mode_watcher.set_value(plasma_utils.kde_globals_light())
+
+    return light_mode_watcher
```

### Comparing `kde-material-you-colors-1.8.0/src/kde_material_you_colors/utils/notify.py` & `kde_material_you_colors-1.9.1/src/kde_material_you_colors/utils/notify.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import dbus
 import logging
+import dbus
 
 
 def send_notification(heading="", content="", icon=None):
     try:
         bus = dbus.SessionBus()
         notify = dbus.Interface(
             bus.get_object(
```

### Comparing `kde-material-you-colors-1.8.0/src/kde_material_you_colors/utils/pywal_sequences_timeout.py` & `kde_material_you_colors-1.9.1/src/kde_material_you_colors/utils/pywal_sequences_timeout.py`

 * *Files identical despite different names*

### Comparing `kde-material-you-colors-1.8.0/src/kde_material_you_colors/utils/pywal_utils.py` & `kde_material_you_colors-1.9.1/src/kde_material_you_colors/utils/pywal_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
-from .color_utils import hex2rgb
-from .. import settings
-from ..schemeconfigs import ThemeConfig
+from kde_material_you_colors.utils.color_utils import hex2rgb
+from kde_material_you_colors import settings
+from kde_material_you_colors.schemeconfigs import ThemeConfig
 
 if settings.USER_HAS_PYWAL:
+    from kde_material_you_colors.utils import pywal_sequences_timeout
     import pywal
-    from . import pywal_sequences_timeout
 
 
 def apply_schemes(
     light=None,
     pywal_light=None,
     use_pywal=None,
     schemes: ThemeConfig = None,
```

### Comparing `kde-material-you-colors-1.8.0/src/kde_material_you_colors/utils/timeout_utils.py` & `kde_material_you_colors-1.9.1/src/kde_material_you_colors/utils/timeout_utils.py`

 * *Files identical despite different names*

### Comparing `kde-material-you-colors-1.8.0/src/kde_material_you_colors/utils/titlebar_utils.py` & `kde_material_you_colors-1.9.1/src/kde_material_you_colors/utils/titlebar_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import logging
 import configparser
 import os
-from .. import settings
-from . import math_utils
-from . import string_utils
+from kde_material_you_colors import settings
+from kde_material_you_colors.utils import math_utils
+from kde_material_you_colors.utils import string_utils
+from kde_material_you_colors.schemeconfigs import ThemeConfig
 
 
-def sierra_breeze_button_colors(schemes, light=None):
+def sierra_breeze_button_colors(schemes: ThemeConfig, light=None):
     if light == True:
         colors = schemes.get_sierra_breeze_light_colors()
     elif light == False:
         colors = schemes.get_sierra_breeze_dark_colors()
 
     breezerc = configparser.ConfigParser()
     # preserve case
@@ -116,25 +117,25 @@
                     logging.info("Applying Klassy titlebar opacity")
                     with open(settings.KLASSY_RC, "w", encoding="utf-8") as configfile:
                         conf_file.write(configfile, space_around_delimiters=False)
             except Exception as e:
                 logging.exception(f"Error writing Klassy titlebar opacity:\n{e}")
 
 
-def klassy_windeco_outline_color(schemes, light=None):
+def klassy_windeco_outline_color(schemes: ThemeConfig, light=None):
     """Tint Klassy window decoration outline https://github.com/paulmcauley/klassy
 
     Args:
         schemes (ThemeConfig): generated color schemes
         light (bool, optional): Light or dark mode. Defaults to None.
     """
-    if light == True:
-        outline_color = schemes.get_extras()["dark"]["selectionAlt"]
-    elif light == False:
-        outline_color = schemes.get_extras()["dark"]["selectionAlt"]
+    if light:
+        outline_color = schemes.get_material_schemes()["light"]["surfaceTint"]
+    else:
+        outline_color = schemes.get_material_schemes()["dark"]["surfaceTint"]
 
     klassyrc = configparser.ConfigParser()
     # preserve case
     klassyrc.optionxform = str
     if os.path.exists(settings.KLASSY_RC):
         try:
             klassyrc.read(settings.KLASSY_RC)
```

### Comparing `kde-material-you-colors-1.8.0/src/kde_material_you_colors/utils/utils.py` & `kde_material_you_colors-1.9.1/src/kde_material_you_colors/utils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import signal
 import subprocess
 import argparse
 import sys
 import re
 import shutil
 import configparser
-from .. import settings
+from kde_material_you_colors import settings
 
 
 def run_hook(hook):
     if hook is not None:
         subprocess.Popen(hook, shell=True)
 
 
@@ -49,52 +49,61 @@
             )
         except shutil.Error as err:
             logging.error(f"Error: {err}")
             sys.exit(1)
 
 
 def update_desktop_entry():
-    if not settings.IN_PATH:
-        entries = [
-            {
-                "dest": settings.USER_APPS_PATH + settings.AUTOSTART_SCRIPT,
-                "cmd": settings.PKG_BIN,
-            },
-            {
-                "dest": settings.USER_APPS_PATH + settings.STOP_SCRIPT,
-                "cmd": settings.PKG_BIN + " --stop",
-            },
-            {
-                "dest": settings.USER_AUTOSTART_SCRIPT_PATH + settings.AUTOSTART_SCRIPT,
-                "cmd": settings.PKG_BIN,
-            },
-        ]
-        for entry in entries:
-            if os.path.exists(entry["dest"]):
-                logging.debug(f'Updating Exec {entry["dest"]}')
-                config = configparser.ConfigParser()
-                config.optionxform = str
-                config.read(entry["dest"])
-                config.set("Desktop Entry", "Exec", entry["cmd"])
-                with open(entry["dest"], "w", encoding="utf-8") as f:
-                    config.write(f, space_around_delimiters=False)
-        # create symbolic link to user PATH
-
-        if not os.path.exists(settings.USER_LOCAL_BIN_PATH):
-            os.makedirs(settings.USER_LOCAL_BIN_PATH)
-        link_path = settings.USER_LOCAL_BIN_PATH + "kde-material-you-colors"
-        if os.path.islink(link_path):
-            os.unlink(link_path)
-            logging.debug(f"Updating link {settings.PKG_BIN} -> {link_path}")
-        else:
-            logging.debug(f"Creating link {settings.PKG_BIN} -> {link_path}")
-        os.symlink(
-            settings.PKG_BIN,
-            link_path,
-        )
+    # This is now executed when creating/updating the desktop entries.
+    # https://github.com/luisbocanegra/kde-material-you-colors/issues/193
+    # Even when the executable is already on ~/.local/bin/
+    # Saves the user from having to add the install location to $PATH e.g:
+    #  $ cat $HOME/.config/plasma-workspace/env/path.sh
+    #  export PATH=$HOME/.local/bin:$PATH
+    # by always setting the absolute location of the executable.
+    #
+    # Also makes sure the alias exists (for advanced users not using pipx)
+    # so the widget can make use of it
+    entries = [
+        {
+            "dest": settings.USER_APPS_PATH + settings.AUTOSTART_SCRIPT,
+            "cmd": settings.PKG_BIN,
+        },
+        {
+            "dest": settings.USER_APPS_PATH + settings.STOP_SCRIPT,
+            "cmd": settings.PKG_BIN + " --stop",
+        },
+        {
+            "dest": settings.USER_AUTOSTART_SCRIPT_PATH + settings.AUTOSTART_SCRIPT,
+            "cmd": settings.PKG_BIN,
+        },
+    ]
+    for entry in entries:
+        if os.path.exists(entry["dest"]):
+            logging.debug(f'Updating Exec {entry["dest"]}')
+            config = configparser.ConfigParser()
+            config.optionxform = str
+            config.read(entry["dest"])
+            config.set("Desktop Entry", "Exec", entry["cmd"])
+            with open(entry["dest"], "w", encoding="utf-8") as f:
+                config.write(f, space_around_delimiters=False)
+
+    # create symbolic link to user PATH
+    if not os.path.exists(settings.USER_LOCAL_BIN_PATH):
+        os.makedirs(settings.USER_LOCAL_BIN_PATH)
+    link_path = settings.USER_LOCAL_BIN_PATH + "kde-material-you-colors"
+    if os.path.islink(link_path):
+        os.unlink(link_path)
+        logging.debug(f"Updating link {settings.PKG_BIN} -> {link_path}")
+    else:
+        logging.debug(f"Creating link {settings.PKG_BIN} -> {link_path}")
+    os.symlink(
+        settings.PKG_BIN,
+        link_path,
+    )
 
 
 def one_shot_actions(args):
     if args.autostart is True:
         # Autostart desktop entries
         dests = [
             {
```

### Comparing `kde-material-you-colors-1.8.0/src/kde_material_you_colors/utils/wallpaper_utils.py` & `kde_material_you_colors-1.9.1/src/kde_material_you_colors/utils/wallpaper_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import logging
 import dbus
-from .. import settings
-from . import color_utils
-from . import file_utils
-from . import math_utils
-from . import kwin_utils
-from ..config import Configs
+from kde_material_you_colors import settings
+from kde_material_you_colors.utils import color_utils
+from kde_material_you_colors.utils import file_utils
+from kde_material_you_colors.utils import math_utils
+from kde_material_you_colors.utils import kwin_utils
+from kde_material_you_colors.config import Configs
 
 
 class WallpaperReader:
     """Class containing the current wallpaper properties"""
 
     def __init__(self, config: Configs):
         """
@@ -18,18 +18,20 @@
             config (Configs): Current configuration from args and file.
         """
         self._monitor = self.validate_monitor(config.read("monitor"))
         self._screenshot_only_mode = config.read("screenshot_only_mode")
         self._file = config.read("file")
         self._color = config.read("color")
         self._light = config.read("light")
+        self._qdbus_executable = config.read("qdbus_executable") or "qdbus6"
         self._plugin = None
         self._type = None
         self._source = None
         self._error = None
+        self._skip_screenshot = False
         self.reload()
 
     def __str__(self) -> str:
         return f"Wallpaper: {self._plugin} ({self._type}): {self._source}"
 
     @staticmethod
     def validate_monitor(monitor) -> int:
@@ -83,21 +85,25 @@
             "plugin": self._plugin,
             "type": self._type,
             "source": self._source,
             "error": self._error,
         }
         return o
 
-    def screenshot(self):
+    def screenshot(self, skip_screenshot):
         self._type = "screenshot"
+        if skip_screenshot:
+            return
         if settings.SCREENSHOT_HELPER_PATH is None:
             self._error = "Screenshot helper is not installed. Use another wallpaper plugin or install the helper"
             return
         try:
-            screenshot_taken = get_desktop_screenshot(self._monitor)
+            screenshot_taken = get_desktop_screenshot(
+                self._monitor, self._qdbus_executable
+            )
         except Exception as e:
             logging.exception(e)
             self._error = str(e)
             return
 
         if screenshot_taken:
             self._source = settings.SCREENSHOT_PATH
@@ -105,15 +111,15 @@
             error = "Could not take Desktop screenshot"
             logging.error(error)
             self._error = error
 
     def reload(self):
         """Reload current wallpaper"""
         if self._screenshot_only_mode:
-            self.screenshot()
+            self.screenshot(self._skip_screenshot)
             return
 
         # Validate color
         self.validate_color()
         if self._source:
             return
 
@@ -168,20 +174,21 @@
             if isinstance(wallpaper, list):
                 self._error = f"Could not get compatible image from plugin {plugin}, using screenshot method"
             else:
                 self._source = wallpaper
                 return
         else:
             # if everything fails, try taking a screenshot of the desktop
-            self.screenshot()
+            self.screenshot(self._skip_screenshot)
 
-    def update(self, config: Configs):
+    def update(self, config: Configs, skip_screenshot=False):
         """Update from config and reload wallpaper"""
         self._monitor = self.validate_monitor(config.read("monitor"))
         self._screenshot_only_mode = config.read("screenshot_only_mode")
+        self._skip_screenshot = skip_screenshot
         self._file = config.read("file")
         self._color = config.read("color")
         self._light = config.read("light")
         self._plugin = None
         self._type = None
         self._source = None
         self._error = None
@@ -214,18 +221,18 @@
     except dbus.DBusException as e:
         error = f"Error getting wallpaper from dbus: {e.get_dbus_message()}"
         logging.exception(error)
         raise
     return script_output
 
 
-def get_desktop_screenshot(screen=0):
+def get_desktop_screenshot(screen=0, qdbus_executable="qdbus6"):
     # take screenshot of desktop
     try:
-        window_handle = kwin_utils.get_desktop_window_id(screen)
+        window_handle = kwin_utils.get_desktop_window_id(screen, qdbus_executable)
     except Exception as e:
         logging.exception(e)
         raise
 
     screenshot_taken = False
     if window_handle is not None:
         try:
```

### Comparing `kde-material-you-colors-1.8.0/src/kde_material_you_colors.egg-info/PKG-INFO` & `kde_material_you_colors-1.9.1/src/kde_material_you_colors.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kde-material-you-colors
-Version: 1.8.0
+Version: 1.9.1
 Summary: Automatic Material You Colors Generator from your wallpaper for the Plasma Desktop
 Author-email: Luis Bocanegra <luisbocanegra17b@gmail.com>
 Project-URL: Homepage, https://github.com/luisbocanegra/kde-material-you-colors
 Project-URL: Repository, https://github.com/luisbocanegra/kde-material-you-colors
 Project-URL: Bug Tracker, https://github.com/luisbocanegra/kde-material-you-colors/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -12,184 +12,215 @@
 Classifier: Environment :: X11 Applications :: KDE
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dbus-python>=1.3.2
 Requires-Dist: numpy>=1.20
-Requires-Dist: material-color-utilities-python>=0.1.5
+Requires-Dist: pillow>=9.2.0
+Requires-Dist: materialyoucolor>=2.0.8
 Provides-Extra: cli
 Requires-Dist: pywal>=3.3.0; extra == "cli"
 
 <div align="center">
 
 # 🎨 KDE Material You Colors
 
 <img src="https://github.com/luisbocanegra/kde-material-you-colors/assets/15076387/6bd4e04a-48a7-48bc-8dd1-3a75524cd10e" alt="Screenshot" height="250px">
 
-Automatically generate Light/Dark Color Themes for KDE (and pywal if installed) from your current wallpaper, using [Python implementation](https://github.com/avanishsubbiah/material-color-utilities-python) of Google's [Material Color Utilities](https://github.com/material-foundation/material-color-utilities)
+Automatically generate light/dark color themes for KDE (and pywal if installed) from your current wallpaper, using [@T-Dynamos Python implementation](https://github.com/T-Dynamos/materialyoucolor-python) of Google's [Material Color Utilities](https://github.com/material-foundation/material-color-utilities)
 
 [![AUR version](https://img.shields.io/aur/version/kde-material-you-colors?style=for-the-badge&logo=archlinux&labelColor=2d333b&color=1f425f)](https://aur.archlinux.org/packages/kde-material-you-colors)
 [![PyPI - Version](https://img.shields.io/pypi/v/kde-material-you-colors?style=for-the-badge&logo=python&labelColor=2d333b&color=1f425f)](https://pypi.org/project/kde-material-you-colors/)
-[![Dynamic JSON Badge](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fraw.githubusercontent.com%2Fluisbocanegra%2Fkde-material-you-colors%2Fmain%2Fsrc%2Fplasmoid%2Fpackage%2Fmetadata.json&query=KPlugin.Version&style=for-the-badge&color=1f425f&labelColor=2d333b&logo=kde&label=Plasmoid)](https://store.kde.org/p/2073783)
+[![Dynamic JSON Badge](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fraw.githubusercontent.com%2Fluisbocanegra%2Fkde-material-you-colors%2Fmain%2Fsrc%2Fplasmoid%2Fpackage%2Fmetadata.json&query=KPlugin.Version&style=for-the-badge&color=1f425f&labelColor=2d333b&logo=kde&label=Plasmoid)](https://store.kde.org/p/2136963)
 
 </div>
 
 [![Screenshots](https://user-images.githubusercontent.com/15076387/188578458-8171e42b-f36c-44c1-9eb0-506c301d4f16.gif)](https://user-images.githubusercontent.com/15076387/188578458-8171e42b-f36c-44c1-9eb0-506c301d4f16.gif)
 
-# Features
+## Features
 
-## Plasma specific
+### Plasma specific
 
-- [Plasma Widget](https://store.kde.org/p/2073783)
+- [Plasma Widget](https://store.kde.org/p/2136963) (Plasma 6 version)
 - Support for all Wallpaper plugins (color, image, slideshows, animated, Plasma 5.26+ dark wallpaper variants)
 - Update automatically on wallpaper change
 - Change icon themes
 - Start automatically on login
 - Make titlebar darker to match specified applications like terminals, code editors and other programs themed by pywal
 - Follow Plasma Material You Dark/Light change to work with theme schedulers like [Koi](https://github.com/baduhai/Koi)
 - **Plasma addons**
   - Tint [SierraBreeze](https://github.com/kay0u/SierraBreeze) window decoration buttons
   - TitleBar opacity control for [Klassy](https://github.com/paulmcauley/klassy) and [SierraBreezeEnhanced](https://github.com/kupiqu/SierraBreezeEnhanced) window decorations
   - ToolBar opacity control for [Lightly](https://github.com/Luwx/Lightly) Application style
   - Tint [Klassy](https://github.com/paulmcauley/klassy) window decoration outline
 
-## Themeable programs
+### Themeable programs
 
 - Konsole color scheme
   - opacity control
 - **[Pywal](https://github.com/dylanaraps/pywal) support to theme other programs using Material You Colors**
 - Basic KSyntaxHighlighting support (Kate, KWrite, KDevelop...)
 
-## Theming options
+### Theming options
 
 - Alternative Material You color selection if the wallpaper provides more than one
 - Use your favorite color to generate Material You color schemes
 - Custom colors list used for konsole/pywal
-- Custom amount for background color tint
+- Custom amount for colorfulness and brightness of theme
+- Color scheme variants from Material You (Vibrant, Monochrome, Neutral...)
 - Dark/light Color schemes (Plasma and pywal/konsole independently)
 - Set a script that will be executed on start or wallpaper/dark/light/settings change
 - Configuration file
 
-# Installing
+## Installing
 
-## 1. Backend
+1. Install `pipx` system packages from your distribution packages.
 
-Using pypi with `pipx` (recommended) using this command,
-```sh
-pipx install kde-material-you-colors
-# Optional
-# pywal to theme other programs using Material You Colors
-pipx inject kde-material-you-colors pywal
-```
+2. Install the backend
 
-or `pip` using this command
-```sh
-pip install kde-material-you-colors
-# Optional
-# pywal to theme other programs using Material You Colors
-pip install pywal
-```
+    **For Plasma 5** this is the last version, development has switched to plasma 6
+
+    ```sh
+    pipx install kde-material-you-colors==1.7.1
+    pipx inject kde-material-you-colors pywal
+    ```
+
+    **For Plasma 6**
+
+    ```sh
+    pipx install kde-material-you-colors
+    pipx inject kde-material-you-colors pywal
+    # to upgrade to newer version
+    pipx upgrade kde-material-you-colors
+    ```
+
+    **Note:** You may need to install `gcc python-dbus-dev libglib2.0-dev` system packages or their equivalent for your distribution. Additionally, installing some libraries for Pillow may be necessary, see [Pillow docs](https://pillow.readthedocs.io/en/latest/installation.html#external-libraries)
+
+3. Install the widget from the KDE Store [Plasma 6 version](https://store.kde.org/p/2136963) | [Plasma 5 version](https://www.pling.com/p/2073783/)
+
+   1. **Right click on the Panel** > **Add Widgets** > **Get New Widgets** > **Download New Plasma Widgets**
+   2. **Search** for "**KDE Material You Colors**", install & add it to your Panel/Desktop.
+
+4. Install the screenshot helper. **Optional but recommended if you use other than default Image wallpaper plugin**
+
+    **Plasma 6**
+
+    Install `git extra-cmake-modules` system packages or their equivalent for your distribution.
+
+    ```sh
+    git clone https://github.com/luisbocanegra/kde-material-you-colors
+    ./install-screenshot-helper.sh
+    ```
 
-> [!IMPORTANT]
-> You may need to install `gcc python-dbus-dev libglib2.0-dev` system packages or their equivalent for your distribution. Additionally, installing some libraries for Pillow may be necessary, see [Pillow docs](https://pillow.readthedocs.io/en/latest/installation.html#external-libraries)
+    **Plasma 5**
 
-## 2. Plasma widget and desktop screenshot helper (support for all wallpaper plugins)
+    Install `git extra-cmake-modules` system packages or their equivalent for your distribution.
 
-Install `extra-cmake-modules qt5-qttools-devel kf5-plasma-devel` system packages or their equivalent for your distribution.
+    ```sh
+    git clone https://github.com/luisbocanegra/kde-material-you-colors -b plasma5
+    ./install-screenshot-helper.sh
+    ```
 
-### User install
+To upgrade to a new version repeat these steps.
+
+**Note:** When you upgrade te widget to a newer version it will inform you if it requires a new version of the backend.
+
+### Arch Linux
+
+- [AUR](https://aur.archlinux.org/packages/kde-material-you-colors) use your preferred AUR helper e.g:
 
 ```sh
-cmake -B build -S . -DCMAKE_INSTALL_PREFIX=~/.local -DINSTALL_PLASMOID=ON
-cmake --build build
-cmake --install build
+yay -S kde-material-you-colors
 ```
 
-### System-wide install
+## Running
+
+You can Start and change the configuration from the widget.
+
+### From terminal
 
 ```sh
-cmake -B build -S . -DCMAKE_INSTALL_PREFIX=/usr -DINSTALL_PLASMOID=ON
-cmake --build build
-sudo cmake --install build
+kde-material-you-colors
 ```
 
-> [!NOTE]
-> You can also install the widget from the [KDE Store](https://store.kde.org/p/2073783) and set `-DINSTALL_PLASMOID=OFF` in the command above
->
-> 1. Right click on panel > Add Widgets > Get New Widgets > Download New Plasma Widgets
-> 2. Search for "KDE Material You Colors"
+Run `kde-material-you-colors -h` to see the list of available options (Flags take precedence over configuration file)
 
-### Arch Linux
+### Starting/Stopping Desktop entries
 
-- [AUR](https://aur.archlinux.org/packages/kde-material-you-colors) use your preferred AUR helper
+**If not installed by your package manager**, run `kde-material-you-colors -cl`
 
-### Optional features
+- To start the program launch **KDE Material You Colors** from your applications list
+- To stop, launch **Stop KDE Material You Colors** from your applications list
+
+### Running on Startup
+
+```sh
+kde-material-you-colors -a
+```
 
-- Install the [pywal](https://pypi.org/project/pywal/) python module to theme other programs using Material You Colors
-  - Check [pywal Customization Wiki](https://github.com/dylanaraps/pywal/wiki/Customization) to theme supported programs
+#### Removing from autostart
 
-# Running from terminal to debug your configuration
+1. Open **System Settings** > **Autostart**
+2. Remove **kde-material-you-colors** by clicking on the **Trash** button.
 
-- Run `kde-material-you-colors`
+## Configuration file
 
-- Flags take precedence over configuration file, run `kde-material-you-colors -h` to see the list of available options
+The preferred way to change the configuration is from the widget. If the configuration doesn't exist, it will be automatically created by the widget.
 
-## Starting/Stopping Desktop entries
+**Editing manually**
 
-> [!NOTE]
-> **If not installed by your package manager**, run `kde-material-you-colors -cl` to copy desktop entries to ~/.local/share/applications/
+The default configuration file can be created by running `kde-material-you-colors -c` the location is `~/.config/kde-material-you-colors/config.conf`
 
-- To start the program launch **KDE Material You Colors** from your applications list
-- To stop it launch **Stop KDE Material You Colors** from your applications list
+Run `kde-material-you-colors` with no arguments from terminal to test your changes in real time.
 
-# Running on Startup
+Due to Qt limitations, comments are removed from the configuration file by the widget. **You can view the sample configuration file with comments [here](https://github.com/luisbocanegra/kde-material-you-colors/blob/main/src/kde_material_you_colors/data/sample_config.conf)**.
 
-After finishing the setup, you can make it run automatically on boot
+## FAQ
 
-1. Copy the default configuration to ~/.config/kde-material-you-colors/config.conf:
+**Q.** How does this different from Plasma's "**Accent Color From Wallpaper**" and "**Tint all colors with accent color**"?
 
-    `kde-material-you-colors -c`
+There are some key differences:
 
-2. Set the program to automatically start with Plasma:
+- Brighter accent/buttons colors
+- Option to choose another color if the wallpaper returns more than one
+- Can also apply colors to Konsole and pywal (both from wallpaper and custom ones)
+- Colors comparison https://imgur.com/a/a28uZka (kde-material-you-colors top, default tint option bottom)
 
-    `kde-material-you-colors -a`
+**Q.** Why there are duplicated color schemes in **System Settings**
 
-3. Reboot or logout/login and test the changes
+To update color with `plasma-apply-colorscheme` (utility provided by KDE developers), the file containing the new color scheme must have a different name than the current one, to workaround that, this program creates two color scheme files with different names, then applies one after the other. As a result you end up with duplicated color schemes and maybe some lag while updating schemes.
 
-## Removing from autostart
+**Q.** Can't get wallpaper colors of the default wallpaper
 
-1. Open `System Settings` > `Startup and Shutdown`
-2. Remove `kde-material-you-colors` by clicking on the `-` button.
+If you are using the default Image wallpaper plugin try changing the image to something else at least once first.
 
-# Configuration file
+**Q.** Slideshow wallpaper (or any other Plugin) doesn't update colors correctly
 
-- Copy default configuration: run `kde-material-you-colors -c`
-- Edit ~/.config/kde-material-you-colors/config.conf
-- Run `kde-material-you-colors` with no arguments from terminal to test it.
-- **You can view the sample configuration file [here](https://github.com/luisbocanegra/kde-material-you-colors/blob/main/src/kde_material_you_colors/data/sample_config.conf)**
+Try enabling **Only use screenshot method** from the widget **Advanced settings**
 
-# Notes
+**Q.** How does wallpaper detection work and why it fails sometimes?
 
-- To update color with `plasma-apply-colorscheme` (utility provided by plasma developers), the file containing the new color scheme must have a different name than the current one, to workaround this the program creates two scheme files with different names, then applies one after the other. As a result you end up with duplicated color schemes and maybe some lag while updating schemes.
+The wallpaper is obtained in the following order:
 
-- The wallpaper is obtained in the following order:
+- First, uses the [Plasma Desktop Scripting API](https://develop.kde.org/docs/plasma/scripting/api/) to read Wallpaper plugin configuration.
+- If the previous fails, the screenshot helper (if installed) is used
 
-  - First, uses the [Plasma Desktop Scripting API](https://develop.kde.org/docs/plasma/scripting/api/) to read Wallpaper plugin configuration.
-  - If the previous fails, the screenshot helper (if installed) is used
+The backend uses the [KWin Scripting API](https://develop.kde.org/docs/plasma/kwin/api/) and calls the screenshot helper to take a Screenshot of the Desktop view using the [KWin's Screenshot plugin](https://github.com/KDE/kwin/tree/master/src/plugins/screenshot)
 
-    The backend uses the [KWin Scripting API](https://develop.kde.org/docs/plasma/kwin/api/) and calls the screenshot helper to take a Screenshot of the Desktop view using the [KWin's Screenshot plugin](https://github.com/KDE/kwin/tree/master/src/plugins/screenshot)
+Both methods are somewhat robust but there are edge cases when detection will fail, which are [explained here](https://github.com/luisbocanegra/kde-material-you-colors/issues/187)
 
 ## Bug reporting / Feature requests / Contributing
 
-Please read the [Contributing guidelines in this repository](CONTRIBUTING.md)
+Please read the [Contributing guidelines in this repository](https://github.com/luisbocanegra/kde-material-you-colors/blob/main/CONTRIBUTING.md)
 
-# Credits
+## Credits
 
-- [Python Implementation](https://github.com/avanishsubbiah/material-color-utilities-python) of Material Color Utilities used by this project.
+- [@T-Dynamos Python Implementation](https://github.com/T-Dynamos/materialyoucolor-python) of Material Color Utilities used by this project.
+- [@avanisubbiah Python Implementation](https://github.com/avanishsubbiah/material-color-utilities-python) of Material Color Utilities (used until v1.8.0).
 - [Material Color Utilities](https://github.com/material-foundation/material-color-utilities)
 - [Pywal](https://github.com/dylanaraps/pywal) used to apply material colors to pywal supported software
 - [MaterialColorUtilities (C#)](https://github.com/albi005/MaterialColorUtilities) (used until v0.8.0).
 - [xdg-desktop-portal-kde](https://invent.kde.org/plasma/xdg-desktop-portal-kde) base for desktop screenshot helper.
 - [kdotool](https://github.com/jinliu/kdotool) base for getting desktop window id.
-- [Google LLC. / Pictogrammers](https://pictogrammers.com/library/mdi/) for the widget icon.
+- [Google LLC. / Pictogrammers](https://pictogrammers.com/library/mdi/) for the widget icon assets.
 - [This comment on Reddit](https://www.reddit.com/r/kde/comments/mg6wr4/comment/gssbtqe/?utm_source=share&utm_medium=web2x&context=3) and [ksetwallpaper](https://github.com/pashazz/ksetwallpaper) for the code to get the current Wallpaper that served me as inspiration.
```

### Comparing `kde-material-you-colors-1.8.0/src/kde_material_you_colors.egg-info/SOURCES.txt` & `kde_material_you_colors-1.9.1/src/kde_material_you_colors.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kde-material-you-colors-1.8.0/src/plasmoid/CMakeLists.txt` & `kde_material_you_colors-1.9.1/src/plasmoid/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `kde-material-you-colors-1.8.0/src/plasmoid/package/contents/icons/icon.svg` & `kde_material_you_colors-1.9.1/src/plasmoid/package/contents/icons/icon.svg`

 * *Files identical despite different names*

### Comparing `kde-material-you-colors-1.8.0/src/plasmoid/package/contents/ui/CompactRepresentation.qml` & `kde_material_you_colors-1.9.1/src/plasmoid/package/contents/ui/CompactRepresentation.qml`

 * *Files identical despite different names*

### Comparing `kde-material-you-colors-1.8.0/src/plasmoid/package/contents/ui/FullRepresentation.qml` & `kde_material_you_colors-1.9.1/src/plasmoid/package/contents/ui/FullRepresentation.qml`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import QtQuick
 import QtQuick.Dialogs
 import QtQuick.Controls
 import QtQuick.Layouts
 
 import "components" as Components
+import org.kde.coreaddons 1.0 as KCoreAddons
 import org.kde.kirigami as Kirigami
 import org.kde.kquickcontrols
 import org.kde.plasma.components as PlasmaComponents3
 import org.kde.plasma.core as PlasmaCore
 import org.kde.plasma.plasma5support as P5Support
 import org.kde.plasma.extras as PlasmaExtras
 import org.kde.plasma.plasmoid
@@ -23,27 +24,27 @@
     Layout.preferredWidth: rootRep.width
     Layout.preferredHeight: rootRep.height
 
     property bool autoHide: true
     property bool backendRunning: true
     property string homeDir: StandardPaths.writableLocation(
                             StandardPaths.HomeLocation).toString().substring(7)
-    property string username: ""
+    property string username: kuser.loginName
 
     property string execName: 'kde-material-you-colors'
     property string execPath: ""
     property string checkBackendCommand: 'ps -o user,pid,cmd -C '+execName+' --no-headers | grep -e "'+username+'" | grep -v "<defunct>" | grep -ve "--version" | grep "" | awk \'{print $2}\''
     property string startBackendCommand: execPath
     property string autoStartBackendCommand: execPath + ' --autostart;' + execPath
     property string backendVersionCommand: execPath + ' --version'
     property string backendVersion: ""
     property string backendVersionDisplay: backendVersion !== "" ? backendVersion : "unknown"
-    property string recommendedVersion: "1.8.0"
+    property string recommendedVersion: "1.9.1"
     property string versionStatus: "same"
-    property string versionMessage: "You're using a "+versionStatus+" version of the backend (<strong>" + backendVersionDisplay + "</strong>) than this widget version was written for (<strong>"+ recommendedVersion+ "</strong>). Some features may be missing or not work as intended. You can find the latest versions of the widget <a href='https://store.kde.org/p/2073783'>here</a> and the backend <a href='https://github.com/luisbocanegra/kde-material-you-colors'>here</a>."
+    property string versionMessage: "You're using a "+versionStatus+" version of the backend (<strong>" + backendVersionDisplay + "</strong>) than this widget version was written for (<strong>"+ recommendedVersion+ "</strong>). Some features may be missing or not work as intended. You can find the latest versions of the widget <a href='https://store.kde.org/p/2136963'>here</a> and the backend <a href='https://github.com/luisbocanegra/kde-material-you-colors'>here</a>."
     property bool showVersionMessage: false
 
     property bool onDesktop: plasmoid.location === PlasmaCore.Types.Floating
     property bool plasmoidExpanded: main.expanded
     property bool autoReloadEnabled: onDesktop || plasmoidExpanded
 
     // used to trigger reload from parent if true
@@ -58,14 +59,18 @@
 
     property bool pauseMode: false
 
     signal savePauseMode()
 
     property Item parentMain
 
+    KCoreAddons.KUser {
+        id: kuser
+    }
+
     Connections {
         target: parentMain
         function onTogglePauseMode() {
             fullRepresentation.pauseMode = !fullRepresentation.pauseMode
             parentMain.pauseModeMain = fullRepresentation.pauseMode
             savePauseMode()
         }
@@ -85,14 +90,27 @@
     // Non escaped version: find /usr/share/icons ~/.local/share/icons -maxdepth 2 -type f -path '*/icons/*/index.theme' ! -path '*/share/icons' ! -exec grep -q '^Hidden=true' {} \; ! -execdir test -d cursors \; -printf '%p\n' | while read line; do echo "$(basename $(dirname $line)),$(grep '^Name=' $line | sed 's/^Name=//')"; done
     property string getIconThemesCommand: "find /usr/share/icons " +homeDir+"/.local/share/icons -maxdepth 2 -type f -path '*/icons/*/index.theme' ! -path '*/share/icons' ! -exec grep -q '^Hidden=true' {} \\; ! -execdir test -d cursors \\; -printf '%p\\n' | while read line; do echo \"$(basename $(dirname $line)),$(grep '^Name=' $line | sed 's/^Name=//;s/-/ /')\"; done | sort --field-separator=, --key=2n -k2,2"
 
     ListModel {
         id: iconThemeList
     }
 
+    ListModel {
+        id: schemeVariantsModel
+        ListElement { text: "Content"; value: 0 }
+        ListElement { text: "Expressive"; value: 1 }
+        ListElement { text: "Fidelity"; value: 2 }
+        ListElement { text: "Monochrome"; value: 3 }
+        ListElement { text: "Neutral"; value: 4 }
+        ListElement { text: "TonalSpot"; value: 5 }
+        ListElement { text: "Vibrant"; value: 6 }
+        ListElement { text: "Rainbow"; value: 7 }
+        ListElement { text: "FruitSalad"; value: 8 }
+    }
+
     onPlasmoidExpandedChanged: {
         checkConfigChange.exec(checkConfigChangeCommand)
         findExecutablePath()
     }
 
     onConfigSha1Changed: {
         // trigger a reload when config changes to update view
@@ -107,24 +125,17 @@
         if (temp == "") {
             temp = StandardPaths.findExecutable(execName,
                         homeDir+"/.local/bin").toString().substring(7)
         }
         execPath = temp
 
     }
-    function getUsername() {
-        var parts = homeDir.split('/');
-        if (parts.length > 2 && parts[1] === "home") {
-            username = parts[2];
-        }
-    }
 
     Component.onCompleted: {
         findExecutablePath()
-        getUsername()
     }
 
     P5Support.DataSource {
         id: checkBackend
         engine: "executable"
         connectedSources: []
 
@@ -503,16 +514,14 @@
                                     property string color_last: "#d0265c"; \
                                     property string custom_colors_list; \
                                     property string custom_colors_list_last; \
                                     property bool light: false; \
                                     property int ncolor: 0; \
                                     property bool pywal:false; \
                                     property bool pywal_light: false; \
-                                    property real light_blend_multiplier: 1.0; \
-                                    property real dark_blend_multiplier: 1.0; \
                                     property real light_saturation_multiplier: 1.0; \
                                     property real dark_saturation_multiplier: 1.0; \
                                     property real light_brightness_multiplier: 1.0; \
                                     property real dark_brightness_multiplier: 1.0; \
                                     property bool plasma_follows_scheme: true; \
                                     property bool pywal_follows_scheme: true; \
                                     property bool disable_konsole: false; \
@@ -532,14 +541,18 @@
                                     property bool use_startup_delay: false; \
                                     property int startup_delay: 0; \
                                     property int main_loop_delay: 1; \
                                     property int screenshot_delay: 900; \
                                     property bool once_after_change: false; \
                                     property bool pause_mode: false; \
                                     property bool screenshot_only_mode: false; \
+                                    property int scheme_variant: 5; \
+                                    property real chroma_multiplier: 1.0; \
+                                    property real tone_multiplier: 1.0; \
+                                    property string qdbus_executable; \
                                 }';
 
                             settings = Qt.createQmlObject(settingsString, mainLayout, "settingsObject");
                             settings.fileName = StandardPaths.writableLocation(
                                         StandardPaths.HomeLocation).toString().substring(7) +
                                         "/.config/kde-material-you-colors/config.conf"
                             customTextColorsCheck.checked = settings.custom_colors_list == ""
@@ -660,19 +673,31 @@
                             Layout.preferredWidth: mainLayout.width
                             spacing: Kirigami.Units.smallSpacing
 
                             RowLayout {
                                 Item { Layout.fillWidth: true }
                                 // visible: fullRepresentation.versionStatus !== "same"
                                 visible: fullRepresentation.showVersionMessage
-                                Label {
+                                TextEdit {
                                     Layout.fillWidth: true
                                     text: fullRepresentation.versionMessage
-                                    onLinkActivated: Qt.openUrlExternally(link)
                                     wrapMode: Text.WordWrap
+                                    textFormat: TextEdit.RichText
+                                    readOnly: true
+
+                                    color: Kirigami.Theme.textColor
+                                    selectedTextColor: Kirigami.Theme.highlightedTextColor
+                                    selectionColor: Kirigami.Theme.highlightColor
+
+                                    onLinkActivated: (url) => Qt.openUrlExternally(url)
+
+                                    HoverHandler {
+                                        acceptedButtons: Qt.NoButton
+                                        cursorShape: parent.hoveredLink ? Qt.PointingHandCursor : Qt.ArrowCursor
+                                    }
                                 }
 
                                 ToolButton { // PlasmaComponents3 one doesnt take colors??
                                     icon.name: "dialog-warning"
                                     visible: fullRepresentation.showVersionMessage
                                     opacity: 0.8
                                     Kirigami.Theme.inherit: false
@@ -1179,100 +1204,137 @@
                                 height: 1
                                 color: dividerColor
                                 opacity: dividerOpacity
                             }
 
                             PlasmaExtras.Heading {
                                 level: 1
-                                text: "Color amount"
+                                text: "Color scheme"
                                 Layout.alignment: Qt.AlignHCenter
                             }
 
-                            // Dark blend
+                            // RowLayout {
+                            //     PlasmaComponents3.Label {
+                            //         text: "Variant"
+                            //         Layout.alignment: Qt.AlignLeft
+                            //     }
+                            //     PlasmaComponents3.ComboBox {
+                            //         model: schemeVariantsModel
+                            //         Layout.fillWidth: true
+                            //         textRole: "text"
+                            //         valueRole: "value"
+                            //         currentIndex: settings.scheme_variant
+
+                            //         onCurrentIndexChanged: {
+                            //             settings.scheme_variant = model.get(currentIndex)["value"]
+                            //         }
+                            //     }
+                            // }
+
+                            Flow {
+                                Layout.preferredWidth: mainLayout.width
+                                spacing: 6
+
+                                ButtonGroup { id: buttonGroup }
+
+                                Repeater {
+                                    model: schemeVariantsModel
+
+                                    PlasmaComponents3.Button {
+                                        checkable: true
+                                        ButtonGroup.group: buttonGroup
+                                        text: checked ? model.text : model.text
+                                        checked: index === settings.scheme_variant
+                                        onCheckedChanged: {
+                                            if (checked) settings.scheme_variant = index
+                                        }
+                                    }
+                                }
+                            }
+
+                            // Chroma mult
                             RowLayout {
+                                width: parent.width
+                                Layout.fillWidth: true
+
                                 PlasmaComponents3.Label {
-                                    text: "Dark blend"
+                                    text: "Colorfulness"
                                     Layout.alignment: Qt.AlignLeft
                                 }
 
                                 PlasmaComponents3.Slider {
-                                    id: darkBlend
-                                    value: settings.dark_blend_multiplier
+                                    id: lightBlend
+                                    value: settings.chroma_multiplier
                                     from: 0
-                                    to: 4.0
-                                    stepSize: 0.2
+                                    to: 10
                                     Layout.fillWidth: true
                                     onValueChanged: {
-                                        settings.dark_blend_multiplier = Math.round(value * 10) / 10
+                                        settings.chroma_multiplier = Math.round(value * 10) / 10
                                     }
                                 }
 
                                 PlasmaComponents3.TextField {
-                                    id: darkBlendManual
+                                    id: lightBlendManual
                                     Layout.preferredWidth: controlWidth
-                                    placeholderText: "0-4"
+                                    placeholderText: "0-10"
                                     horizontalAlignment: TextInput.AlignHCenter
-                                    text: parseFloat(settings.dark_blend_multiplier)
+                                    text: parseFloat(settings.chroma_multiplier)
 
                                     validator: DoubleValidator {
-                                        bottom: 0.0
-                                        top: 4.0
+                                        bottom: 0
+                                        top: 10
                                         decimals: 1
                                         notation: DoubleValidator.StandardNotation
                                     }
 
                                     onAccepted: {
-                                        settings.dark_blend_multiplier = parseFloat(text)
+                                        settings.chroma_multiplier = parseFloat(text)
                                     }
                                 }
                             }
 
-
-                            // Light blend
+                            // Tone mult
                             RowLayout {
-                                width: parent.width
-                                Layout.fillWidth: true
-
                                 PlasmaComponents3.Label {
-                                    text: "Light blend"
+                                    text: "Brightness"
                                     Layout.alignment: Qt.AlignLeft
                                 }
 
                                 PlasmaComponents3.Slider {
-                                    id: lightBlend
-                                    value: settings.light_blend_multiplier
-                                    from: 0
-                                    to: 4.0
-                                    stepSize: 0.2
+                                    id: darkBlend
+                                    value: settings.tone_multiplier
+                                    from: 0.5
+                                    to: 1.5
                                     Layout.fillWidth: true
                                     onValueChanged: {
-                                        settings.light_blend_multiplier = Math.round(value * 10) / 10
+                                        settings.tone_multiplier = Math.round(value * 10) / 10
                                     }
                                 }
 
                                 PlasmaComponents3.TextField {
-                                    id: lightBlendManual
+                                    id: darkBlendManual
                                     Layout.preferredWidth: controlWidth
                                     placeholderText: "0-4"
                                     horizontalAlignment: TextInput.AlignHCenter
-                                    text: parseFloat(settings.light_blend_multiplier)
+                                    text: parseFloat(settings.tone_multiplier)
 
                                     validator: DoubleValidator {
-                                        bottom: 0.0
-                                        top: 4.0
+                                        bottom: 0.5
+                                        top: 1.5
                                         decimals: 1
                                         notation: DoubleValidator.StandardNotation
                                     }
 
                                     onAccepted: {
-                                        settings.light_blend_multiplier = parseFloat(text)
+                                        settings.tone_multiplier = parseFloat(text)
                                     }
                                 }
                             }
 
+
                             PlasmaComponents3.ToolButton {
                                 Layout.alignment: Qt.AlignHCenter
                                 text: fullRepresentation.showAdvanced?"Hide advanced settings":"Show advanced settings"
                                 icon.name: 'configure'
                                 checked: fullRepresentation.showAdvanced
                                 onClicked: {
                                     fullRepresentation.showAdvanced = !fullRepresentation.showAdvanced
@@ -1730,14 +1792,63 @@
                             Rectangle {
                                 Layout.preferredWidth: mainLayout.width
                                 height: 1
                                 color: dividerColor
                                 opacity: dividerOpacity
                             }
 
+                            RowLayout {
+                                Layout.alignment: Qt.AlignHCenter
+                                PlasmaExtras.Heading {
+                                    level: 1
+                                    text: "QDbus executable"
+                                }
+                                PlasmaComponents3.ToolButton {
+                                    id: qdbusInfoBtn
+                                    icon.name: "help-hint"
+                                    opacity: 0.7
+                                    hoverEnabled: true
+                                    onClicked: qdbusInfoPopup.open()
+
+                                    PlasmaComponents3.ToolTip {
+                                        id: qdbusInfoPopup
+                                        x: qdbusInfoBtn.width / 2
+                                        y: qdbusInfoBtn.height
+                                        text: "Name or location of the QDbus executable e.g qdbus6, qdbus-qt6... (default is qdbus6)"
+                                    }
+                                }
+                            }
+
+                            RowLayout {
+                                PlasmaComponents3.Label {
+                                    text: "Executable"
+                                }
+                                PlasmaComponents3.TextField {
+                                    placeholderText: qsTr("e.g qdbus6, qdbus-qt6... (default is qdbus6)")
+                                    Layout.fillWidth: true
+                                    text: settings.qdbus_executable
+                                    onAccepted: {
+                                        settings.qdbus_executable = text
+                                    }
+                                }
+                                PlasmaComponents3.Button {
+                                    icon.name: "document-open"
+                                    onClicked: {
+                                        fileDialogQdbusExec.open()
+                                    }
+                                }
+                            }
+
+                            Rectangle {
+                                Layout.preferredWidth: mainLayout.width
+                                height: 1
+                                color: dividerColor
+                                opacity: dividerOpacity
+                            }
+
                             PlasmaExtras.Heading {
                                 level: 1
                                 text: "Delay & screenshot options"
                                 Layout.alignment: Qt.AlignHCenter
                             }
 
                             RowLayout{
@@ -1928,41 +2039,58 @@
                                     wrapMode: Text.WordWrap
                                     horizontalAlignment: Text.AlignHCenter
                                 }
 
                                 PlasmaComponents3.Label {
                                     text: "Plasmoid version: " + Plasmoid.metaData.version
                                     Layout.alignment: Qt.AlignHCenter
-                                    onLinkActivated: Qt.openUrlExternally(link)
                                 }
 
                                 PlasmaComponents3.Label {
                                     text: "Backend version: " + fullRepresentation.backendVersionDisplay
                                     Layout.alignment: Qt.AlignHCenter
-                                    onLinkActivated: Qt.openUrlExternally(link)
                                 }
 
-                                PlasmaComponents3.Label {
-                                    text: "If you like the project you can leave a review in <a href='https://store.kde.org/p/2073783'>KDE Store</a> or give it a star on <a href='https://github.com/luisbocanegra/kde-material-you-colors'>Github</a>. For bugs and feature requests please go to the <a href='https://github.com/luisbocanegra/kde-material-you-colors/issues'>issues page</a>."
-                                    onLinkActivated: Qt.openUrlExternally(link)
+                                TextEdit {
+                                    text: "If you like the project you can leave a review in <a href='https://store.kde.org/p/2136963'>KDE Store</a> or give it a star on <a href='https://github.com/luisbocanegra/kde-material-you-colors'>Github</a>. For bugs and feature requests please go to the <a href='https://github.com/luisbocanegra/kde-material-you-colors/issues'>issues page</a>."
                                     wrapMode: Text.WordWrap
+                                    readOnly: true
+                                    textFormat: TextEdit.RichText
                                     Layout.alignment: Qt.AlignHCenter
                                     Layout.preferredWidth: mainLayout.width
                                     horizontalAlignment: Text.AlignHCenter
+
+                                    color: Kirigami.Theme.textColor
+                                    selectedTextColor: Kirigami.Theme.highlightedTextColor
+                                    selectionColor: Kirigami.Theme.highlightColor
+
+                                    onLinkActivated: (url) => Qt.openUrlExternally(url)
+
+                                    HoverHandler {
+                                        acceptedButtons: Qt.NoButton
+                                        cursorShape: parent.hoveredLink ? Qt.PointingHandCursor : Qt.ArrowCursor
+                                    }
                                 }
                             }
 
                             FileDialog {
                                 id: fileDialogHookExec
                                 onAccepted: {
                                     mainLayout.settings.on_change_hook = fileDialogHookExec.fileUrl.toString().substring(7)
                                 }
                             }
 
                             FileDialog {
+                                id: fileDialogQdbusExec
+                                onAccepted: {
+                                    mainLayout.settings.qdbus_executable = fileDialogQdbusExec.fileUrl.toString().substring(7)
+                                }
+                            }
+
+                            FileDialog {
                                 id: fileDialogBackendExec
                                 onAccepted: {
                                     mainLayout.settings.gui_custom_exec_location = fileDialogBackendExec.fileUrl.toString().substring(7)
                                 }
                             }
                         }
```

#### html2text {}

```diff
@@ -1,74 +1,79 @@
 import Qt.labs.platform import Qt.labs.settings import
 Qt5Compat.GraphicalEffects import QtQuick import QtQuick.Dialogs import
 QtQuick.Controls import QtQuick.Layouts import "components" as Components
-import org.kde.kirigami as Kirigami import org.kde.kquickcontrols import
-org.kde.plasma.components as PlasmaComponents3 import org.kde.plasma.core as
-PlasmaCore import org.kde.plasma.plasma5support as P5Support import
-org.kde.plasma.extras as PlasmaExtras import org.kde.plasma.plasmoid
-ColumnLayout { id: fullRepresentation Layout.minimumWidth:
-Kirigami.Units.gridUnit * 20 Layout.minimumHeight: Kirigami.Units.gridUnit * 19
-Layout.preferredWidth: rootRep.width Layout.preferredHeight: rootRep.height
-property bool autoHide: true property bool backendRunning: true property string
-homeDir: StandardPaths.writableLocation( StandardPaths.HomeLocation).toString
-().substring(7) property string username: "" property string execName: 'kde-
-material-you-colors' property string execPath: "" property string
-checkBackendCommand: 'ps -o user,pid,cmd -C '+execName+' --no-headers | grep -
-e "'+username+'" | grep -v "" | grep -ve "--version" | grep "" | awk \'{print
-$2}\'' property string startBackendCommand: execPath property string
+import org.kde.coreaddons 1.0 as KCoreAddons import org.kde.kirigami as
+Kirigami import org.kde.kquickcontrols import org.kde.plasma.components as
+PlasmaComponents3 import org.kde.plasma.core as PlasmaCore import
+org.kde.plasma.plasma5support as P5Support import org.kde.plasma.extras as
+PlasmaExtras import org.kde.plasma.plasmoid ColumnLayout { id:
+fullRepresentation Layout.minimumWidth: Kirigami.Units.gridUnit * 20
+Layout.minimumHeight: Kirigami.Units.gridUnit * 19 Layout.preferredWidth:
+rootRep.width Layout.preferredHeight: rootRep.height property bool autoHide:
+true property bool backendRunning: true property string homeDir:
+StandardPaths.writableLocation( StandardPaths.HomeLocation).toString
+().substring(7) property string username: kuser.loginName property string
+execName: 'kde-material-you-colors' property string execPath: "" property
+string checkBackendCommand: 'ps -o user,pid,cmd -C '+execName+' --no-headers |
+grep -e "'+username+'" | grep -v "" | grep -ve "--version" | grep "" | awk \'
+{print $2}\'' property string startBackendCommand: execPath property string
 autoStartBackendCommand: execPath + ' --autostart;' + execPath property string
 backendVersionCommand: execPath + ' --version' property string backendVersion:
 "" property string backendVersionDisplay: backendVersion !== "" ?
-backendVersion : "unknown" property string recommendedVersion: "1.8.0" property
+backendVersion : "unknown" property string recommendedVersion: "1.9.1" property
 string versionStatus: "same" property string versionMessage: "You're using a
 "+versionStatus+" version of the backend ("" ++ bbaacckkeennddVVeerrssiioonnDDiissppllaayy ++ "") than
 this widget version was written for (""++ rreeccoommmmeennddeeddVVeerrssiioonn++ ""). Some features
 may be missing or not work as intended. You can find the latest versions of the
 widget _h_e_r_e and the backend _h_e_r_e." property bool showVersionMessage: false
 property bool onDesktop: plasmoid.location === PlasmaCore.Types.Floating
 property bool plasmoidExpanded: main.expanded property bool autoReloadEnabled:
 onDesktop || plasmoidExpanded // used to trigger reload from parent if true
 property bool doSettingsReload // used to trigger a reload if the config file
 has changed property string configPath: homeDir + "/.config/kde-material-you-
 colors/config.conf" property string checkConfigChangeCommand: "sha1sum " +
 configPath+" 2> /dev/null" property string configSha1 property bool
 showAdvanced: false property bool pauseMode: false signal savePauseMode()
-property Item parentMain Connections { target: parentMain function
-onTogglePauseMode() { fullRepresentation.pauseMode =
+property Item parentMain KCoreAddons.KUser { id: kuser } Connections { target:
+parentMain function onTogglePauseMode() { fullRepresentation.pauseMode =
 !fullRepresentation.pauseMode parentMain.pauseModeMain =
 fullRepresentation.pauseMode savePauseMode() } } Connections { target:
 parentMain function onUpdatePauseMode() { parentMain.pauseModeMain =
 fullRepresentation.pauseMode } } // Get a list of installed icon themes as
 id,name // - discard hidden themes // - discard cursor themes // Non escaped
 version: find /usr/share/icons ~/.local/share/icons -maxdepth 2 -type f -path
 '*/icons/*/index.theme' ! -path '*/share/icons' ! -exec grep -q '^Hidden=true'
 {} \; ! -execdir test -d cursors \; -printf '%p\n' | while read line; do echo
 "$(basename $(dirname $line)),$(grep '^Name=' $line | sed 's/^Name=//')"; done
 property string getIconThemesCommand: "find /usr/share/icons "
 +homeDir+"/.local/share/icons -maxdepth 2 -type f -path '*/icons/*/index.theme'
 ! -path '*/share/icons' ! -exec grep -q '^Hidden=true' {} \\; ! -execdir test -
 d cursors \\; -printf '%p\\n' | while read line; do echo \"$(basename $(dirname
 $line)),$(grep '^Name=' $line | sed 's/^Name=//;s/-/ /')\"; done | sort --
-field-separator=, --key=2n -k2,2" ListModel { id: iconThemeList }
-onPlasmoidExpandedChanged: { checkConfigChange.exec(checkConfigChangeCommand)
-findExecutablePath() } onConfigSha1Changed: { // trigger a reload when config
-changes to update view console.log("@@@@@ RELOADING ID:", plasmoid.id)
-doSettingsReload = true doSettingsReload = false } function findExecutablePath
-() { var temp = "" temp = StandardPaths.findExecutable(execName).toString
-().substring(7) if (temp == "") { temp = StandardPaths.findExecutable(execName,
-homeDir+"/.local/bin").toString().substring(7) } execPath = temp } function
-getUsername() { var parts = homeDir.split('/'); if (parts.length > 2 && parts
-[1] === "home") { username = parts[2]; } } Component.onCompleted:
-{ findExecutablePath() getUsername() } P5Support.DataSource { id: checkBackend
-engine: "executable" connectedSources: [] onNewData: function(source, data)
-{ var exitCode = data["exit code"] var exitStatus = data["exit status"] var
-stdout = data["stdout"] var stderr = data["stderr"] exited(source, exitCode,
-exitStatus, stdout, stderr) disconnectSource(source) // cmd finished } function
-exec(cmd) { checkBackend.connectSource(cmd ) } signal exited(string cmd, int
-exitCode, int exitStatus, string stdout, string stderr) } Connections { target:
+field-separator=, --key=2n -k2,2" ListModel { id: iconThemeList } ListModel
+{ id: schemeVariantsModel ListElement { text: "Content"; value: 0 } ListElement
+{ text: "Expressive"; value: 1 } ListElement { text: "Fidelity"; value: 2 }
+ListElement { text: "Monochrome"; value: 3 } ListElement { text: "Neutral";
+value: 4 } ListElement { text: "TonalSpot"; value: 5 } ListElement { text:
+"Vibrant"; value: 6 } ListElement { text: "Rainbow"; value: 7 } ListElement
+{ text: "FruitSalad"; value: 8 } } onPlasmoidExpandedChanged:
+{ checkConfigChange.exec(checkConfigChangeCommand) findExecutablePath() }
+onConfigSha1Changed: { // trigger a reload when config changes to update view
+console.log("@@@@@ RELOADING ID:", plasmoid.id) doSettingsReload = true
+doSettingsReload = false } function findExecutablePath() { var temp = "" temp =
+StandardPaths.findExecutable(execName).toString().substring(7) if (temp == "")
+{ temp = StandardPaths.findExecutable(execName, homeDir+"/.local/bin").toString
+().substring(7) } execPath = temp } Component.onCompleted: { findExecutablePath
+() } P5Support.DataSource { id: checkBackend engine: "executable"
+connectedSources: [] onNewData: function(source, data) { var exitCode = data
+["exit code"] var exitStatus = data["exit status"] var stdout = data["stdout"]
+var stderr = data["stderr"] exited(source, exitCode, exitStatus, stdout,
+stderr) disconnectSource(source) // cmd finished } function exec(cmd)
+{ checkBackend.connectSource(cmd ) } signal exited(string cmd, int exitCode,
+int exitStatus, string stdout, string stderr) } Connections { target:
 checkBackend function onExited(cmd, exitCode, exitStatus, stdout, stderr) { /
 / console.log("CHECK BACKEND"); // console.log("cmd:",cmd); // console.log
 ("exitCode:",exitCode); // console.log("stdout:",stdout); // console.log
 ("stderr:",stderr); backendRunning = stdout.replace('\n', '').trim().length>0 }
 } P5Support.DataSource { id: checkBackendVersion engine: "executable"
 connectedSources: [] onNewData: function(source, data) { var exitCode = data
 ["exit code"] var exitStatus = data["exit status"] var stdout = data["stdout"]
@@ -180,41 +185,42 @@
 / save relevant configs with _last suffix to recover them after reenable
 property var settings: null function createSettings() { var settingsString =
 'import Qt.labs.settings 1.0; \ Settings { \ category: "CUSTOM"; \ property int
 monitor: 0; \ property string color; \ property string color_last: "#d0265c"; \
 property string custom_colors_list; \ property string custom_colors_list_last;
 \ property bool light: false; \ property int ncolor: 0; \ property bool pywal:
 false; \ property bool pywal_light: false; \ property real
-light_blend_multiplier: 1.0; \ property real dark_blend_multiplier: 1.0; \
-property real light_saturation_multiplier: 1.0; \ property real
-dark_saturation_multiplier: 1.0; \ property real light_brightness_multiplier:
-1.0; \ property real dark_brightness_multiplier: 1.0; \ property bool
-plasma_follows_scheme: true; \ property bool pywal_follows_scheme: true; \
-property bool disable_konsole: false; \ property string iconslight; \ property
-string iconsdark; \ property int konsole_opacity: 100; \ property int
-konsole_opacity_dark: 100; \ property int titlebar_opacity: 100; \ property int
-titlebar_opacity_dark: 100; \ property int toolbar_opacity: 100; \ property int
-toolbar_opacity_dark: 100; \ property bool sierra_breeze_buttons_color: false;
-\ property bool klassy_windeco_outline: false; \ property string
-darker_window_list; \ property string on_change_hook; \ property string
-gui_custom_exec_location; \ property bool use_startup_delay: false; \ property
-int startup_delay: 0; \ property int main_loop_delay: 1; \ property int
-screenshot_delay: 900; \ property bool once_after_change: false; \ property
-bool pause_mode: false; \ property bool screenshot_only_mode: false; \ }';
-settings = Qt.createQmlObject(settingsString, mainLayout, "settingsObject");
-settings.fileName = StandardPaths.writableLocation
-( StandardPaths.HomeLocation).toString().substring(7) + "/.config/kde-material-
-you-colors/config.conf" customTextColorsCheck.checked =
-settings.custom_colors_list == "" customColorCheck.checked = settings.color ==
-"" } function destroySettings() { settings.destroy() // settings = null }
-function saveCustomColorsList() { var colors = []; for (var i = 0; i <
-colorPickerRepeater.count; i++) { var colorBtn = colorPickerRepeater.itemAt(i);
-colors.push(colorBtn.color.toString()); } // do not re-enable custom colors if
-is disabled if (customTextColorsCheck.checked) { settings.custom_colors_list =
-"" } else { settings.custom_colors_list = colors.join(" ");
+light_saturation_multiplier: 1.0; \ property real dark_saturation_multiplier:
+1.0; \ property real light_brightness_multiplier: 1.0; \ property real
+dark_brightness_multiplier: 1.0; \ property bool plasma_follows_scheme: true; \
+property bool pywal_follows_scheme: true; \ property bool disable_konsole:
+false; \ property string iconslight; \ property string iconsdark; \ property
+int konsole_opacity: 100; \ property int konsole_opacity_dark: 100; \ property
+int titlebar_opacity: 100; \ property int titlebar_opacity_dark: 100; \
+property int toolbar_opacity: 100; \ property int toolbar_opacity_dark: 100; \
+property bool sierra_breeze_buttons_color: false; \ property bool
+klassy_windeco_outline: false; \ property string darker_window_list; \ property
+string on_change_hook; \ property string gui_custom_exec_location; \ property
+bool use_startup_delay: false; \ property int startup_delay: 0; \ property int
+main_loop_delay: 1; \ property int screenshot_delay: 900; \ property bool
+once_after_change: false; \ property bool pause_mode: false; \ property bool
+screenshot_only_mode: false; \ property int scheme_variant: 5; \ property real
+chroma_multiplier: 1.0; \ property real tone_multiplier: 1.0; \ property string
+qdbus_executable; \ }'; settings = Qt.createQmlObject(settingsString,
+mainLayout, "settingsObject"); settings.fileName =
+StandardPaths.writableLocation( StandardPaths.HomeLocation).toString
+().substring(7) + "/.config/kde-material-you-colors/config.conf"
+customTextColorsCheck.checked = settings.custom_colors_list == ""
+customColorCheck.checked = settings.color == "" } function destroySettings()
+{ settings.destroy() // settings = null } function saveCustomColorsList() { var
+colors = []; for (var i = 0; i < colorPickerRepeater.count; i++) { var colorBtn
+= colorPickerRepeater.itemAt(i); colors.push(colorBtn.color.toString()); } /
+/ do not re-enable custom colors if is disabled if
+(customTextColorsCheck.checked) { settings.custom_colors_list = "" } else
+{ settings.custom_colors_list = colors.join(" ");
 settings.custom_colors_list_last = colors.join(" "); } } P5Support.DataSource
 { id: readMaterialYouData engine: "executable" connectedSources: [] onNewData:
 function(source, data) { var exitCode = data["exit code"] var exitStatus = data
 ["exit status"] var stdout = data["stdout"] var stderr = data["stderr"] exited
 (source, exitCode, exitStatus, stdout, stderr) disconnectSource(source) // cmd
 finished } function exec() { readMaterialYouData.connectSource( "cat /tmp/kde-
 material-you-colors-"+username+".json" ) } signal exited(string cmd, int
@@ -240,22 +246,27 @@
 testenv/bin/kde-material-you-colors -cl" Layout.alignment: Qt.AlignHCenter
 color: Kirigami.Theme.neutralTextColor wrapMode: Text.WordWrap
 horizontalAlignment: Text.AlignHCenter visible: fullRepresentation.execPath ==
 "" } // NORMAL SETTINGS ColumnLayout { visible:
 !fullRepresentation.showAdvanced Layout.preferredWidth: mainLayout.width
 spacing: Kirigami.Units.smallSpacing RowLayout { Item { Layout.fillWidth: true
 } // visible: fullRepresentation.versionStatus !== "same" visible:
-fullRepresentation.showVersionMessage Label { Layout.fillWidth: true text:
-fullRepresentation.versionMessage onLinkActivated: Qt.openUrlExternally(link)
-wrapMode: Text.WordWrap } ToolButton { // PlasmaComponents3 one doesnt take
-colors?? icon.name: "dialog-warning" visible:
-fullRepresentation.showVersionMessage opacity: 0.8 Kirigami.Theme.inherit:
-false Kirigami.Theme.textColor: Kirigami.Theme.neutralTextColor
-Kirigami.Theme.highlightColor: Kirigami.Theme.neutralTextColor hoverEnabled:
-true onClicked: { fullRepresentation.showVersionMessage =
+fullRepresentation.showVersionMessage TextEdit { Layout.fillWidth: true text:
+fullRepresentation.versionMessage wrapMode: Text.WordWrap textFormat:
+TextEdit.RichText readOnly: true color: Kirigami.Theme.textColor
+selectedTextColor: Kirigami.Theme.highlightedTextColor selectionColor:
+Kirigami.Theme.highlightColor onLinkActivated: (url) => Qt.openUrlExternally
+(url) HoverHandler { acceptedButtons: Qt.NoButton cursorShape:
+parent.hoveredLink ? Qt.PointingHandCursor : Qt.ArrowCursor } } ToolButton { /
+/ PlasmaComponents3 one doesnt take colors?? icon.name: "dialog-warning"
+visible: fullRepresentation.showVersionMessage opacity: 0.8
+Kirigami.Theme.inherit: false Kirigami.Theme.textColor:
+Kirigami.Theme.neutralTextColor Kirigami.Theme.highlightColor:
+Kirigami.Theme.neutralTextColor hoverEnabled: true onClicked:
+{ fullRepresentation.showVersionMessage =
 !fullRepresentation.showVersionMessage } Layout.alignment:
 Qt.AlignHRight|Qt.AlignTop PlasmaComponents3.ToolTip { x: parent.width / 2 y:
 parent.height text: "Tap to hide" } } } // COLOR SELECTION FROM WALLPAPER OR
 CUSTOM COLOR RowLayout { Item { Layout.fillWidth: true } PlasmaExtras.Heading
 { level: 1 text: "Colors source" anchors.centerIn: parent } ToolButton { /
 / PlasmaComponents3 one doesnt take colors?? id: versionInfoBtn icon.name:
 "dialog-warning" visible: !fullRepresentation.showVersionMessage &&
@@ -396,36 +407,44 @@
 PlasmaComponents3.RadioButton { checked: !pywalEnableDark.checked &&
 !pywalFollowScheme.checked//settings.light text: qsTr("Disabled")
 ButtonGroup.group: pywalModeGroup } PlasmaComponents3.RadioButton { id:
 pywalFollowScheme checked: settings.pywal_follows_scheme text: qsTr("Follow
 color scheme") onCheckedChanged: { settings.pywal_follows_scheme = checked }
 ButtonGroup.group: pywalModeGroup } } } // pywal dark Rectangle
 { Layout.preferredWidth: mainLayout.width height: 1 color: dividerColor
-opacity: dividerOpacity } PlasmaExtras.Heading { level: 1 text: "Color amount"
-Layout.alignment: Qt.AlignHCenter } // Dark blend RowLayout
-{ PlasmaComponents3.Label { text: "Dark blend" Layout.alignment: Qt.AlignLeft }
-PlasmaComponents3.Slider { id: darkBlend value: settings.dark_blend_multiplier
-from: 0 to: 4.0 stepSize: 0.2 Layout.fillWidth: true onValueChanged:
-{ settings.dark_blend_multiplier = Math.round(value * 10) / 10 } }
-PlasmaComponents3.TextField { id: darkBlendManual Layout.preferredWidth:
+opacity: dividerOpacity } PlasmaExtras.Heading { level: 1 text: "Color scheme"
+Layout.alignment: Qt.AlignHCenter } // RowLayout { // PlasmaComponents3.Label
+{ // text: "Variant" // Layout.alignment: Qt.AlignLeft // } /
+/ PlasmaComponents3.ComboBox { // model: schemeVariantsModel /
+/ Layout.fillWidth: true // textRole: "text" // valueRole: "value" /
+/ currentIndex: settings.scheme_variant // onCurrentIndexChanged: { /
+/ settings.scheme_variant = model.get(currentIndex)["value"] // } // } // }
+Flow { Layout.preferredWidth: mainLayout.width spacing: 6 ButtonGroup { id:
+buttonGroup } Repeater { model: schemeVariantsModel PlasmaComponents3.Button
+{ checkable: true ButtonGroup.group: buttonGroup text: checked ? model.text :
+model.text checked: index === settings.scheme_variant onCheckedChanged: { if
+(checked) settings.scheme_variant = index } } } } // Chroma mult RowLayout
+{ width: parent.width Layout.fillWidth: true PlasmaComponents3.Label { text:
+"Colorfulness" Layout.alignment: Qt.AlignLeft } PlasmaComponents3.Slider { id:
+lightBlend value: settings.chroma_multiplier from: 0 to: 10 Layout.fillWidth:
+true onValueChanged: { settings.chroma_multiplier = Math.round(value * 10) / 10
+} } PlasmaComponents3.TextField { id: lightBlendManual Layout.preferredWidth:
+controlWidth placeholderText: "0-10" horizontalAlignment:
+TextInput.AlignHCenter text: parseFloat(settings.chroma_multiplier) validator:
+DoubleValidator { bottom: 0 top: 10 decimals: 1 notation:
+DoubleValidator.StandardNotation } onAccepted: { settings.chroma_multiplier =
+parseFloat(text) } } } // Tone mult RowLayout { PlasmaComponents3.Label { text:
+"Brightness" Layout.alignment: Qt.AlignLeft } PlasmaComponents3.Slider { id:
+darkBlend value: settings.tone_multiplier from: 0.5 to: 1.5 Layout.fillWidth:
+true onValueChanged: { settings.tone_multiplier = Math.round(value * 10) / 10 }
+} PlasmaComponents3.TextField { id: darkBlendManual Layout.preferredWidth:
 controlWidth placeholderText: "0-4" horizontalAlignment: TextInput.AlignHCenter
-text: parseFloat(settings.dark_blend_multiplier) validator: DoubleValidator
-{ bottom: 0.0 top: 4.0 decimals: 1 notation: DoubleValidator.StandardNotation }
-onAccepted: { settings.dark_blend_multiplier = parseFloat(text) } } } // Light
-blend RowLayout { width: parent.width Layout.fillWidth: true
-PlasmaComponents3.Label { text: "Light blend" Layout.alignment: Qt.AlignLeft }
-PlasmaComponents3.Slider { id: lightBlend value:
-settings.light_blend_multiplier from: 0 to: 4.0 stepSize: 0.2 Layout.fillWidth:
-true onValueChanged: { settings.light_blend_multiplier = Math.round(value * 10)
-/ 10 } } PlasmaComponents3.TextField { id: lightBlendManual
-Layout.preferredWidth: controlWidth placeholderText: "0-4" horizontalAlignment:
-TextInput.AlignHCenter text: parseFloat(settings.light_blend_multiplier)
-validator: DoubleValidator { bottom: 0.0 top: 4.0 decimals: 1 notation:
-DoubleValidator.StandardNotation } onAccepted:
-{ settings.light_blend_multiplier = parseFloat(text) } } }
+text: parseFloat(settings.tone_multiplier) validator: DoubleValidator { bottom:
+0.5 top: 1.5 decimals: 1 notation: DoubleValidator.StandardNotation }
+onAccepted: { settings.tone_multiplier = parseFloat(text) } } }
 PlasmaComponents3.ToolButton { Layout.alignment: Qt.AlignHCenter text:
 fullRepresentation.showAdvanced?"Hide advanced settings":"Show advanced
 settings" icon.name: 'configure' checked: fullRepresentation.showAdvanced
 onClicked: { fullRepresentation.showAdvanced = !fullRepresentation.showAdvanced
 } } } // ADVANCED SECTION ColumnLayout { id: advancedSection visible:
 fullRepresentation.showAdvanced Layout.preferredWidth: mainLayout.width
 onVisibleChanged: { if (visible) { scrollTimer.start() } } // Konsole
@@ -532,86 +551,103 @@
 wallpaper/dark/light/settings change" } } } RowLayout { PlasmaComponents3.Label
 { text: "Script" } PlasmaComponents3.TextField { placeholderText: qsTr("e.g /
 home/"+username+"/scripts/script.sh") Layout.fillWidth: true text:
 settings.on_change_hook onAccepted: { settings.on_change_hook = text } }
 PlasmaComponents3.Button { icon.name: "document-open" onClicked:
 { fileDialogHookExec.open() } } } Rectangle { Layout.preferredWidth:
 mainLayout.width height: 1 color: dividerColor opacity: dividerOpacity }
-PlasmaExtras.Heading { level: 1 text: "Delay & screenshot options"
-Layout.alignment: Qt.AlignHCenter } RowLayout{ PlasmaComponents3.Label { text:
-"Startup delay (seconds)" } PlasmaComponents3.TextField
-{ Layout.preferredWidth: controlWidth * 1.5 placeholderText: "0-?"
-horizontalAlignment: TextInput.AlignHCenter text: parseInt
-(settings.startup_delay) // Layout.fillWidth: true validator: IntValidator
-{ bottom: 0 } onAccepted: { settings.startup_delay = parseInt(text) // reset
-color selection settings.use_startup_delay = settings.startup_delay > 0 } }
-PlasmaComponents3.ToolButton { id: startupDelayBtn icon.name: "help-contents"
-hoverEnabled: true onClicked: startupDelayPopup.open()
-PlasmaComponents3.ToolTip { id: startupDelayPopup x: startupDelayBtn.width / 2
-y: startupDelayBtn.height text: "Delay before doing anything\nUseful for
-waiting for other utilities that may change themes on boot (default is 0)" } }
-} RowLayout { PlasmaComponents3.Label { text: "Wallpaper detection delay" }
+RowLayout { Layout.alignment: Qt.AlignHCenter PlasmaExtras.Heading { level: 1
+text: "QDbus executable" } PlasmaComponents3.ToolButton { id: qdbusInfoBtn
+icon.name: "help-hint" opacity: 0.7 hoverEnabled: true onClicked:
+qdbusInfoPopup.open() PlasmaComponents3.ToolTip { id: qdbusInfoPopup x:
+qdbusInfoBtn.width / 2 y: qdbusInfoBtn.height text: "Name or location of the
+QDbus executable e.g qdbus6, qdbus-qt6... (default is qdbus6)" } } } RowLayout
+{ PlasmaComponents3.Label { text: "Executable" } PlasmaComponents3.TextField
+{ placeholderText: qsTr("e.g qdbus6, qdbus-qt6... (default is qdbus6)")
+Layout.fillWidth: true text: settings.qdbus_executable onAccepted:
+{ settings.qdbus_executable = text } } PlasmaComponents3.Button { icon.name:
+"document-open" onClicked: { fileDialogQdbusExec.open() } } } Rectangle
+{ Layout.preferredWidth: mainLayout.width height: 1 color: dividerColor
+opacity: dividerOpacity } PlasmaExtras.Heading { level: 1 text: "Delay &
+screenshot options" Layout.alignment: Qt.AlignHCenter } RowLayout
+{ PlasmaComponents3.Label { text: "Startup delay (seconds)" }
 PlasmaComponents3.TextField { Layout.preferredWidth: controlWidth * 1.5
 placeholderText: "0-?" horizontalAlignment: TextInput.AlignHCenter text:
-parseInt(settings.main_loop_delay) // Layout.fillWidth: true validator:
-IntValidator { bottom: 0 } onAccepted: { settings.main_loop_delay = parseInt
-(text) // reset color selection } } PlasmaComponents3.ToolButton { id:
-mainDelayBtn icon.name: "help-contents" hoverEnabled: true onClicked:
-mainDelayPopup.open() PlasmaComponents3.ToolTip { id: mainDelayPopup x:
-mainDelayBtn.width / 2 y: mainDelayBtn.height text: "Main loop delay (in
-seconds).\nUseful for decreasing unnecessary detections or save a bit of power
-(default is 1)" } } } RowLayout { PlasmaComponents3.Label { text: "Screenshot
-method delay" } PlasmaComponents3.TextField { Layout.preferredWidth:
+parseInt(settings.startup_delay) // Layout.fillWidth: true validator:
+IntValidator { bottom: 0 } onAccepted: { settings.startup_delay = parseInt
+(text) // reset color selection settings.use_startup_delay =
+settings.startup_delay > 0 } } PlasmaComponents3.ToolButton { id:
+startupDelayBtn icon.name: "help-contents" hoverEnabled: true onClicked:
+startupDelayPopup.open() PlasmaComponents3.ToolTip { id: startupDelayPopup x:
+startupDelayBtn.width / 2 y: startupDelayBtn.height text: "Delay before doing
+anything\nUseful for waiting for other utilities that may change themes on boot
+(default is 0)" } } } RowLayout { PlasmaComponents3.Label { text: "Wallpaper
+detection delay" } PlasmaComponents3.TextField { Layout.preferredWidth:
 controlWidth * 1.5 placeholderText: "0-?" horizontalAlignment:
-TextInput.AlignHCenter text: parseInt(settings.screenshot_delay) /
+TextInput.AlignHCenter text: parseInt(settings.main_loop_delay) /
 / Layout.fillWidth: true validator: IntValidator { bottom: 0 } onAccepted:
-{ settings.screenshot_delay = parseInt(text) // reset color selection } }
-PlasmaComponents3.ToolButton { id: screenshotDelayBtn icon.name: "help-
-contents" hoverEnabled: true onClicked: screenshotDelayPopup.open()
-PlasmaComponents3.ToolTip { id: screenshotDelayPopup x:
-screenshotDelayBtn.width / 2 y: screenshotDelayBtn.height text: "Delay after
-taking screenshot (in seconds).\nUseful for live wallpapers that display a
-constant transition based on time or other circumstances, which would trigger
-colors generation too often (default is 900)" } } } RowLayout
-{ PlasmaComponents3.Label { text: "Only use screenshot method"
-Layout.alignment: Qt.AlignLeft } PlasmaComponents3.CheckBox { checked:
-settings.screenshot_only_mode onCheckedChanged: { settings.screenshot_only_mode
-= checked } } PlasmaComponents3.ToolButton { icon.name: "help-contents"
-hoverEnabled: true onClicked: screenshotModePopup.open()
-PlasmaComponents3.ToolTip { id: screenshotModePopup x: parent.width / 2 y:
-parent.height text: "Forces the backend to take screenshot of the desktop,
-instead of trying to get the wallpaper from Plasma.\nThis method uses more
-resources if the time between screenshots is too small!" } } } RowLayout
-{ PlasmaComponents3.Label { text: "Single screenshot mode" Layout.alignment:
-Qt.AlignLeft } PlasmaComponents3.CheckBox { checked: settings.once_after_change
-onCheckedChanged: { settings.once_after_change = checked } }
-PlasmaComponents3.ToolButton { icon.name: "help-contents" hoverEnabled: true
-onClicked: pauseScreenshotDelayPopup.open() PlasmaComponents3.ToolTip { id:
-pauseScreenshotDelayPopup x: parent.width / 2 y: parent.height text: "Only
-extract colors from screenshot after changing wallpaper plugin. This option
-makes sense for wallpaper plugins that display an animated loop that never
-stops. Makes the color extraction run only a single time instead of detecting
-every change." } } } Rectangle { Layout.topMargin: Kirigami.Units.mediumSpacing
-Layout.preferredWidth: mainLayout.width height: 1 color: dividerColor opacity:
-dividerOpacity } ColumnLayout { spacing: Kirigami.Units.mediumSpacing opacity:
-0.9 PlasmaExtras.Heading { level: 2 text: "About " + Plasmoid.metaData.name
-Layout.alignment: Qt.AlignHCenter wrapMode: Text.WordWrap horizontalAlignment:
-Text.AlignHCenter } PlasmaComponents3.Label { text: "Plasmoid version: " +
-Plasmoid.metaData.version Layout.alignment: Qt.AlignHCenter onLinkActivated:
-Qt.openUrlExternally(link) } PlasmaComponents3.Label { text: "Backend version:
-" + fullRepresentation.backendVersionDisplay Layout.alignment: Qt.AlignHCenter
-onLinkActivated: Qt.openUrlExternally(link) } PlasmaComponents3.Label { text:
-"If you like the project you can leave a review in _K_D_E_ _S_t_o_r_e or give it a star
-on _G_i_t_h_u_b. For bugs and feature requests please go to the _i_s_s_u_e_s_ _p_a_g_e."
-onLinkActivated: Qt.openUrlExternally(link) wrapMode: Text.WordWrap
-Layout.alignment: Qt.AlignHCenter Layout.preferredWidth: mainLayout.width
-horizontalAlignment: Text.AlignHCenter } } FileDialog { id: fileDialogHookExec
-onAccepted: { mainLayout.settings.on_change_hook =
-fileDialogHookExec.fileUrl.toString().substring(7) } } FileDialog { id:
-fileDialogBackendExec onAccepted:
+{ settings.main_loop_delay = parseInt(text) // reset color selection } }
+PlasmaComponents3.ToolButton { id: mainDelayBtn icon.name: "help-contents"
+hoverEnabled: true onClicked: mainDelayPopup.open() PlasmaComponents3.ToolTip
+{ id: mainDelayPopup x: mainDelayBtn.width / 2 y: mainDelayBtn.height text:
+"Main loop delay (in seconds).\nUseful for decreasing unnecessary detections or
+save a bit of power (default is 1)" } } } RowLayout { PlasmaComponents3.Label
+{ text: "Screenshot method delay" } PlasmaComponents3.TextField
+{ Layout.preferredWidth: controlWidth * 1.5 placeholderText: "0-?"
+horizontalAlignment: TextInput.AlignHCenter text: parseInt
+(settings.screenshot_delay) // Layout.fillWidth: true validator: IntValidator
+{ bottom: 0 } onAccepted: { settings.screenshot_delay = parseInt(text) // reset
+color selection } } PlasmaComponents3.ToolButton { id: screenshotDelayBtn
+icon.name: "help-contents" hoverEnabled: true onClicked:
+screenshotDelayPopup.open() PlasmaComponents3.ToolTip { id:
+screenshotDelayPopup x: screenshotDelayBtn.width / 2 y:
+screenshotDelayBtn.height text: "Delay after taking screenshot (in
+seconds).\nUseful for live wallpapers that display a constant transition based
+on time or other circumstances, which would trigger colors generation too often
+(default is 900)" } } } RowLayout { PlasmaComponents3.Label { text: "Only use
+screenshot method" Layout.alignment: Qt.AlignLeft } PlasmaComponents3.CheckBox
+{ checked: settings.screenshot_only_mode onCheckedChanged:
+{ settings.screenshot_only_mode = checked } } PlasmaComponents3.ToolButton
+{ icon.name: "help-contents" hoverEnabled: true onClicked:
+screenshotModePopup.open() PlasmaComponents3.ToolTip { id: screenshotModePopup
+x: parent.width / 2 y: parent.height text: "Forces the backend to take
+screenshot of the desktop, instead of trying to get the wallpaper from
+Plasma.\nThis method uses more resources if the time between screenshots is too
+small!" } } } RowLayout { PlasmaComponents3.Label { text: "Single screenshot
+mode" Layout.alignment: Qt.AlignLeft } PlasmaComponents3.CheckBox { checked:
+settings.once_after_change onCheckedChanged: { settings.once_after_change =
+checked } } PlasmaComponents3.ToolButton { icon.name: "help-contents"
+hoverEnabled: true onClicked: pauseScreenshotDelayPopup.open()
+PlasmaComponents3.ToolTip { id: pauseScreenshotDelayPopup x: parent.width / 2
+y: parent.height text: "Only extract colors from screenshot after changing
+wallpaper plugin. This option makes sense for wallpaper plugins that display an
+animated loop that never stops. Makes the color extraction run only a single
+time instead of detecting every change." } } } Rectangle { Layout.topMargin:
+Kirigami.Units.mediumSpacing Layout.preferredWidth: mainLayout.width height: 1
+color: dividerColor opacity: dividerOpacity } ColumnLayout { spacing:
+Kirigami.Units.mediumSpacing opacity: 0.9 PlasmaExtras.Heading { level: 2 text:
+"About " + Plasmoid.metaData.name Layout.alignment: Qt.AlignHCenter wrapMode:
+Text.WordWrap horizontalAlignment: Text.AlignHCenter } PlasmaComponents3.Label
+{ text: "Plasmoid version: " + Plasmoid.metaData.version Layout.alignment:
+Qt.AlignHCenter } PlasmaComponents3.Label { text: "Backend version: " +
+fullRepresentation.backendVersionDisplay Layout.alignment: Qt.AlignHCenter }
+TextEdit { text: "If you like the project you can leave a review in _K_D_E_ _S_t_o_r_e
+or give it a star on _G_i_t_h_u_b. For bugs and feature requests please go to the
+_i_s_s_u_e_s_ _p_a_g_e." wrapMode: Text.WordWrap readOnly: true textFormat:
+TextEdit.RichText Layout.alignment: Qt.AlignHCenter Layout.preferredWidth:
+mainLayout.width horizontalAlignment: Text.AlignHCenter color:
+Kirigami.Theme.textColor selectedTextColor: Kirigami.Theme.highlightedTextColor
+selectionColor: Kirigami.Theme.highlightColor onLinkActivated: (url) =>
+Qt.openUrlExternally(url) HoverHandler { acceptedButtons: Qt.NoButton
+cursorShape: parent.hoveredLink ? Qt.PointingHandCursor : Qt.ArrowCursor } } }
+FileDialog { id: fileDialogHookExec onAccepted:
+{ mainLayout.settings.on_change_hook = fileDialogHookExec.fileUrl.toString
+().substring(7) } } FileDialog { id: fileDialogQdbusExec onAccepted:
+{ mainLayout.settings.qdbus_executable = fileDialogQdbusExec.fileUrl.toString
+().substring(7) } } FileDialog { id: fileDialogBackendExec onAccepted:
 { mainLayout.settings.gui_custom_exec_location =
 fileDialogBackendExec.fileUrl.toString().substring(7) } } } Timer { id:
 scrollTimer interval: 20 repeat: false onTriggered: { scrollView.scrollToTop()
 } } Timer { id: statupTimer interval: 1000 repeat: false onTriggered: { /
 / Default colors // FIXME: for some reason color_last starts with red?? if
 (settings.color_last==="" || settings.color_last ==="red")
 { settings.color_last = "#d0265c" } if (settings.custom_colors_list_last==="")
```

### Comparing `kde-material-you-colors-1.8.0/src/plasmoid/package/contents/ui/components/CustomColorButton.qml` & `kde_material_you_colors-1.9.1/src/plasmoid/package/contents/ui/components/CustomColorButton.qml`

 * *Files identical despite different names*

### Comparing `kde-material-you-colors-1.8.0/src/plasmoid/package/contents/ui/components/FadeBehavior.qml` & `kde_material_you_colors-1.9.1/src/plasmoid/package/contents/ui/components/FadeBehavior.qml`

 * *Files identical despite different names*

### Comparing `kde-material-you-colors-1.8.0/src/plasmoid/package/contents/ui/components/PlasmoidIcon.qml` & `kde_material_you_colors-1.9.1/src/plasmoid/package/contents/ui/components/PlasmoidIcon.qml`

 * *Files identical despite different names*

### Comparing `kde-material-you-colors-1.8.0/src/plasmoid/package/contents/ui/configGeneral.qml` & `kde_material_you_colors-1.9.1/src/plasmoid/package/contents/ui/configGeneral.qml`

 * *Files identical despite different names*

### Comparing `kde-material-you-colors-1.8.0/src/plasmoid/package/contents/ui/main.qml` & `kde_material_you_colors-1.9.1/src/plasmoid/package/contents/ui/main.qml`

 * *Files identical despite different names*

### Comparing `kde-material-you-colors-1.8.0/src/plasmoid/package/metadata.json` & `kde_material_you_colors-1.9.1/src/plasmoid/package/metadata.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9949999999999999%*

 * *Differences: {"'KPlugin'": "{'Version': '0.4.1'}"}*

```diff
@@ -10,14 +10,14 @@
         "BugReportUrl": "https://github.com/luisbocanegra/kde-material-you-colors/issues",
         "Category": "System Information",
         "Description": "Companion widget for KDE Material You Colors",
         "Icon": "preferences-desktop-theme-global",
         "Id": "luisbocanegra.kdematerialyou.colors",
         "License": "GPL-3.0",
         "Name": "KDE Material You Colors",
-        "Version": "0.3.0",
+        "Version": "0.4.1",
         "Website": "https://github.com/luisbocanegra/kde-material-you-colors"
     },
     "X-Plasma-API-Minimum-Version": "6.0",
     "X-Plasma-NotificationArea": true,
     "X-Plasma-NotificationAreaCategory": "ApplicationStatus"
 }
```

### Comparing `kde-material-you-colors-1.8.0/src/screenshot_helper/main.cpp` & `kde_material_you_colors-1.9.1/src/screenshot_helper/main.cpp`

 * *Files identical despite different names*

