# Comparing `tmp/notolog-0.9.1b4.tar.gz` & `tmp/notolog-0.9.1b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notolog-0.9.1b4.tar", last modified: Sun May 12 16:48:59 2024, max compression
+gzip compressed data, was "notolog-0.9.1b6.tar", last modified: Sun May 19 22:39:55 2024, max compression
```

## Comparing `notolog-0.9.1b4.tar` & `notolog-0.9.1b6.tar`

### file list

```diff
@@ -1,352 +1,357 @@
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.310927 notolog-0.9.1b4/
--rw-r--r--   0 vadikus    (501) staff       (20)     7403 2024-05-12 16:16:12.000000 notolog-0.9.1b4/CHANGELOG.md
--rw-r--r--   0 vadikus    (501) staff       (20)     3490 2024-05-11 12:17:28.000000 notolog-0.9.1b4/CODE_OF_CONDUCT.md
--rw-r--r--   0 vadikus    (501) staff       (20)     1073 2024-05-04 21:27:31.000000 notolog-0.9.1b4/LICENSE
--rw-r--r--   0 vadikus    (501) staff       (20)      433 2024-05-11 12:17:28.000000 notolog-0.9.1b4/MANIFEST.in
--rw-r--r--   0 vadikus    (501) staff       (20)    17439 2024-05-12 16:48:59.232380 notolog-0.9.1b4/PKG-INFO
--rw-r--r--   0 vadikus    (501) staff       (20)    15349 2024-05-12 14:50:00.000000 notolog-0.9.1b4/README.md
--rw-r--r--   0 vadikus    (501) staff       (20)       87 2024-05-05 14:33:15.000000 notolog-0.9.1b4/app_config.toml
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:58.838428 notolog-0.9.1b4/docs/
--rw-r--r--   0 vadikus    (501) staff       (20)     8631 2024-05-11 12:17:28.000000 notolog-0.9.1b4/docs/Examples.md
--rw-r--r--   0 vadikus    (501) staff       (20)   247033 2024-05-04 21:27:32.000000 notolog-0.9.1b4/docs/notolog-ui-settings.png
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:58.866873 notolog-0.9.1b4/notolog/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4777 2024-05-12 14:50:00.000000 notolog-0.9.1b4/notolog/app_config.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:58.875902 notolog-0.9.1b4/notolog/assets/
--rw-r--r--   0 vadikus    (501) staff       (20)     4202 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/notolog-example-image.png
--rw-r--r--   0 vadikus    (501) staff       (20)    88211 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/notolog-logo.png
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:58.824162 notolog-0.9.1b4/notolog/assets/themes/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:58.886726 notolog-0.9.1b4/notolog/assets/themes/calligraphy/
--rw-r--r--   0 vadikus    (501) staff       (20)      777 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/calligraphy/about_popup.css
--rw-r--r--   0 vadikus    (501) staff       (20)      365 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/calligraphy/ai_assistant.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2767 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/calligraphy/default.ini
--rw-r--r--   0 vadikus    (501) staff       (20)       56 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/calligraphy/editor.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2311 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/assets/themes/calligraphy/md.ini
--rw-r--r--   0 vadikus    (501) staff       (20)      885 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/calligraphy/settings_dialog.css
--rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/calligraphy/statusbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)     6818 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/calligraphy/styles.css
--rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/calligraphy/toolbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)      743 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/calligraphy/tree_view.css
--rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/calligraphy/viewer.css
--rw-r--r--   0 vadikus    (501) staff       (20)       80 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/calligraphy/viewer.ini
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:58.901661 notolog-0.9.1b4/notolog/assets/themes/default/
--rw-r--r--   0 vadikus    (501) staff       (20)      798 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/about_popup.css
--rw-r--r--   0 vadikus    (501) staff       (20)      253 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/ai_assistant.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2775 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/default.ini
--rw-r--r--   0 vadikus    (501) staff       (20)      174 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/editor.css
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:58.955776 notolog-0.9.1b4/notolog/assets/themes/default/icons/
--rw-r--r--   0 vadikus    (501) staff       (20)     1093 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/LICENSE
--rw-r--r--   0 vadikus    (501) staff       (20)      349 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/arrow-clockwise.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      567 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/arrow-repeat.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      736 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/balloon-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      797 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/balloon.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      812 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/bandaid-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      959 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/bandaid.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      528 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/box-arrow-up-right.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      538 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/box-arrow-up.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      265 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/caret-down-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      265 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/caret-up-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/code-slash.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      694 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/cursor-text.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      459 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/eyedropper.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      403 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/eyeglasses.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      479 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/file-earmark-lock2.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      394 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/file-earmark-plus-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      481 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/file-earmark-x.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      294 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/file-earmark.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      547 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/filetype-html.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      705 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/filetype-md.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      524 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/filetype-txt.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      401 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/floppy2-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      606 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/floppy2.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      428 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/folder-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      708 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/folder-symlink.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      527 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/folder.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      708 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/github.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      518 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/link-45deg.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      666 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/linkedin.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      575 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/pencil-square.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      261 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/power.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      582 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/quote.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      996 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/robot.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      316 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/share-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      653 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/shield-lock-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)     1057 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/shield-lock.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      399 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/star-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      623 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/star.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      272 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/three-dots.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      577 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/trash3-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      656 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/trash3.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      301 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/twitter-x.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      465 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/type-bold.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      351 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/type-italic.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      574 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/type-strikethrough.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      319 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/type-underline.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      351 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/x-circle-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      397 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/x-square-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      491 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/x-square.svg
--rw-r--r--   0 vadikus    (501) staff       (20)     2363 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/assets/themes/default/md.ini
--rw-r--r--   0 vadikus    (501) staff       (20)      721 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/settings_dialog.css
--rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/statusbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)     8472 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/assets/themes/default/styles.css
--rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/toolbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)      744 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/tree_view.css
--rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/viewer.css
--rw-r--r--   0 vadikus    (501) staff       (20)       82 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/viewer.ini
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:58.973013 notolog-0.9.1b4/notolog/assets/themes/noir_dark/
--rw-r--r--   0 vadikus    (501) staff       (20)      777 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/noir_dark/about_popup.css
--rw-r--r--   0 vadikus    (501) staff       (20)      347 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/noir_dark/ai_assistant.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2745 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/noir_dark/default.ini
--rw-r--r--   0 vadikus    (501) staff       (20)       56 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/noir_dark/editor.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2480 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/assets/themes/noir_dark/md.ini
--rw-r--r--   0 vadikus    (501) staff       (20)     1435 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/noir_dark/settings_dialog.css
--rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/noir_dark/statusbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)     6935 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/noir_dark/styles.css
--rw-r--r--   0 vadikus    (501) staff       (20)      280 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/noir_dark/toolbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)      711 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/noir_dark/tree_view.css
--rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/noir_dark/viewer.css
--rw-r--r--   0 vadikus    (501) staff       (20)       76 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/noir_dark/viewer.ini
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:58.984706 notolog-0.9.1b4/notolog/assets/themes/strawberry/
--rw-r--r--   0 vadikus    (501) staff       (20)      790 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/strawberry/about_popup.css
--rw-r--r--   0 vadikus    (501) staff       (20)      317 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/strawberry/ai_assistant.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2775 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/strawberry/default.ini
--rw-r--r--   0 vadikus    (501) staff       (20)       50 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/strawberry/editor.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2408 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/assets/themes/strawberry/md.ini
--rw-r--r--   0 vadikus    (501) staff       (20)      753 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/strawberry/settings_dialog.css
--rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/strawberry/statusbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)     8451 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/strawberry/styles.css
--rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/strawberry/toolbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)      764 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/strawberry/tree_view.css
--rw-r--r--   0 vadikus    (501) staff       (20)       60 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/strawberry/viewer.css
--rw-r--r--   0 vadikus    (501) staff       (20)       84 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/strawberry/viewer.ini
--rw-r--r--   0 vadikus    (501) staff       (20)     7823 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/edit_widget.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4196 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/editor_state.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:58.990144 notolog-0.9.1b4/notolog/encrypt/
--rw-r--r--   0 vadikus    (501) staff       (20)      152 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/encrypt/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4341 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/encrypt/enc_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6076 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/encrypt/enc_new_password_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)      626 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/encrypt/enc_password.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4172 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/encrypt/enc_password_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3211 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/encrypt/enc_password_reset_dialog.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:58.996856 notolog-0.9.1b4/notolog/enums/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/enums/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1433 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/enums/ai_model_names.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5624 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/enums/colors.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1125 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/enums/enum_base.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1367 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/enums/languages.py
--rw-r--r--   0 vadikus    (501) staff       (20)      451 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/enums/themes.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4516 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/etree_extension.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.001391 notolog-0.9.1b4/notolog/exceptions/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/exceptions/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)       52 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/exceptions/file_header_empty_exception.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7559 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/file_header.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2856 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/file_system_watcher.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.014476 notolog-0.9.1b4/notolog/helpers/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/helpers/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)      187 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/helpers/clipboard_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4227 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/helpers/file_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5511 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/helpers/theme_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1036 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/helpers/tooltip_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7411 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/helpers/update_helper.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.026023 notolog-0.9.1b4/notolog/highlight/
--rw-r--r--   0 vadikus    (501) staff       (20)      126 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/highlight/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9213 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/highlight/main_highlighter.py
--rw-r--r--   0 vadikus    (501) staff       (20)    51699 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/highlight/md_highlighter.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8475 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/highlight/view_highlighter.py
--rw-r--r--   0 vadikus    (501) staff       (20)    10614 2024-05-12 16:23:25.000000 notolog-0.9.1b4/notolog/image_downloader.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.029491 notolog-0.9.1b4/notolog/lexemes/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/__init__.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.037097 notolog-0.9.1b4/notolog/lexemes/de/
--rw-r--r--   0 vadikus    (501) staff       (20)      830 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/de/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7202 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/de/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6586 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/de/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2267 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/de/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3788 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/de/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1225 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/de/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2757 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/de/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.045950 notolog-0.9.1b4/notolog/lexemes/en/
--rw-r--r--   0 vadikus    (501) staff       (20)      827 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/en/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7096 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/en/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6051 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/en/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2181 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/en/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3586 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/en/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1201 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/en/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2573 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/en/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.060050 notolog-0.9.1b4/notolog/lexemes/es/
--rw-r--r--   0 vadikus    (501) staff       (20)      882 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/es/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7309 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/es/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6560 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/es/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2316 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/es/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3890 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/es/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1222 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/es/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2793 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/es/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.065996 notolog-0.9.1b4/notolog/lexemes/fi/
--rw-r--r--   0 vadikus    (501) staff       (20)      856 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/fi/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7559 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/fi/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6292 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/fi/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2261 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/fi/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3759 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/fi/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1334 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/fi/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2662 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/fi/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.073713 notolog-0.9.1b4/notolog/lexemes/fr/
--rw-r--r--   0 vadikus    (501) staff       (20)      886 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/fr/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7247 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/fr/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6716 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/fr/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2344 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/fr/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3978 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/fr/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1236 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/fr/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2824 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/fr/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.079264 notolog-0.9.1b4/notolog/lexemes/ge/
--rw-r--r--   0 vadikus    (501) staff       (20)     1323 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ge/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)    10627 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ge/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9735 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/ge/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3459 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ge/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5742 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ge/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1583 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ge/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4107 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ge/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.085114 notolog-0.9.1b4/notolog/lexemes/gr/
--rw-r--r--   0 vadikus    (501) staff       (20)     1100 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/gr/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8990 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/gr/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8668 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/gr/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2907 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/gr/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5016 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/gr/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1561 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/gr/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3679 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/gr/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.089773 notolog-0.9.1b4/notolog/lexemes/in/
--rw-r--r--   0 vadikus    (501) staff       (20)     1208 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/in/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9434 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/in/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)    10078 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/in/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3124 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/in/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5546 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/in/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1549 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/in/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3828 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/in/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.099736 notolog-0.9.1b4/notolog/lexemes/it/
--rw-r--r--   0 vadikus    (501) staff       (20)      864 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/it/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7263 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/it/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6366 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/it/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2302 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/it/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3825 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/it/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1238 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/it/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2780 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/it/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.109845 notolog-0.9.1b4/notolog/lexemes/ja/
--rw-r--r--   0 vadikus    (501) staff       (20)      931 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ja/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8464 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ja/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7248 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/ja/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2443 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ja/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4014 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ja/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1242 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ja/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3000 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ja/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.116368 notolog-0.9.1b4/notolog/lexemes/ko/
--rw-r--r--   0 vadikus    (501) staff       (20)      848 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ko/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7597 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ko/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6775 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/ko/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2268 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ko/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3697 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ko/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1221 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ko/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2666 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ko/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.123756 notolog-0.9.1b4/notolog/lexemes/la/
--rw-r--r--   0 vadikus    (501) staff       (20)      842 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/la/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7538 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/la/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6245 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/la/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2297 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/la/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3753 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/la/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1257 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/la/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2736 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/la/toolbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3739 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/lexemes.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.129926 notolog-0.9.1b4/notolog/lexemes/nl/
--rw-r--r--   0 vadikus    (501) staff       (20)      840 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/nl/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7094 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/nl/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6475 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/nl/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2229 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/nl/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3673 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/nl/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1220 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/nl/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2647 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/nl/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.136130 notolog-0.9.1b4/notolog/lexemes/pt/
--rw-r--r--   0 vadikus    (501) staff       (20)      898 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/pt/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7304 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/pt/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6357 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/pt/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2326 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/pt/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3830 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/pt/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1223 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/pt/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2830 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/pt/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.142253 notolog-0.9.1b4/notolog/lexemes/ru/
--rw-r--r--   0 vadikus    (501) staff       (20)      997 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ru/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9135 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ru/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7938 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/ru/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2883 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ru/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4896 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ru/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1428 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ru/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3453 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ru/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.154224 notolog-0.9.1b4/notolog/lexemes/se/
--rw-r--r--   0 vadikus    (501) staff       (20)      835 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/se/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7048 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/se/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6253 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/se/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2216 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/se/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3627 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/se/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1220 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/se/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2611 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/se/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.161795 notolog-0.9.1b4/notolog/lexemes/tr/
--rw-r--r--   0 vadikus    (501) staff       (20)      809 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/tr/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7401 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/tr/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6154 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/tr/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2276 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/tr/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3733 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/tr/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1240 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/tr/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2735 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/tr/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.170044 notolog-0.9.1b4/notolog/lexemes/zh/
--rw-r--r--   0 vadikus    (501) staff       (20)      792 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/zh/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7074 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/zh/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5777 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/zh/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2175 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/zh/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3476 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/zh/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1202 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/zh/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2559 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/zh/toolbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2860 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/main.py
--rw-r--r--   0 vadikus    (501) staff       (20)   178083 2024-05-12 16:26:17.000000 notolog-0.9.1b4/notolog/notolog_editor.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6260 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/settings.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3481 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/text_block_data.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6022 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/theme.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.187675 notolog-0.9.1b4/notolog/ui/
--rw-r--r--   0 vadikus    (501) staff       (20)      152 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/ui/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8224 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/ui/about_popup.py
--rw-r--r--   0 vadikus    (501) staff       (20)    16816 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/ui/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2099 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/ui/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3509 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/ui/common_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1306 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/ui/enum_combo_box.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5615 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/ui/file_system_model.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6999 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/ui/line_numbers.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2610 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/ui/rename_file_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1229 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/ui/rotating_label.py
--rw-r--r--   0 vadikus    (501) staff       (20)    37284 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/ui/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3197 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/ui/sort_filter_proxy_model.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6840 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/ui/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)    12804 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/ui/toolbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/ui/vertical_line_spacer.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8191 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/view_decorator.py
--rw-r--r--   0 vadikus    (501) staff       (20)    16132 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/view_processor.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2446 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/view_widget.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.230873 notolog-0.9.1b4/notolog.egg-info/
--rw-r--r--   0 vadikus    (501) staff       (20)    17439 2024-05-12 16:48:58.000000 notolog-0.9.1b4/notolog.egg-info/PKG-INFO
--rw-r--r--   0 vadikus    (501) staff       (20)    11469 2024-05-12 16:48:58.000000 notolog-0.9.1b4/notolog.egg-info/SOURCES.txt
--rw-r--r--   0 vadikus    (501) staff       (20)        1 2024-05-12 16:48:58.000000 notolog-0.9.1b4/notolog.egg-info/dependency_links.txt
--rw-r--r--   0 vadikus    (501) staff       (20)       46 2024-05-12 16:48:58.000000 notolog-0.9.1b4/notolog.egg-info/entry_points.txt
--rw-r--r--   0 vadikus    (501) staff       (20)      320 2024-05-12 16:48:58.000000 notolog-0.9.1b4/notolog.egg-info/requires.txt
--rw-r--r--   0 vadikus    (501) staff       (20)       14 2024-05-12 16:48:58.000000 notolog-0.9.1b4/notolog.egg-info/top_level.txt
--rw-r--r--   0 vadikus    (501) staff       (20)      320 2024-05-12 14:50:00.000000 notolog-0.9.1b4/requirements.txt
--rw-r--r--   0 vadikus    (501) staff       (20)       38 2024-05-12 16:48:59.311224 notolog-0.9.1b4/setup.cfg
--rw-r--r--   0 vadikus    (501) staff       (20)     2377 2024-05-12 14:50:00.000000 notolog-0.9.1b4/setup.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.228632 notolog-0.9.1b4/tests/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:31.000000 notolog-0.9.1b4/tests/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5983 2024-05-11 09:19:41.000000 notolog-0.9.1b4/tests/test_enc_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2309 2024-05-11 09:19:41.000000 notolog-0.9.1b4/tests/test_enc_password.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9888 2024-05-11 09:19:41.000000 notolog-0.9.1b4/tests/test_file_header.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3974 2024-05-11 09:19:41.000000 notolog-0.9.1b4/tests/test_html_view.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5814 2024-05-11 09:19:41.000000 notolog-0.9.1b4/tests/test_lexemes.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5839 2024-05-11 09:19:41.000000 notolog-0.9.1b4/tests/test_notolog_editor.py
--rw-r--r--   0 vadikus    (501) staff       (20)      903 2024-05-12 14:50:00.000000 notolog-0.9.1b4/tests/test_pkg_integration.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3948 2024-05-12 16:42:21.000000 notolog-0.9.1b4/tests/test_qt_async.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2919 2024-05-12 16:16:12.000000 notolog-0.9.1b4/tests/test_qt_ui.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1178 2024-05-11 09:19:41.000000 notolog-0.9.1b4/tests/test_settings.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4975 2024-05-11 09:19:41.000000 notolog-0.9.1b4/tests/test_text_block_data.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4484 2024-05-11 09:19:41.000000 notolog-0.9.1b4/tests/test_theme_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6226 2024-05-11 09:19:41.000000 notolog-0.9.1b4/tests/test_themes.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.931540 notolog-0.9.1b6/
+-rw-r--r--   0 vadikus    (501) staff       (20)     9022 2024-05-19 18:30:10.000000 notolog-0.9.1b6/CHANGELOG.md
+-rw-r--r--   0 vadikus    (501) staff       (20)     3490 2024-05-11 12:17:28.000000 notolog-0.9.1b6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 vadikus    (501) staff       (20)     1073 2024-05-04 21:27:31.000000 notolog-0.9.1b6/LICENSE
+-rw-r--r--   0 vadikus    (501) staff       (20)      433 2024-05-11 12:17:28.000000 notolog-0.9.1b6/MANIFEST.in
+-rw-r--r--   0 vadikus    (501) staff       (20)    20127 2024-05-19 22:39:55.930500 notolog-0.9.1b6/PKG-INFO
+-rw-r--r--   0 vadikus    (501) staff       (20)    18001 2024-05-19 22:31:49.000000 notolog-0.9.1b6/README.md
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.502797 notolog-0.9.1b6/docs/
+-rw-r--r--   0 vadikus    (501) staff       (20)     8633 2024-05-19 18:30:10.000000 notolog-0.9.1b6/docs/Examples.md
+-rw-r--r--   0 vadikus    (501) staff       (20)   241693 2024-05-19 18:30:10.000000 notolog-0.9.1b6/docs/notolog-ui-settings-strawberry-ja.png
+-rw-r--r--   0 vadikus    (501) staff       (20)   247033 2024-05-04 21:27:32.000000 notolog-0.9.1b6/docs/notolog-ui-settings.png
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.554797 notolog-0.9.1b6/notolog/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8264 2024-05-19 22:39:28.000000 notolog-0.9.1b6/notolog/app_config.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.563407 notolog-0.9.1b6/notolog/assets/
+-rw-r--r--   0 vadikus    (501) staff       (20)     4202 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/notolog-example-image.png
+-rw-r--r--   0 vadikus    (501) staff       (20)    88211 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/notolog-logo.png
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.476812 notolog-0.9.1b6/notolog/assets/themes/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.577156 notolog-0.9.1b6/notolog/assets/themes/calligraphy/
+-rw-r--r--   0 vadikus    (501) staff       (20)      777 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/calligraphy/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      365 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/calligraphy/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2767 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/calligraphy/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)       56 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/calligraphy/editor.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2311 2024-05-11 12:17:28.000000 notolog-0.9.1b6/notolog/assets/themes/calligraphy/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      885 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/calligraphy/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/calligraphy/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     6818 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/calligraphy/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/calligraphy/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      743 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/calligraphy/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/calligraphy/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       80 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/calligraphy/viewer.ini
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.602894 notolog-0.9.1b6/notolog/assets/themes/default/
+-rw-r--r--   0 vadikus    (501) staff       (20)      798 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      253 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2775 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      174 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/editor.css
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.683410 notolog-0.9.1b6/notolog/assets/themes/default/icons/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1093 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/LICENSE
+-rw-r--r--   0 vadikus    (501) staff       (20)      349 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/arrow-clockwise.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      567 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/arrow-repeat.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      736 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/balloon-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      797 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/balloon.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      812 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/bandaid-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      959 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/bandaid.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      528 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/box-arrow-up-right.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      538 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/box-arrow-up.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      265 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/caret-down-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      265 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/caret-up-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/code-slash.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      694 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/cursor-text.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      459 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/eyedropper.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      403 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/eyeglasses.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      479 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/file-earmark-lock2.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      394 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/file-earmark-plus-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      481 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/file-earmark-x.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      294 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/file-earmark.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      547 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/filetype-html.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      705 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/filetype-md.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      524 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/filetype-txt.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      401 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/floppy2-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      606 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/floppy2.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      428 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/folder-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      708 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/folder-symlink.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      527 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/folder.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      708 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/github.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      518 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/link-45deg.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      666 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/linkedin.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      575 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/pencil-square.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      261 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/power.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      582 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/quote.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      996 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/robot.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      316 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/share-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      653 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/shield-lock-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)     1057 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/shield-lock.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      399 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/star-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      623 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/star.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      272 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/three-dots.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      577 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/trash3-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      656 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/trash3.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      301 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/twitter-x.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      465 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/type-bold.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      351 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/type-italic.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      574 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/type-strikethrough.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      319 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/type-underline.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      351 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/x-circle-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      397 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/x-square-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      491 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/icons/x-square.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)     2363 2024-05-11 12:17:28.000000 notolog-0.9.1b6/notolog/assets/themes/default/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      721 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     8472 2024-05-11 12:17:28.000000 notolog-0.9.1b6/notolog/assets/themes/default/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      744 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       82 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/default/viewer.ini
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.705578 notolog-0.9.1b6/notolog/assets/themes/noir_dark/
+-rw-r--r--   0 vadikus    (501) staff       (20)      777 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/noir_dark/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      347 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/noir_dark/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2745 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/noir_dark/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)       56 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/noir_dark/editor.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2480 2024-05-11 12:17:28.000000 notolog-0.9.1b6/notolog/assets/themes/noir_dark/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)     1435 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/noir_dark/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/noir_dark/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     6935 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/noir_dark/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      280 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/noir_dark/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      711 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/noir_dark/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/noir_dark/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       76 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/noir_dark/viewer.ini
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.716326 notolog-0.9.1b6/notolog/assets/themes/strawberry/
+-rw-r--r--   0 vadikus    (501) staff       (20)      790 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/strawberry/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      317 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/strawberry/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2775 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/strawberry/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)       50 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/strawberry/editor.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2408 2024-05-11 12:17:28.000000 notolog-0.9.1b6/notolog/assets/themes/strawberry/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      753 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/strawberry/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/strawberry/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     8451 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/strawberry/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/strawberry/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      764 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/strawberry/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       60 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/strawberry/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       84 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/assets/themes/strawberry/viewer.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)     3774 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/async_highlighter.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7959 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/edit_widget.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4247 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/editor_state.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.725046 notolog-0.9.1b6/notolog/encrypt/
+-rw-r--r--   0 vadikus    (501) staff       (20)      152 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/encrypt/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4345 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/encrypt/enc_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5603 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/encrypt/enc_new_password_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      626 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/encrypt/enc_password.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3686 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/encrypt/enc_password_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3215 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/encrypt/enc_password_reset_dialog.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.730318 notolog-0.9.1b6/notolog/enums/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/enums/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1433 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/enums/ai_model_names.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5624 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/enums/colors.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1125 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/enums/enum_base.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1367 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/enums/languages.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      451 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/enums/themes.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4500 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/etree_extension.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.731706 notolog-0.9.1b6/notolog/exceptions/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/exceptions/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)       52 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/exceptions/file_header_empty_exception.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7563 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/file_header.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2860 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/file_system_watcher.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.737113 notolog-0.9.1b6/notolog/helpers/
+-rw-r--r--   0 vadikus    (501) staff       (20)       36 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/helpers/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      187 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/helpers/clipboard_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4221 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/helpers/file_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3338 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/helpers/settings_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5644 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/helpers/theme_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1036 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/helpers/tooltip_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7536 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/helpers/update_helper.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.741677 notolog-0.9.1b6/notolog/highlight/
+-rw-r--r--   0 vadikus    (501) staff       (20)      126 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/highlight/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9219 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/highlight/main_highlighter.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    51824 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/highlight/md_highlighter.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8475 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/highlight/view_highlighter.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    10886 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/image_downloader.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.743100 notolog-0.9.1b6/notolog/lexemes/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/__init__.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.751232 notolog-0.9.1b6/notolog/lexemes/de/
+-rw-r--r--   0 vadikus    (501) staff       (20)      830 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/de/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7202 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/de/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6586 2024-05-11 12:17:28.000000 notolog-0.9.1b6/notolog/lexemes/de/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2267 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/de/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3788 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/de/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1225 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/de/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2757 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/de/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.760936 notolog-0.9.1b6/notolog/lexemes/en/
+-rw-r--r--   0 vadikus    (501) staff       (20)      827 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/en/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7096 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/en/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6051 2024-05-11 12:17:28.000000 notolog-0.9.1b6/notolog/lexemes/en/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2181 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/en/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3586 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/en/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1201 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/en/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2573 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/en/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.768715 notolog-0.9.1b6/notolog/lexemes/es/
+-rw-r--r--   0 vadikus    (501) staff       (20)      882 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/es/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7309 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/es/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6560 2024-05-11 12:17:28.000000 notolog-0.9.1b6/notolog/lexemes/es/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2316 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/es/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3890 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/es/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1222 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/es/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2793 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/es/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.777367 notolog-0.9.1b6/notolog/lexemes/fi/
+-rw-r--r--   0 vadikus    (501) staff       (20)      856 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/fi/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7559 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/fi/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6292 2024-05-11 12:17:28.000000 notolog-0.9.1b6/notolog/lexemes/fi/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2261 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/fi/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3759 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/fi/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1334 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/fi/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2662 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/fi/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.783288 notolog-0.9.1b6/notolog/lexemes/fr/
+-rw-r--r--   0 vadikus    (501) staff       (20)      886 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/fr/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7247 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/fr/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6716 2024-05-11 12:17:28.000000 notolog-0.9.1b6/notolog/lexemes/fr/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2344 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/fr/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3978 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/fr/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1236 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/fr/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2824 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/fr/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.789188 notolog-0.9.1b6/notolog/lexemes/ge/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1323 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/ge/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    10627 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/ge/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9735 2024-05-11 12:17:28.000000 notolog-0.9.1b6/notolog/lexemes/ge/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3459 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/ge/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5742 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/ge/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1583 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/ge/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4107 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/ge/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.794451 notolog-0.9.1b6/notolog/lexemes/gr/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1100 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/gr/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8990 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/gr/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8668 2024-05-11 12:17:28.000000 notolog-0.9.1b6/notolog/lexemes/gr/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2907 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/gr/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5016 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/gr/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1561 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/gr/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3679 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/gr/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.802359 notolog-0.9.1b6/notolog/lexemes/in/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1208 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/in/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9434 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/in/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    10078 2024-05-11 12:17:28.000000 notolog-0.9.1b6/notolog/lexemes/in/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3124 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/in/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5546 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/in/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1549 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/in/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3828 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/in/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.813748 notolog-0.9.1b6/notolog/lexemes/it/
+-rw-r--r--   0 vadikus    (501) staff       (20)      864 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/it/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7263 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/it/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6366 2024-05-11 12:17:28.000000 notolog-0.9.1b6/notolog/lexemes/it/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2302 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/it/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3825 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/it/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1238 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/it/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2780 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/it/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.821746 notolog-0.9.1b6/notolog/lexemes/ja/
+-rw-r--r--   0 vadikus    (501) staff       (20)      931 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/ja/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8464 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/ja/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7248 2024-05-11 12:17:28.000000 notolog-0.9.1b6/notolog/lexemes/ja/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2443 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/ja/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4014 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/ja/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1242 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/ja/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3000 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/ja/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.827500 notolog-0.9.1b6/notolog/lexemes/ko/
+-rw-r--r--   0 vadikus    (501) staff       (20)      848 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/ko/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7597 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/ko/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6775 2024-05-11 12:17:28.000000 notolog-0.9.1b6/notolog/lexemes/ko/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2268 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/ko/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3697 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/ko/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1221 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/ko/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2666 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/ko/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.833711 notolog-0.9.1b6/notolog/lexemes/la/
+-rw-r--r--   0 vadikus    (501) staff       (20)      842 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/la/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7538 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/la/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6245 2024-05-11 12:17:28.000000 notolog-0.9.1b6/notolog/lexemes/la/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2297 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/la/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3753 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/la/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1257 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/la/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2736 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/la/toolbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3842 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/lexemes/lexemes.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.844406 notolog-0.9.1b6/notolog/lexemes/nl/
+-rw-r--r--   0 vadikus    (501) staff       (20)      840 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/nl/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7094 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/nl/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6475 2024-05-11 12:17:28.000000 notolog-0.9.1b6/notolog/lexemes/nl/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2229 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/nl/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3673 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/nl/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1220 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/nl/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2647 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/nl/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.856724 notolog-0.9.1b6/notolog/lexemes/pt/
+-rw-r--r--   0 vadikus    (501) staff       (20)      898 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/pt/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7304 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/pt/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6357 2024-05-11 12:17:28.000000 notolog-0.9.1b6/notolog/lexemes/pt/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2326 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/pt/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3830 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/pt/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1223 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/pt/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2830 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/pt/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.865382 notolog-0.9.1b6/notolog/lexemes/ru/
+-rw-r--r--   0 vadikus    (501) staff       (20)      997 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/ru/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9135 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/ru/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7938 2024-05-11 12:17:28.000000 notolog-0.9.1b6/notolog/lexemes/ru/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2883 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/ru/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4896 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/ru/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1428 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/ru/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3453 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/ru/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.875388 notolog-0.9.1b6/notolog/lexemes/se/
+-rw-r--r--   0 vadikus    (501) staff       (20)      835 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/se/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7048 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/se/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6253 2024-05-11 12:17:28.000000 notolog-0.9.1b6/notolog/lexemes/se/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2216 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/se/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3627 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/se/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1220 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/se/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2611 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/se/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.880707 notolog-0.9.1b6/notolog/lexemes/tr/
+-rw-r--r--   0 vadikus    (501) staff       (20)      809 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/tr/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7401 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/tr/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6154 2024-05-11 12:17:28.000000 notolog-0.9.1b6/notolog/lexemes/tr/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2276 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/tr/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3733 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/tr/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1240 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/tr/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2735 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/tr/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.887034 notolog-0.9.1b6/notolog/lexemes/zh/
+-rw-r--r--   0 vadikus    (501) staff       (20)      792 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/zh/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7074 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/zh/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5777 2024-05-11 12:17:28.000000 notolog-0.9.1b6/notolog/lexemes/zh/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2175 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/zh/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3476 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/zh/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1202 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/zh/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2559 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/lexemes/zh/toolbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3290 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/main.py
+-rw-r--r--   0 vadikus    (501) staff       (20)   175254 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/notolog_editor.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7318 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/settings.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3481 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/text_block_data.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5977 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/theme.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.903329 notolog-0.9.1b6/notolog/ui/
+-rw-r--r--   0 vadikus    (501) staff       (20)      152 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/ui/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8248 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/ui/about_popup.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    17345 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/ui/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2103 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/ui/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3551 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/ui/common_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1306 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/ui/enum_combo_box.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5615 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/ui/file_system_model.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7001 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/ui/line_numbers.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2614 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/ui/rename_file_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1229 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/ui/rotating_label.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    37315 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/ui/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3248 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/ui/sort_filter_proxy_model.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6844 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/ui/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    12808 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/ui/toolbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-05-11 09:19:41.000000 notolog-0.9.1b6/notolog/ui/vertical_line_spacer.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8195 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/view_decorator.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    16117 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/view_processor.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2452 2024-05-19 18:30:10.000000 notolog-0.9.1b6/notolog/view_widget.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.929125 notolog-0.9.1b6/notolog.egg-info/
+-rw-r--r--   0 vadikus    (501) staff       (20)    20127 2024-05-19 22:39:55.000000 notolog-0.9.1b6/notolog.egg-info/PKG-INFO
+-rw-r--r--   0 vadikus    (501) staff       (20)    11632 2024-05-19 22:39:55.000000 notolog-0.9.1b6/notolog.egg-info/SOURCES.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)        1 2024-05-19 22:39:55.000000 notolog-0.9.1b6/notolog.egg-info/dependency_links.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)       46 2024-05-19 22:39:55.000000 notolog-0.9.1b6/notolog.egg-info/entry_points.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)      335 2024-05-19 22:39:55.000000 notolog-0.9.1b6/notolog.egg-info/requires.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)       14 2024-05-19 22:39:55.000000 notolog-0.9.1b6/notolog.egg-info/top_level.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)      335 2024-05-19 18:30:10.000000 notolog-0.9.1b6/requirements.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)       38 2024-05-19 22:39:55.931893 notolog-0.9.1b6/setup.cfg
+-rw-r--r--   0 vadikus    (501) staff       (20)     2384 2024-05-19 22:39:28.000000 notolog-0.9.1b6/setup.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.925176 notolog-0.9.1b6/tests/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1245 2024-05-19 18:30:10.000000 notolog-0.9.1b6/tests/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6151 2024-05-19 18:30:10.000000 notolog-0.9.1b6/tests/test_enc_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2309 2024-05-11 09:19:41.000000 notolog-0.9.1b6/tests/test_enc_password.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9948 2024-05-19 18:30:10.000000 notolog-0.9.1b6/tests/test_file_header.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3983 2024-05-19 18:30:10.000000 notolog-0.9.1b6/tests/test_html_view.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5814 2024-05-11 09:19:41.000000 notolog-0.9.1b6/tests/test_lexemes.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5857 2024-05-19 18:30:10.000000 notolog-0.9.1b6/tests/test_notolog_editor.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      903 2024-05-12 14:50:00.000000 notolog-0.9.1b6/tests/test_pkg_integration.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2203 2024-05-19 18:30:10.000000 notolog-0.9.1b6/tests/test_qt_async.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1959 2024-05-19 18:30:10.000000 notolog-0.9.1b6/tests/test_settings.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4975 2024-05-11 09:19:41.000000 notolog-0.9.1b6/tests/test_text_block_data.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4461 2024-05-19 18:30:10.000000 notolog-0.9.1b6/tests/test_theme_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6412 2024-05-19 18:30:10.000000 notolog-0.9.1b6/tests/test_themes.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-19 22:39:55.928141 notolog-0.9.1b6/tests/ui_tests/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1226 2024-05-19 18:30:10.000000 notolog-0.9.1b6/tests/ui_tests/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2544 2024-05-19 18:30:10.000000 notolog-0.9.1b6/tests/ui_tests/test_ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2325 2024-05-19 18:30:10.000000 notolog-0.9.1b6/tests/ui_tests/test_qt_ui.py
```

### Comparing `notolog-0.9.1b4/CHANGELOG.md` & `notolog-0.9.1b6/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,34 @@
 # Changelog
 All notologable changes to this project will be documented in this file.
 
