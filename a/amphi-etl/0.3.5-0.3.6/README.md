# Comparing `tmp/amphi-etl-0.3.5.tar.gz` & `tmp/amphi-etl-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amphi-etl-0.3.5.tar", last modified: Fri May 17 21:51:16 2024, max compression
+gzip compressed data, was "amphi-etl-0.3.6.tar", last modified: Mon May 20 17:03:09 2024, max compression
```

## Comparing `amphi-etl-0.3.5.tar` & `amphi-etl-0.3.6.tar`

### file list

```diff
@@ -1,98 +1,115 @@
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:51:16.109182 amphi-etl-0.3.5/
--rw-r--r--   0 thibaut    (501) staff       (20)     3795 2024-03-22 17:55:16.000000 amphi-etl-0.3.5/LICENSE
--rw-r--r--   0 thibaut    (501) staff       (20)      646 2024-05-17 20:22:58.000000 amphi-etl-0.3.5/MANIFEST.in
--rw-r--r--   0 thibaut    (501) staff       (20)     6889 2024-05-17 21:51:16.108924 amphi-etl-0.3.5/PKG-INFO
--rw-r--r--   0 thibaut    (501) staff       (20)     1770 2024-03-22 18:05:50.000000 amphi-etl-0.3.5/README.md
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:51:16.090795 amphi-etl-0.3.5/amphi/
--rw-r--r--   0 thibaut    (501) staff       (20)       20 2024-05-15 18:36:08.000000 amphi-etl-0.3.5/amphi/__init__.py
--rw-r--r--   0 thibaut    (501) staff       (20)      171 2024-05-17 21:50:49.000000 amphi-etl-0.3.5/amphi/_version.py
--rw-r--r--   0 thibaut    (501) staff       (20)      890 2024-05-17 21:35:45.000000 amphi-etl-0.3.5/amphi/main.py
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:51:16.091414 amphi-etl-0.3.5/amphi/theme-light/
--rw-r--r--   0 thibaut    (501) staff       (20)    23618 2024-05-17 21:47:42.000000 amphi-etl-0.3.5/amphi/theme-light/build_log.json
--rw-r--r--   0 thibaut    (501) staff       (20)     2699 2024-05-17 21:47:43.000000 amphi-etl-0.3.5/amphi/theme-light/package.json
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:51:16.093155 amphi-etl-0.3.5/amphi/theme-light/static/
--rw-r--r--   0 thibaut    (501) staff       (20)     1584 2024-05-17 21:47:43.000000 amphi-etl-0.3.5/amphi/theme-light/static/lib_index_js.76fd05e25cd1622361b8.js
--rw-r--r--   0 thibaut    (501) staff       (20)      933 2024-05-17 21:47:43.000000 amphi-etl-0.3.5/amphi/theme-light/static/lib_index_js.76fd05e25cd1622361b8.js.map
--rw-r--r--   0 thibaut    (501) staff       (20)    27264 2024-05-17 21:47:43.000000 amphi-etl-0.3.5/amphi/theme-light/static/remoteEntry.020f6c95bb859ea9639f.js
--rw-r--r--   0 thibaut    (501) staff       (20)    25995 2024-05-17 21:47:43.000000 amphi-etl-0.3.5/amphi/theme-light/static/remoteEntry.020f6c95bb859ea9639f.js.map
--rw-r--r--   0 thibaut    (501) staff       (20)      118 2024-05-17 21:47:42.000000 amphi-etl-0.3.5/amphi/theme-light/static/style.js
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:51:16.088143 amphi-etl-0.3.5/amphi/theme-light/themes/
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:51:16.088196 amphi-etl-0.3.5/amphi/theme-light/themes/@amphi/
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:51:16.094031 amphi-etl-0.3.5/amphi/theme-light/themes/@amphi/theme-light/
--rw-r--r--   0 thibaut    (501) staff       (20)    37754 2024-05-17 21:47:43.000000 amphi-etl-0.3.5/amphi/theme-light/themes/@amphi/theme-light/index.css
--rw-r--r--   0 thibaut    (501) staff       (20)        0 2024-05-17 21:47:43.000000 amphi-etl-0.3.5/amphi/theme-light/themes/@amphi/theme-light/index.js
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:51:16.094513 amphi-etl-0.3.5/amphi/ui-component/
--rw-r--r--   0 thibaut    (501) staff       (20)    22518 2024-05-17 21:47:47.000000 amphi-etl-0.3.5/amphi/ui-component/build_log.json
--rw-r--r--   0 thibaut    (501) staff       (20)     2764 2024-05-17 21:47:47.000000 amphi-etl-0.3.5/amphi/ui-component/package.json
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:51:16.098912 amphi-etl-0.3.5/amphi/ui-component/static/
--rw-r--r--   0 thibaut    (501) staff       (20)    64203 2024-05-17 21:47:47.000000 amphi-etl-0.3.5/amphi/ui-component/static/lib_index_js.3a5d11eaa6df06cb0ee7.js
--rw-r--r--   0 thibaut    (501) staff       (20)    37982 2024-05-17 21:47:47.000000 amphi-etl-0.3.5/amphi/ui-component/static/lib_index_js.3a5d11eaa6df06cb0ee7.js.map
--rw-r--r--   0 thibaut    (501) staff       (20)    58944 2024-05-17 21:47:47.000000 amphi-etl-0.3.5/amphi/ui-component/static/node_modules_css-loader_dist_cjs_js_style_output_css-node_modules_style-loader_dist_runtime_i-dc6767.e55ff0d3e2b5f4c1df14.js
--rw-r--r--   0 thibaut    (501) staff       (20)    73309 2024-05-17 21:47:47.000000 amphi-etl-0.3.5/amphi/ui-component/static/node_modules_css-loader_dist_cjs_js_style_output_css-node_modules_style-loader_dist_runtime_i-dc6767.e55ff0d3e2b5f4c1df14.js.map
--rw-r--r--   0 thibaut    (501) staff       (20)    30264 2024-05-17 21:47:47.000000 amphi-etl-0.3.5/amphi/ui-component/static/remoteEntry.15dfea293b8af56eb37f.js
--rw-r--r--   0 thibaut    (501) staff       (20)    29057 2024-05-17 21:47:47.000000 amphi-etl-0.3.5/amphi/ui-component/static/remoteEntry.15dfea293b8af56eb37f.js.map
--rw-r--r--   0 thibaut    (501) staff       (20)      162 2024-05-17 21:47:47.000000 amphi-etl-0.3.5/amphi/ui-component/static/style.js
--rw-r--r--   0 thibaut    (501) staff       (20)    14477 2024-05-17 21:47:47.000000 amphi-etl-0.3.5/amphi/ui-component/static/style_index_js.7002c9447c653e7de570.js
--rw-r--r--   0 thibaut    (501) staff       (20)     5614 2024-05-17 21:47:47.000000 amphi-etl-0.3.5/amphi/ui-component/static/style_index_js.7002c9447c653e7de570.js.map
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:51:16.099814 amphi-etl-0.3.5/amphi_etl.egg-info/
--rw-r--r--   0 thibaut    (501) staff       (20)     6889 2024-05-17 21:51:16.000000 amphi-etl-0.3.5/amphi_etl.egg-info/PKG-INFO
--rw-r--r--   0 thibaut    (501) staff       (20)     3257 2024-05-17 21:51:16.000000 amphi-etl-0.3.5/amphi_etl.egg-info/SOURCES.txt
--rw-r--r--   0 thibaut    (501) staff       (20)        1 2024-05-17 21:51:16.000000 amphi-etl-0.3.5/amphi_etl.egg-info/dependency_links.txt
--rw-r--r--   0 thibaut    (501) staff       (20)       42 2024-05-17 21:51:16.000000 amphi-etl-0.3.5/amphi_etl.egg-info/entry_points.txt
--rw-r--r--   0 thibaut    (501) staff       (20)       57 2024-05-17 21:51:16.000000 amphi-etl-0.3.5/amphi_etl.egg-info/requires.txt
--rw-r--r--   0 thibaut    (501) staff       (20)        6 2024-05-17 21:51:16.000000 amphi-etl-0.3.5/amphi_etl.egg-info/top_level.txt
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:51:16.088579 amphi-etl-0.3.5/config/
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:51:16.099936 amphi-etl-0.3.5/config/labconfig/
--rw-r--r--   0 thibaut    (501) staff       (20)      680 2024-05-15 22:02:31.000000 amphi-etl-0.3.5/config/labconfig/page_config.json
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:51:16.100188 amphi-etl-0.3.5/config/settings/
--rw-r--r--   0 thibaut    (501) staff       (20)     2679 2024-05-15 22:26:33.000000 amphi-etl-0.3.5/config/settings/overrides.json
--rw-r--r--   0 thibaut    (501) staff       (20)     3187 2024-05-17 21:36:13.000000 amphi-etl-0.3.5/package.json
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:51:16.088883 amphi-etl-0.3.5/packages/
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:51:16.100786 amphi-etl-0.3.5/packages/theme-light/
--rw-r--r--   0 thibaut    (501) staff       (20)     2583 2024-05-17 20:42:53.000000 amphi-etl-0.3.5/packages/theme-light/package.json
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:51:16.101010 amphi-etl-0.3.5/packages/theme-light/src/
--rw-r--r--   0 thibaut    (501) staff       (20)      683 2024-03-22 18:05:01.000000 amphi-etl-0.3.5/packages/theme-light/src/index.ts
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:51:16.101616 amphi-etl-0.3.5/packages/theme-light/style/
--rw-r--r--   0 thibaut    (501) staff       (20)    23116 2024-05-16 05:20:56.000000 amphi-etl-0.3.5/packages/theme-light/style/index.css
--rw-r--r--   0 thibaut    (501) staff       (20)    14663 2024-05-15 22:00:45.000000 amphi-etl-0.3.5/packages/theme-light/style/variables.css
--rw-r--r--   0 thibaut    (501) staff       (20)      135 2024-03-22 18:05:01.000000 amphi-etl-0.3.5/packages/theme-light/tsconfig.json
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:51:16.102377 amphi-etl-0.3.5/packages/ui-component/
--rw-r--r--   0 thibaut    (501) staff       (20)     2622 2024-05-17 20:42:59.000000 amphi-etl-0.3.5/packages/ui-component/package.json
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:51:16.103338 amphi-etl-0.3.5/packages/ui-component/src/
--rw-r--r--   0 thibaut    (501) staff       (20)     7188 2024-03-22 18:05:02.000000 amphi-etl-0.3.5/packages/ui-component/src/BrowseFileDialog.tsx
--rw-r--r--   0 thibaut    (501) staff       (20)     2814 2024-03-22 18:05:02.000000 amphi-etl-0.3.5/packages/ui-component/src/Dropzone.tsx
--rw-r--r--   0 thibaut    (501) staff       (20)       74 2024-03-22 18:05:02.000000 amphi-etl-0.3.5/packages/ui-component/src/declarations.d.ts
--rw-r--r--   0 thibaut    (501) staff       (20)     1831 2024-03-22 18:05:02.000000 amphi-etl-0.3.5/packages/ui-component/src/icons.ts
--rw-r--r--   0 thibaut    (501) staff       (20)     5084 2024-05-15 17:04:08.000000 amphi-etl-0.3.5/packages/ui-component/src/index.ts
--rw-r--r--   0 thibaut    (501) staff       (20)    12567 2024-05-15 16:58:31.000000 amphi-etl-0.3.5/packages/ui-component/src/launcher.tsx
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:51:16.104405 amphi-etl-0.3.5/packages/ui-component/style/
--rw-r--r--   0 thibaut    (501) staff       (20)      403 2024-03-22 18:05:02.000000 amphi-etl-0.3.5/packages/ui-component/style/base.css
-drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-17 21:51:16.108525 amphi-etl-0.3.5/packages/ui-component/style/icons/
--rw-r--r--   0 thibaut    (501) staff       (20)     2857 2024-03-22 20:46:02.000000 amphi-etl-0.3.5/packages/ui-component/style/icons/amphi-square-logo.svg
--rw-r--r--   0 thibaut    (501) staff       (20)     3001 2024-03-22 20:45:41.000000 amphi-etl-0.3.5/packages/ui-component/style/icons/amphi-square-logo_nonpaths.svg
--rw-r--r--   0 thibaut    (501) staff       (20)     2838 2024-03-22 20:46:22.000000 amphi-etl-0.3.5/packages/ui-component/style/icons/amphi.svg
--rw-r--r--   0 thibaut    (501) staff       (20)     1227 2024-03-22 18:05:02.000000 amphi-etl-0.3.5/packages/ui-component/style/icons/bug-16.svg
--rw-r--r--   0 thibaut    (501) staff       (20)     1204 2024-03-22 18:05:02.000000 amphi-etl-0.3.5/packages/ui-component/style/icons/bug-24.svg
--rw-r--r--   0 thibaut    (501) staff       (20)      465 2024-03-22 18:05:02.000000 amphi-etl-0.3.5/packages/ui-component/style/icons/code-16.svg
--rw-r--r--   0 thibaut    (501) staff       (20)      496 2024-03-22 18:05:02.000000 amphi-etl-0.3.5/packages/ui-component/style/icons/code-24.svg
--rw-r--r--   0 thibaut    (501) staff       (20)      432 2024-03-22 18:05:02.000000 amphi-etl-0.3.5/packages/ui-component/style/icons/docs-16.svg
--rw-r--r--   0 thibaut    (501) staff       (20)      479 2024-03-22 18:05:02.000000 amphi-etl-0.3.5/packages/ui-component/style/icons/docs-24.svg
--rw-r--r--   0 thibaut    (501) staff       (20)      924 2024-03-22 18:05:02.000000 amphi-etl-0.3.5/packages/ui-component/style/icons/network-24.svg
--rw-r--r--   0 thibaut    (501) staff       (20)      330 2024-03-22 18:05:02.000000 amphi-etl-0.3.5/packages/ui-component/style/icons/p5-asterisk.svg
--rw-r--r--   0 thibaut    (501) staff       (20)     2895 2024-03-22 18:05:02.000000 amphi-etl-0.3.5/packages/ui-component/style/icons/p5-square-logo.svg
--rw-r--r--   0 thibaut    (501) staff       (20)      687 2024-03-22 18:05:02.000000 amphi-etl-0.3.5/packages/ui-component/style/icons/pipeline-16.svg
--rw-r--r--   0 thibaut    (501) staff       (20)      702 2024-03-22 18:05:02.000000 amphi-etl-0.3.5/packages/ui-component/style/icons/pipeline-24.svg
--rw-r--r--   0 thibaut    (501) staff       (20)     2703 2024-03-22 18:05:02.000000 amphi-etl-0.3.5/packages/ui-component/style/icons/pipeline.svg
--rw-r--r--   0 thibaut    (501) staff       (20)     2717 2024-03-22 18:05:02.000000 amphi-etl-0.3.5/packages/ui-component/style/icons/pipeline_negative.svg
--rw-r--r--   0 thibaut    (501) staff       (20)      845 2024-03-22 18:05:02.000000 amphi-etl-0.3.5/packages/ui-component/style/icons/shield-check-24.svg
--rw-r--r--   0 thibaut    (501) staff       (20)      472 2024-03-22 18:05:02.000000 amphi-etl-0.3.5/packages/ui-component/style/icons/upload-16.svg
--rw-r--r--   0 thibaut    (501) staff       (20)      289 2024-03-22 18:05:02.000000 amphi-etl-0.3.5/packages/ui-component/style/index.css
--rw-r--r--   0 thibaut    (501) staff       (20)      307 2024-03-22 18:05:02.000000 amphi-etl-0.3.5/packages/ui-component/style/index.js
--rw-r--r--   0 thibaut    (501) staff       (20)    18439 2024-05-15 17:05:28.000000 amphi-etl-0.3.5/packages/ui-component/style/output.css
--rw-r--r--   0 thibaut    (501) staff       (20)      277 2024-05-15 16:52:04.000000 amphi-etl-0.3.5/packages/ui-component/tailwind.config.js
--rw-r--r--   0 thibaut    (501) staff       (20)      620 2024-03-22 18:05:02.000000 amphi-etl-0.3.5/packages/ui-component/tsconfig.json
--rw-r--r--   0 thibaut    (501) staff       (20)     2603 2024-05-17 20:43:36.000000 amphi-etl-0.3.5/pyproject.toml
--rw-r--r--   0 thibaut    (501) staff       (20)       38 2024-05-17 21:51:16.109241 amphi-etl-0.3.5/setup.cfg
--rw-r--r--   0 thibaut    (501) staff       (20)     1745 2024-05-17 21:51:05.000000 amphi-etl-0.3.5/setup.py
--rw-r--r--   0 thibaut    (501) staff       (20)       66 2024-03-22 17:55:16.000000 amphi-etl-0.3.5/tsconfig.eslint.json
--rw-r--r--   0 thibaut    (501) staff       (20)      513 2024-03-22 17:55:16.000000 amphi-etl-0.3.5/tsconfigbase.json
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-20 17:03:09.615304 amphi-etl-0.3.6/
+-rw-r--r--   0 thibaut    (501) staff       (20)     3795 2024-03-22 17:55:16.000000 amphi-etl-0.3.6/LICENSE
+-rw-r--r--   0 thibaut    (501) staff       (20)      646 2024-05-17 20:22:58.000000 amphi-etl-0.3.6/MANIFEST.in
+-rw-r--r--   0 thibaut    (501) staff       (20)     6889 2024-05-20 17:03:09.615044 amphi-etl-0.3.6/PKG-INFO
+-rw-r--r--   0 thibaut    (501) staff       (20)     1770 2024-03-22 18:05:50.000000 amphi-etl-0.3.6/README.md
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-20 17:03:09.588052 amphi-etl-0.3.6/amphi/
+-rw-r--r--   0 thibaut    (501) staff       (20)       20 2024-05-15 18:36:08.000000 amphi-etl-0.3.6/amphi/__init__.py
+-rw-r--r--   0 thibaut    (501) staff       (20)      171 2024-05-20 17:02:44.000000 amphi-etl-0.3.6/amphi/_version.py
+-rw-r--r--   0 thibaut    (501) staff       (20)     1104 2024-05-20 16:45:52.000000 amphi-etl-0.3.6/amphi/main.py
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-20 17:03:09.589115 amphi-etl-0.3.6/amphi/theme-light/
+-rw-r--r--   0 thibaut    (501) staff       (20)    23166 2024-05-20 16:53:22.000000 amphi-etl-0.3.6/amphi/theme-light/build_log.json
+-rw-r--r--   0 thibaut    (501) staff       (20)     2699 2024-05-20 16:53:22.000000 amphi-etl-0.3.6/amphi/theme-light/package.json
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-20 17:03:09.591202 amphi-etl-0.3.6/amphi/theme-light/static/
+-rw-r--r--   0 thibaut    (501) staff       (20)     1584 2024-05-20 16:53:22.000000 amphi-etl-0.3.6/amphi/theme-light/static/lib_index_js.76fd05e25cd1622361b8.js
+-rw-r--r--   0 thibaut    (501) staff       (20)      933 2024-05-20 16:53:22.000000 amphi-etl-0.3.6/amphi/theme-light/static/lib_index_js.76fd05e25cd1622361b8.js.map
+-rw-r--r--   0 thibaut    (501) staff       (20)    27264 2024-05-20 16:53:22.000000 amphi-etl-0.3.6/amphi/theme-light/static/remoteEntry.bf309478c3347f5f051d.js
+-rw-r--r--   0 thibaut    (501) staff       (20)    25995 2024-05-20 16:53:22.000000 amphi-etl-0.3.6/amphi/theme-light/static/remoteEntry.bf309478c3347f5f051d.js.map
+-rw-r--r--   0 thibaut    (501) staff       (20)      118 2024-05-20 16:53:22.000000 amphi-etl-0.3.6/amphi/theme-light/static/style.js
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-20 17:03:09.582836 amphi-etl-0.3.6/amphi/theme-light/themes/
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-20 17:03:09.582888 amphi-etl-0.3.6/amphi/theme-light/themes/@amphi/
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-20 17:03:09.592331 amphi-etl-0.3.6/amphi/theme-light/themes/@amphi/theme-light/
+-rw-r--r--   0 thibaut    (501) staff       (20)    37896 2024-05-20 16:53:23.000000 amphi-etl-0.3.6/amphi/theme-light/themes/@amphi/theme-light/index.css
+-rw-r--r--   0 thibaut    (501) staff       (20)        0 2024-05-20 16:53:23.000000 amphi-etl-0.3.6/amphi/theme-light/themes/@amphi/theme-light/index.js
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-20 17:03:09.593364 amphi-etl-0.3.6/amphi/ui-component/
+-rw-r--r--   0 thibaut    (501) staff       (20)    22066 2024-05-20 16:53:25.000000 amphi-etl-0.3.6/amphi/ui-component/build_log.json
+-rw-r--r--   0 thibaut    (501) staff       (20)     2764 2024-05-20 16:53:26.000000 amphi-etl-0.3.6/amphi/ui-component/package.json
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-20 17:03:09.598412 amphi-etl-0.3.6/amphi/ui-component/static/
+-rw-r--r--   0 thibaut    (501) staff       (20)    64203 2024-05-20 16:53:26.000000 amphi-etl-0.3.6/amphi/ui-component/static/lib_index_js.3a5d11eaa6df06cb0ee7.js
+-rw-r--r--   0 thibaut    (501) staff       (20)    37982 2024-05-20 16:53:26.000000 amphi-etl-0.3.6/amphi/ui-component/static/lib_index_js.3a5d11eaa6df06cb0ee7.js.map
+-rw-r--r--   0 thibaut    (501) staff       (20)    58944 2024-05-20 16:53:26.000000 amphi-etl-0.3.6/amphi/ui-component/static/node_modules_css-loader_dist_cjs_js_style_output_css-node_modules_style-loader_dist_runtime_i-dc6767.e55ff0d3e2b5f4c1df14.js
+-rw-r--r--   0 thibaut    (501) staff       (20)    73309 2024-05-20 16:53:26.000000 amphi-etl-0.3.6/amphi/ui-component/static/node_modules_css-loader_dist_cjs_js_style_output_css-node_modules_style-loader_dist_runtime_i-dc6767.e55ff0d3e2b5f4c1df14.js.map
+-rw-r--r--   0 thibaut    (501) staff       (20)    30264 2024-05-20 16:53:26.000000 amphi-etl-0.3.6/amphi/ui-component/static/remoteEntry.d516e88595b29cbc0207.js
+-rw-r--r--   0 thibaut    (501) staff       (20)    29057 2024-05-20 16:53:26.000000 amphi-etl-0.3.6/amphi/ui-component/static/remoteEntry.d516e88595b29cbc0207.js.map
+-rw-r--r--   0 thibaut    (501) staff       (20)      162 2024-05-20 16:53:25.000000 amphi-etl-0.3.6/amphi/ui-component/static/style.js
+-rw-r--r--   0 thibaut    (501) staff       (20)    14477 2024-05-20 16:53:26.000000 amphi-etl-0.3.6/amphi/ui-component/static/style_index_js.7002c9447c653e7de570.js
+-rw-r--r--   0 thibaut    (501) staff       (20)     5614 2024-05-20 16:53:26.000000 amphi-etl-0.3.6/amphi/ui-component/static/style_index_js.7002c9447c653e7de570.js.map
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-20 17:03:09.599452 amphi-etl-0.3.6/amphi_etl.egg-info/
+-rw-r--r--   0 thibaut    (501) staff       (20)     6889 2024-05-20 17:03:09.000000 amphi-etl-0.3.6/amphi_etl.egg-info/PKG-INFO
+-rw-r--r--   0 thibaut    (501) staff       (20)     3816 2024-05-20 17:03:09.000000 amphi-etl-0.3.6/amphi_etl.egg-info/SOURCES.txt
+-rw-r--r--   0 thibaut    (501) staff       (20)        1 2024-05-20 17:03:09.000000 amphi-etl-0.3.6/amphi_etl.egg-info/dependency_links.txt
+-rw-r--r--   0 thibaut    (501) staff       (20)       42 2024-05-20 17:03:09.000000 amphi-etl-0.3.6/amphi_etl.egg-info/entry_points.txt
+-rw-r--r--   0 thibaut    (501) staff       (20)       57 2024-05-20 17:03:09.000000 amphi-etl-0.3.6/amphi_etl.egg-info/requires.txt
+-rw-r--r--   0 thibaut    (501) staff       (20)        6 2024-05-20 17:03:09.000000 amphi-etl-0.3.6/amphi_etl.egg-info/top_level.txt
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-20 17:03:09.583279 amphi-etl-0.3.6/config/
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-20 17:03:09.599586 amphi-etl-0.3.6/config/labconfig/
+-rw-r--r--   0 thibaut    (501) staff       (20)      680 2024-05-15 22:02:31.000000 amphi-etl-0.3.6/config/labconfig/page_config.json
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-20 17:03:09.599862 amphi-etl-0.3.6/config/settings/
+-rw-r--r--   0 thibaut    (501) staff       (20)     2679 2024-05-15 22:26:33.000000 amphi-etl-0.3.6/config/settings/overrides.json
+-rw-r--r--   0 thibaut    (501) staff       (20)     3187 2024-05-20 17:02:44.000000 amphi-etl-0.3.6/package.json
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-20 17:03:09.583688 amphi-etl-0.3.6/packages/
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-20 17:03:09.600535 amphi-etl-0.3.6/packages/theme-light/
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-20 17:03:09.601648 amphi-etl-0.3.6/packages/theme-light/lib/
+-rw-r--r--   0 thibaut    (501) staff       (20)      214 2024-05-20 16:47:00.000000 amphi-etl-0.3.6/packages/theme-light/lib/index.d.ts
+-rw-r--r--   0 thibaut    (501) staff       (20)      584 2024-05-20 16:47:00.000000 amphi-etl-0.3.6/packages/theme-light/lib/index.js
+-rw-r--r--   0 thibaut    (501) staff       (20)     2583 2024-05-17 20:42:53.000000 amphi-etl-0.3.6/packages/theme-light/package.json
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-20 17:03:09.601908 amphi-etl-0.3.6/packages/theme-light/src/
+-rw-r--r--   0 thibaut    (501) staff       (20)      683 2024-03-22 18:05:01.000000 amphi-etl-0.3.6/packages/theme-light/src/index.ts
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-20 17:03:09.602911 amphi-etl-0.3.6/packages/theme-light/style/
+-rw-r--r--   0 thibaut    (501) staff       (20)    23258 2024-05-20 00:42:39.000000 amphi-etl-0.3.6/packages/theme-light/style/index.css
+-rw-r--r--   0 thibaut    (501) staff       (20)    14663 2024-05-20 00:30:35.000000 amphi-etl-0.3.6/packages/theme-light/style/variables.css
+-rw-r--r--   0 thibaut    (501) staff       (20)      135 2024-03-22 18:05:01.000000 amphi-etl-0.3.6/packages/theme-light/tsconfig.json
+-rw-r--r--   0 thibaut    (501) staff       (20)    62340 2024-05-20 16:47:00.000000 amphi-etl-0.3.6/packages/theme-light/tsconfig.tsbuildinfo
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-20 17:03:09.603942 amphi-etl-0.3.6/packages/ui-component/
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-20 17:03:09.606925 amphi-etl-0.3.6/packages/ui-component/lib/
+-rw-r--r--   0 thibaut    (501) staff       (20)      465 2024-05-20 16:47:05.000000 amphi-etl-0.3.6/packages/ui-component/lib/BrowseFileDialog.d.ts
+-rw-r--r--   0 thibaut    (501) staff       (20)     6922 2024-05-20 16:47:05.000000 amphi-etl-0.3.6/packages/ui-component/lib/BrowseFileDialog.js
+-rw-r--r--   0 thibaut    (501) staff       (20)      729 2024-05-20 16:47:05.000000 amphi-etl-0.3.6/packages/ui-component/lib/Dropzone.d.ts
+-rw-r--r--   0 thibaut    (501) staff       (20)     2229 2024-05-20 16:47:05.000000 amphi-etl-0.3.6/packages/ui-component/lib/Dropzone.js
+-rw-r--r--   0 thibaut    (501) staff       (20)      529 2024-05-20 16:47:05.000000 amphi-etl-0.3.6/packages/ui-component/lib/icons.d.ts
+-rw-r--r--   0 thibaut    (501) staff       (20)     1861 2024-05-20 16:47:05.000000 amphi-etl-0.3.6/packages/ui-component/lib/icons.js
+-rw-r--r--   0 thibaut    (501) staff       (20)      255 2024-05-20 16:47:05.000000 amphi-etl-0.3.6/packages/ui-component/lib/index.d.ts
+-rw-r--r--   0 thibaut    (501) staff       (20)     5217 2024-05-20 16:47:05.000000 amphi-etl-0.3.6/packages/ui-component/lib/index.js
+-rw-r--r--   0 thibaut    (501) staff       (20)     1127 2024-05-20 16:47:05.000000 amphi-etl-0.3.6/packages/ui-component/lib/launcher.d.ts
+-rw-r--r--   0 thibaut    (501) staff       (20)    13920 2024-05-20 16:47:05.000000 amphi-etl-0.3.6/packages/ui-component/lib/launcher.js
+-rw-r--r--   0 thibaut    (501) staff       (20)     2622 2024-05-17 20:42:59.000000 amphi-etl-0.3.6/packages/ui-component/package.json
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-20 17:03:09.608313 amphi-etl-0.3.6/packages/ui-component/src/
+-rw-r--r--   0 thibaut    (501) staff       (20)     7188 2024-03-22 18:05:02.000000 amphi-etl-0.3.6/packages/ui-component/src/BrowseFileDialog.tsx
+-rw-r--r--   0 thibaut    (501) staff       (20)     2814 2024-03-22 18:05:02.000000 amphi-etl-0.3.6/packages/ui-component/src/Dropzone.tsx
+-rw-r--r--   0 thibaut    (501) staff       (20)       74 2024-03-22 18:05:02.000000 amphi-etl-0.3.6/packages/ui-component/src/declarations.d.ts
+-rw-r--r--   0 thibaut    (501) staff       (20)     1831 2024-03-22 18:05:02.000000 amphi-etl-0.3.6/packages/ui-component/src/icons.ts
+-rw-r--r--   0 thibaut    (501) staff       (20)     5084 2024-05-15 17:04:08.000000 amphi-etl-0.3.6/packages/ui-component/src/index.ts
+-rw-r--r--   0 thibaut    (501) staff       (20)    12567 2024-05-15 16:58:31.000000 amphi-etl-0.3.6/packages/ui-component/src/launcher.tsx
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-20 17:03:09.609478 amphi-etl-0.3.6/packages/ui-component/style/
+-rw-r--r--   0 thibaut    (501) staff       (20)      403 2024-03-22 18:05:02.000000 amphi-etl-0.3.6/packages/ui-component/style/base.css
+drwxr-xr-x   0 thibaut    (501) staff       (20)        0 2024-05-20 17:03:09.614613 amphi-etl-0.3.6/packages/ui-component/style/icons/
+-rw-r--r--   0 thibaut    (501) staff       (20)     2857 2024-03-22 20:46:02.000000 amphi-etl-0.3.6/packages/ui-component/style/icons/amphi-square-logo.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)     3001 2024-03-22 20:45:41.000000 amphi-etl-0.3.6/packages/ui-component/style/icons/amphi-square-logo_nonpaths.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)     2838 2024-03-22 20:46:22.000000 amphi-etl-0.3.6/packages/ui-component/style/icons/amphi.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)     1227 2024-03-22 18:05:02.000000 amphi-etl-0.3.6/packages/ui-component/style/icons/bug-16.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)     1204 2024-03-22 18:05:02.000000 amphi-etl-0.3.6/packages/ui-component/style/icons/bug-24.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)      465 2024-03-22 18:05:02.000000 amphi-etl-0.3.6/packages/ui-component/style/icons/code-16.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)      496 2024-03-22 18:05:02.000000 amphi-etl-0.3.6/packages/ui-component/style/icons/code-24.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)      432 2024-03-22 18:05:02.000000 amphi-etl-0.3.6/packages/ui-component/style/icons/docs-16.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)      479 2024-03-22 18:05:02.000000 amphi-etl-0.3.6/packages/ui-component/style/icons/docs-24.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)      924 2024-03-22 18:05:02.000000 amphi-etl-0.3.6/packages/ui-component/style/icons/network-24.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)      330 2024-03-22 18:05:02.000000 amphi-etl-0.3.6/packages/ui-component/style/icons/p5-asterisk.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)     2895 2024-03-22 18:05:02.000000 amphi-etl-0.3.6/packages/ui-component/style/icons/p5-square-logo.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)      687 2024-03-22 18:05:02.000000 amphi-etl-0.3.6/packages/ui-component/style/icons/pipeline-16.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)      702 2024-03-22 18:05:02.000000 amphi-etl-0.3.6/packages/ui-component/style/icons/pipeline-24.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)     2703 2024-03-22 18:05:02.000000 amphi-etl-0.3.6/packages/ui-component/style/icons/pipeline.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)     2717 2024-03-22 18:05:02.000000 amphi-etl-0.3.6/packages/ui-component/style/icons/pipeline_negative.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)      845 2024-03-22 18:05:02.000000 amphi-etl-0.3.6/packages/ui-component/style/icons/shield-check-24.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)      472 2024-03-22 18:05:02.000000 amphi-etl-0.3.6/packages/ui-component/style/icons/upload-16.svg
+-rw-r--r--   0 thibaut    (501) staff       (20)      289 2024-03-22 18:05:02.000000 amphi-etl-0.3.6/packages/ui-component/style/index.css
+-rw-r--r--   0 thibaut    (501) staff       (20)      307 2024-03-22 18:05:02.000000 amphi-etl-0.3.6/packages/ui-component/style/index.js
+-rw-r--r--   0 thibaut    (501) staff       (20)    18439 2024-05-15 17:05:28.000000 amphi-etl-0.3.6/packages/ui-component/style/output.css
+-rw-r--r--   0 thibaut    (501) staff       (20)      277 2024-05-15 16:52:04.000000 amphi-etl-0.3.6/packages/ui-component/tailwind.config.js
+-rw-r--r--   0 thibaut    (501) staff       (20)      620 2024-03-22 18:05:02.000000 amphi-etl-0.3.6/packages/ui-component/tsconfig.json
+-rw-r--r--   0 thibaut    (501) staff       (20)    70461 2024-05-20 16:47:05.000000 amphi-etl-0.3.6/packages/ui-component/tsconfig.tsbuildinfo
+-rw-r--r--   0 thibaut    (501) staff       (20)     2603 2024-05-17 20:43:36.000000 amphi-etl-0.3.6/pyproject.toml
+-rw-r--r--   0 thibaut    (501) staff       (20)       38 2024-05-20 17:03:09.615351 amphi-etl-0.3.6/setup.cfg
+-rw-r--r--   0 thibaut    (501) staff       (20)     1745 2024-05-20 17:02:44.000000 amphi-etl-0.3.6/setup.py
+-rw-r--r--   0 thibaut    (501) staff       (20)       66 2024-03-22 17:55:16.000000 amphi-etl-0.3.6/tsconfig.eslint.json
+-rw-r--r--   0 thibaut    (501) staff       (20)      513 2024-03-22 17:55:16.000000 amphi-etl-0.3.6/tsconfigbase.json
+-rw-r--r--   0 thibaut    (501) staff       (20)   363863 2024-05-20 16:46:47.000000 amphi-etl-0.3.6/yarn.lock
```

### Comparing `amphi-etl-0.3.5/LICENSE` & `amphi-etl-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/MANIFEST.in` & `amphi-etl-0.3.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/PKG-INFO` & `amphi-etl-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amphi-etl
-Version: 0.3.5
+Version: 0.3.6
 Summary: Amphi is a python-based ETL
 Author: Thibaut Gourdel
 Author-email: tgourdel@amphi.ai
 License: Elastic License 2.0 \(ELv2\)
         
         **Acceptance** By using the software, you agree to all of the terms and conditions below.