+## [0.9.1b5] - 2024-05-19
+
+### Added
+- Introduced a GitHub workflow for tests, incorporating Flake8 and pytest coverage reports to maintain high standards of code quality and ensure comprehensive test coverage.
+- Added the app's organization name, app name, and version to facilitate correct settings storage.
+- Added a media directory to the app_config.toml.
+- App settings now support encrypted values to keep sensitive data, like API keys, secure. The encryption key is generated once and stored in the app config file. A Settings helper class was also added.
+- New tomli_w package added to support TOML-file writing.
+
+### Updated
+- Tests updated to support multi-platform execution.
+- Used `os.sep` to ensure correct path separators on each OS and `os.path.normpath()` to normalize path separators.
+- Updated the description and disclaimers text in README.md; added a "Code Quality and Test Coverage" paragraph.
+
+### Changed
+- Changed the approach to not create a resource directory upfront before any file is available to save.
+- Moved async highlighter functionality to a dedicated file.
+- Adjusted links markdown highlighter to allow highlighting web links within lines of markdown blocks, and adjusted the web links regex accordingly.
+- Refined the AppConfig object to implement the singleton pattern, enabling it to automatically generate the app's config file rather than relying on a predefined version.
+
+### Fixed
+- Fixed a potential error in the image downloader when the property is None upon canceling tasks on exiting the app.
+- Updated the resource folder path according to the currently active file.
+
 ## [0.9.1b4] - 2024-05-12
 
 ### Added
 - Introduced the pytest-asyncio package to support testing of asyncio code with pytest, enhancing the robustness and reliability of unit tests.
 - Added the `.gitattributes` file that was previously omitted to ensure consistent Git configurations across various environments.
 
 ### Updated
```

### Comparing `notolog-0.9.1b4/CODE_OF_CONDUCT.md` & `notolog-0.9.1b6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/LICENSE` & `notolog-0.9.1b6/LICENSE`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/PKG-INFO` & `notolog-0.9.1b6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: notolog
-Version: 0.9.1b4
+Version: 0.9.1b6
 Summary: Notolog - Python Markdown Editor
 Home-page: https://github.com/notolog/notolog-editor
 Author: Vadim Bakhrenkov
 License: MIT
 Project-URL: Bug Reports, https://github.com/notolog/notolog-editor/issues
 Project-URL: Source, https://github.com/notolog/notolog-editor/
-Keywords: notolog,python,markdown,editor,ai,text
+Keywords: notolog,python,markdown,editor,ai,text,notes
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
@@ -47,23 +47,24 @@
 Requires-Dist: PySide6_Essentials==6.7.0
 Requires-Dist: pytest==8.2.0
 Requires-Dist: pytest-asyncio==0.23.6
 Requires-Dist: pytest-mock==3.14.0
 Requires-Dist: qasync==0.27.1
 Requires-Dist: shiboken6==6.7.0
 Requires-Dist: tomli==2.0.1
+Requires-Dist: tomli_w==1.0.0
 
-<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-12 13:57:34.333369"}} -->
+<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-19 23:29:34.439703"}} -->
 # Notolog
 
 ![Notolog - Python Markdown Editor](https://raw.githubusercontent.com/notolog/notolog-editor/main/notolog/assets/notolog-example-image.png)
 
 ## Python Markdown Editor
 
-![PyPI - License](https://img.shields.io/pypi/l/notolog)&nbsp;![PyPI - Version](https://img.shields.io/pypi/v/notolog)&nbsp;![PyPI - Python Version](https://img.shields.io/pypi/pyversions/notolog)
+[![PyPI - Version](https://img.shields.io/pypi/v/notolog)](https://pypi.org/project/notolog/) [![GitHub License](https://img.shields.io/github/license/notolog/notolog-editor)](https://github.com/notolog/notolog-editor/blob/master/LICENSE) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/notolog)](https://pypi.org/project/notolog/) [![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/notolog/notolog-editor/tests.yaml)](https://github.com/notolog/notolog-editor/actions/workflows/tests.yaml)
 
 Notolog is an open-source markdown editor developed with Python and PySide6. Born from a personal endeavor to tackle daily programming challenges and deepen Python proficiency, Notolog serves as a proof-of-concept that seamlessly blends simplicity with functionality. It offers an intuitive user experience across various platforms, ensuring users can efficiently manage and edit markdown files with ease.
 
 ---
 
 ![Notolog UI example](https://raw.githubusercontent.com/notolog/notolog-editor/main/docs/notolog-ui-settings.png)
 
@@ -104,19 +105,45 @@
 * AI Assistant UI to get all things you need in one place:
 	* At the moment the OpenAI API is supported with plans to extend support with other providers.
 * Notolog includes specialized highlighting for TODOs. Simply type '@todo something' to mark tasks, enhancing the ability to track and manage future plans efficiently.
 
 There is no classical web engine integration to make overall package more lightweight and to achieve the best possible performance.
 
 
+## Translations
+
+The Notolog Editor supports several language translations out of the box. Here is the list of languages included alongside the default English translation:
+
+* Chinese (Simplified)
+* Dutch
+* Finnish
+* French
+* Georgian
+* German
+* Greek
+* Hindi
+* Italian
+* Japanese
+* Korean
+* Latin
+* Portuguese
+* Russian
+* Spanish
+* Swedish
+* Turkish
+
+Here's an example of what it looks like in the actual UI, featuring the lovely Strawberry theme and Japanese translation:
+
+![Notolog UI translation example](https://raw.githubusercontent.com/notolog/notolog-editor/main/docs/notolog-ui-settings-strawberry-ja.png)
+
 ## Prerequisites
 
 **Python 3.9 or higher installed on your system.**
 
-If you haven't already, download and install Python from the official website [python.org](python.org).
+Ensure Python 3.9 or higher is installed on your system. Visit [python.org](https://python.org) for more details.
 
 Check the version of Python available with this command `python3 -V`.
 
 **pip (Python package installer) should be available.**
 
 You can check if pip is installed by running `pip --version` in your terminal/command prompt.
 
@@ -169,15 +196,15 @@
 ```
 </details>
 
 ### Virtual Environments
 
 The instructions below contain steps of how to set up **venv** virtual environment to run a Python app safely. Starting from Python 3.6 **venv** is a recommended way to create virtual environments. For more information check [Creation of virtual environments](https://docs.python.org/3/library/venv.html). Alternatively, you can execute the Notolog code and set up virtual environment with your favorite Python code editor.
 
-#### MacOS and Linux
+#### Linux and macOS
 
 ##### Set Up Virtual Environment
 1. Open Terminal.
 2. Navigate to your project directory using the cd command.
 3. Create a virtual environment by running `python3 -m venv notolog`. Replace **notolog** with the desired name for your virtual environment.
 
 ##### Activate Virtual Environment:
@@ -259,14 +286,15 @@
 
 - **Bootstrap Icons**: Icons for UI elements. [Project Details](https://icons.getbootstrap.com/), [License Details](https://github.com/twbs/icons/blob/main/LICENSE)
 - **pytest**: Used for unit testing. It provides powerful features like fixtures, assertions, and test parameterization to facilitate writing and running Python tests. [Project Details](https://pytest.org/), [License Details](https://docs.pytest.org/en/8.0.x/license.html)
 - **pytest-mock**: Enhances pytest for unit tests by offering a simple interface to powerful mocking functionalities. [License Details](https://github.com/pytest-dev/pytest-mock/blob/main/LICENSE), [PyPI](https://pypi.org/project/pytest-mock/)
 - **cffi**: Used for interfacing with C code. [License Details](https://github.com/python-cffi/cffi/blob/main/LICENSE), [PyPI](https://pypi.org/project/cffi/)
 - **iniconfig**: For parsing and working with INI configuration files. [License Details](https://github.com/pytest-dev/iniconfig/blob/main/LICENSE), [PyPI](https://pypi.org/project/iniconfig/)
 - **tomli**: A Python library used for parsing TOML configuration files effortlessly. [License Details](https://github.com/hukkin/tomli/blob/master/LICENSE), [PyPI](https://pypi.org/project/tomli/)
+- **tomli_w**: A Python library used for writing TOML configuration files effortlessly. [License Details](https://github.com/hukkin/tomli-w/blob/master/LICENSE), [PyPI](https://pypi.org/project/tomli-w/)
 - **pluggy**: For creating and managing plugin systems in Python applications. [License Details](https://github.com/pytest-dev/pluggy/blob/main/LICENSE), [PyPI](https://pypi.org/project/pluggy/)
 
 #### BSD Licenses
 
 - **Python-Markdown**: Markdown to HTML conversion. [Project Details](https://python-markdown.github.io/), [BSD 3-Clause License](https://github.com/Python-Markdown/markdown/blob/master/LICENSE.md)
 - **Emoji library**: Converts emoji text-code to emojis. [New BSD License](https://github.com/carpedm20/emoji/blob/master/LICENSE.txt), [PyPI](https://pypi.org/project/emoji/)
 - **qasync**: Async support for Python. [BSD 2-Clause "Simplified" License](https://github.com/CabbageDevelopment/qasync/blob/master/LICENSE), [PyPI](https://pypi.org/project/qasync/)
@@ -293,23 +321,49 @@
 
 Please note that while the majority of this project is licensed under the MIT License, certain components may have different licensing terms. Always refer to the documentation of each library for detailed information about its license and terms of use.
 
 ### APIs
 
 #### OpenAI API Disclaimer
 
-**Disclaimer:** This project is independent and neither affiliated with, endorsed by, nor sponsored by OpenAI. Integration of the OpenAI API in this project is provided on an "as is" basis, without any official partnership or endorsement by OpenAI. The creators of this project disclaim all liability for any misuse, harm, or other consequences resulting from the use of the OpenAI API.
+**Disclaimer:** This project is independent and not affiliated with, endorsed by, or sponsored by OpenAI. The integration of the OpenAI API is provided on an "as is" basis, and the creators disclaim all liability for any misuse or consequences resulting from the use of the OpenAI API.
 
-**Usage:** Our project employs the OpenAI API to enhance natural language processing capabilities. Users are required to provide their own OpenAI API keys and should refer to the [OpenAI API reference](https://platform.openai.com/docs/api-reference) for detailed usage guidelines.
+**Usage:** This project uses the OpenAI API to access AI assistant capabilities and enhance natural language processing. Users must provide their own OpenAI API keys and should refer to the [OpenAI API reference](https://platform.openai.com/docs/api-reference) for detailed usage guidelines.
 
-**Responsibility:** Users are responsible for obtaining, configuring, and managing their OpenAI API keys in accordance with OpenAI's terms of service and usage policies.
+**Responsibility:** Users are responsible for obtaining and managing their OpenAI API keys in compliance with OpenAI's terms of service.
 
-**Security:** It is crucial for users to manage their API keys securely, ensuring they are not exposed or shared in public forums.
+**Security:** Users are expected to handle their API keys securely to avoid unauthorized access.
 
 *This section was generated with the assistance of AI to ensure accurate and concise information regarding the use of the OpenAI API.*
 
 ## Security Disclaimer
 
-This application is primarily designed for educational purposes and uses PBKDF2HMAC for key derivation. It employs Fernet, which utilizes AES-128 in CBC mode. The key is initially created at 256 bits but truncated to 128 bits for encryption. The encryption salt and iteration counts are stored unencrypted in the file's header, making this setup suitable for educational and non-critical applications only. As such, while this software provides basic security, it is not intended for high-security needs. Users are encouraged to choose strong passwords to enhance data protection. Distributed under the MIT License, this open-source application requires users to ensure compliance with applicable laws, and the developers disclaim liability for misuse or legal non-compliance.
+This application is designed for educational purposes and offers security features through optional file encryption and protected application settings.
+
+### Optional File Encryption
+
+* **Encryption Details:** The application uses PBKDF2HMAC for key derivation and Fernet for encryption, utilizing AES-128 in CBC mode. Although the key material generated is 256 bits, only the first 128 bits (16 bytes) are used for encryption.
+* **File Headers:** The encryption salt and iteration counts are stored unencrypted in the file's header. This approach is primarily intended for non-critical applications where data exposure has limited risk.
+* **Strong Passwords:** Users are encouraged to use strong passwords to enhance the protection of their encrypted data.
+
+### Protected Application Settings
+
+* **Settings Encryption:** The application may encrypt sensitive data like API keys because these Qt app settings might otherwise be stored as open data. However, the encryption key used is stored on the PC and can be accessed by anyone with physical or user-level access to the computer. This could expose sensitive data to potential unauthorized access.
+
+### General Information
+
+* **Open Source:** This application is open-source and distributed under the MIT License. Users must comply with applicable laws and regulations when using this software.
+* **Liability:** The developers disclaim any liability for misuse or legal non-compliance related to the use of this software.
+
+
+## Code Quality and Test Coverage
+
+To maintain high standards of code quality and ensure comprehensive test coverage, we use several tools:
+
+- **Flake8**: A tool that enforces coding style and checks the quality of Python code by combining PyFlakes, pycodestyle, and McCabe's complexity checker. [MIT License](https://github.com/PyCQA/flake8/blob/main/LICENSE)
+- **coverage**: Measures the effectiveness of tests by showing which parts of your code are being executed and which are not. [Apache License 2.0](https://github.com/nedbat/coveragepy/blob/master/LICENSE.txt)
+- **pytest-cov**: A pytest plugin that provides test coverage reports, extending pytest to measure code coverage alongside running tests. [MIT License](https://github.com/pytest-dev/pytest-cov/blob/master/LICENSE)
+
+These tools help us maintain a clean and reliable codebase by catching potential issues early and documenting where our tests might be lacking.
 
 ---
-This README.md file has been carefully crafted and edited using the Notolog editor itself.
+_This README.md file has been carefully crafted and edited using the Notolog editor itself._
```

### Comparing `notolog-0.9.1b4/README.md` & `notolog-0.9.1b6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-12 13:57:34.333369"}} -->
+<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-19 23:29:34.439703"}} -->
 # Notolog
 
 ![Notolog - Python Markdown Editor](https://raw.githubusercontent.com/notolog/notolog-editor/main/notolog/assets/notolog-example-image.png)
 
 ## Python Markdown Editor
 
-![PyPI - License](https://img.shields.io/pypi/l/notolog)&nbsp;![PyPI - Version](https://img.shields.io/pypi/v/notolog)&nbsp;![PyPI - Python Version](https://img.shields.io/pypi/pyversions/notolog)
+[![PyPI - Version](https://img.shields.io/pypi/v/notolog)](https://pypi.org/project/notolog/) [![GitHub License](https://img.shields.io/github/license/notolog/notolog-editor)](https://github.com/notolog/notolog-editor/blob/master/LICENSE) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/notolog)](https://pypi.org/project/notolog/) [![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/notolog/notolog-editor/tests.yaml)](https://github.com/notolog/notolog-editor/actions/workflows/tests.yaml)
 
 Notolog is an open-source markdown editor developed with Python and PySide6. Born from a personal endeavor to tackle daily programming challenges and deepen Python proficiency, Notolog serves as a proof-of-concept that seamlessly blends simplicity with functionality. It offers an intuitive user experience across various platforms, ensuring users can efficiently manage and edit markdown files with ease.
 
 ---
 
 ![Notolog UI example](https://raw.githubusercontent.com/notolog/notolog-editor/main/docs/notolog-ui-settings.png)
 
@@ -50,19 +50,45 @@
 * AI Assistant UI to get all things you need in one place:
 	* At the moment the OpenAI API is supported with plans to extend support with other providers.
 * Notolog includes specialized highlighting for TODOs. Simply type '@todo something' to mark tasks, enhancing the ability to track and manage future plans efficiently.
 
 There is no classical web engine integration to make overall package more lightweight and to achieve the best possible performance.
 
 
+## Translations
+
+The Notolog Editor supports several language translations out of the box. Here is the list of languages included alongside the default English translation:
+
+* Chinese (Simplified)
+* Dutch
+* Finnish
+* French
+* Georgian
+* German
+* Greek
+* Hindi
+* Italian
+* Japanese
+* Korean
+* Latin
+* Portuguese
+* Russian
+* Spanish
+* Swedish
+* Turkish
+
+Here's an example of what it looks like in the actual UI, featuring the lovely Strawberry theme and Japanese translation:
+
+![Notolog UI translation example](https://raw.githubusercontent.com/notolog/notolog-editor/main/docs/notolog-ui-settings-strawberry-ja.png)
+
 ## Prerequisites
 
 **Python 3.9 or higher installed on your system.**
 
-If you haven't already, download and install Python from the official website [python.org](python.org).
+Ensure Python 3.9 or higher is installed on your system. Visit [python.org](https://python.org) for more details.
 
 Check the version of Python available with this command `python3 -V`.
 
 **pip (Python package installer) should be available.**
 
 You can check if pip is installed by running `pip --version` in your terminal/command prompt.
 
@@ -115,15 +141,15 @@
 ```
 </details>
 
 ### Virtual Environments
 
 The instructions below contain steps of how to set up **venv** virtual environment to run a Python app safely. Starting from Python 3.6 **venv** is a recommended way to create virtual environments. For more information check [Creation of virtual environments](https://docs.python.org/3/library/venv.html). Alternatively, you can execute the Notolog code and set up virtual environment with your favorite Python code editor.
 
-#### MacOS and Linux
+#### Linux and macOS
 
 ##### Set Up Virtual Environment
 1. Open Terminal.
 2. Navigate to your project directory using the cd command.
 3. Create a virtual environment by running `python3 -m venv notolog`. Replace **notolog** with the desired name for your virtual environment.
 
 ##### Activate Virtual Environment:
@@ -205,14 +231,15 @@
 
 - **Bootstrap Icons**: Icons for UI elements. [Project Details](https://icons.getbootstrap.com/), [License Details](https://github.com/twbs/icons/blob/main/LICENSE)
 - **pytest**: Used for unit testing. It provides powerful features like fixtures, assertions, and test parameterization to facilitate writing and running Python tests. [Project Details](https://pytest.org/), [License Details](https://docs.pytest.org/en/8.0.x/license.html)
 - **pytest-mock**: Enhances pytest for unit tests by offering a simple interface to powerful mocking functionalities. [License Details](https://github.com/pytest-dev/pytest-mock/blob/main/LICENSE), [PyPI](https://pypi.org/project/pytest-mock/)
 - **cffi**: Used for interfacing with C code. [License Details](https://github.com/python-cffi/cffi/blob/main/LICENSE), [PyPI](https://pypi.org/project/cffi/)
 - **iniconfig**: For parsing and working with INI configuration files. [License Details](https://github.com/pytest-dev/iniconfig/blob/main/LICENSE), [PyPI](https://pypi.org/project/iniconfig/)
 - **tomli**: A Python library used for parsing TOML configuration files effortlessly. [License Details](https://github.com/hukkin/tomli/blob/master/LICENSE), [PyPI](https://pypi.org/project/tomli/)
+- **tomli_w**: A Python library used for writing TOML configuration files effortlessly. [License Details](https://github.com/hukkin/tomli-w/blob/master/LICENSE), [PyPI](https://pypi.org/project/tomli-w/)
 - **pluggy**: For creating and managing plugin systems in Python applications. [License Details](https://github.com/pytest-dev/pluggy/blob/main/LICENSE), [PyPI](https://pypi.org/project/pluggy/)
 
 #### BSD Licenses
 
 - **Python-Markdown**: Markdown to HTML conversion. [Project Details](https://python-markdown.github.io/), [BSD 3-Clause License](https://github.com/Python-Markdown/markdown/blob/master/LICENSE.md)
 - **Emoji library**: Converts emoji text-code to emojis. [New BSD License](https://github.com/carpedm20/emoji/blob/master/LICENSE.txt), [PyPI](https://pypi.org/project/emoji/)
 - **qasync**: Async support for Python. [BSD 2-Clause "Simplified" License](https://github.com/CabbageDevelopment/qasync/blob/master/LICENSE), [PyPI](https://pypi.org/project/qasync/)
@@ -239,23 +266,49 @@
 
 Please note that while the majority of this project is licensed under the MIT License, certain components may have different licensing terms. Always refer to the documentation of each library for detailed information about its license and terms of use.
 
 ### APIs
 
 #### OpenAI API Disclaimer
 
-**Disclaimer:** This project is independent and neither affiliated with, endorsed by, nor sponsored by OpenAI. Integration of the OpenAI API in this project is provided on an "as is" basis, without any official partnership or endorsement by OpenAI. The creators of this project disclaim all liability for any misuse, harm, or other consequences resulting from the use of the OpenAI API.
+**Disclaimer:** This project is independent and not affiliated with, endorsed by, or sponsored by OpenAI. The integration of the OpenAI API is provided on an "as is" basis, and the creators disclaim all liability for any misuse or consequences resulting from the use of the OpenAI API.
 
-**Usage:** Our project employs the OpenAI API to enhance natural language processing capabilities. Users are required to provide their own OpenAI API keys and should refer to the [OpenAI API reference](https://platform.openai.com/docs/api-reference) for detailed usage guidelines.
+**Usage:** This project uses the OpenAI API to access AI assistant capabilities and enhance natural language processing. Users must provide their own OpenAI API keys and should refer to the [OpenAI API reference](https://platform.openai.com/docs/api-reference) for detailed usage guidelines.
 
-**Responsibility:** Users are responsible for obtaining, configuring, and managing their OpenAI API keys in accordance with OpenAI's terms of service and usage policies.
+**Responsibility:** Users are responsible for obtaining and managing their OpenAI API keys in compliance with OpenAI's terms of service.
 
-**Security:** It is crucial for users to manage their API keys securely, ensuring they are not exposed or shared in public forums.
+**Security:** Users are expected to handle their API keys securely to avoid unauthorized access.
 
 *This section was generated with the assistance of AI to ensure accurate and concise information regarding the use of the OpenAI API.*
 
 ## Security Disclaimer
 
-This application is primarily designed for educational purposes and uses PBKDF2HMAC for key derivation. It employs Fernet, which utilizes AES-128 in CBC mode. The key is initially created at 256 bits but truncated to 128 bits for encryption. The encryption salt and iteration counts are stored unencrypted in the file's header, making this setup suitable for educational and non-critical applications only. As such, while this software provides basic security, it is not intended for high-security needs. Users are encouraged to choose strong passwords to enhance data protection. Distributed under the MIT License, this open-source application requires users to ensure compliance with applicable laws, and the developers disclaim liability for misuse or legal non-compliance.
+This application is designed for educational purposes and offers security features through optional file encryption and protected application settings.
+
+### Optional File Encryption
+
+* **Encryption Details:** The application uses PBKDF2HMAC for key derivation and Fernet for encryption, utilizing AES-128 in CBC mode. Although the key material generated is 256 bits, only the first 128 bits (16 bytes) are used for encryption.
+* **File Headers:** The encryption salt and iteration counts are stored unencrypted in the file's header. This approach is primarily intended for non-critical applications where data exposure has limited risk.
+* **Strong Passwords:** Users are encouraged to use strong passwords to enhance the protection of their encrypted data.
+
+### Protected Application Settings
+
+* **Settings Encryption:** The application may encrypt sensitive data like API keys because these Qt app settings might otherwise be stored as open data. However, the encryption key used is stored on the PC and can be accessed by anyone with physical or user-level access to the computer. This could expose sensitive data to potential unauthorized access.
+
+### General Information
+
+* **Open Source:** This application is open-source and distributed under the MIT License. Users must comply with applicable laws and regulations when using this software.
+* **Liability:** The developers disclaim any liability for misuse or legal non-compliance related to the use of this software.
+
+
+## Code Quality and Test Coverage
+
+To maintain high standards of code quality and ensure comprehensive test coverage, we use several tools:
+
+- **Flake8**: A tool that enforces coding style and checks the quality of Python code by combining PyFlakes, pycodestyle, and McCabe's complexity checker. [MIT License](https://github.com/PyCQA/flake8/blob/main/LICENSE)
+- **coverage**: Measures the effectiveness of tests by showing which parts of your code are being executed and which are not. [Apache License 2.0](https://github.com/nedbat/coveragepy/blob/master/LICENSE.txt)
+- **pytest-cov**: A pytest plugin that provides test coverage reports, extending pytest to measure code coverage alongside running tests. [MIT License](https://github.com/pytest-dev/pytest-cov/blob/master/LICENSE)
+
+These tools help us maintain a clean and reliable codebase by catching potential issues early and documenting where our tests might be lacking.
 
 ---
-This README.md file has been carefully crafted and edited using the Notolog editor itself.
+_This README.md file has been carefully crafted and edited using the Notolog editor itself._
```

### Comparing `notolog-0.9.1b4/docs/Examples.md` & `notolog-0.9.1b6/docs/Examples.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!-- {"notolog.app": {"created": "2024-03-26 00:19:36.466439", "updated": "2024-05-11 12:23:43.657587"}} -->
+<!-- {"notolog.app": {"created": "2024-03-26 00:19:36.466439", "updated": "2024-05-18 12:32:49.515851"}} -->
 # Markdown syntax
 
 ## Headings
 
 Keep space between the `#` sign and the heading itself.
 
 # Header 1
@@ -242,8 +242,8 @@
 	<details>
 		<summary>Nested blocks support</summary>
 	This feature is experimental, and some nested syntax highlighting may not function entirely as expected. Nonetheless, it proves helpful in condensing lengthy content into expandable links. Support for this block will be expanded in the future.
 	</details>
 </details>
 
 ---
-This README.md file has been carefully crafted and edited using the Notolog editor itself.
+_This README.md file has been carefully crafted and edited using the Notolog editor itself._
```

### Comparing `notolog-0.9.1b4/docs/notolog-ui-settings.png` & `notolog-0.9.1b6/docs/notolog-ui-settings.png`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/notolog-example-image.png` & `notolog-0.9.1b6/notolog/assets/notolog-example-image.png`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/notolog-logo.png` & `notolog-0.9.1b6/notolog/assets/notolog-logo.png`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/calligraphy/about_popup.css` & `notolog-0.9.1b6/notolog/assets/themes/calligraphy/about_popup.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/calligraphy/default.ini` & `notolog-0.9.1b6/notolog/assets/themes/calligraphy/default.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/calligraphy/md.ini` & `notolog-0.9.1b6/notolog/assets/themes/calligraphy/md.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/calligraphy/settings_dialog.css` & `notolog-0.9.1b6/notolog/assets/themes/calligraphy/settings_dialog.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/calligraphy/styles.css` & `notolog-0.9.1b6/notolog/assets/themes/calligraphy/styles.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/calligraphy/tree_view.css` & `notolog-0.9.1b6/notolog/assets/themes/calligraphy/tree_view.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/default/about_popup.css` & `notolog-0.9.1b6/notolog/assets/themes/default/about_popup.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/default/default.ini` & `notolog-0.9.1b6/notolog/assets/themes/default/default.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/default/icons/LICENSE` & `notolog-0.9.1b6/notolog/assets/themes/default/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/default/icons/arrow-repeat.svg` & `notolog-0.9.1b6/notolog/assets/themes/default/icons/arrow-repeat.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/default/icons/balloon-fill.svg` & `notolog-0.9.1b6/notolog/assets/themes/default/icons/balloon-fill.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/default/icons/balloon.svg` & `notolog-0.9.1b6/notolog/assets/themes/default/icons/balloon.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/default/icons/bandaid-fill.svg` & `notolog-0.9.1b6/notolog/assets/themes/default/icons/bandaid-fill.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/default/icons/bandaid.svg` & `notolog-0.9.1b6/notolog/assets/themes/default/icons/bandaid.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/default/icons/box-arrow-up-right.svg` & `notolog-0.9.1b6/notolog/assets/themes/default/icons/box-arrow-up-right.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/default/icons/box-arrow-up.svg` & `notolog-0.9.1b6/notolog/assets/themes/default/icons/box-arrow-up.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/default/icons/cursor-text.svg` & `notolog-0.9.1b6/notolog/assets/themes/default/icons/cursor-text.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/default/icons/filetype-html.svg` & `notolog-0.9.1b6/notolog/assets/themes/default/icons/filetype-html.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/default/icons/filetype-md.svg` & `notolog-0.9.1b6/notolog/assets/themes/default/icons/filetype-md.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/default/icons/filetype-txt.svg` & `notolog-0.9.1b6/notolog/assets/themes/default/icons/filetype-txt.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/default/icons/floppy2.svg` & `notolog-0.9.1b6/notolog/assets/themes/default/icons/floppy2.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/default/icons/folder-symlink.svg` & `notolog-0.9.1b6/notolog/assets/themes/default/icons/folder-symlink.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/default/icons/folder.svg` & `notolog-0.9.1b6/notolog/assets/themes/default/icons/folder.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/default/icons/github.svg` & `notolog-0.9.1b6/notolog/assets/themes/default/icons/github.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/default/icons/link-45deg.svg` & `notolog-0.9.1b6/notolog/assets/themes/default/icons/link-45deg.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/default/icons/linkedin.svg` & `notolog-0.9.1b6/notolog/assets/themes/default/icons/linkedin.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/default/icons/pencil-square.svg` & `notolog-0.9.1b6/notolog/assets/themes/default/icons/pencil-square.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/default/icons/quote.svg` & `notolog-0.9.1b6/notolog/assets/themes/default/icons/quote.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/default/icons/robot.svg` & `notolog-0.9.1b6/notolog/assets/themes/default/icons/robot.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/default/icons/shield-lock-fill.svg` & `notolog-0.9.1b6/notolog/assets/themes/default/icons/shield-lock-fill.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/default/icons/shield-lock.svg` & `notolog-0.9.1b6/notolog/assets/themes/default/icons/shield-lock.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/default/icons/star.svg` & `notolog-0.9.1b6/notolog/assets/themes/default/icons/star.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/default/icons/trash3-fill.svg` & `notolog-0.9.1b6/notolog/assets/themes/default/icons/trash3-fill.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/default/icons/trash3.svg` & `notolog-0.9.1b6/notolog/assets/themes/default/icons/trash3.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/default/icons/type-strikethrough.svg` & `notolog-0.9.1b6/notolog/assets/themes/default/icons/type-strikethrough.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/default/md.ini` & `notolog-0.9.1b6/notolog/assets/themes/default/md.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/default/settings_dialog.css` & `notolog-0.9.1b6/notolog/assets/themes/default/settings_dialog.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/default/styles.css` & `notolog-0.9.1b6/notolog/assets/themes/default/styles.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/default/tree_view.css` & `notolog-0.9.1b6/notolog/assets/themes/default/tree_view.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/noir_dark/about_popup.css` & `notolog-0.9.1b6/notolog/assets/themes/noir_dark/about_popup.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/noir_dark/default.ini` & `notolog-0.9.1b6/notolog/assets/themes/noir_dark/default.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/noir_dark/md.ini` & `notolog-0.9.1b6/notolog/assets/themes/noir_dark/md.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/noir_dark/settings_dialog.css` & `notolog-0.9.1b6/notolog/assets/themes/noir_dark/settings_dialog.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/noir_dark/styles.css` & `notolog-0.9.1b6/notolog/assets/themes/noir_dark/styles.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/noir_dark/tree_view.css` & `notolog-0.9.1b6/notolog/assets/themes/noir_dark/tree_view.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/strawberry/about_popup.css` & `notolog-0.9.1b6/notolog/assets/themes/strawberry/about_popup.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/strawberry/default.ini` & `notolog-0.9.1b6/notolog/assets/themes/strawberry/default.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/strawberry/md.ini` & `notolog-0.9.1b6/notolog/assets/themes/strawberry/md.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/strawberry/settings_dialog.css` & `notolog-0.9.1b6/notolog/assets/themes/strawberry/settings_dialog.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/strawberry/styles.css` & `notolog-0.9.1b6/notolog/assets/themes/strawberry/styles.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/assets/themes/strawberry/tree_view.css` & `notolog-0.9.1b6/notolog/assets/themes/strawberry/tree_view.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/edit_widget.py` & `notolog-0.9.1b6/notolog/edit_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from PySide6.QtCore import Qt, Signal
-from PySide6.QtGui import QTextCursor, QTextBlockUserData, QTextBlock, QFont
+from PySide6.QtGui import QTextCursor, QTextBlock, QFont
 from PySide6.QtWidgets import QPlainTextEdit
 
-from typing import Union
+from typing import TYPE_CHECKING, Union
 
 from .app_config import AppConfig
-from .text_block_data import TextBlockData
 
 import logging
 
+if TYPE_CHECKING:
+    from PySide6.QtGui import QTextBlockUserData  # noqa
+    from .text_block_data import TextBlockData  # noqa
+
 
 class EditWidget(QPlainTextEdit):
     # Class to extend or to modify of the original QPlainTextEdit
 
     content_set = Signal()
 
     def __init__(self, parent=None):
@@ -20,20 +23,21 @@
         Args:
             parent (optional): Parent object
         """
         super(EditWidget, self).__init__(parent)
 
         # Get app's global font size
         font = QFont()
-        font.setPointSize(AppConfig.get_font_size())
+        font.setPointSize(AppConfig().get_font_size())
         self.setFont(font)
 
         self.logger = logging.getLogger('edit_widget')
 
-        self.debug = AppConfig.get_debug()
+        self.logging = AppConfig().get_logging()
+        self.debug = AppConfig().get_debug()
 
     def setDocument(self, document):
         # Override setDocument() to allow additional actions like emit the document set signal
         super().setDocument(document)
         # Emit document set signal to notify listeners
         self.content_set.emit()
```

### Comparing `notolog-0.9.1b4/notolog/editor_state.py` & `notolog-0.9.1b6/notolog/editor_state.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,16 @@
 
 class EditorState(QObject):
     value_changed = Signal(object)
 
     def __init__(self, parent=None):
         super(EditorState, self).__init__(parent)
 
-        self.debug = AppConfig.get_debug()
+        self.logging = AppConfig().get_logging()
+        self.debug = AppConfig().get_debug()
 
         self.logger = logging.getLogger('editor_state')
 
         self._mode = None
         self._source = None
         self._encryption = None
```

### Comparing `notolog-0.9.1b4/notolog/encrypt/enc_helper.py` & `notolog-0.9.1b6/notolog/encrypt/enc_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     Remember to re-encrypt the source.
     """
     DEFAULT_ITERATIONS = 768000
 
     def __init__(self, enc_password: EncPassword = None, salt: str = None, iterations: int = None):
         super().__init__()
 
-        self.logging = AppConfig.get_logging()
-        self.debug = AppConfig.get_debug()
+        self.logging = AppConfig().get_logging()
+        self.debug = AppConfig().get_debug()
 
         self.logger = logging.getLogger('enc_helper')
 
         self.enc_password = enc_password
         self.salt = salt
         self.iterations = iterations
```

### Comparing `notolog-0.9.1b4/notolog/encrypt/enc_new_password_dialog.py` & `notolog-0.9.1b6/notolog/encrypt/enc_new_password_dialog.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,16 +23,16 @@
             # Apply font from the main window to the dialog
             self.setFont(self.parent.font())
 
         self.settings = Settings(parent=self)
 
         self.logger = logging.getLogger('enc_new_password_dialog')
 
-        self.logging = AppConfig.get_logging()
-        self.debug = AppConfig.get_debug()
+        self.logging = AppConfig().get_logging()
+        self.debug = AppConfig().get_debug()
 
         # Default language setup, change to settings value to modify it via UI
         self.lexemes = Lexemes(self.settings.app_language, default_scope='common')
 
         self.theme_helper = ThemeHelper()
 
         title = self.lexemes.get('dialog_encrypt_new_password_title')
@@ -127,23 +127,7 @@
         self.setMinimumWidth(title_width + 150)  # Add some padding
 
     def set_font_size(self, widget, percent):
         default_font_size = self.font().pointSizeF()
         font = widget.font()
         font.setPointSizeF(default_font_size * (percent / 100))
         widget.setFont(font)
-
-    """
-    Example of class standalone usage:
-    def dialog_show():
-        dialog = EncNewPasswordDialog()
-        if dialog.exec() == QDialog.DialogCode.Accepted:
-            return dialog.password_edit.text(), dialog.hint_edit.text()
-        return None, None
-
-    if __name__ == "__main__":
-        app = QApplication(sys.argv)
-        password, hint = dialog_show()
-        print("Password:", password)
-        print("Hint:", hint)
-        sys.exit(app.exec())
-    """
```

### Comparing `notolog-0.9.1b4/notolog/encrypt/enc_password.py` & `notolog-0.9.1b6/notolog/encrypt/enc_password.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/encrypt/enc_password_dialog.py` & `notolog-0.9.1b6/notolog/encrypt/enc_password_dialog.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from PySide6.QtCore import Qt
-from PySide6.QtWidgets import QDialog, QLabel, QLineEdit, QPushButton, QHBoxLayout, QVBoxLayout, QStyle, QMessageBox
+from PySide6.QtWidgets import QDialog, QLabel, QLineEdit, QPushButton, QHBoxLayout, QVBoxLayout, QStyle
 from PySide6.QtGui import QFontMetrics, QFont
 
 from . import Settings
 from . import AppConfig
 from . import Lexemes
 from . import ThemeHelper
 
@@ -21,16 +21,16 @@
             # Apply font from the main window to the dialog
             self.setFont(self.parent.font())
 
         self.settings = Settings(parent=self)
 
         self.logger = logging.getLogger('enc_password_dialog')
 
-        self.logging = AppConfig.get_logging()
-        self.debug = AppConfig.get_debug()
+        self.logging = AppConfig().get_logging()
+        self.debug = AppConfig().get_debug()
 
         # Default language setup, change to settings value to modify it via UI
         self.lexemes = Lexemes(self.settings.app_language, default_scope='common')
 
         self.theme_helper = ThemeHelper()
 
         title = self.lexemes.get('dialog_encrypt_password_title')
@@ -89,23 +89,7 @@
     def adjust_minimum_width(self, title):
         # Calculate width required for the title text
         font_metrics = QFontMetrics(self.font())
         title_width = font_metrics.horizontalAdvance(title)
 
         # Set minimum width for the dialog
         self.setMinimumWidth(title_width + 150)  # Add some padding
-
-    """
-    Example of class standalone usage:
-    def dialog_show():
-        dialog = EncNewPasswordDialog()
-        if dialog.exec() == QDialog.DialogCode.Accepted:
-            return dialog.password_edit.text(), dialog.hint_edit.text()
-        return None, None
-
-    if __name__ == "__main__":
-        app = QApplication(sys.argv)
-        password, hint = dialog_show()
-        print("Password:", password)
-        print("Hint:", hint)
-        sys.exit(app.exec())
-    """
```

### Comparing `notolog-0.9.1b4/notolog/encrypt/enc_password_reset_dialog.py` & `notolog-0.9.1b6/notolog/encrypt/enc_password_reset_dialog.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,16 +22,16 @@
             # Apply font from the main window to the dialog
             self.setFont(self.parent.font())
 
         self.settings = Settings(parent=self)
 
         self.logger = logging.getLogger('enc_password_reset_dialog')
 
-        self.logging = AppConfig.get_logging()
-        self.debug = AppConfig.get_debug()
+        self.logging = AppConfig().get_logging()
+        self.debug = AppConfig().get_debug()
 
         # Default language setup, change to settings value to modify it via UI
         self.lexemes = Lexemes(self.settings.app_language, default_scope='common')
 
         title = self.lexemes.get('dialog_encrypt_password_reset_title')
         self.setWindowTitle(title)
         self.setObjectName('dialog_encrypt_password_reset_title')
```

### Comparing `notolog-0.9.1b4/notolog/enums/ai_model_names.py` & `notolog-0.9.1b6/notolog/enums/ai_model_names.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/enums/colors.py` & `notolog-0.9.1b6/notolog/enums/colors.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/enums/enum_base.py` & `notolog-0.9.1b6/notolog/enums/enum_base.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/enums/languages.py` & `notolog-0.9.1b6/notolog/enums/languages.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/etree_extension.py` & `notolog-0.9.1b6/notolog/etree_extension.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 class ElementTreeExtension(Extension):
     """
     Custom markdown extension.
     """
 
     logger = logging.getLogger('tree_extension')
 
-    logging = AppConfig.get_logging()
-    debug = AppConfig.get_debug()
+    logging = AppConfig().get_logging()
+    debug = AppConfig().get_debug()
 
     def extendMarkdown(self, md: Markdown) -> None:
         if self.debug:
             self.logger.info('%s extension engaged' % self.__class__.__qualname__)
         # Registering extension
         md.registerExtension(self)
         # noinspection SpellCheckingInspection
@@ -32,16 +32,16 @@
 class ElementTreeProcessor(Treeprocessor):
     """
     Custom markdown extension tree processor.
     """
 
     logger = logging.getLogger('tree_processor')
 
-    logging = AppConfig.get_logging()
-    debug = AppConfig.get_debug()
+    logging = AppConfig().get_logging()
+    debug = AppConfig().get_debug()
 
     def run(self, root):
         # Customize elements tree here
         for idx, elem in enumerate(root.iter()):
             if self.debug:
                 self.logger.debug('Process elements > %d: %s' % (idx, elem.tag))
             # Process <table> elements
@@ -78,20 +78,18 @@
             elem.set('class', '_nl_tbl')
             elem.set('cellpadding', '0')
             elem.set('cellspacing', '0')
 
     def process_table_td(self, elem):
         # Replace 'style' with 'class' as css doesn't work otherwise
         if elem.get('style') and elem.get('style').startswith('text-align'):
-            """
-            re = QRegularExpression(r'^text-align:\s?(.*?);$')
-            match = re.match(elem.get('style'))
-            if match.capturedTexts() and match.captured(1):
-                ...
-            """
+            # re = QRegularExpression(r'^text-align:\s?(.*?);$')
+            # match = re.match(elem.get('style'))
+            # if match.capturedTexts() and match.captured(1):
+            #    ...
             pattern = re.compile(r'^text-align:\s?(.*?);$')
             match = pattern.search(elem.get('style'))
             if match:
                 del elem.attrib['style']
                 elem.set('class', match.group(1))
 
     def process_image(self, elem):
@@ -119,8 +117,8 @@
                 # Remove `a` element
                 elem.remove(c_elem)
                 # Insert `br` element
                 elem.insert(id_xy, br_elem)
                 # Setup class as a flag to determine re-inserted `a` element
                 c_elem.set('class', '_re-inserted')
                 # Re-insert the `a` element with a new class
-                elem.insert(id_xy + 1, c_elem)
+                elem.insert(id_xy + 1, c_elem)
```

### Comparing `notolog-0.9.1b4/notolog/file_header.py` & `notolog-0.9.1b6/notolog/file_header.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     HEADER_TPL = '<!-- %s -->'
 
     def __init__(self):
         super(FileHeader, self).__init__()
 
         self.logger = logging.getLogger('header')
 
-        self.logging = AppConfig.get_logging()
-        self.debug = AppConfig.get_debug()
+        self.logging = AppConfig().get_logging()
+        self.debug = AppConfig().get_debug()
 
         if self.debug:
             self.logger.debug('Header helper is engaged')
 
         self.header = None
 
     def get_new(self, is_enc: bool = False):
```

### Comparing `notolog-0.9.1b4/notolog/file_system_watcher.py` & `notolog-0.9.1b6/notolog/file_system_watcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     def __init__(self):
         if getattr(self, '_initialized', False):
             return
         self._initialized = True
 
         self.logger = logging.getLogger('file_system_watcher')
 
-        self.logging = AppConfig.get_logging()
-        self.debug = AppConfig.get_debug()
+        self.logging = AppConfig().get_logging()
+        self.debug = AppConfig().get_debug()
 
         self.dir = None
 
         self.files = set()
 
         self.watcher = QFileSystemWatcher()
         self.watcher.directoryChanged.connect(self.on_dir_changed)
```

### Comparing `notolog-0.9.1b4/notolog/helpers/file_helper.py` & `notolog-0.9.1b6/notolog/helpers/file_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Helper for file operations.
 """
 
-from PySide6.QtCore import QFile, QDir
+from PySide6.QtCore import QDir
 
 import os
 import sys
 
 from typing import Union
 
 
@@ -119,8 +119,8 @@
         str: The text stripped of any trailing digits, if they exist.
     """
     # Start from the end of the string and find the first non-digit character
     i = len(text)
     while i > 0 and text[i - 1].isdigit():
         i -= 1
     # Return the string up to the first trailing digit
-    return text[:i]
+    return text[:i]
```

### Comparing `notolog-0.9.1b4/notolog/helpers/theme_helper.py` & `notolog-0.9.1b6/notolog/helpers/theme_helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from PySide6.QtGui import QColor, QIcon, QPixmap, QPainter
 
 import os
 import logging
 
 from typing import Union
 
-from ..app_config import AppConfig
+from . import AppConfig
+
 from ..settings import Settings
 from ..theme import Theme
 from ..enums.themes import Themes
 
 
 class ThemeHelper:
     """
@@ -19,14 +20,15 @@
     """
 
     def __init__(self):
         super().__init__()
 
         self.logger = logging.getLogger('theme_helper')
 
+        self.logging = AppConfig().get_logging()
         self.debug = AppConfig().get_debug()
 
         if self.debug:
             self.logger.info('Theme helper is engaged')
 
         self.settings = Settings()
 
@@ -94,14 +96,16 @@
         """
         Get QIcon by params
 
         Args:
             theme_icon (str): Theme icon file name
             system_icon (str, optional): System icon name as a fallback
             color (QColor, optional): Color of the SVG icon
+            width (int, optional): Icon width
+            height (int, optional): Icon height
 
         Returns:
             QIcon: Either from file or from the system theme
         """
         theme_icon_dir = os.path.join(self.theme.get_theme_dir(), 'icons')
         if not os.path.exists(theme_icon_dir):
             # Get default icons then
```

### Comparing `notolog-0.9.1b4/notolog/helpers/tooltip_helper.py` & `notolog-0.9.1b6/notolog/helpers/tooltip_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/helpers/update_helper.py` & `notolog-0.9.1b6/notolog/helpers/update_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,24 @@
-from PySide6.QtCore import QObject, Signal, Slot, QUrl, QByteArray
+from PySide6.QtCore import QObject, Signal, Slot, QUrl
 from PySide6.QtNetwork import QNetworkAccessManager, QNetworkRequest, QNetworkReply, QSslSocket
 
 from packaging import version
+from typing import TYPE_CHECKING
 
 import json
 import logging
 
+from . import AppConfig
+
 from ..settings import Settings
-from ..app_config import AppConfig
 from ..lexemes.lexemes import Lexemes
 
+if TYPE_CHECKING:
+    from PySide6.QtCore import QByteArray  # noqa
+
 
 class UpdateHelper(QObject):
     """
     # How to use example:
     update_helper = UpdateHelper()
     update_helper.new_version_available.connect(lambda v:
                                                 QMessageBox.information(None, "Update Available",
@@ -30,24 +35,24 @@
     def __init__(self):
         super().__init__()
 
         self.settings = Settings(parent=self)
 
         self.logger = logging.getLogger('update_helper')
 
-        self.logging = AppConfig.get_logging()
-        self.debug = AppConfig.get_debug()
+        self.logging = AppConfig().get_logging()
+        self.debug = AppConfig().get_debug()
 
         if self.logging:
             self.logger.info("SSL supported: %s" % QSslSocket.supportsSsl())
 
         # Default language setup, change to settings value to modify it via UI
         self.lexemes = Lexemes(self.settings.app_language, default_scope='common')
 
-        self.current_version = version.parse(AppConfig.get_app_version())
+        self.current_version = version.parse(AppConfig().get_app_version())
 
         self.manager = QNetworkAccessManager(self)
 
     def check_for_updates(self):
         # Updates url
         release_url = AppConfig.get_repository_github_release_url()
         request = QNetworkRequest(QUrl(release_url))
@@ -106,15 +111,16 @@
                 if self.debug:
                     self.logger.debug(f"Result JSON: {json_data}")
 
                 latest_version_str = json_data['tag_name']
                 latest_version = version.parse(latest_version_str)
 
                 if latest_version > self.current_version:
-                    update_link = '<a href="%s">%s</a>' % (AppConfig.get_repository_github_release_url(), latest_version)
+                    update_link = ('<a href="%s">%s</a>'
+                                   % (AppConfig().get_repository_github_release_url(), latest_version))
                     result_message = self.lexemes.get('update_helper_new_version_is_available',
                                                       latest_version=update_link)
                     if self.logging:
                         self.logger.info("New version of the app is available: %s. Current version is %s. Response: %s}"
                                          % (latest_version, self.current_version, reply.errorString()))
                     # Emit the new version signal
                     self.new_version_check_response.emit(
```

### Comparing `notolog-0.9.1b4/notolog/highlight/main_highlighter.py` & `notolog-0.9.1b6/notolog/highlight/main_highlighter.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,19 +48,19 @@
     re_rules = []
 
     def __init__(self, document: QTextDocument = None):
         super().__init__(document)
 
         self.logger = logging.getLogger('highlighter')
 
-        self.logging = AppConfig.get_logging()
-        self.debug = False  # AppConfig.get_debug()
+        self.logging = AppConfig().get_logging()
+        self.debug = False  # AppConfig().get_debug()
 
         # Get app's global font size
-        self.font_size = AppConfig.get_font_size()
+        self.font_size = AppConfig().get_font_size()
 
         # Walk rules to create QRegExp for each pattern
         self.rules = [(self.get_regex(pattern), nth, tag, group, duple, fmt, reckon)
                       for (pattern, nth, tag, group, duple, fmt, reckon) in self.re_rules]
 
         # Collect found tokens
         self.tokens = {}
```

### Comparing `notolog-0.9.1b4/notolog/highlight/md_highlighter.py` & `notolog-0.9.1b6/notolog/highlight/md_highlighter.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,26 +198,24 @@
         (r'(!\[[^\]]*?\]\[[^\]]*?\])', 1, 'img', 'img', False, theme['img'], None),
         # reference either image or link, footnotes also
         (r'((?<!\*)\[[^\]]*?\]:)', 1, 'ref', 'ref', False, theme['ref'], None),
         # (r'(\[[^\]]*?\]:)(\S*?)$', 2, 'ref_data', 'ref', False, theme['ref_data'], None),
         # abbreviations
         (r'(\*\[.*?\]:.*?)', 1, 'abbr', 'abbr', False, theme['abbr'], None),
         (r'(\*\[(.*?)\]:.*?)', 2, 'abbr_text', 'abbr', False, theme['abbr_text'], None),
+        # hyperlinks (before the web links block to allow style overriding)
+        (r'((?<!!)\[.*?\]\(.*?\))', 1, 'a', 'a', False, theme['a'], None),
         # Web link
         # A word boundary \b matches the position between a word character (e.g., alphanumeric character or underscore)
         # and a non-word character (e.g., whitespace, punctuation, or the beginning/end of a string).
         # It allows you to match patterns only at the boundaries of words.
         # RFC 3986: uri = "[A-Za-z0-9\-._~:/?#\[\]@!$&\'()*+,;=%]"
-        (
-            r'(\b(?:https?|ftp):\/\/(?:\S+(?::\S*)?@)?(?:\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}|(?!-)[A-Za-z0-9-]{1,63}'
-            r'(?:(?:\.(?!-)[A-Za-z0-9-]{1,63})+)?(?:\:[0-9]+)?)?(?:\/(?:[^\:\?#\s\/]+)?)*(?:\?[^\s]*)?(?:#[^\s]*)?\b)',
-            1, 'link', 'link', False, theme['link'], None
-        ),
-        # hyperlinks
-        (r'((?<!!)\[.*?\]\(.*?\))', 1, 'a', 'a', False, theme['a'], None),
+        (r'((?:https?|ftp):\/\/(?:\S+(?::\S*)?@)?'
+         r'(?:\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}|(?!-)[A-Za-z0-9-]{1,63}(?:\.(?!-)[A-Za-z0-9-]{1,63})+)?(?:\:[0-9]+)?'
+         r'(?:\/(?:[^\:\?#\s\/\)]+)?)*(?:\?[^\s]*)?(?:#[^\s]*)?)', 1, 'link', 'link', False, theme['link'], None),
         # horizontal line
         (r'^(?:[\s>]*?)([\-\*_]{3,}(?:[\s]*?))$', 1, 'hr', 'hr', False, theme['hr'], None),
         # Comments
         # TODO: highlight by code lang
         (r'^([\s\t]*?[#]{1,}\s*?.*)$', 1, 'comment', 'comment', False, theme['comment'],
          lambda s: s.is_in_code()),
         (r'^((?:\s*?)"""(?!").*?(?<!")""")(?:\s*?)$', 1, 'comment', 'comment', False, theme['comment'],
@@ -676,15 +674,15 @@
                         elif tag in close_tokens:
                             for _r in self.get_open_close_token_map():
                                 if _r['group'] == group and _r['close'] == tag and _r['open'] in self.tokens:
                                     self.tokens[_r['open']]['o'] = False
 
                 # Comment """ block
                 if tag == 'cclop' and self.is_in_code():
-                    if not 'o' in self.tokens[tag]:
+                    if 'o' not in self.tokens[tag]:
                         self.tokens[tag]['o'] = True
                     elif self.tokens[tag]['o']:
                         self.tokens[tag]['o'] = False
                     else:
                         self.tokens[tag]['o'] = True
 
                 # Table
@@ -708,14 +706,16 @@
                         self.prev_user_data.put(tag='table_d', opened=False, within=True, closed=True)
                 elif tag == 'table_d' and self.tokens['table_d']['o']:
                     self.user_data.put(tag=tag, opened=False, within=True, closed=False)
                 if (group == 'table'
                         # Skip if not in table context yet
                         and not (self.user_data.get_param('table_d', 'within')
                                  or ('table_d' in self.tokens and self.tokens['table_d']['o']))):
+                    if self.debug:
+                        self.logger.debug('Skipping table block')
                     continue
                 # No save to block's data as it will be self stored for next block re-highlight iteration
 
                 # Prevent passing reference of the dict
                 cfc = cf_data.copy()
 
                 # Within the code block
```

### Comparing `notolog-0.9.1b4/notolog/highlight/view_highlighter.py` & `notolog-0.9.1b6/notolog/highlight/view_highlighter.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/image_downloader.py` & `notolog-0.9.1b6/notolog/image_downloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from .settings import Settings
 from .app_config import AppConfig
 from .lexemes.lexemes import Lexemes
 from .helpers.file_helper import size_f, save_file
 
 from urllib.parse import urlparse
+from typing import Union
 
 from qasync import asyncSlot
 import asyncio
 
 import os
 import re
 import hashlib
@@ -22,57 +23,61 @@
 
     # Signal to emit upon single resource was downloaded
     downloaded = Signal(dict)
 
     # Signal to emit upon all downloading tasks in queue have been finished
     finished = Signal(int)
 
-    RESOURCE_DIR = 'images'
+    RESOURCE_DIR = AppConfig().get_editor_media_dir()
 
     def __init__(self, base_folder: str = None):
 
         super().__init__()
 
         self.settings = Settings(parent=self)
 
         self.logger = logging.getLogger('image_downloader')
 
-        self.logging = AppConfig.get_logging()
-        self.debug = AppConfig.get_debug()
+        self.logging = AppConfig().get_logging()
+        self.debug = AppConfig().get_debug()
 
         self.lexemes = Lexemes()
 
         # Async event loop
         self.event_loop = asyncio.get_event_loop()
         # async download tasks queue
         self.resource_tasks = []
 
+        # Active folder to work with resources
+        self.folder = Union[QDir, None]
+
         # Downloaded counter till finished emitted
         self.downloaded_cnt = 0
 
-        # Validate folder and make it QDir
-        self.folder = self.get_resource_folder(base_folder)
-
-        if self.debug:
-            self.logger.debug(f'Folder to save downloaded resources: {self.folder.path()}')
-
-        os.makedirs(self.folder.path(), exist_ok=True)
+        self.update_resource_folder(base_folder)
 
         self.network_manager = QNetworkAccessManager()
 
     def get_resource_folder(self, base_folder: str = None) -> QDir:
         # Check folder and make it QDir
         if base_folder:
             folder = os.path.join(base_folder, self.RESOURCE_DIR)
         else:
             folder = os.path.join(QDir.currentPath(), self.RESOURCE_DIR)
         if isinstance(folder, str):
             folder = QDir(folder)
         return folder
 
+    def update_resource_folder(self, base_folder: str = None) -> None:
+        # Validate folder and make it QDir
+        self.folder = self.get_resource_folder(base_folder)
+
+        if self.debug:
+            self.logger.debug(f'Folder to save downloaded resources: {self.folder.path()}')
+
     def download_image(self, url: str) -> None:
         if not self.is_external_url(url):
             if self.debug:
                 self.logger.debug(f"Skip downloading as the provided url is not an external url: {url}")
             return
 
         if self.debug:
@@ -85,14 +90,16 @@
         reply.finished.connect(lambda _reply=reply: self.handle_network_reply(_reply))
         # Connecting error signal
         reply.errorOccurred.connect(lambda error, _reply=reply: self.handle_network_reply(_reply, error))
 
     def save_image(self, url: str, data: QByteArray) -> None:
         # file_name = os.path.basename(url)
         file_name = self.url_to_filename(url)
+        # Create resource folder if not yet created
+        os.makedirs(self.folder.path(), exist_ok=True)
         # File path to save
         file_path = os.path.join(self.folder.path(), file_name)
         # Save received data
         if save_file(file_path, data, as_bytearray=True):
             if self.debug:
                 self.logger.debug(f"Resource saved {url} to {file_path} [{size_f(len(data))}]")
         else:
@@ -225,17 +232,15 @@
         parsed_url = urlparse(url)
         return not (parsed_url.netloc == '' or parsed_url.netloc.endswith(base_domain))
 
     @staticmethod
     def url_to_filename(url):
         """
         Generate a filename from a URL by hashing the URL except its basename and combining it with the basename.
-
-        # Convert a URL into a safe filename by replacing non-alphanumeric characters with underscores.
-        return re.sub(r'\W+', '_', url)
+        Convert a URL into a safe filename by replacing non-alphanumeric characters with underscores.
         """
         # Extract the basename
         basename = os.path.basename(url)
 
         # Hash the URL excluding the basename
         url_hash = hashlib.sha256(url.replace(basename, '').encode('utf-8')).hexdigest()
         short_hash = url_hash[:8]  # Use only first 8 characters of the hash
```

### Comparing `notolog-0.9.1b4/notolog/lexemes/de/ai_assistant.py` & `notolog-0.9.1b6/notolog/lexemes/de/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/de/color_picker_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/de/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/de/common.py` & `notolog-0.9.1b6/notolog/lexemes/de/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/de/main_menu.py` & `notolog-0.9.1b6/notolog/lexemes/de/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/de/settings_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/de/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/de/statusbar.py` & `notolog-0.9.1b6/notolog/lexemes/de/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/de/toolbar.py` & `notolog-0.9.1b6/notolog/lexemes/de/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/en/ai_assistant.py` & `notolog-0.9.1b6/notolog/lexemes/en/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/en/color_picker_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/en/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/en/common.py` & `notolog-0.9.1b6/notolog/lexemes/en/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/en/main_menu.py` & `notolog-0.9.1b6/notolog/lexemes/en/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/en/settings_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/en/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/en/statusbar.py` & `notolog-0.9.1b6/notolog/lexemes/en/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/en/toolbar.py` & `notolog-0.9.1b6/notolog/lexemes/en/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/es/ai_assistant.py` & `notolog-0.9.1b6/notolog/lexemes/es/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/es/color_picker_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/es/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/es/common.py` & `notolog-0.9.1b6/notolog/lexemes/es/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/es/main_menu.py` & `notolog-0.9.1b6/notolog/lexemes/es/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/es/settings_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/es/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/es/statusbar.py` & `notolog-0.9.1b6/notolog/lexemes/es/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/es/toolbar.py` & `notolog-0.9.1b6/notolog/lexemes/es/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/fi/ai_assistant.py` & `notolog-0.9.1b6/notolog/lexemes/fi/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/fi/color_picker_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/fi/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/fi/common.py` & `notolog-0.9.1b6/notolog/lexemes/fi/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/fi/main_menu.py` & `notolog-0.9.1b6/notolog/lexemes/fi/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/fi/settings_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/fi/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/fi/statusbar.py` & `notolog-0.9.1b6/notolog/lexemes/fi/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/fi/toolbar.py` & `notolog-0.9.1b6/notolog/lexemes/fi/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/fr/ai_assistant.py` & `notolog-0.9.1b6/notolog/lexemes/fr/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/fr/color_picker_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/fr/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/fr/common.py` & `notolog-0.9.1b6/notolog/lexemes/fr/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/fr/main_menu.py` & `notolog-0.9.1b6/notolog/lexemes/fr/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/fr/settings_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/fr/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/fr/statusbar.py` & `notolog-0.9.1b6/notolog/lexemes/fr/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/fr/toolbar.py` & `notolog-0.9.1b6/notolog/lexemes/fr/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/ge/ai_assistant.py` & `notolog-0.9.1b6/notolog/lexemes/ge/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/ge/color_picker_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/ge/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/ge/common.py` & `notolog-0.9.1b6/notolog/lexemes/ge/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/ge/main_menu.py` & `notolog-0.9.1b6/notolog/lexemes/ge/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/ge/settings_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/ge/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/ge/statusbar.py` & `notolog-0.9.1b6/notolog/lexemes/ge/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/ge/toolbar.py` & `notolog-0.9.1b6/notolog/lexemes/ge/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/gr/ai_assistant.py` & `notolog-0.9.1b6/notolog/lexemes/gr/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/gr/color_picker_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/gr/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/gr/common.py` & `notolog-0.9.1b6/notolog/lexemes/gr/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/gr/main_menu.py` & `notolog-0.9.1b6/notolog/lexemes/gr/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/gr/settings_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/gr/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/gr/statusbar.py` & `notolog-0.9.1b6/notolog/lexemes/gr/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/gr/toolbar.py` & `notolog-0.9.1b6/notolog/lexemes/gr/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/in/ai_assistant.py` & `notolog-0.9.1b6/notolog/lexemes/in/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/in/color_picker_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/in/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/in/common.py` & `notolog-0.9.1b6/notolog/lexemes/in/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/in/main_menu.py` & `notolog-0.9.1b6/notolog/lexemes/in/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/in/settings_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/in/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/in/statusbar.py` & `notolog-0.9.1b6/notolog/lexemes/in/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/in/toolbar.py` & `notolog-0.9.1b6/notolog/lexemes/in/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/it/ai_assistant.py` & `notolog-0.9.1b6/notolog/lexemes/it/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/it/color_picker_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/it/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/it/common.py` & `notolog-0.9.1b6/notolog/lexemes/it/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/it/main_menu.py` & `notolog-0.9.1b6/notolog/lexemes/it/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/it/settings_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/it/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/it/statusbar.py` & `notolog-0.9.1b6/notolog/lexemes/it/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/it/toolbar.py` & `notolog-0.9.1b6/notolog/lexemes/it/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/ja/ai_assistant.py` & `notolog-0.9.1b6/notolog/lexemes/ja/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/ja/color_picker_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/ja/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/ja/common.py` & `notolog-0.9.1b6/notolog/lexemes/ja/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/ja/main_menu.py` & `notolog-0.9.1b6/notolog/lexemes/ja/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/ja/settings_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/ja/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/ja/statusbar.py` & `notolog-0.9.1b6/notolog/lexemes/ja/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/ja/toolbar.py` & `notolog-0.9.1b6/notolog/lexemes/ja/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/ko/ai_assistant.py` & `notolog-0.9.1b6/notolog/lexemes/ko/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/ko/color_picker_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/ko/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/ko/common.py` & `notolog-0.9.1b6/notolog/lexemes/ko/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/ko/main_menu.py` & `notolog-0.9.1b6/notolog/lexemes/ko/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/ko/settings_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/ko/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/ko/statusbar.py` & `notolog-0.9.1b6/notolog/lexemes/ko/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/ko/toolbar.py` & `notolog-0.9.1b6/notolog/lexemes/ko/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/la/ai_assistant.py` & `notolog-0.9.1b6/notolog/lexemes/la/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/la/color_picker_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/la/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/la/common.py` & `notolog-0.9.1b6/notolog/lexemes/la/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/la/main_menu.py` & `notolog-0.9.1b6/notolog/lexemes/la/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/la/settings_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/la/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/la/statusbar.py` & `notolog-0.9.1b6/notolog/lexemes/la/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/la/toolbar.py` & `notolog-0.9.1b6/notolog/lexemes/la/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/lexemes.py` & `notolog-0.9.1b6/notolog/lexemes/lexemes.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,16 @@
         if isinstance(lexeme, bytes):
             lexeme = lexeme.decode('utf-8')
 
         if kwargs:
             # Process placeholders if set, e.g. name="abc" in a string like "... {name} ..." become "... abc ..."
             try:
                 lexeme = lexeme.format(**kwargs)
+            except AttributeError:
+                self.logger.warning('Lexeme "%s" not found' % name)
             except KeyError:
                 self.logger.warning('Lexeme "%s" params [%s] not found for replacement'
                                     % (lexeme, ', '.join(kwargs.keys())))
         return lexeme
 
     def get_all(self):
         # Return all lexemes set
```

### Comparing `notolog-0.9.1b4/notolog/lexemes/nl/ai_assistant.py` & `notolog-0.9.1b6/notolog/lexemes/nl/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/nl/color_picker_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/nl/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/nl/common.py` & `notolog-0.9.1b6/notolog/lexemes/nl/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/nl/main_menu.py` & `notolog-0.9.1b6/notolog/lexemes/nl/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/nl/settings_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/nl/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/nl/statusbar.py` & `notolog-0.9.1b6/notolog/lexemes/nl/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/nl/toolbar.py` & `notolog-0.9.1b6/notolog/lexemes/nl/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/pt/ai_assistant.py` & `notolog-0.9.1b6/notolog/lexemes/pt/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/pt/color_picker_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/pt/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/pt/common.py` & `notolog-0.9.1b6/notolog/lexemes/pt/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/pt/main_menu.py` & `notolog-0.9.1b6/notolog/lexemes/pt/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/pt/settings_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/pt/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/pt/statusbar.py` & `notolog-0.9.1b6/notolog/lexemes/pt/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/pt/toolbar.py` & `notolog-0.9.1b6/notolog/lexemes/pt/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/ru/ai_assistant.py` & `notolog-0.9.1b6/notolog/lexemes/ru/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/ru/color_picker_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/ru/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/ru/common.py` & `notolog-0.9.1b6/notolog/lexemes/ru/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/ru/main_menu.py` & `notolog-0.9.1b6/notolog/lexemes/ru/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/ru/settings_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/ru/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/ru/statusbar.py` & `notolog-0.9.1b6/notolog/lexemes/ru/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/ru/toolbar.py` & `notolog-0.9.1b6/notolog/lexemes/ru/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/se/ai_assistant.py` & `notolog-0.9.1b6/notolog/lexemes/se/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/se/color_picker_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/se/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/se/common.py` & `notolog-0.9.1b6/notolog/lexemes/se/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/se/main_menu.py` & `notolog-0.9.1b6/notolog/lexemes/se/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/se/settings_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/se/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/se/statusbar.py` & `notolog-0.9.1b6/notolog/lexemes/se/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/se/toolbar.py` & `notolog-0.9.1b6/notolog/lexemes/se/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/tr/ai_assistant.py` & `notolog-0.9.1b6/notolog/lexemes/tr/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/tr/color_picker_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/tr/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/tr/common.py` & `notolog-0.9.1b6/notolog/lexemes/tr/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/tr/main_menu.py` & `notolog-0.9.1b6/notolog/lexemes/tr/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/tr/settings_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/tr/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/tr/statusbar.py` & `notolog-0.9.1b6/notolog/lexemes/tr/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/tr/toolbar.py` & `notolog-0.9.1b6/notolog/lexemes/tr/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/zh/ai_assistant.py` & `notolog-0.9.1b6/notolog/lexemes/zh/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/zh/color_picker_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/zh/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/zh/common.py` & `notolog-0.9.1b6/notolog/lexemes/zh/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/zh/main_menu.py` & `notolog-0.9.1b6/notolog/lexemes/zh/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/zh/settings_dialog.py` & `notolog-0.9.1b6/notolog/lexemes/zh/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/zh/statusbar.py` & `notolog-0.9.1b6/notolog/lexemes/zh/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/lexemes/zh/toolbar.py` & `notolog-0.9.1b6/notolog/lexemes/zh/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/main.py` & `notolog-0.9.1b6/notolog/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # - Copyright 2024 Vadim Bakhrenkov
 # - License: MIT License
 
 
 from PySide6.QtWidgets import QStyleFactory
 from qasync import QEventLoop, QApplication
 
-# from notolog.app_config import AppConfig
+from notolog.app_config import AppConfig
 from notolog.notolog_editor import NotologEditor
 
 import platform
 import logging
 import asyncio
 import sys
 import os
@@ -46,34 +46,44 @@
     Possible params:
     filename='notolog.log'
     format='%(asctime)s:%(levelname)s:%(name)s:%(message)s'
     """
     logging.basicConfig(level=logging.DEBUG, format='[%(name)s] %(funcName)s: %(levelname)s: %(message)s')
 
     # Enable logging, uncomment or change app config
-    # AppConfig.set_logging(True)
+    # AppConfig().set_logging(True)
     # Enable debug mode (a lot of logs), uncomment or change app config
-    # AppConfig.set_debug(False)
+    # AppConfig().set_debug(False)
+
+    logger = logging.getLogger('notolog')
+    if AppConfig().get_logging():
+        logger.info("%s v%s" % (AppConfig().get_app_name(), AppConfig().get_app_version()))
+        logger.info("%s" % (AppConfig().get_app_license()))
 
     # Main application
     app = QApplication(sys.argv)
+    # To correctly set up app settings
+    app.setOrganizationName('Notolog')
+    app.setApplicationName('notolog_editor')
+    app.setApplicationVersion(AppConfig().get_app_version())
 
     # Detect the operating system to choose the style
     current_os = platform.system()
     if current_os == "Windows":
         app.setStyle(QStyleFactory.create("WindowsVista"))
-    # elif current_os == "Darwin":  # MacOS
+    # elif current_os == "Darwin":  # macOS
     #    app.setStyle(QStyleFactory.create("Macintosh"))  # Renders not as expected
     else:  # Or: current_os == "Linux"
         app.setStyle(QStyleFactory.create("Fusion"))  # Fusion is a cross-platform choice
 
     # Maintain a unique style regardless of the user's system settings
     app.setDesktopSettingsAware(False)
 
-    logging.getLogger('notolog').info('Application dir path "%s"' % QApplication.applicationDirPath())
+    if AppConfig().get_debug():
+        logger.debug('Application dir path "%s"' % QApplication.applicationDirPath())
 
     # Get the screen to pass it to the main module
     screen = app.screens()[0]
 
     # Main loop
     loop = QEventLoop(app)
     asyncio.set_event_loop(loop)
```

### Comparing `notolog-0.9.1b4/notolog/notolog_editor.py` & `notolog-0.9.1b6/notolog/notolog_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from .app_config import AppConfig
 from .file_header import FileHeader
 from .edit_widget import EditWidget
 from .view_widget import ViewWidget
 from .view_processor import ViewProcessor
 from .view_decorator import ViewDecorator
 from .image_downloader import ImageDownloader
+from .async_highlighter import AsyncHighlighter
 
 # UI
 from .ui.file_system_model import FileSystemModel
 from .ui.sort_filter_proxy_model import SortFilterProxyModel
 from .ui.toolbar import ToolBar
 from .ui.statusbar import StatusBar
 from .ui.line_numbers import LineNumbers
@@ -144,16 +145,16 @@
     ]
 
     def __init__(self, parent = None, **kwargs):
         super(NotologEditor, self).__init__(parent=parent)
 
         self.logger = logging.getLogger('notolog')
 
-        self.logging  = AppConfig.get_logging()
-        self.debug = AppConfig.get_debug()
+        self.logging = AppConfig().get_logging()
+        self.debug = AppConfig().get_debug()
 
         self.settings = Settings(parent=self)
         self.settings.value_changed.connect(
             lambda v: self.settings_update_handler(v))
         """
         Set theme:
         self.settings.theme = 'bordo'
@@ -239,31 +240,31 @@
 
         # Markdown instance
         self.md = None  # type: Union[markdown.Markdown, None]
 
         # Highlighters
         self.md_highlighter = None  # type: Union[MdHighlighter, None]
         self.view_highlighter = None  # type: Union[ViewHighlighter, None]
-        # async re-highlight tasks queue
-        self.rehighlight_tasks = []
+
+        # Async highlighter
+        self.async_highlighter = AsyncHighlighter(callback=lambda is_full: self.rehighlight_editor(is_full))
 
         # Resource Downloader
         self.resource_downloader = None  # type: Union[ImageDownloader, None]
         # async download tasks queue
         self.resource_tasks = []
 
         # File tree and variable
         self.tree_container = None  # type: Union[QWidget, None]
         self.file_model = None  # type: Union[FileSystemModel, None]
         self.tree_view = None  # type: Union[QListView, None]
         self.tree_filter = None  # type: Union[QLineEdit, None]
         self.tree_proxy_model = None  # type: Union[SortFilterProxyModel, None]
         self.file_watcher = None  # type: Union[QFileSystemWatcher, None]
 
-        # self.supported_file_types = ['*.md', '*.txt', '*.html', '*.enc']
         self.supported_file_extensions = ['md', 'txt', 'html', 'enc']
 
         # Line numbers within the document
         self.line_numbers = None  # type: Union[LineNumbers, None]
 
         # Toolbar
         self.toolbar = None  # type: Union[ToolBar, QToolBar, None]
@@ -323,15 +324,15 @@
         shortcut_search.activated.connect(self.search_text)
 
     def init_font(self):
         # Use default ratio
         font_size_ratio = 1.0
         font_size = int(float(self.settings.app_font_size) * font_size_ratio)
 
-        AppConfig.set_font_size(font_size)
+        AppConfig().set_font_size(font_size)
 
         font = QFont()  # Accept args like "Sans Serif"
         font.setPointSize(font_size)
 
         if self.debug:
             self.logger.debug('Font point size set to %d, font size ratio %.2f'
                               % (font.pointSize(), font_size_ratio))
@@ -344,15 +345,15 @@
         Can be resource greedy.
 
         @param data: dict, say {"show_line_numbers": True}
         @return: None
         """
 
         if self.debug:
-            self.logger.debug('Settings update handler in use "%s"' % data)
+            self.logger.debug('Settings update handler is in use "%s"' % data)
 
         if 'show_line_numbers' in data and hasattr(self, 'line_numbers'):
             # Show / hide line numbers area
             self.line_numbers.update_numbers()
 
         if 'app_font_size' in data and hasattr(self, 'theme_helper'):
             # Set up global font params
@@ -459,15 +460,15 @@
     def editor_state_update_handler(self, data: dict) -> None:
         """
         Perform actions belonging to the editor state changed, say mode toggle event.
         When switching between VIEW and EDIT mode some icons and texts may look differ, have different actions, etc.
         """
 
         if self.debug:
-            self.logger.debug('Editor state update handler in use "%s"' % data)
+            self.logger.debug('Editor state update handler is in use "%s"' % data)
 
         # Initially the elements may not exist, but apper later on
         if hasattr(self, 'statusbar'):
             if data['c'] == Mode:
                 mode_label_text = self.lexemes.get(
                     'statusbar_mode_label_mode_%s' % Mode(self.get_mode()).name.lower(), scope='statusbar')
                 self.statusbar['mode_label'].setText(mode_label_text)
@@ -861,16 +862,15 @@
         self.file_model.setRootPath(QDir.currentPath())  # Or it can be just a '.'
         """
         Also: QDir.AllEntries, QDir.Filter.NoDotAndDotDot
         """
         self.file_model.setFilter(QDir.Filter.NoDot | QDir.Filter.Dirs | QDir.Filter.Files)
         """
         Show only these files in the list (implemented via proxy sort model)
-        filters = self.supported_file_types
-        self.file_model.setNameFilters(filters)
+        self.file_model.setNameFilters(['*.md', '*.txt', '*.html', '*.enc'])
         """
         # Do not show greyed filter results
         self.file_model.setNameFilterDisables(False)
 
         # Either QTreeView(self) or QListView(self) are working fine
         self.tree_view = QListView(self)
         # Apply font from the main window to the widget
@@ -985,15 +985,15 @@
 
         # View document
         view_doc = self.get_view_doc()  # type: QTextDocument
         # Set up document's base resource path
         """
         If a resource file not found QTextBrowser will try to search either this script or package root path (IDE run).
         """
-        view_doc.setBaseUrl(QUrl.fromLocalFile(dir_path + '/'))
+        view_doc.setBaseUrl(QUrl.fromLocalFile(dir_path + os.sep))
 
     def get_current_file_path(self, is_base: bool = False) -> str:
         """
         Get current file path.
         """
         return os.path.dirname(self.file_path) if is_base else self.file_path
 
@@ -1707,106 +1707,39 @@
         return self.text_view
 
     @asyncClose
     async def closeEvent(self, event):
         if self.logging:
             self.logger.info('Stopping events loop, closing the app... Sayonara!')
 
-        # Cancel all pending tasks if exist
-        if hasattr(self, 'rehighlight_tasks'):
-            tasks_total = len(self.rehighlight_tasks)
-            for i, task in enumerate(self.rehighlight_tasks):
-                if not task.done():
-                    task_res = task.cancel()
-                    if self.logging:
-                        self.logger.info(f'[{i+1}/{tasks_total}] Pending task "{task.get_name()}" canceled with result "{task_res}"')
-                    # Gather all tasks to ensure they are completed before closing
-                    await asyncio.gather(*self.rehighlight_tasks, return_exceptions=True)
+        # Cancel all re-highlight tasks if they are exist
+        if hasattr(self, 'async_highlighter') and self.async_highlighter:
+            await self.async_highlighter.cancel_tasks()
 
         # Cancel all resource downloading tasks if they are exist
-        if hasattr(self, 'resource_downloader'):
+        if hasattr(self, 'resource_downloader') and self.resource_downloader:
             await self.resource_downloader.cancel_tasks()
 
         if self.get_mode() == Mode.EDIT:
             # Save any unsaved changes
             self.save_active_file(clear_after=False)
         else:
             # Save cursor position (block start)
             self.store_doc_cursor_pos(self.get_mode())
 
         self.settings.mode = self.get_mode().value
         self.settings.source = self.get_source().value
 
         event.accept()
 
-    @asyncSlot()
-    async def rehighlight_in_queue(self, full_rehighlight: bool = False) -> Any:
-        """
-        More info about asyncio tasks: https://docs.python.org/3/library/asyncio-task.html
-        """
-        if self.debug:
-            self.logger.debug('Re-highlight %d tasks in queue' % len(self.rehighlight_tasks))
-
-        postpone = False if len(self.rehighlight_tasks) == 0 else True
-        if self.debug:
-            self.logger.debug('Re-highlight is to postpone "%r"' % postpone)
-
-        task = None
-        # To keep only a few tasks in queue
-        if len(self.rehighlight_tasks) < 3:
-            task = asyncio.ensure_future(self.rehighlight_async(full_rehighlight, postpone))
-            # task = asyncio.create_task(self.rehighlight_async(full_rehighlight, postpone))
-            # Add task to the local pool first
-            self.rehighlight_tasks.append(task)
-            # Callback method to set up further actions
-            task.add_done_callback(lambda _task: self.rehighlight_task_callback(_task))
-
-        done, pending = await asyncio.wait(
-            self.rehighlight_tasks,
-            return_when=asyncio.ALL_COMPLETED,  # There is no pending tasks check
-        )
-
-        if self.debug:
-            self.logger.debug(f'Re-highlight tasks progress. Done {len(done)}, pending {len(pending)}')
-
-        return task
-
-    def rehighlight_task_callback(self, task) -> None:
-        if self.debug:
-            self.logger.debug('%s from total %d completed with callback'
-                              % (task.get_name(), len(self.rehighlight_tasks)))
-
-        self.rehighlight_tasks.remove(task)
-
-        if len(self.rehighlight_tasks) == 0:
-            QTimer.singleShot(750, lambda: self.rehighlight_editor(True))
-
-    async def rehighlight_async(self, full_rehighlight: bool = False, postpone: bool = False) -> None:
-        """
-        Run this method not too often to avoid overwhelming the system.
-        """
+    def rehighlight_editor(self, full_rehighlight: bool = False) -> None:
         # First of all check it's necessary
-        if self.get_mode() == Mode.EDIT and self.get_source() == Source.MARKDOWN:
-            # Postpone before re-highlighting if a few tasks
-            if postpone:
-                if self.debug:
-                    self.logger.debug('Re-highlighting the text > postpone')
-                # Keep this method particular amount of time to avoid overwhelming
-                await asyncio.sleep(0.25, self.loop)
-            # Re-highlight
-            self.rehighlight_editor(full_rehighlight)
-            if self.debug:
-                self.logger.debug('Async re-highlighting queue task processed')
-            # Postpone after re-highlighting to keep the queue busy
-            if self.debug:
-                self.logger.debug('Re-highlighting the text > wait to return')
-            # Keep this method particular amount of time to avoid overwhelming
-            await asyncio.sleep(0.5, self.loop)
+        if not (self.get_mode() == Mode.EDIT and self.get_source() == Source.MARKDOWN):
+            return
 
-    def rehighlight_editor(self, full_rehighlight: bool = False) -> None:
         # Edit widget
         edit_widget = self.get_edit_widget()  # type: Union[EditWidget, QPlainTextEdit]
 
         # Prevent QTextEdit's on_text_changed() method invocation by blocking signals
         was_blocked = edit_widget.blockSignals(True)
         if self.debug:
             self.logger.debug(f'Re-highlighting the text > signals was blocked "{was_blocked}"')
@@ -1856,15 +1789,16 @@
         if hasattr(self.toolbar, 'toolbar_save_button'):
             self.toolbar.toolbar_save_button.setDisabled(False)
 
         full_rehighlight = (self.get_block_data_param('code', 'opened')
                             or self.get_block_data_param('code', 'closed'))
 
         # Schedule async whole doc re-highlighting task in queue
-        self.rehighlight_in_queue(full_rehighlight)
+        if hasattr(self, 'async_highlighter') and self.async_highlighter:
+            self.async_highlighter.rehighlight_in_queue(full_rehighlight)
         """
         Opposed way, synchronous highlighting direct call:
         self.rehighlight_editor(full_rehighlight)
         """
 
     def on_modification_changed(self, changed) -> None:
         """
@@ -2856,21 +2790,19 @@
 
         # Get cursor position to check any selected text there
         cursor = targeting_widget.textCursor()
 
         selected_text = ''  # Default
         if cursor.hasSelection():
             selected_text = cursor.selectedText()
-            """
             # Make possible to undo selected text formatting:
-            re = QRegularExpression(r'^(<span style="color:\s*?[a-zA-z]+;?">)(.*?)(<\/span>)$')
-            match = re.match(selected_text)
-            if match.capturedTexts() and match.captured(2):
-                cursor.insertText(match.captured(2))
-            """
+            # re = QRegularExpression(r'^(<span style="color:\s*?[a-zA-z]+;?">)(.*?)(<\/span>)$')
+            # match = re.match(selected_text)
+            # if match.capturedTexts() and match.captured(2):
+            #    cursor.insertText(match.captured(2))
         updated_text = f'<span style="color: {color}">{selected_text}</span>'
 
         if self.get_mode() == Mode.EDIT:
             # Set True to keep inserted fragment selected
             cursor.setKeepPositionOnInsert(True)
             # Replace selected text with formatted one
             cursor.insertText(updated_text)
@@ -2944,15 +2876,15 @@
         Send bug report here.
         Or, redirect to the repository's page to create a task.
         """
 
         if self.debug:
             self.logger.debug('Sending bug report...')
 
-        url = AppConfig.get_repository_github_bug_report_url()
+        url = AppConfig().get_repository_github_bug_report_url()
 
         self.common_dialog(
             self.lexemes.get('dialog_open_link_title'),
             self.lexemes.get(name='dialog_open_link_text', url=url),
                 # Open url with system browser
                 callback=lambda dialog_callback:
                 # Open link in a system browser and run dialog's callback
@@ -3127,15 +3059,15 @@
                             # return self.load_default_page(ignore_settings=True)
                             return False
                         elif self.get_enc_password_dialog_cnt() > 0:
                             # Do not ask confirmation to reset the password as it has been confirmed already
                             self.reset_encrypt_helper()
                         else:
                             """
-                            Ask to reset current password that in use by currently opened file.
+                            Request to change the password for the currently opened file to a new one.
                             Try to load the file by switch to it if the encryption password has been reset.
                             """
                             self.enc_password_reset_dialog()
                     else:
                         """
                         If no password set.
                         Remove saved start up page from settings
@@ -3652,17 +3584,21 @@
     def process_document_images(self, text_document):
         """
         Extract image urls from the given document
         """
 
         # Init image downloader instance
         if self.resource_downloader is None:
-            self.resource_downloader = ImageDownloader()
+            # Init new instance and set up signal handlers
+            self.resource_downloader = ImageDownloader(self.get_active_dir())
             self.resource_downloader.downloaded.connect(self.resource_downloaded_handler)  # Single resource downloaded
             self.resource_downloader.finished.connect(self.resource_downloader_finished_handler)  # All tasks finished
+        else:
+            # Refresh active resource folder
+            self.resource_downloader.update_resource_folder(self.get_active_dir())
 
         block = text_document.begin()
         # Check doc's block
         while block.isValid():
             it = block.begin()
             while not it.atEnd():
                 fragment = it.fragment()
```

### Comparing `notolog-0.9.1b4/notolog/settings.py` & `notolog-0.9.1b6/notolog/settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from PySide6.QtCore import Signal, QSettings
 
 from .app_config import AppConfig
 from .enums.themes import Themes
 from .enums.languages import Languages
 from .enums.ai_model_names import AiModelNames
+from .helpers.settings_helper import SettingsHelper
 
 from typing import Any, Union
 
 import logging
 
 
 class Settings(QSettings):
@@ -22,33 +23,35 @@
         Args:
             parent (optional): Parent object
         """
         super(Settings, self).__init__(parent)
 
         self.logger = logging.getLogger('settings')
 
-        self.logging = AppConfig.get_logging()
-        self.debug = AppConfig.get_debug()
+        self.logging = AppConfig().get_logging()
+        self.debug = AppConfig().get_debug()
 
         self.settings = QSettings()
+        self.settings_helper = SettingsHelper()
 
         if self.debug:
             # Attributes may not be set at the very beginning
             self.logger.debug('Window size %d x %d' % (getattr(self, 'ui_width', 0), getattr(self, 'ui_height', 0)))
 
         self.value_changed.connect(lambda v: self.settings.sync())
 
+        self.protected_attr = []
         self.init_fields()
 
     def init_fields(self):
         # App's UI settings
         self.create_property("app_theme", str, str(Themes.default()))
         self.create_property("app_language", str, str(Languages.default()))
-        self.create_property("app_font_size", int, AppConfig.get_font_base_size(),
-                             set_prev_func=lambda: AppConfig.set_prev_font_size(self.settings.value("app_font_size")))
+        self.create_property("app_font_size", int, AppConfig().get_font_base_size(),
+                             set_prev_func=lambda prev_value: AppConfig().set_prev_font_size(prev_value))
         # Window positioning and size
         self.create_property("ui_width", int, 0)
         self.create_property("ui_height", int, 0)
         self.create_property("ui_pos_x", int, 0)
         self.create_property("ui_pos_y", int, 0)
         # Splitter between navigation tree and view/edit widget position
         self.create_property("ui_splitter_pos", int, 0)
@@ -72,35 +75,54 @@
         self.create_property("viewer_save_resources", bool, True)
         # Icons to show on the toolbar. Can be checked like:
         # if value is not None and value.isValid() and isinstance(value.toInt()[0], int): ...
         self.create_property("toolbar_icons", int, None)
         self.create_property("enc_iterations", int, None)
         # AI assistant
         self.create_property("ai_config_openai_url", str, "https://api.openai.com/v1/chat/completions")
-        self.create_property("ai_config_openai_key", str, "")
+        self.create_property("ai_config_openai_key", str, "", encrypt=True)
         self.create_property("ai_config_openai_model", str, str(AiModelNames.default()))
         self.create_property("ai_config_base_system_prompt", str, "")
         self.create_property("ai_config_base_response_max_tokens", int, 512)
 
-    def create_property(self, param_name: str, param_type: Any, default_value: Any, set_prev_func: Any = None):
+    def create_property(self, param_name: str, param_type: Any, default_value: Any, set_prev_func: Any = None,
+                        encrypt: bool = False):
         def getter(_self):
             # Type is crucial here
-            return param_type(_self.settings.value(param_name, default_value, type=param_type))
+            value = _self.settings.value(param_name, default_value, type=param_type)
+            if encrypt:
+                try:
+                    value = self.settings_helper.decrypt_data(value)
+                except (ValueError, EnvironmentError) as e:
+                    if self.logging:
+                        self.logger.warning(f'Settings protected parameter "{param_name}" getting error: {e}')
+            return param_type(value)
 
         def setter(_self, value):
-            if _self.settings.value(param_name) != value:
+            _prev_value = _self.settings.value(param_name)
+            if _prev_value != value:
                 if callable(set_prev_func):
                     # Save previous value
-                    set_prev_func()
+                    set_prev_func(_prev_value)
+                if encrypt:
+                    try:
+                        value = self.settings_helper.encrypt_data(value)
+                    except (ValueError, EnvironmentError) as e:
+                        if self.logging:
+                            self.logger.warning(f'Settings protected parameter "{param_name}" setting error: {e}')
                 _self.settings.setValue(param_name, value)
                 _self.value_changed.emit({param_name: value})
 
         # Dynamically create the property and its setter
         setattr(Settings, param_name, property(getter, setter))
 
+        # Add param to the protected list if applicable
+        if encrypt:
+            self.protected_attr.append(param_name)
+
     """
     Example of how to set up for each settings property
     """
 
     @property
     def show_main_menu(self) -> bool:
         # From settings UI dialog
```

### Comparing `notolog-0.9.1b4/notolog/text_block_data.py` & `notolog-0.9.1b6/notolog/text_block_data.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/theme.py` & `notolog-0.9.1b6/notolog/theme.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,30 +14,27 @@
 class Theme:
 
     ASSETS_DIR_NAME = "assets"
 
     _instance = None
 
     def __new__(cls, *args, **kwargs):
-        if cls._instance is None or AppConfig.get_test_mode():  # No cache in test mode
+        if cls._instance is None or AppConfig().get_test_mode():  # No cache in test mode
             cls._instance = super().__new__(cls)
         return cls._instance
 
     def __init__(self, theme: str = None):
         # Load exact theme once
         if getattr(self, 'theme', None) and self.theme == theme:
             return
 
-        # Logger
         self.logger = logging.getLogger('themes')
 
-        # Logging
-        self.logging = AppConfig.get_logging()
-        # Debug
-        self.debug = AppConfig.get_debug()
+        self.logging = AppConfig().get_logging()
+        self.debug = AppConfig().get_debug()
 
         # Custom Enum logic return name.lower() when cast to string
         # Same as: Themes.default().name.lower()
         self.default_theme = str(Themes.default())
 
         if not theme or theme in ('.', '..'):  # in case of file dependant
             theme = self.default_theme
```

### Comparing `notolog-0.9.1b4/notolog/ui/about_popup.py` & `notolog-0.9.1b6/notolog/ui/about_popup.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,16 +29,16 @@
         # Apply font from the dialog instance to the label
         self.setFont(self.parent.font())
 
         self.settings = Settings(parent=self)
 
         self.logger = logging.getLogger('about_popup')
 
-        self.logging = AppConfig.get_logging()
-        self.debug = AppConfig.get_debug()
+        self.logging = AppConfig().get_logging()
+        self.debug = AppConfig().get_debug()
 
         # Default language setup, change to settings value to modify it via UI
         self.lexemes = Lexemes(self.settings.app_language, default_scope='common')
 
         # Theme helper
         self.theme_helper = ThemeHelper()
 
@@ -81,38 +81,38 @@
         frame_layout.addWidget(icon_label, 0, 1, Qt.AlignmentFlag.AlignLeft, 1)
 
         app_name_widget = QWidget(self)
         app_name_layout = QVBoxLayout(app_name_widget)
         app_name_layout.setSpacing(0)
         app_name_layout.setContentsMargins(0, 0, 0, 0)
 
-        app_name = QLabel(AppConfig.get_app_name(), app_name_widget)
+        app_name = QLabel(AppConfig().get_app_name(), app_name_widget)
         app_name_font = self.font()
         app_name_font.setPointSizeF(app_name_font.pointSize() * 1.7)
         app_name.setFont(app_name_font)
         app_name.setObjectName('app_name')
         app_name_layout.addWidget(app_name)
         app_name_caption = QLabel(self.lexemes.get('popup_about_app_name_description'), app_name_widget)
         app_name_caption.sizeHint()
         app_name_caption.setObjectName('app_name_caption')
         app_name_layout.addWidget(app_name_caption)
 
         frame_layout.addWidget(app_name_widget, 0, 2, Qt.AlignmentFlag.AlignLeft, 2)
 
         # Information fields
         info_fields = [
-            (self.lexemes.get('popup_about_version'), AppConfig.get_app_version(), []),
-            (self.lexemes.get('popup_about_license'), AppConfig.get_app_license(), []),
-            (self.lexemes.get('popup_about_website'), AppConfig.get_app_website(),
-             [{'icon': 'box-arrow-up-right.svg', 'link': AppConfig.get_app_website()}]),
-            (self.lexemes.get('popup_about_repository'), AppConfig.get_app_repository(),
-             [{'icon': 'star-fill.svg', 'link': AppConfig.get_app_repository()}]),
-            (self.lexemes.get('popup_about_pypi'), AppConfig.get_app_pypi(),
-             [{'icon': 'box-arrow-up-right.svg', 'link': AppConfig.get_app_pypi()}]),
-            (self.lexemes.get('popup_about_date'), AppConfig.get_app_date(), [])
+            (self.lexemes.get('popup_about_version'), AppConfig().get_app_version(), []),
+            (self.lexemes.get('popup_about_license'), AppConfig().get_app_license(), []),
+            (self.lexemes.get('popup_about_website'), AppConfig().get_app_website(),
+             [{'icon': 'box-arrow-up-right.svg', 'link': AppConfig().get_app_website()}]),
+            (self.lexemes.get('popup_about_repository'), AppConfig().get_app_repository(),
+             [{'icon': 'star-fill.svg', 'link': AppConfig().get_app_repository()}]),
+            (self.lexemes.get('popup_about_pypi'), AppConfig().get_app_pypi(),
+             [{'icon': 'box-arrow-up-right.svg', 'link': AppConfig().get_app_pypi()}]),
+            (self.lexemes.get('popup_about_date'), AppConfig().get_app_date(), [])
         ]
 
         for i, row in enumerate(info_fields):
             label, value, value_icons = row
             # Label widget
             label_widget = QLabel(f"{label}:", self)
             label_widget.sizeHint()
```

### Comparing `notolog-0.9.1b4/notolog/ui/ai_assistant.py` & `notolog-0.9.1b6/notolog/ui/ai_assistant.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 from PySide6.QtWidgets import QDialog, QVBoxLayout, QWidget, QLineEdit, QTextEdit, QPushButton
 from PySide6.QtWidgets import QLabel, QSizePolicy, QHBoxLayout
 from PySide6.QtGui import QPixmap
 
 import json
 import logging
 
+from typing import Union
+
 from . import Settings
 from . import AppConfig
 from . import Lexemes
 from . import ThemeHelper
 
 from .vertical_line_spacer import VerticalLineSpacer
 
@@ -39,16 +41,16 @@
         self.parent = parent
 
         # Apply font from the dialog instance to the label
         self.setFont(self.parent.font())
 
         self.logger = logging.getLogger('ai_assistant')
 
-        self.logging = AppConfig.get_logging()
-        self.debug = AppConfig.get_debug()
+        self.logging = AppConfig().get_logging()
+        self.debug = AppConfig().get_debug()
 
         self.settings = Settings(parent=self)
 
         # TODO add more AI providers and a setting of which one is in use
         self.api_url = self.settings.ai_config_openai_url
         self.api_key = self.settings.ai_config_openai_key
         self.inference_model = AiModelNames.__getitem__(self.settings.ai_config_openai_model).value
@@ -61,14 +63,27 @@
         # Default language setup, change to settings value to modify it via UI
         self.lexemes = Lexemes(self.settings.app_language, default_scope='ai_assistant')
 
         self.layout = QVBoxLayout(self)
 
         self.setWindowTitle(self.lexemes.get('dialog_title'))
 
+        # UI element variables
+        self.prompt_input = Union[QLineEdit, None]
+        self.response_output = Union[QTextEdit, None]
+        self.background_label = Union[QLabel, None]
+        self.model_label = Union[QLabel, None]
+        self.tokens_prompt_label = Union[QLabel, None]
+        self.tokens_answer_label = Union[QLabel, None]
+        self.tokens_total_label = Union[QLabel, None]
+        self.send_button = Union[QPushButton, None]
+
+        self.init_ui()
+
+    def init_ui(self):
         # Set dialog size derived from the main window size
         main_window_size = self.parent.size()
         dialog_width = int(main_window_size.width() * 0.5)
         dialog_height = int(main_window_size.height() * 0.5)
         # self.setMinimumSize(dialog_width, dialog_height)
         self.resize(dialog_width, dialog_height)
```

### Comparing `notolog-0.9.1b4/notolog/ui/color_picker_dialog.py` & `notolog-0.9.1b6/notolog/ui/color_picker_dialog.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 
         self.parent = parent
 
         self.settings = Settings(parent=self)
 
         self.logger = logging.getLogger('color_picker_dialog')
 
-        self.logging = AppConfig.get_logging()
-        self.debug = AppConfig.get_debug()
+        self.logging = AppConfig().get_logging()
+        self.debug = AppConfig().get_debug()
 
         # Default language setup, change to settings value to modify it via UI
         self.lexemes = Lexemes(self.settings.app_language, default_scope='color_picker_dialog')
 
         self.setWindowTitle(self.lexemes.get('color_picker_title'))
         self.setCursor(Qt.CursorShape.PointingHandCursor)
```

### Comparing `notolog-0.9.1b4/notolog/ui/common_dialog.py` & `notolog-0.9.1b6/notolog/ui/common_dialog.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from . import AppConfig
 
 import logging
 
 
 class CommonDialog(QDialog):
 
-    debug = AppConfig.get_debug()
+    logging = AppConfig().get_logging()
+    debug = AppConfig().get_debug()
 
     def __init__(self, title=str, text=str, callback=None, parent=None):
         super().__init__(parent)
 
         self.parent = parent
 
         if self.parent and hasattr(self.parent, 'font'):
```

### Comparing `notolog-0.9.1b4/notolog/ui/enum_combo_box.py` & `notolog-0.9.1b6/notolog/ui/enum_combo_box.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/ui/file_system_model.py` & `notolog-0.9.1b6/notolog/ui/file_system_model.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/ui/line_numbers.py` & `notolog-0.9.1b6/notolog/ui/line_numbers.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         QWidget.__init__(self, editor)
 
         self.editor = editor
 
         """
         # Alternatively it can be get from AppConfig:
         font = QFont()
-        font.setPointSize(AppConfig.get_font_size())
+        font.setPointSize(AppConfig().get_font_size())
         self.setFont(font)
         """
         self.setFont(self.editor.document().defaultFont())  # Set global font to the line area
 
         # Theme helper
         self.theme_helper = ThemeHelper()
```

### Comparing `notolog-0.9.1b4/notolog/ui/rename_file_dialog.py` & `notolog-0.9.1b6/notolog/ui/rename_file_dialog.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,16 +20,16 @@
             # Apply font from the main window to the dialog
             self.setFont(self.parent.font())
 
         self.settings = Settings(parent=self)
 
         self.logger = logging.getLogger('rename_file_dialog')
 
-        self.logging = AppConfig.get_logging()
-        self.debug = AppConfig.get_debug()
+        self.logging = AppConfig().get_logging()
+        self.debug = AppConfig().get_debug()
 
         # Default language setup, change to settings value to modify it via UI
         self.lexemes = Lexemes(self.settings.app_language, default_scope='common')
 
         self.init_ui()
 
     def init_ui(self):
```

### Comparing `notolog-0.9.1b4/notolog/ui/rotating_label.py` & `notolog-0.9.1b6/notolog/ui/rotating_label.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/notolog/ui/settings_dialog.py` & `notolog-0.9.1b6/notolog/ui/settings_dialog.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,16 @@
         # Use parent's settings to allow the Settings emitted signals to be caught
         self.settings = self.parent.settings  # type: ignore
 
         self.theme_helper = ThemeHelper()
 
         self.logger = logging.getLogger('settings_dialog')
 
-        self.logging = AppConfig.get_logging()
-        self.debug = AppConfig.get_debug()
+        self.logging = AppConfig().get_logging()
+        self.debug = AppConfig().get_debug()
 
         # Default language setup, change to settings value to modify it via UI
         self.lexemes = Lexemes(self.settings.app_language, default_scope='settings_dialog')
 
         self.setWindowTitle(self.lexemes.get('window_title'))
 
         self.setSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
@@ -162,15 +162,16 @@
             {"type": QLabel, "name": "settings_dialog_general_app_font_size_label",
              "alignment": Qt.AlignmentFlag.AlignLeft, "style": {"bold": True},
              "text": self.lexemes.get('general_app_font_size_label', size=self.settings.app_font_size),
              "callback": lambda obj: tab_general_layout.addWidget(obj, alignment=Qt.AlignmentFlag.AlignTop)},
             {"type": QSlider, "args": [Qt.Orientation.Horizontal],
              "props": {'setFocusPolicy': Qt.FocusPolicy.StrongFocus, 'setTickPosition': QSlider.TickPosition.TicksAbove,
                        'setTickInterval': 5, 'setSingleStep': 1,
-                       'setMinimum': AppConfig.get_font_min_size(), 'setMaximum': AppConfig.get_font_max_size()},
+                       'setMinimum': AppConfig().get_font_min_size(),
+                       'setMaximum': AppConfig().get_font_max_size()},
              "name": "settings_dialog_general_app_font_size_slider:app_font_size",  # Lexeme key : Object name
              "callback": lambda obj: tab_general_layout.addWidget(obj),
              "accessible_description":
                  self.lexemes.get('general_app_font_size_slider_accessible_description')},
             # Spacer to keep elements above on top
             {"type": QWidget, "name": None, "size_policy": (QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding),
              "callback": lambda obj: tab_general_layout.addWidget(obj)},
```

### Comparing `notolog-0.9.1b4/notolog/ui/sort_filter_proxy_model.py` & `notolog-0.9.1b6/notolog/ui/sort_filter_proxy_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 class SortFilterProxyModel(QSortFilterProxyModel):
 
     def __init__(self, extensions: list = None, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.logger = logging.getLogger('sort_filter_proxy_model')
 
-        self.debug = AppConfig.get_debug()
+        self.logging = AppConfig().get_logging()
+        self.debug = AppConfig().get_debug()
 
         self._extensions = extensions  # Allow specific file extensions
 
     def get_extensions(self):
         # Get allowed file extensions
         return self._extensions
```

### Comparing `notolog-0.9.1b4/notolog/ui/statusbar.py` & `notolog-0.9.1b6/notolog/ui/statusbar.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
         if self.parent and hasattr(self.parent, 'font'):
             # Apply font from the dialog instance to the label
             self.setFont(self.parent.font())
 
         self.logger = logging.getLogger('statusbar')
 
-        self.logging = AppConfig.get_logging()
-        self.debug = AppConfig.get_debug()
+        self.logging = AppConfig().get_logging()
+        self.debug = AppConfig().get_debug()
 
         self.settings = Settings(parent=self)
 
         self.theme_helper = ThemeHelper()
 
         # Default language setup, change to settings value to modify it via UI
         self.lexemes = Lexemes(self.settings.app_language, default_scope='statusbar')
```

### Comparing `notolog-0.9.1b4/notolog/ui/toolbar.py` & `notolog-0.9.1b6/notolog/ui/toolbar.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 
         if self.parent and hasattr(self.parent, 'font'):
             # Apply font from the main window to the dialog
             self.setFont(self.parent.font())
 
         self.logger = logging.getLogger('toolbar')
 
-        self.logging = AppConfig.get_logging()
-        self.debug = AppConfig.get_debug()
+        self.logging = AppConfig().get_logging()
+        self.debug = AppConfig().get_debug()
 
         self.actions = actions if actions else {}
         self.buttons = buttons if buttons else {}
         self.refresh = refresh
 
         self.settings = Settings()
```

### Comparing `notolog-0.9.1b4/notolog/view_decorator.py` & `notolog-0.9.1b6/notolog/view_decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,16 +41,16 @@
         Args:
             highlighter (Union[QSyntaxHighlighter, ViewHighlighter]):
             Highlighter that holds document to apply any modifications.
         """
         self.highlighter = highlighter
         self.doc = self.highlighter.document()
 
-        self.logging = AppConfig.get_logging()
-        self.debug = AppConfig.get_debug()
+        self.logging = AppConfig().get_logging()
+        self.debug = AppConfig().get_debug()
 
         self.settings = Settings()
 
         self.logger = logging.getLogger('view_decorator')
 
         if self.debug:
             self.logger.info('Characters count %d' % self.doc.characterCount())
```

### Comparing `notolog-0.9.1b4/notolog/view_processor.py` & `notolog-0.9.1b6/notolog/view_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,16 @@
         Args:
             highlighter (Union[QSyntaxHighlighter, ViewHighlighter]):
             Highlighter that holds document to apply any modifications.
         """
         self.highlighter = highlighter
         self.doc = self.highlighter.document()
 
-        self.logging = AppConfig.get_logging()
-        self.debug = AppConfig.get_debug()
+        self.logging = AppConfig().get_logging()
+        self.debug = AppConfig().get_debug()
 
         self.settings = Settings()
 
         self.logger = logging.getLogger('view_processor')
 
         # Default language setup, change to settings value to modify it via UI
         self.lexemes = Lexemes(self.settings.app_language, default_scope='common')
@@ -243,20 +243,19 @@
                 summary = self.lexemes.get('expandable_block_default_title')
                 if match:
                     summary = f"{match.group(1).strip()}"
                     pos_open_summary = match.start()
                     pos_close_summary = match.end()
                     selected_text = selected_text[:pos_open_summary] + selected_text[pos_close_summary:]
 
-                """
-                There is a possible situation where the formatted html may become invalid.
-                Say, "<p>...\n<details> </p>\n\n<summary>". That's because of markdown lib may process paragraph that way.
-                Double check it with with a something like exp below, but keep in mind the open tag is also exists:
-                pattern = r"<details.*?>[\s]*?(</p>)"
-                """
+                # There is a possible situation where the formatted html may become invalid.
+                # Say, "<p>...\n<details> </p>\n\n<summary>".
+                # That's because of markdown lib may process paragraph that way.
+                # Double check it with a something like exp below, but keep in mind the open tag is also exists:
+                # pattern = r"<details.*?>[\s]*?(</p>)"
 
                 selected_text = selected_text.strip()
                 encoded_text = base64.b64encode(selected_text.encode('utf-8'))
                 """
                 Insert as a TEXT here, not as an HTML or tags will be stripped after.
                 Place extra spaces on each side to allow smooth anchor detection upon click.
                 """
```

### Comparing `notolog-0.9.1b4/notolog/view_widget.py` & `notolog-0.9.1b6/notolog/view_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,21 +20,21 @@
         Args:
             parent (optional): Parent object
         """
         super(ViewWidget, self).__init__(parent)
 
         # Get app's global font size
         font = QFont()
-        font.setPointSize(AppConfig.get_font_size())
+        font.setPointSize(AppConfig().get_font_size())
         self.setFont(font)
 
         self.logger = logging.getLogger('view_widget')
 
-        self.logging = AppConfig.get_logging()
-        self.debug = AppConfig.get_debug()
+        self.logging = AppConfig().get_logging()
+        self.debug = AppConfig().get_debug()
 
     def setDocument(self, document):
         # Override setDocument() to allow additional actions like emit the document set signal
         super().setDocument(document)
         # Emit document set signal to notify listeners
         self.content_set.emit()
```

### Comparing `notolog-0.9.1b4/notolog.egg-info/PKG-INFO` & `notolog-0.9.1b6/notolog.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: notolog
-Version: 0.9.1b4
+Version: 0.9.1b6
 Summary: Notolog - Python Markdown Editor
 Home-page: https://github.com/notolog/notolog-editor
 Author: Vadim Bakhrenkov
 License: MIT
 Project-URL: Bug Reports, https://github.com/notolog/notolog-editor/issues
 Project-URL: Source, https://github.com/notolog/notolog-editor/
-Keywords: notolog,python,markdown,editor,ai,text
+Keywords: notolog,python,markdown,editor,ai,text,notes
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
@@ -47,23 +47,24 @@
 Requires-Dist: PySide6_Essentials==6.7.0
 Requires-Dist: pytest==8.2.0
 Requires-Dist: pytest-asyncio==0.23.6
 Requires-Dist: pytest-mock==3.14.0
 Requires-Dist: qasync==0.27.1
 Requires-Dist: shiboken6==6.7.0
 Requires-Dist: tomli==2.0.1
+Requires-Dist: tomli_w==1.0.0
 
-<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-12 13:57:34.333369"}} -->
+<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-19 23:29:34.439703"}} -->
 # Notolog
 
 ![Notolog - Python Markdown Editor](https://raw.githubusercontent.com/notolog/notolog-editor/main/notolog/assets/notolog-example-image.png)
 
 ## Python Markdown Editor
 
-![PyPI - License](https://img.shields.io/pypi/l/notolog)&nbsp;![PyPI - Version](https://img.shields.io/pypi/v/notolog)&nbsp;![PyPI - Python Version](https://img.shields.io/pypi/pyversions/notolog)
+[![PyPI - Version](https://img.shields.io/pypi/v/notolog)](https://pypi.org/project/notolog/) [![GitHub License](https://img.shields.io/github/license/notolog/notolog-editor)](https://github.com/notolog/notolog-editor/blob/master/LICENSE) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/notolog)](https://pypi.org/project/notolog/) [![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/notolog/notolog-editor/tests.yaml)](https://github.com/notolog/notolog-editor/actions/workflows/tests.yaml)
 
 Notolog is an open-source markdown editor developed with Python and PySide6. Born from a personal endeavor to tackle daily programming challenges and deepen Python proficiency, Notolog serves as a proof-of-concept that seamlessly blends simplicity with functionality. It offers an intuitive user experience across various platforms, ensuring users can efficiently manage and edit markdown files with ease.
 
 ---
 
 ![Notolog UI example](https://raw.githubusercontent.com/notolog/notolog-editor/main/docs/notolog-ui-settings.png)
 
@@ -104,19 +105,45 @@
 * AI Assistant UI to get all things you need in one place:
 	* At the moment the OpenAI API is supported with plans to extend support with other providers.
 * Notolog includes specialized highlighting for TODOs. Simply type '@todo something' to mark tasks, enhancing the ability to track and manage future plans efficiently.
 
 There is no classical web engine integration to make overall package more lightweight and to achieve the best possible performance.
 
 
+## Translations
+
+The Notolog Editor supports several language translations out of the box. Here is the list of languages included alongside the default English translation:
+
+* Chinese (Simplified)
+* Dutch
+* Finnish
+* French
+* Georgian
+* German
+* Greek
+* Hindi
+* Italian
+* Japanese
+* Korean
+* Latin
+* Portuguese
+* Russian
+* Spanish
+* Swedish
+* Turkish
+
+Here's an example of what it looks like in the actual UI, featuring the lovely Strawberry theme and Japanese translation:
+
+![Notolog UI translation example](https://raw.githubusercontent.com/notolog/notolog-editor/main/docs/notolog-ui-settings-strawberry-ja.png)
+
 ## Prerequisites
 
 **Python 3.9 or higher installed on your system.**
 
-If you haven't already, download and install Python from the official website [python.org](python.org).
+Ensure Python 3.9 or higher is installed on your system. Visit [python.org](https://python.org) for more details.
 
 Check the version of Python available with this command `python3 -V`.
 
 **pip (Python package installer) should be available.**
 
 You can check if pip is installed by running `pip --version` in your terminal/command prompt.
 
@@ -169,15 +196,15 @@
 ```
 </details>
 
 ### Virtual Environments
 
 The instructions below contain steps of how to set up **venv** virtual environment to run a Python app safely. Starting from Python 3.6 **venv** is a recommended way to create virtual environments. For more information check [Creation of virtual environments](https://docs.python.org/3/library/venv.html). Alternatively, you can execute the Notolog code and set up virtual environment with your favorite Python code editor.
 
-#### MacOS and Linux
+#### Linux and macOS
 
 ##### Set Up Virtual Environment
 1. Open Terminal.
 2. Navigate to your project directory using the cd command.
 3. Create a virtual environment by running `python3 -m venv notolog`. Replace **notolog** with the desired name for your virtual environment.
 
 ##### Activate Virtual Environment:
@@ -259,14 +286,15 @@
 
 - **Bootstrap Icons**: Icons for UI elements. [Project Details](https://icons.getbootstrap.com/), [License Details](https://github.com/twbs/icons/blob/main/LICENSE)
 - **pytest**: Used for unit testing. It provides powerful features like fixtures, assertions, and test parameterization to facilitate writing and running Python tests. [Project Details](https://pytest.org/), [License Details](https://docs.pytest.org/en/8.0.x/license.html)
 - **pytest-mock**: Enhances pytest for unit tests by offering a simple interface to powerful mocking functionalities. [License Details](https://github.com/pytest-dev/pytest-mock/blob/main/LICENSE), [PyPI](https://pypi.org/project/pytest-mock/)
 - **cffi**: Used for interfacing with C code. [License Details](https://github.com/python-cffi/cffi/blob/main/LICENSE), [PyPI](https://pypi.org/project/cffi/)
 - **iniconfig**: For parsing and working with INI configuration files. [License Details](https://github.com/pytest-dev/iniconfig/blob/main/LICENSE), [PyPI](https://pypi.org/project/iniconfig/)
 - **tomli**: A Python library used for parsing TOML configuration files effortlessly. [License Details](https://github.com/hukkin/tomli/blob/master/LICENSE), [PyPI](https://pypi.org/project/tomli/)
+- **tomli_w**: A Python library used for writing TOML configuration files effortlessly. [License Details](https://github.com/hukkin/tomli-w/blob/master/LICENSE), [PyPI](https://pypi.org/project/tomli-w/)
 - **pluggy**: For creating and managing plugin systems in Python applications. [License Details](https://github.com/pytest-dev/pluggy/blob/main/LICENSE), [PyPI](https://pypi.org/project/pluggy/)
 
 #### BSD Licenses
 
 - **Python-Markdown**: Markdown to HTML conversion. [Project Details](https://python-markdown.github.io/), [BSD 3-Clause License](https://github.com/Python-Markdown/markdown/blob/master/LICENSE.md)
 - **Emoji library**: Converts emoji text-code to emojis. [New BSD License](https://github.com/carpedm20/emoji/blob/master/LICENSE.txt), [PyPI](https://pypi.org/project/emoji/)
 - **qasync**: Async support for Python. [BSD 2-Clause "Simplified" License](https://github.com/CabbageDevelopment/qasync/blob/master/LICENSE), [PyPI](https://pypi.org/project/qasync/)
@@ -293,23 +321,49 @@
 
 Please note that while the majority of this project is licensed under the MIT License, certain components may have different licensing terms. Always refer to the documentation of each library for detailed information about its license and terms of use.
 
 ### APIs
 
 #### OpenAI API Disclaimer
 
-**Disclaimer:** This project is independent and neither affiliated with, endorsed by, nor sponsored by OpenAI. Integration of the OpenAI API in this project is provided on an "as is" basis, without any official partnership or endorsement by OpenAI. The creators of this project disclaim all liability for any misuse, harm, or other consequences resulting from the use of the OpenAI API.
+**Disclaimer:** This project is independent and not affiliated with, endorsed by, or sponsored by OpenAI. The integration of the OpenAI API is provided on an "as is" basis, and the creators disclaim all liability for any misuse or consequences resulting from the use of the OpenAI API.
 
-**Usage:** Our project employs the OpenAI API to enhance natural language processing capabilities. Users are required to provide their own OpenAI API keys and should refer to the [OpenAI API reference](https://platform.openai.com/docs/api-reference) for detailed usage guidelines.
+**Usage:** This project uses the OpenAI API to access AI assistant capabilities and enhance natural language processing. Users must provide their own OpenAI API keys and should refer to the [OpenAI API reference](https://platform.openai.com/docs/api-reference) for detailed usage guidelines.
 
-**Responsibility:** Users are responsible for obtaining, configuring, and managing their OpenAI API keys in accordance with OpenAI's terms of service and usage policies.
+**Responsibility:** Users are responsible for obtaining and managing their OpenAI API keys in compliance with OpenAI's terms of service.
 
-**Security:** It is crucial for users to manage their API keys securely, ensuring they are not exposed or shared in public forums.
+**Security:** Users are expected to handle their API keys securely to avoid unauthorized access.
 
 *This section was generated with the assistance of AI to ensure accurate and concise information regarding the use of the OpenAI API.*
 
 ## Security Disclaimer
 
-This application is primarily designed for educational purposes and uses PBKDF2HMAC for key derivation. It employs Fernet, which utilizes AES-128 in CBC mode. The key is initially created at 256 bits but truncated to 128 bits for encryption. The encryption salt and iteration counts are stored unencrypted in the file's header, making this setup suitable for educational and non-critical applications only. As such, while this software provides basic security, it is not intended for high-security needs. Users are encouraged to choose strong passwords to enhance data protection. Distributed under the MIT License, this open-source application requires users to ensure compliance with applicable laws, and the developers disclaim liability for misuse or legal non-compliance.
+This application is designed for educational purposes and offers security features through optional file encryption and protected application settings.
+
+### Optional File Encryption
+
+* **Encryption Details:** The application uses PBKDF2HMAC for key derivation and Fernet for encryption, utilizing AES-128 in CBC mode. Although the key material generated is 256 bits, only the first 128 bits (16 bytes) are used for encryption.
+* **File Headers:** The encryption salt and iteration counts are stored unencrypted in the file's header. This approach is primarily intended for non-critical applications where data exposure has limited risk.
+* **Strong Passwords:** Users are encouraged to use strong passwords to enhance the protection of their encrypted data.
+
+### Protected Application Settings
+
+* **Settings Encryption:** The application may encrypt sensitive data like API keys because these Qt app settings might otherwise be stored as open data. However, the encryption key used is stored on the PC and can be accessed by anyone with physical or user-level access to the computer. This could expose sensitive data to potential unauthorized access.
+
+### General Information
+
+* **Open Source:** This application is open-source and distributed under the MIT License. Users must comply with applicable laws and regulations when using this software.
+* **Liability:** The developers disclaim any liability for misuse or legal non-compliance related to the use of this software.
+
+
+## Code Quality and Test Coverage
+
+To maintain high standards of code quality and ensure comprehensive test coverage, we use several tools:
+
+- **Flake8**: A tool that enforces coding style and checks the quality of Python code by combining PyFlakes, pycodestyle, and McCabe's complexity checker. [MIT License](https://github.com/PyCQA/flake8/blob/main/LICENSE)
+- **coverage**: Measures the effectiveness of tests by showing which parts of your code are being executed and which are not. [Apache License 2.0](https://github.com/nedbat/coveragepy/blob/master/LICENSE.txt)
+- **pytest-cov**: A pytest plugin that provides test coverage reports, extending pytest to measure code coverage alongside running tests. [MIT License](https://github.com/pytest-dev/pytest-cov/blob/master/LICENSE)
+
+These tools help us maintain a clean and reliable codebase by catching potential issues early and documenting where our tests might be lacking.
 
 ---
-This README.md file has been carefully crafted and edited using the Notolog editor itself.
+_This README.md file has been carefully crafted and edited using the Notolog editor itself._
```

### Comparing `notolog-0.9.1b4/notolog.egg-info/SOURCES.txt` & `notolog-0.9.1b6/notolog.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 CHANGELOG.md
 CODE_OF_CONDUCT.md
 LICENSE
 MANIFEST.in
 README.md
-app_config.toml
 requirements.txt
 setup.py
 docs/Examples.md
+docs/notolog-ui-settings-strawberry-ja.png
 docs/notolog-ui-settings.png
 notolog/__init__.py
 notolog/app_config.py
+notolog/async_highlighter.py
 notolog/edit_widget.py
 notolog/editor_state.py
 notolog/etree_extension.py
 notolog/file_header.py
 notolog/file_system_watcher.py
 notolog/image_downloader.py
 notolog/main.py
@@ -143,14 +144,15 @@
 notolog/enums/languages.py
 notolog/enums/themes.py
 notolog/exceptions/__init__.py
 notolog/exceptions/file_header_empty_exception.py
 notolog/helpers/__init__.py
 notolog/helpers/clipboard_helper.py
 notolog/helpers/file_helper.py
+notolog/helpers/settings_helper.py
 notolog/helpers/theme_helper.py
 notolog/helpers/tooltip_helper.py
 notolog/helpers/update_helper.py
 notolog/highlight/__init__.py
 notolog/highlight/main_highlighter.py
 notolog/highlight/md_highlighter.py
 notolog/highlight/view_highlighter.py
@@ -302,12 +304,14 @@
 tests/test_enc_password.py
 tests/test_file_header.py
 tests/test_html_view.py
 tests/test_lexemes.py
 tests/test_notolog_editor.py
 tests/test_pkg_integration.py
 tests/test_qt_async.py
-tests/test_qt_ui.py
 tests/test_settings.py
 tests/test_text_block_data.py
 tests/test_theme_helper.py
-tests/test_themes.py
+tests/test_themes.py
+tests/ui_tests/__init__.py
+tests/ui_tests/test_ai_assistant.py
+tests/ui_tests/test_qt_ui.py
```

### Comparing `notolog-0.9.1b4/setup.py` & `notolog-0.9.1b6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Read the contents of README file
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='notolog',
-    version='0.9.1b4',
+    version='0.9.1b6',
     description='Notolog - Python Markdown Editor',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/notolog/notolog-editor',
     author='Vadim Bakhrenkov',
     license='MIT',
     # py_modules=['main'],  # This refers to the standalone 'main.py' at the top-level directory
@@ -49,9 +49,9 @@
     include_package_data=True,  # Include data files specified in MANIFEST.in
     python_requires='>=3.9, <4',
     install_requires=[line.strip() for line in open("requirements.txt", "r")],
     project_urls={
         'Bug Reports': 'https://github.com/notolog/notolog-editor/issues',
         'Source': 'https://github.com/notolog/notolog-editor/',
     },
-    keywords='notolog, python, markdown, editor, ai, text',
+    keywords='notolog, python, markdown, editor, ai, text, notes',
 )
```

### Comparing `notolog-0.9.1b4/tests/test_enc_helper.py` & `notolog-0.9.1b6/tests/test_enc_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,17 @@
         yield _enc_password
 
     @pytest.fixture(scope="function", autouse=True)
     def test_obj_enc_helper(self, mocker, test_obj_enc_password, request):
         # Get the parameter value(s) from the request
         salt, iterations = request.param
 
+        # Force fallback default to avoid settings default
+        mocker.patch.object(EncHelper, 'get_default_iterations', return_value=EncHelper.DEFAULT_ITERATIONS)
+
         mocker.patch('secrets.token_urlsafe', return_value='RANDOM_SALT')
         _helper = EncHelper(enc_password=test_obj_enc_password, salt=salt, iterations=iterations)
 
         yield _helper
 
     @pytest.fixture(scope="function")
     def test_exp_params_fixture(self, request):
```

### Comparing `notolog-0.9.1b4/tests/test_enc_password.py` & `notolog-0.9.1b6/tests/test_enc_password.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/tests/test_file_header.py` & `notolog-0.9.1b6/tests/test_file_header.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from notolog.file_header import FileHeader
 
 from notolog.exceptions.file_header_empty_exception import FileHeaderEmptyException
 
 from logging import Logger
 
+import time
 import pytest
 
 
 class TestFileHeader:
 
     @pytest.fixture(scope="function")
     def test_obj_file_header_empty(self):
@@ -62,25 +63,27 @@
         assert test_obj_file_header_new.set_param('created', 'Smth-to-Test') is None
         assert test_obj_file_header_new.get_param('created') == 'Smth-to-Test'
 
         # Save created and updated params
         created = test_obj_file_header_new.get_param('created')
         updated = test_obj_file_header_new.get_param('updated')
         # Refresh the header
+        time.sleep(0.1)
         test_obj_file_header_new.refresh()
         # Check update has changed
         assert test_obj_file_header_new.get_param('created') == created
         assert test_obj_file_header_new.get_param('updated') != updated
 
         # Save created and updated params
         created = test_obj_file_header_new.get_param('created')
         updated = test_obj_file_header_new.get_param('updated')
         # Reset created param
         test_obj_file_header_new.set_param('created', None)
         # Refresh the header
+        time.sleep(0.1)
         test_obj_file_header_new.refresh()
         # Check update has changed
         assert test_obj_file_header_new.get_param('created') is not None
         assert test_obj_file_header_new.get_param('created') != created
         assert test_obj_file_header_new.get_param('updated') != updated
 
         # Just to check the method reads first line of the file, check the current one
```

### Comparing `notolog-0.9.1b4/tests/test_html_view.py` & `notolog-0.9.1b6/tests/test_html_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         "test_obj_doc, test_text_fixture, test_style_fixture",
         [
             (("<b>Test text bold</b>", "setHtml"), "text", "bold"),
             (("<i>Test text italic</i>", "setHtml"), "text", "italic"),
             (("<u>Test text underline</u>", "setHtml"), "text", "underline"),
             (("<s>Test text strikethrough</s>", "setHtml"), "text", "strikeOut"),
             #(("~~Test text strikethrough~~", "setHtml"), "text", "strikeOut"), # TODO decorator result
-            # Markdown is a proof of concept here as not in use for result render
+            # Markdown is a proof of concept here as it is not in use for result rendering
             (("**Test text bold**", "setMarkdown"), "text", "bold"),
             (("*Test text bold*", "setMarkdown"), "text", "italic"),
             (("***Test text bold***", "setMarkdown"), "text", "bold"),
             (("***Test text bold***", "setMarkdown"), "text", "italic"),
             (("~~Test text strikethrough~~", "setMarkdown"), "text", "strikeOut"),
         ],
         indirect=True
```

### Comparing `notolog-0.9.1b4/tests/test_lexemes.py` & `notolog-0.9.1b6/tests/test_lexemes.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/tests/test_notolog_editor.py` & `notolog-0.9.1b6/tests/test_notolog_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         # Current working directory
         # test_run_from_dir = os.getcwd()
         test_file_dir = os.path.dirname(os.path.realpath(__file__))
         test_file_parent_dir = os.path.dirname(test_file_dir)
         # Assert that the method was called once
         mock_method1.assert_not_called()
         # Assert that the method was called once with the param(s)
-        mock_method2.assert_called_once_with('%s/README.md' % test_file_parent_dir)
+        mock_method2.assert_called_once_with(os.path.normpath('%s/README.md') % test_file_parent_dir)
 
     def test_notolog_editor_load_default_page_any(self, mocker, test_obj_notolog_editor, test_obj_settings):
         """
         Check that an any page is loaded instead of default page
         @param mocker: pytest fixture
         @param test_obj_notolog_editor: NotologEditor instance
         @param test_obj_settings: Settings instance
```

### Comparing `notolog-0.9.1b4/tests/test_pkg_integration.py` & `notolog-0.9.1b6/tests/test_pkg_integration.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/tests/test_qt_ui.py` & `notolog-0.9.1b6/tests/ui_tests/test_qt_ui.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,39 @@
+# tests/ui/test_qt_ui.py
+
 from PySide6.QtCore import Qt
-from PySide6.QtWidgets import QApplication
 from PySide6.QtTest import QTest
 
 from notolog.notolog_editor import NotologEditor
-from notolog.enums.languages import Languages
 from notolog.settings import Settings
+from notolog.enums.languages import Languages
+
+from . import test_app
 
-import os
-import sys
 import pytest
 
 
 class TestQtUi:
 
-    @pytest.fixture(autouse=True, scope="session")
-    def qt_app(self):
-        # Check to avoid:
-        # RuntimeError: Please destroy the QApplication singleton before creating a new QApplication instance.
-        app = QApplication.instance()
-        if not app:
-            # Force Qt style override
-            """
-            QApplication: invalid style override 'kvantum' passed, ignoring it.
-                Available styles: Windows, Fusion
-            """
-            os.environ["QT_STYLE_OVERRIDE"] = "Fusion"
-            # Fixture to initialize QApplication.
-            app = QApplication(sys.argv)
-
-        yield app
-
-        # Properly close the QApplication after each test
-        app.quit()
-
     @pytest.fixture
-    def settings_obj(self, qt_app):
+    def settings_obj(self):
         # Fixture to create and return settings instance
         settings = Settings()
         yield settings
 
     @pytest.fixture
-    def main_window(self, mocker, qt_app):
+    def main_window(self, mocker, test_app):
         # Force to override system language as a default
         mocker.patch.object(Languages, 'default', return_value='la')
 
+        # Do not show actual window; return object instance only
+        mocker.patch.object(NotologEditor, 'show', return_value=None)
+
         # Fixture to create and return main window instance
-        window = NotologEditor(screen=qt_app.screens()[0])
+        window = NotologEditor(screen=test_app.screens()[0])
         yield window
 
     def test_editor_state(self, main_window, settings_obj):
         # Check app language set correctly
         assert settings_obj.app_language == 'la'
 
         # Check default window title
```

### Comparing `notolog-0.9.1b4/tests/test_text_block_data.py` & `notolog-0.9.1b6/tests/test_text_block_data.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b4/tests/test_theme_helper.py` & `notolog-0.9.1b6/tests/test_theme_helper.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,47 @@
 # tests/test_themes.py
 
 from notolog.helpers.theme_helper import ThemeHelper
-from notolog.enums.themes import Themes
 from notolog.theme import Theme
 from notolog.settings import Settings
 from notolog.app_config import AppConfig
 
 from logging import Logger
 
 import os
 import pytest
 
 
 class TestThemeHelper:
 
-    @pytest.fixture(scope="function", autouse=True)
-    def test_settings_fixture(self):
-
-        settings = Settings()
-
-        yield settings
+    @pytest.fixture(autouse=True)
+    def test_settings_fixture(self, request):
+        setting = Settings()
+        # Get the parameter value(s) from the request
+        setting.app_theme = request.param
+        yield setting
 
-    @pytest.fixture(scope="function", autouse=True)
-    def test_obj_theme_helper(self, test_settings_fixture, mocker, request):
+    @pytest.fixture(autouse=True)
+    def test_obj_theme_helper(self, mocker, test_settings_fixture):
         """
         Testing object fixture.
         May contain minimal logic for testing purposes.
         """
 
-        # Get the parameter value(s) from the request
-        theme = request.param if hasattr(request, 'param') else None
-
         mocker.patch.object(AppConfig, 'get_debug', return_value=False)
-        # Or: monkeypatch.setattr(Settings, 'theme', theme)
-        # mocker.patch('app.settings.Settings.app_theme', theme)
-        test_settings_fixture.app_theme = theme
 
         """
         If themes dir is set read themes from there.
         For test purposes to check theme files are readable.
         """
         test_themes_dir = os.path.join(os.path.dirname(__file__), 'test_themes')
         mocker.patch.object(Theme, 'get_themes_dir', return_value=test_themes_dir)
 
         # Allow to change theme name during test cycle with no caching
-        AppConfig.set_test_mode(True)
+        AppConfig().set_test_mode(True)
 
         yield ThemeHelper()
 
     @pytest.fixture(scope="function")
     def test_exp_params_fixture(self, request):
         """
         Fixture to pass params and get expected results.
@@ -57,71 +50,71 @@
 
         # Get the parameter value(s) from the request
         param_values = request.param
 
         yield param_values
 
     @pytest.mark.parametrize(
-        "test_obj_theme_helper, test_exp_params_fixture",
+        "test_settings_fixture, test_obj_theme_helper, test_exp_params_fixture",
         [
-            ((None), ('default')),
-            ((''), ('default')),
-            (('default'), ('default')),  # Because of method default()
-            (('DEFAULT'), ('default')),
-            (('anyval'), ('default')),
+            ((None), (None), ('default')),
+            ((''), (None), ('default')),
+            (('default'), (None), ('default')),  # Because of method default()
+            (('DEFAULT'), (None), ('default')),
+            (('anyval'), (None), ('default')),
         ],
         indirect=True
     )
-    def test_theme_helper_init(self, test_obj_theme_helper, test_exp_params_fixture):
+    def test_theme_helper_init(self,test_settings_fixture,  test_obj_theme_helper, test_exp_params_fixture):
         """
         Test and check initial params are exist in the testing object.
         """
         assert isinstance(test_obj_theme_helper.logger, Logger)
 
         exp_theme = test_exp_params_fixture
 
         assert hasattr(test_obj_theme_helper, 'theme')
         assert isinstance(test_obj_theme_helper.theme, Theme)
         assert isinstance(test_obj_theme_helper.settings, Settings)
         assert test_obj_theme_helper.theme.theme == exp_theme
 
     @pytest.mark.parametrize(
-        "test_obj_theme_helper, test_exp_params_fixture",
+        "test_settings_fixture, test_obj_theme_helper, test_exp_params_fixture",
         [
-            (None, (None, None, None)),
-            ('default', ('test_red', None, 0xFF0000)),
-            ('default', ('test_green', True, '#00FF00')),
-            ('default', ('test_blue', False, 0x0000FF)),
-            ('default', ('test_undefined', None, None)),
+            (None, None, (None, None, None)),
+            ('default', None, ('test_red', None, 0xFF0000)),
+            ('default', None, ('test_green', True, '#00FF00')),
+            ('default', None, ('test_blue', False, 0x0000FF)),
+            ('default', None, ('test_undefined', None, None)),
             # 'noir_dark' is real as it can be checked with Themes enum
-            ('noir_dark', ('test_non_red', False, 0x00FFFF)),
-            ('noir_dark', ('test_light', True, '#FFFFFF')),
-            ('test_undefined', (None, None, None)),
-            ('test_undefined', ('undefined_name', True, None)),
+            ('noir_dark', None, ('test_non_red', False, 0x00FFFF)),
+            ('noir_dark', None, ('test_light', True, '#FFFFFF')),
+            ('test_undefined', None, (None, None, None)),
+            ('test_undefined', None, ('undefined_name', True, None)),
         ],
         indirect=True
     )
-    def test_themes_get_color(self, test_obj_theme_helper, test_exp_params_fixture):
+    def test_themes_get_color(self, test_settings_fixture, test_obj_theme_helper, test_exp_params_fixture):
         """
         Test getter for correctly loaded and really existent theme's colors.
         """
         param_name, param_css_format, exp_result = test_exp_params_fixture
 
         assert test_obj_theme_helper.get_color(param_name, param_css_format) == exp_result
 
     @pytest.mark.parametrize(
-        "test_obj_theme_helper, test_exp_params_fixture",
+        "test_settings_fixture, test_obj_theme_helper, test_exp_params_fixture",
         [
-            (None, (None, None)),
-            ('default', ('test_smth', None)),
-            ('default', ('test_styles', 'QTextEdit {}')),
-            ('noir_dark', ('test_smth', 'QTextEdit {}')),
+            (None, None, (None, None)),
+            ('default', None, ('test_smth', None)),
+            ('default', None, ('test_styles', 'QTextEdit {}')),
+            ('noir_dark', None, ('test_smth', 'QTextEdit {}')),
         ],
         indirect=True
     )
-    def test_themes_get_css(self, test_obj_theme_helper, test_exp_params_fixture):
+    def test_themes_get_css(self, test_settings_fixture, test_obj_theme_helper, test_exp_params_fixture):
         """
         Test getter for correctly loaded and really existent theme's css files.
         """
         param_css_name, exp_result = test_exp_params_fixture
 
         assert test_obj_theme_helper.get_css(param_css_name) == exp_result
```

### Comparing `notolog-0.9.1b4/tests/test_themes.py` & `notolog-0.9.1b6/tests/test_themes.py`

 * *Files 8% similar despite different names*

```diff
@@ -104,15 +104,17 @@
 
         assert test_obj_themes.get_themes_dir() == exp_themes_dir
 
     def test_themes_get_default_theme_dir(self, test_obj_themes):
         """
         Test default theme dir path.
         """
-        exp_themes_dir = 'test_themes/default'
+
+        # Use os.sep to ensure correct path separators on each OS, or os.path.normpath() to normalize path separators
+        exp_themes_dir = 'test_themes' + os.sep + 'default'
 
         default_theme_dir_parts = test_obj_themes.get_default_theme_dir().split(os.path.sep)[-2:]
 
         assert os.path.join(*default_theme_dir_parts) == exp_themes_dir
 
     @pytest.mark.parametrize(
         "test_obj_themes, test_exp_params_fixture",
@@ -160,17 +162,17 @@
         assert hasattr(test_obj_themes, 'theme')
         assert test_obj_themes.theme == exp_theme
         assert test_obj_themes.get_colors() == exp_colors
 
     @pytest.mark.parametrize(
         "test_obj_themes, test_exp_params_fixture",
         [
-            (None, ('default', {'test_styles': 'default/test_styles.css'})),
-            ('default', ('default', {'test_styles': 'default/test_styles.css'})),
-            ('noir_dark', ('noir_dark', {'test_smth': 'noir_dark/test_smth.css'})),
+            (None, ('default', {'test_styles': os.path.normpath('default/test_styles.css')})),
+            ('default', ('default', {'test_styles': os.path.normpath('default/test_styles.css')})),
+            ('noir_dark', ('noir_dark', {'test_smth': os.path.normpath('noir_dark/test_smth.css')})),
         ],
         indirect=True
     )
     def test_themes_get_theme_css(self, mocker, test_obj_themes, test_exp_params_fixture):
         """
         Test actual theme colors loaded.
         """
```