```

### Comparing `amphi-etl-0.3.5/README.md` & `amphi-etl-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/amphi/main.py` & `amphi-etl-0.3.6/amphi/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import subprocess
 import sys
 import argparse
+import os
 
 def main():
     parser = argparse.ArgumentParser(description='Amphi ETL Command Line Interface')
     parser.add_argument('command', choices=['start'], help='Command to execute')
     parser.add_argument('-w', '--workspace', default='.', help='Workspace directory for JupyterLab')
 
     args = parser.parse_args()
 
     # Debugging logs
     print(f"Received command: {args.command}")
     print(f"Workspace directory: {args.workspace}")
+    print(f"Python executable: {sys.executable}")
+    print(f"Environment PATH: {os.environ.get('PATH')}")
+    print(f"Node.js version: {subprocess.check_output(['node', '--version']).decode().strip()}")
 
     if args.command == 'start':
         jupyter_command = [sys.executable, '-m', 'jupyter', 'lab', f'--notebook-dir={args.workspace}']
         print(f"Running JupyterLab command: {' '.join(jupyter_command)}")
         try:
             subprocess.check_call(jupyter_command)
         except subprocess.CalledProcessError as e:
```

### Comparing `amphi-etl-0.3.5/amphi/theme-light/build_log.json` & `amphi-etl-0.3.6/amphi/ui-component/build_log.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.49562279972029327%*

 * *Differences: {'0': "{'output': {'path': '/Users/thibaut/Documents/amphi-etl/amphi/ui-component/static'}, "*

 * *      "'plugins': {1: {'_options': {'name': '@amphi/ui-component', 'library': {'name': {insert: "*

 * *      "[(1, '@amphi/ui-component')], delete: [1]}}, 'exposes': {'./index': "*

 * *      "'/Users/thibaut/Documents/amphi-etl/packages/ui-component/lib/index.js', './extension': "*

 * *      "'/Users/thibaut/Documents/amphi-etl/packages/ui-component/lib/index.js', './style': "*

 * *      "'/Users/thibaut/Documents/amphi-etl/packages/u […]*

```diff
@@ -88,41 +88,42 @@
                     ]
                 }
             ]
         },
         "output": {
             "filename": "[name].[contenthash].js",
             "hashFunction": "sha256",
-            "path": "/Users/thibaut/Documents/amphi-etl/amphi/theme-light/static",
+            "path": "/Users/thibaut/Documents/amphi-etl/amphi/ui-component/static",
             "publicPath": "auto"
         },
         "plugins": [
             {
                 "definitions": {
                     "process": "process/browser"
                 }
             },
             {
                 "_options": {
                     "exposes": {
-                        "./extension": "/Users/thibaut/Documents/amphi-etl/packages/theme-light/lib/index.js",
-                        "./index": "/Users/thibaut/Documents/amphi-etl/packages/theme-light/lib/index.js"
+                        "./extension": "/Users/thibaut/Documents/amphi-etl/packages/ui-component/lib/index.js",
+                        "./index": "/Users/thibaut/Documents/amphi-etl/packages/ui-component/lib/index.js",
+                        "./style": "/Users/thibaut/Documents/amphi-etl/packages/ui-component/style/index.js"
                     },
                     "filename": "remoteEntry.[contenthash].js",
                     "library": {
                         "name": [
                             "_JUPYTERLAB",
-                            "@amphi/theme-light"
+                            "@amphi/ui-component"
                         ],
                         "type": "var"
                     },
-                    "name": "@amphi/theme-light",
+                    "name": "@amphi/ui-component",
                     "shared": {
-                        "@amphi/theme-light": {
-                            "import": "/Users/thibaut/Documents/amphi-etl/packages/theme-light/lib/index.js",
+                        "@amphi/ui-component": {
+                            "import": "/Users/thibaut/Documents/amphi-etl/packages/ui-component/lib/index.js",
                             "singleton": true,
                             "version": "0.1.0"
                         },
                         "@codemirror/language": {
                             "import": false,
                             "requiredVersion": "^6.0.0",
                             "singleton": true
@@ -135,457 +136,444 @@
                         "@codemirror/view": {
                             "import": false,
                             "requiredVersion": "^6.9.6",
                             "singleton": true
                         },
                         "@jupyter/react-components": {
                             "import": false,
-                            "requiredVersion": "^0.15.3",
+                            "requiredVersion": "^0.13.3",
                             "singleton": true
                         },
                         "@jupyter/web-components": {
                             "import": false,
-                            "requiredVersion": "^0.15.3",
+                            "requiredVersion": "^0.13.3",
                             "singleton": true
                         },
                         "@jupyter/ydoc": {
                             "import": false,
-                            "requiredVersion": "^2.0.1",
+                            "requiredVersion": "^1.1.1",
                             "singleton": true
                         },
                         "@jupyterlab/application": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/application-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/apputils": {
                             "import": false,
-                            "requiredVersion": "^4.3.0",
+                            "requiredVersion": "^4.2.5",
                             "singleton": true
                         },
                         "@jupyterlab/apputils-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/attachments": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/cell-toolbar": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/cell-toolbar-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/cells": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/celltags-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/codeeditor": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/completer": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/completer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/console": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/console-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/coreutils": {
                             "import": false,
-                            "requiredVersion": "^6.2.0",
+                            "requiredVersion": "^6.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/csvviewer": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/csvviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/debugger": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/debugger-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/docmanager": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/docmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/docregistry": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/documentsearch": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/documentsearch-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/extensionmanager": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/extensionmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/filebrowser": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/filebrowser-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/fileeditor": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/fileeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/help-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/htmlviewer": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/htmlviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/hub-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/imageviewer": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/imageviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/inspector": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/inspector-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/javascript-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/json-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/launcher": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/launcher-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/logconsole": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/logconsole-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/lsp": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/lsp-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/mainmenu": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/mainmenu-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/markdownviewer": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/markdownviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/markedparser-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/mathjax-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/mermaid": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/mermaid-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/metadataform": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/metadataform-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/metapackage": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/nbconvert-css": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/nbformat": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/notebook": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/notebook-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/observables": {
                             "import": false,
-                            "requiredVersion": "^5.2.0"
+                            "requiredVersion": "^5.1.5"
                         },
                         "@jupyterlab/outputarea": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/pdf-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/pluginmanager": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/pluginmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/property-inspector": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/rendermime": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/rendermime-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/rendermime-interfaces": {
                             "import": false,
-                            "requiredVersion": "^3.10.0",
+                            "requiredVersion": "^3.9.5",
                             "singleton": true
                         },
                         "@jupyterlab/running": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/running-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/services": {
                             "import": false,
-                            "requiredVersion": "^7.2.0",
+                            "requiredVersion": "^7.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/settingregistry": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/shortcuts-extension": {
                             "import": false,
-                            "requiredVersion": "^5.0.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/statedb": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/terminal": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/terminal-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/theme-dark-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
-                        },
-                        "@jupyterlab/theme-dark-high-contrast-extension": {
-                            "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/theme-light-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/toc": {
                             "import": false,
-                            "requiredVersion": "^6.2.0",
+                            "requiredVersion": "^6.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/toc-extension": {
                             "import": false,
-                            "requiredVersion": "^6.2.0"
+                            "requiredVersion": "^6.1.5"
                         },
                         "@jupyterlab/tooltip": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/tooltip-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/translation": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/translation-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/ui-components": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/ui-components-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/vega5-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
-                        },
-                        "@jupyterlab/workspaces": {
-                            "import": false,
-                            "requiredVersion": "^4.2.0",
-                            "singleton": true
-                        },
-                        "@jupyterlab/workspaces-extension": {
-                            "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@lezer/common": {
                             "import": false,
                             "requiredVersion": "^1.0.0",
                             "singleton": true
                         },
                         "@lezer/highlight": {
@@ -707,54 +695,9 @@
                 "url": false
             }
         },
         "watchOptions": {
             "aggregateTimeout": 1000,
             "poll": 500
         }
-    },
-    {
-        "entry": {
-            "index": "/Users/thibaut/Documents/amphi-etl/packages/theme-light/style/index.css"
-        },
-        "mode": "production",
-        "module": {
-            "rules": [
-                {
-                    "test": "/\\.css$/",
-                    "use": [
-                        "/Users/thibaut/Documents/amphi-etl/node_modules/mini-css-extract-plugin/dist/loader.js",
-                        "/Users/thibaut/Documents/amphi-etl/node_modules/css-loader/dist/cjs.js"
-                    ]
-                },
-                {
-                    "generator": {},
-                    "test": "/\\.svg/",
-                    "type": "asset/inline"
-                },
-                {
-                    "test": "/\\.(cur|png|jpg|gif|ttf|woff|woff2|eot)(\\?v=[0-9]\\.[0-9]\\.[0-9])?$/",
-                    "type": "asset"
-                }
-            ]
-        },
-        "output": {
-            "filename": "[name].js",
-            "hashFunction": "sha256",
-            "path": "/Users/thibaut/Documents/amphi-etl/amphi/theme-light/themes/@amphi/theme-light"
-        },
-        "plugins": [
-            {
-                "_sortedModulesCache": {},
-                "options": {
-                    "chunkFilename": "[id].css",
-                    "filename": "[name].css",
-                    "ignoreOrder": false,
-                    "runtime": true
-                },
-                "runtimeOptions": {
-                    "linkType": "text/css"
-                }
-            }
-        ]
     }
 ]
```

### Comparing `amphi-etl-0.3.5/amphi/theme-light/package.json` & `amphi-etl-0.3.6/amphi/theme-light/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991319444444444%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.bf309478c3347f5f051d.js'}}"}*

```diff
@@ -30,15 +30,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/amphi-ai/amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.020f6c95bb859ea9639f.js"
+            "load": "static/remoteEntry.bf309478c3347f5f051d.js"
         },
         "extension": true,
         "outputDir": "../../amphi/theme-light",
         "themePath": "style/index.css"
     },
     "keywords": [
         "jupyter",
```

### Comparing `amphi-etl-0.3.5/amphi/theme-light/static/lib_index_js.76fd05e25cd1622361b8.js` & `amphi-etl-0.3.6/amphi/theme-light/static/lib_index_js.76fd05e25cd1622361b8.js`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/amphi/theme-light/static/lib_index_js.76fd05e25cd1622361b8.js.map` & `amphi-etl-0.3.6/amphi/theme-light/static/lib_index_js.76fd05e25cd1622361b8.js.map`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/amphi/theme-light/static/remoteEntry.020f6c95bb859ea9639f.js` & `amphi-etl-0.3.6/amphi/theme-light/static/remoteEntry.bf309478c3347f5f051d.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -821,15 +821,15 @@
             /******/
         });
         /******/
         var installedModules = {};
         /******/
         var moduleToHandlerMapping = {
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 4, 3, 0]))
+            "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 4, 2, 5]))
             /******/
         };
         /******/ // no consumes in initial chunks
         /******/
         var chunkMapping = {
             /******/
             "lib_index_js": [
@@ -1064,8 +1064,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/@amphi/theme-light");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB)["@amphi/theme-light"] = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.020f6c95bb859ea9639f.js.map
+//# sourceMappingURL=remoteEntry.bf309478c3347f5f051d.js.map
```

### Comparing `amphi-etl-0.3.5/amphi/theme-light/static/remoteEntry.020f6c95bb859ea9639f.js.map` & `amphi-etl-0.3.6/amphi/theme-light/static/remoteEntry.bf309478c3347f5f051d.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9206349206349207%*

 * *Differences: {"'file'": "'remoteEntry.bf309478c3347f5f051d.js'",*

 * * "'sourcesContent'": "{insert: [(12, 'var parseVersion = (str) => {\\n\\t// see "*

 * *                     'webpack/lib/util/semver.js for original code\\n\\tvar p=p=>{return '*

 * *                     'p.split(".").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return '*

 * *                     'n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\\n}\\nvar '*

 * *                    […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "remoteEntry.020f6c95bb859ea9639f.js",
+    "file": "remoteEntry.bf309478c3347f5f051d.js",
     "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCjCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA;WACA;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC7CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB;WACA,GAAG;WACH;WACA;;;;;WC9KA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;UErFA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://@amphi/theme-light/webpack/container-entry",
         "webpack://@amphi/theme-light/webpack/bootstrap",
         "webpack://@amphi/theme-light/webpack/runtime/compat get default export",
@@ -31,15 +31,15 @@
         "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + \"76fd05e25cd1622361b8\" + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"@amphi/theme-light:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
         "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"@amphi/theme-light\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"@amphi/theme-light\", \"0.1.0\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && (!scriptUrl || !/^http(s?):/.test(scriptUrl))) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,4,3,0]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\"\n\t]\n};\nvar startedInstallModules = {};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tif(!startedInstallModules[id]) {\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tstartedInstallModules[id] = true;\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t\t}\n\t\t});\n\t}\n}",
+        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,4,2,5]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\"\n\t]\n};\nvar startedInstallModules = {};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tif(!startedInstallModules[id]) {\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tstartedInstallModules[id] = true;\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t\t}\n\t\t});\n\t}\n}",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"@amphi/theme-light\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t}\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunk_amphi_theme_light\"] = self[\"webpackChunk_amphi_theme_light\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/@amphi/theme-light\");\n",
         ""
     ],
     "version": 3
 }
```

### Comparing `amphi-etl-0.3.5/amphi/theme-light/themes/@amphi/theme-light/index.css` & `amphi-etl-0.3.6/amphi/theme-light/themes/@amphi/theme-light/index.css`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     --amphi-interactive-02: #393939;
     --amphi-interactive-03: #5A8F7B;
     --amphi-interactive-04: #5A8F7B;
     --amphi-ui-background: #ffffff;
     /* --amphi-ui-01: #f4f4f4; */
     --amphi-ui-01: #ffffff;
     --amphi-ui-02: #ffffff;
-    --amphi-ui-03: #ffffff;
+    --amphi-ui-03: #F2F4F7;
     --amphi-ui-04: #fff;
     --amphi-ui-05: #161616;
     --amphi-text-01: #161616;
     --amphi-text-02: #525252;
     --amphi-text-03: #a8a8a8;
     --amphi-text-04: #ffffff;
     --amphi-text-05: #6f6f6f;
@@ -625,14 +625,20 @@
   padding-bottom: 4px
 }
 
 .lm-DockPanel-tabBar .lm-TabBar-addButton svg {
   height: 24px
 }
 
+.lm-DockPanel-handle[data-orientation='vertical'] {
+  border-bottom: 1px solid var(--amphi-skeleton-01);
+  background-color: transparent;
+
+}
+
 .lm-CommandPalette-itemLabel {
   line-height: 1rem
 }
 
 .lm-CommandPalette-wrapper:after {
   background-color: #0000;
   right: 1rem
```

### Comparing `amphi-etl-0.3.5/amphi/ui-component/build_log.json` & `amphi-etl-0.3.6/amphi/theme-light/build_log.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.49562279972029327%*

 * *Differences: {'0': "{'output': {'path': '/Users/thibaut/Documents/amphi-etl/amphi/theme-light/static'}, "*

 * *      "'plugins': {1: {'_options': {'name': '@amphi/theme-light', 'library': {'name': {insert: "*

 * *      "[(1, '@amphi/theme-light')], delete: [1]}}, 'exposes': {'./index': "*

 * *      "'/Users/thibaut/Documents/amphi-etl/packages/theme-light/lib/index.js', './extension': "*

 * *      "'/Users/thibaut/Documents/amphi-etl/packages/theme-light/lib/index.js', delete: "*

 * *      "['./style']}, 'shared': {'@jupyterlab/application': {' […]*

```diff
@@ -88,42 +88,41 @@
                     ]
                 }
             ]
         },
         "output": {
             "filename": "[name].[contenthash].js",
             "hashFunction": "sha256",
-            "path": "/Users/thibaut/Documents/amphi-etl/amphi/ui-component/static",
+            "path": "/Users/thibaut/Documents/amphi-etl/amphi/theme-light/static",
             "publicPath": "auto"
         },
         "plugins": [
             {
                 "definitions": {
                     "process": "process/browser"
                 }
             },
             {
                 "_options": {
                     "exposes": {
-                        "./extension": "/Users/thibaut/Documents/amphi-etl/packages/ui-component/lib/index.js",
-                        "./index": "/Users/thibaut/Documents/amphi-etl/packages/ui-component/lib/index.js",
-                        "./style": "/Users/thibaut/Documents/amphi-etl/packages/ui-component/style/index.js"
+                        "./extension": "/Users/thibaut/Documents/amphi-etl/packages/theme-light/lib/index.js",
+                        "./index": "/Users/thibaut/Documents/amphi-etl/packages/theme-light/lib/index.js"
                     },
                     "filename": "remoteEntry.[contenthash].js",
                     "library": {
                         "name": [
                             "_JUPYTERLAB",
-                            "@amphi/ui-component"
+                            "@amphi/theme-light"
                         ],
                         "type": "var"
                     },
-                    "name": "@amphi/ui-component",
+                    "name": "@amphi/theme-light",
                     "shared": {
-                        "@amphi/ui-component": {
-                            "import": "/Users/thibaut/Documents/amphi-etl/packages/ui-component/lib/index.js",
+                        "@amphi/theme-light": {
+                            "import": "/Users/thibaut/Documents/amphi-etl/packages/theme-light/lib/index.js",
                             "singleton": true,
                             "version": "0.1.0"
                         },
                         "@codemirror/language": {
                             "import": false,
                             "requiredVersion": "^6.0.0",
                             "singleton": true
@@ -136,457 +135,444 @@
                         "@codemirror/view": {
                             "import": false,
                             "requiredVersion": "^6.9.6",
                             "singleton": true
                         },
                         "@jupyter/react-components": {
                             "import": false,
-                            "requiredVersion": "^0.15.3",
+                            "requiredVersion": "^0.13.3",
                             "singleton": true
                         },
                         "@jupyter/web-components": {
                             "import": false,
-                            "requiredVersion": "^0.15.3",
+                            "requiredVersion": "^0.13.3",
                             "singleton": true
                         },
                         "@jupyter/ydoc": {
                             "import": false,
-                            "requiredVersion": "^2.0.1",
+                            "requiredVersion": "^1.1.1",
                             "singleton": true
                         },
                         "@jupyterlab/application": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/application-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/apputils": {
                             "import": false,
-                            "requiredVersion": "^4.3.0",
+                            "requiredVersion": "^4.2.5",
                             "singleton": true
                         },
                         "@jupyterlab/apputils-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/attachments": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/cell-toolbar": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/cell-toolbar-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/cells": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/celltags-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/codeeditor": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/completer": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/completer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/console": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/console-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/coreutils": {
                             "import": false,
-                            "requiredVersion": "^6.2.0",
+                            "requiredVersion": "^6.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/csvviewer": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/csvviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/debugger": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/debugger-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/docmanager": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/docmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/docregistry": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/documentsearch": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/documentsearch-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/extensionmanager": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/extensionmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/filebrowser": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/filebrowser-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/fileeditor": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/fileeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/help-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/htmlviewer": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/htmlviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/hub-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/imageviewer": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/imageviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/inspector": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/inspector-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/javascript-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/json-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/launcher": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/launcher-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/logconsole": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/logconsole-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/lsp": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/lsp-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/mainmenu": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/mainmenu-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/markdownviewer": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/markdownviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/markedparser-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/mathjax-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/mermaid": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/mermaid-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/metadataform": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/metadataform-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/metapackage": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/nbconvert-css": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/nbformat": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/notebook": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/notebook-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/observables": {
                             "import": false,
-                            "requiredVersion": "^5.2.0"
+                            "requiredVersion": "^5.1.5"
                         },
                         "@jupyterlab/outputarea": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/pdf-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/pluginmanager": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/pluginmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/property-inspector": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/rendermime": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/rendermime-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/rendermime-interfaces": {
                             "import": false,
-                            "requiredVersion": "^3.10.0",
+                            "requiredVersion": "^3.9.5",
                             "singleton": true
                         },
                         "@jupyterlab/running": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/running-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/services": {
                             "import": false,
-                            "requiredVersion": "^7.2.0",
+                            "requiredVersion": "^7.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/settingregistry": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/shortcuts-extension": {
                             "import": false,
-                            "requiredVersion": "^5.0.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/statedb": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/terminal": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/terminal-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/theme-dark-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
-                        },
-                        "@jupyterlab/theme-dark-high-contrast-extension": {
-                            "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/theme-light-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/toc": {
                             "import": false,
-                            "requiredVersion": "^6.2.0",
+                            "requiredVersion": "^6.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/toc-extension": {
                             "import": false,
-                            "requiredVersion": "^6.2.0"
+                            "requiredVersion": "^6.1.5"
                         },
                         "@jupyterlab/tooltip": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/tooltip-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/translation": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/translation-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/ui-components": {
                             "import": false,
-                            "requiredVersion": "^4.2.0",
+                            "requiredVersion": "^4.1.5",
                             "singleton": true
                         },
                         "@jupyterlab/ui-components-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@jupyterlab/vega5-extension": {
                             "import": false,
-                            "requiredVersion": "^4.2.0"
-                        },
-                        "@jupyterlab/workspaces": {
-                            "import": false,
-                            "requiredVersion": "^4.2.0",
-                            "singleton": true
-                        },
-                        "@jupyterlab/workspaces-extension": {
-                            "import": false,
-                            "requiredVersion": "^4.2.0"
+                            "requiredVersion": "^4.1.5"
                         },
                         "@lezer/common": {
                             "import": false,
                             "requiredVersion": "^1.0.0",
                             "singleton": true
                         },
                         "@lezer/highlight": {
@@ -708,9 +694,54 @@
                 "url": false
             }
         },
         "watchOptions": {
             "aggregateTimeout": 1000,
             "poll": 500
         }
+    },
+    {
+        "entry": {
+            "index": "/Users/thibaut/Documents/amphi-etl/packages/theme-light/style/index.css"
+        },
+        "mode": "production",
+        "module": {
+            "rules": [
+                {
+                    "test": "/\\.css$/",
+                    "use": [
+                        "/Users/thibaut/Documents/amphi-etl/node_modules/mini-css-extract-plugin/dist/loader.js",
+                        "/Users/thibaut/Documents/amphi-etl/node_modules/css-loader/dist/cjs.js"
+                    ]
+                },
+                {
+                    "generator": {},
+                    "test": "/\\.svg/",
+                    "type": "asset/inline"
+                },
+                {
+                    "test": "/\\.(cur|png|jpg|gif|ttf|woff|woff2|eot)(\\?v=[0-9]\\.[0-9]\\.[0-9])?$/",
+                    "type": "asset"
+                }
+            ]
+        },
+        "output": {
+            "filename": "[name].js",
+            "hashFunction": "sha256",
+            "path": "/Users/thibaut/Documents/amphi-etl/amphi/theme-light/themes/@amphi/theme-light"
+        },
+        "plugins": [
+            {
+                "_sortedModulesCache": {},
+                "options": {
+                    "chunkFilename": "[id].css",
+                    "filename": "[name].css",
+                    "ignoreOrder": false,
+                    "runtime": true
+                },
+                "runtimeOptions": {
+                    "linkType": "text/css"
+                }
+            }
+        ]
     }
 ]
```

### Comparing `amphi-etl-0.3.5/amphi/ui-component/package.json` & `amphi-etl-0.3.6/amphi/ui-component/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993386243386243%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.d516e88595b29cbc0207.js'}}"}*

```diff
@@ -39,15 +39,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.15dfea293b8af56eb37f.js",
+            "load": "static/remoteEntry.d516e88595b29cbc0207.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../amphi/ui-component"
     },
     "license": "ELv2",
     "main": "lib/index.js",
```

### Comparing `amphi-etl-0.3.5/amphi/ui-component/static/lib_index_js.3a5d11eaa6df06cb0ee7.js` & `amphi-etl-0.3.6/amphi/ui-component/static/lib_index_js.3a5d11eaa6df06cb0ee7.js`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/amphi/ui-component/static/lib_index_js.3a5d11eaa6df06cb0ee7.js.map` & `amphi-etl-0.3.6/amphi/ui-component/static/lib_index_js.3a5d11eaa6df06cb0ee7.js.map`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/amphi/ui-component/static/node_modules_css-loader_dist_cjs_js_style_output_css-node_modules_style-loader_dist_runtime_i-dc6767.e55ff0d3e2b5f4c1df14.js` & `amphi-etl-0.3.6/amphi/ui-component/static/node_modules_css-loader_dist_cjs_js_style_output_css-node_modules_style-loader_dist_runtime_i-dc6767.e55ff0d3e2b5f4c1df14.js`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/amphi/ui-component/static/node_modules_css-loader_dist_cjs_js_style_output_css-node_modules_style-loader_dist_runtime_i-dc6767.e55ff0d3e2b5f4c1df14.js.map` & `amphi-etl-0.3.6/amphi/ui-component/static/node_modules_css-loader_dist_cjs_js_style_output_css-node_modules_style-loader_dist_runtime_i-dc6767.e55ff0d3e2b5f4c1df14.js.map`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/amphi/ui-component/static/remoteEntry.15dfea293b8af56eb37f.js` & `amphi-etl-0.3.6/amphi/ui-component/static/remoteEntry.d516e88595b29cbc0207.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -829,33 +829,33 @@
             /******/
         });
         /******/
         var installedModules = {};
         /******/
         var moduleToHandlerMapping = {
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/application": () => (loadSingletonVersionCheck("default", "@jupyterlab/application", [1, 4, 2, 0])),
+            "webpack/sharing/consume/default/@jupyterlab/application": () => (loadSingletonVersionCheck("default", "@jupyterlab/application", [1, 4, 1, 5])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/launcher": () => (loadSingletonVersionCheck("default", "@jupyterlab/launcher", [1, 4, 2, 0])),
+            "webpack/sharing/consume/default/@jupyterlab/launcher": () => (loadSingletonVersionCheck("default", "@jupyterlab/launcher", [1, 4, 1, 5])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/ui-components": () => (loadSingletonVersionCheck("default", "@jupyterlab/ui-components", [1, 4, 2, 0])),
+            "webpack/sharing/consume/default/@jupyterlab/ui-components": () => (loadSingletonVersionCheck("default", "@jupyterlab/ui-components", [1, 4, 1, 5])),
             /******/
             "webpack/sharing/consume/default/@lumino/algorithm": () => (loadSingletonVersionCheck("default", "@lumino/algorithm", [1, 2, 0, 0])),
             /******/
             "webpack/sharing/consume/default/react": () => (loadSingletonVersionCheck("default", "react", [1, 18, 2, 0])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/mainmenu": () => (loadSingletonVersionCheck("default", "@jupyterlab/mainmenu", [1, 4, 2, 0])),
+            "webpack/sharing/consume/default/@jupyterlab/mainmenu": () => (loadSingletonVersionCheck("default", "@jupyterlab/mainmenu", [1, 4, 1, 5])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/translation": () => (loadSingletonVersionCheck("default", "@jupyterlab/translation", [1, 4, 2, 0])),
+            "webpack/sharing/consume/default/@jupyterlab/translation": () => (loadSingletonVersionCheck("default", "@jupyterlab/translation", [1, 4, 1, 5])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 4, 3, 0])),
+            "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 4, 2, 5])),
             /******/
             "webpack/sharing/consume/default/@lumino/widgets": () => (loadSingletonVersionCheck("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/filebrowser": () => (loadSingletonVersionCheck("default", "@jupyterlab/filebrowser", [1, 4, 2, 0]))
+            "webpack/sharing/consume/default/@jupyterlab/filebrowser": () => (loadSingletonVersionCheck("default", "@jupyterlab/filebrowser", [1, 4, 1, 5]))
             /******/
         };
         /******/ // no consumes in initial chunks
         /******/
         var chunkMapping = {
             /******/
             "lib_index_js": [
@@ -1117,8 +1117,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/@amphi/ui-component");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB)["@amphi/ui-component"] = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.15dfea293b8af56eb37f.js.map
+//# sourceMappingURL=remoteEntry.d516e88595b29cbc0207.js.map
```

### Comparing `amphi-etl-0.3.5/amphi/ui-component/static/remoteEntry.15dfea293b8af56eb37f.js.map` & `amphi-etl-0.3.6/amphi/ui-component/static/remoteEntry.d516e88595b29cbc0207.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9210526315789475%*

 * *Differences: {"'file'": "'remoteEntry.d516e88595b29cbc0207.js'",*

 * * "'sourcesContent'": "{insert: [(12, 'var parseVersion = (str) => {\\n\\t// see "*

 * *                     'webpack/lib/util/semver.js for original code\\n\\tvar p=p=>{return '*

 * *                     'p.split(".").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return '*

 * *                     'n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\\n}\\nvar '*

 * *                    […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "remoteEntry.15dfea293b8af56eb37f.js",
+    "file": "remoteEntry.d516e88595b29cbc0207.js",
     "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,4MAA4M;WAC1O;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC7CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB;WACA,GAAG;WACH;WACA;;;;;WChMA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://@amphi/ui-component/webpack/container-entry",
         "webpack://@amphi/ui-component/webpack/bootstrap",
         "webpack://@amphi/ui-component/webpack/runtime/compat get default export",
@@ -32,15 +32,15 @@
         "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"node_modules_css-loader_dist_cjs_js_style_output_css-node_modules_style-loader_dist_runtime_i-dc6767\":\"e55ff0d3e2b5f4c1df14\",\"lib_index_js\":\"3a5d11eaa6df06cb0ee7\",\"style_index_js\":\"7002c9447c653e7de570\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"@amphi/ui-component:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
         "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"@amphi/ui-component\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"@amphi/ui-component\", \"0.1.0\", () => (Promise.all([__webpack_require__.e(\"node_modules_css-loader_dist_cjs_js_style_output_css-node_modules_style-loader_dist_runtime_i-dc6767\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && (!scriptUrl || !/^http(s?):/.test(scriptUrl))) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/application\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/application\", [1,4,2,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/launcher\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/launcher\", [1,4,2,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,4,2,0])),\n\t\"webpack/sharing/consume/default/@lumino/algorithm\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/algorithm\", [1,2,0,0])),\n\t\"webpack/sharing/consume/default/react\": () => (loadSingletonVersionCheck(\"default\", \"react\", [1,18,2,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/mainmenu\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/mainmenu\", [1,4,2,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/translation\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/translation\", [1,4,2,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,4,3,0])),\n\t\"webpack/sharing/consume/default/@lumino/widgets\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/widgets\", [1,2,3,1,,\"alpha\",0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/filebrowser\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/filebrowser\", [1,4,2,0]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/application\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/launcher\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\",\n\t\t\"webpack/sharing/consume/default/@lumino/algorithm\",\n\t\t\"webpack/sharing/consume/default/react\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/mainmenu\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/translation\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@lumino/widgets\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/filebrowser\"\n\t]\n};\nvar startedInstallModules = {};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tif(!startedInstallModules[id]) {\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tstartedInstallModules[id] = true;\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t\t}\n\t\t});\n\t}\n}",
+        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/application\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/application\", [1,4,1,5])),\n\t\"webpack/sharing/consume/default/@jupyterlab/launcher\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/launcher\", [1,4,1,5])),\n\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,4,1,5])),\n\t\"webpack/sharing/consume/default/@lumino/algorithm\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/algorithm\", [1,2,0,0])),\n\t\"webpack/sharing/consume/default/react\": () => (loadSingletonVersionCheck(\"default\", \"react\", [1,18,2,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/mainmenu\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/mainmenu\", [1,4,1,5])),\n\t\"webpack/sharing/consume/default/@jupyterlab/translation\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/translation\", [1,4,1,5])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,4,2,5])),\n\t\"webpack/sharing/consume/default/@lumino/widgets\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/widgets\", [1,2,3,1,,\"alpha\",0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/filebrowser\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/filebrowser\", [1,4,1,5]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/application\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/launcher\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\",\n\t\t\"webpack/sharing/consume/default/@lumino/algorithm\",\n\t\t\"webpack/sharing/consume/default/react\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/mainmenu\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/translation\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@lumino/widgets\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/filebrowser\"\n\t]\n};\nvar startedInstallModules = {};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tif(!startedInstallModules[id]) {\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tstartedInstallModules[id] = true;\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t\t}\n\t\t});\n\t}\n}",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"@amphi/ui-component\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t}\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunk_amphi_ui_component\"] = self[\"webpackChunk_amphi_ui_component\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "__webpack_require__.nc = undefined;",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/@amphi/ui-component\");\n",
         ""
     ],
     "version": 3
```

### Comparing `amphi-etl-0.3.5/amphi/ui-component/static/style_index_js.7002c9447c653e7de570.js` & `amphi-etl-0.3.6/amphi/ui-component/static/style_index_js.7002c9447c653e7de570.js`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/amphi/ui-component/static/style_index_js.7002c9447c653e7de570.js.map` & `amphi-etl-0.3.6/amphi/ui-component/static/style_index_js.7002c9447c653e7de570.js.map`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/amphi_etl.egg-info/PKG-INFO` & `amphi-etl-0.3.6/amphi_etl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amphi-etl
-Version: 0.3.5
+Version: 0.3.6
 Summary: Amphi is a python-based ETL
 Author: Thibaut Gourdel
 Author-email: tgourdel@amphi.ai
 License: Elastic License 2.0 \(ELv2\)
         
         **Acceptance** By using the software, you agree to all of the terms and conditions below.
```

### Comparing `amphi-etl-0.3.5/amphi_etl.egg-info/SOURCES.txt` & `amphi-etl-0.3.6/amphi_etl.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -2,53 +2,68 @@
 MANIFEST.in
 README.md
 package.json
 pyproject.toml
 setup.py
 tsconfig.eslint.json
 tsconfigbase.json
+yarn.lock
 amphi/__init__.py
 amphi/_version.py
 amphi/main.py
 amphi/theme-light/build_log.json
 amphi/theme-light/package.json
 amphi/theme-light/static/lib_index_js.76fd05e25cd1622361b8.js
 amphi/theme-light/static/lib_index_js.76fd05e25cd1622361b8.js.map
-amphi/theme-light/static/remoteEntry.020f6c95bb859ea9639f.js
-amphi/theme-light/static/remoteEntry.020f6c95bb859ea9639f.js.map
+amphi/theme-light/static/remoteEntry.bf309478c3347f5f051d.js
+amphi/theme-light/static/remoteEntry.bf309478c3347f5f051d.js.map
 amphi/theme-light/static/style.js
 amphi/theme-light/themes/@amphi/theme-light/index.css
 amphi/theme-light/themes/@amphi/theme-light/index.js
 amphi/ui-component/build_log.json
 amphi/ui-component/package.json
 amphi/ui-component/static/lib_index_js.3a5d11eaa6df06cb0ee7.js
 amphi/ui-component/static/lib_index_js.3a5d11eaa6df06cb0ee7.js.map
 amphi/ui-component/static/node_modules_css-loader_dist_cjs_js_style_output_css-node_modules_style-loader_dist_runtime_i-dc6767.e55ff0d3e2b5f4c1df14.js
 amphi/ui-component/static/node_modules_css-loader_dist_cjs_js_style_output_css-node_modules_style-loader_dist_runtime_i-dc6767.e55ff0d3e2b5f4c1df14.js.map
-amphi/ui-component/static/remoteEntry.15dfea293b8af56eb37f.js
-amphi/ui-component/static/remoteEntry.15dfea293b8af56eb37f.js.map
+amphi/ui-component/static/remoteEntry.d516e88595b29cbc0207.js
+amphi/ui-component/static/remoteEntry.d516e88595b29cbc0207.js.map
 amphi/ui-component/static/style.js
 amphi/ui-component/static/style_index_js.7002c9447c653e7de570.js
 amphi/ui-component/static/style_index_js.7002c9447c653e7de570.js.map
 amphi_etl.egg-info/PKG-INFO
 amphi_etl.egg-info/SOURCES.txt
 amphi_etl.egg-info/dependency_links.txt
 amphi_etl.egg-info/entry_points.txt
 amphi_etl.egg-info/requires.txt
 amphi_etl.egg-info/top_level.txt
 config/labconfig/page_config.json
 config/settings/overrides.json
 packages/theme-light/package.json
 packages/theme-light/tsconfig.json
+packages/theme-light/tsconfig.tsbuildinfo
+packages/theme-light/lib/index.d.ts
+packages/theme-light/lib/index.js
 packages/theme-light/src/index.ts
 packages/theme-light/style/index.css
 packages/theme-light/style/variables.css
 packages/ui-component/package.json
 packages/ui-component/tailwind.config.js
 packages/ui-component/tsconfig.json
+packages/ui-component/tsconfig.tsbuildinfo
+packages/ui-component/lib/BrowseFileDialog.d.ts
+packages/ui-component/lib/BrowseFileDialog.js
+packages/ui-component/lib/Dropzone.d.ts
+packages/ui-component/lib/Dropzone.js
+packages/ui-component/lib/icons.d.ts
+packages/ui-component/lib/icons.js
+packages/ui-component/lib/index.d.ts
+packages/ui-component/lib/index.js
+packages/ui-component/lib/launcher.d.ts
+packages/ui-component/lib/launcher.js
 packages/ui-component/src/BrowseFileDialog.tsx
 packages/ui-component/src/Dropzone.tsx
 packages/ui-component/src/declarations.d.ts
 packages/ui-component/src/icons.ts
 packages/ui-component/src/index.ts
 packages/ui-component/src/launcher.tsx
 packages/ui-component/style/base.css
```

### Comparing `amphi-etl-0.3.5/config/labconfig/page_config.json` & `amphi-etl-0.3.6/config/labconfig/page_config.json`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/config/settings/overrides.json` & `amphi-etl-0.3.6/config/settings/overrides.json`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/package.json` & `amphi-etl-0.3.6/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.3.6'"}*

```diff
@@ -66,15 +66,15 @@
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md,.yml,.yaml}\"",
         "prettier:check": "jlpm prettier:base --check",
         "quickstart": "npm run setup:py && jlpm && jlpm deduplicate && jlpm clean:all && jlpm lint && jlpm build:prod && jlpm dist && jlpm docs && jlpm test",
         "setup:py": "python -m pip install -e \".[dev,lint,test,docs]\"",
         "test": "jlpm test:py",
         "test:py": "pytest"
     },
-    "version": "0.3.4",
+    "version": "0.3.6",
     "workspaces": {
         "packages": [
             "packages/theme-light",
             "packages/ui-component"
         ]
     }
 }
```

### Comparing `amphi-etl-0.3.5/packages/theme-light/package.json` & `amphi-etl-0.3.6/packages/theme-light/package.json`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/packages/theme-light/src/index.ts` & `amphi-etl-0.3.6/packages/theme-light/src/index.ts`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/packages/theme-light/style/index.css` & `amphi-etl-0.3.6/packages/theme-light/style/index.css`

 * *Files 1% similar despite different names*

```diff
@@ -296,14 +296,20 @@
   padding-bottom: 4px
 }
 
 .lm-DockPanel-tabBar .lm-TabBar-addButton svg {
   height: 24px
 }
 
+.lm-DockPanel-handle[data-orientation='vertical'] {
+  border-bottom: 1px solid var(--amphi-skeleton-01);
+  background-color: transparent;
+
+}
+
 .lm-CommandPalette-itemLabel {
   line-height: 1rem
 }
 
 .lm-CommandPalette-wrapper:after {
   background-color: #0000;
   right: 1rem
```

### Comparing `amphi-etl-0.3.5/packages/theme-light/style/variables.css` & `amphi-etl-0.3.6/packages/theme-light/style/variables.css`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     --amphi-interactive-02: #393939;
     --amphi-interactive-03: #5A8F7B;
     --amphi-interactive-04: #5A8F7B;
     --amphi-ui-background: #ffffff;
     /* --amphi-ui-01: #f4f4f4; */
     --amphi-ui-01: #ffffff;
     --amphi-ui-02: #ffffff;
-    --amphi-ui-03: #ffffff;
+    --amphi-ui-03: #F2F4F7;
     --amphi-ui-04: #fff;
     --amphi-ui-05: #161616;
     --amphi-text-01: #161616;
     --amphi-text-02: #525252;
     --amphi-text-03: #a8a8a8;
     --amphi-text-04: #ffffff;
     --amphi-text-05: #6f6f6f;
```

### Comparing `amphi-etl-0.3.5/packages/ui-component/package.json` & `amphi-etl-0.3.6/packages/ui-component/package.json`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/packages/ui-component/src/BrowseFileDialog.tsx` & `amphi-etl-0.3.6/packages/ui-component/src/BrowseFileDialog.tsx`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/packages/ui-component/src/Dropzone.tsx` & `amphi-etl-0.3.6/packages/ui-component/src/Dropzone.tsx`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/packages/ui-component/src/icons.ts` & `amphi-etl-0.3.6/packages/ui-component/src/icons.ts`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/packages/ui-component/src/index.ts` & `amphi-etl-0.3.6/packages/ui-component/src/index.ts`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/packages/ui-component/src/launcher.tsx` & `amphi-etl-0.3.6/packages/ui-component/src/launcher.tsx`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/packages/ui-component/style/icons/amphi-square-logo.svg` & `amphi-etl-0.3.6/packages/ui-component/style/icons/amphi-square-logo.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/packages/ui-component/style/icons/amphi-square-logo_nonpaths.svg` & `amphi-etl-0.3.6/packages/ui-component/style/icons/amphi-square-logo_nonpaths.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/packages/ui-component/style/icons/amphi.svg` & `amphi-etl-0.3.6/packages/ui-component/style/icons/amphi.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/packages/ui-component/style/icons/bug-16.svg` & `amphi-etl-0.3.6/packages/ui-component/style/icons/bug-16.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/packages/ui-component/style/icons/bug-24.svg` & `amphi-etl-0.3.6/packages/ui-component/style/icons/bug-24.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/packages/ui-component/style/icons/network-24.svg` & `amphi-etl-0.3.6/packages/ui-component/style/icons/network-24.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/packages/ui-component/style/icons/p5-square-logo.svg` & `amphi-etl-0.3.6/packages/ui-component/style/icons/p5-square-logo.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/packages/ui-component/style/icons/pipeline-16.svg` & `amphi-etl-0.3.6/packages/ui-component/style/icons/pipeline-16.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/packages/ui-component/style/icons/pipeline-24.svg` & `amphi-etl-0.3.6/packages/ui-component/style/icons/pipeline-24.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/packages/ui-component/style/icons/pipeline.svg` & `amphi-etl-0.3.6/packages/ui-component/style/icons/pipeline.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/packages/ui-component/style/icons/pipeline_negative.svg` & `amphi-etl-0.3.6/packages/ui-component/style/icons/pipeline_negative.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/packages/ui-component/style/icons/shield-check-24.svg` & `amphi-etl-0.3.6/packages/ui-component/style/icons/shield-check-24.svg`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/packages/ui-component/style/output.css` & `amphi-etl-0.3.6/packages/ui-component/style/output.css`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/packages/ui-component/tsconfig.json` & `amphi-etl-0.3.6/packages/ui-component/tsconfig.json`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/pyproject.toml` & `amphi-etl-0.3.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `amphi-etl-0.3.5/setup.py` & `amphi-etl-0.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     collect_files('amphi', 'share/jupyter/labextensions/@amphi') +
     collect_files('config/labconfig', 'etc/jupyter/labconfig') +
     collect_files('config/settings', 'share/jupyter/lab/settings')
 )
 
 setup(
     name='amphi-etl',
-    version='0.3.5',
+    version='0.3.6',
     description='Open-source and Python-based ETL',
     author='Thibaut Gourdel',
     author_email='tgourdel@amphi.ai',
     license='ELv2',
     install_requires=[
         'jupyterlab>=4.1.5',
         'jupyterlab-amphi>=0.3.1',
```

### Comparing `amphi-etl-0.3.5/tsconfigbase.json` & `amphi-etl-0.3.6/tsconfigbase.json`

 * *Files identical despite different names*

