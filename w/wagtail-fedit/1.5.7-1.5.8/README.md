# Comparing `tmp/wagtail_fedit-1.5.7.tar.gz` & `tmp/wagtail_fedit-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.5.7.tar", last modified: Sat May 18 16:17:52 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.5.8.tar", last modified: Mon May 20 10:25:28 2024, max compression
```

## Comparing `wagtail_fedit-1.5.7.tar` & `wagtail_fedit-1.5.8.tar`

### file list

```diff
@@ -1,137 +1,138 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.286909 wagtail_fedit-1.5.7/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.7/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.7/MANIFEST.in
--rw-rw-rw-   0        0        0     3010 2024-05-18 16:17:52.286909 wagtail_fedit-1.5.7/PKG-INFO
--rw-rw-rw-   0        0        0     1812 2024-04-28 14:18:11.000000 wagtail_fedit-1.5.7/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.7/pyproject.toml
--rw-rw-rw-   0        0        0     1186 2024-05-18 16:17:52.288414 wagtail_fedit-1.5.7/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.202686 wagtail_fedit-1.5.7/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.7/wagtail_fedit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.218202 wagtail_fedit-1.5.7/wagtail_fedit/adapters/
--rw-rw-rw-   0        0        0      621 2024-05-18 12:37:42.000000 wagtail_fedit-1.5.7/wagtail_fedit/adapters/__init__.py
--rw-rw-rw-   0        0        0    15018 2024-05-18 12:35:51.000000 wagtail_fedit-1.5.7/wagtail_fedit/adapters/base.py
--rw-rw-rw-   0        0        0     6666 2024-05-18 12:36:09.000000 wagtail_fedit-1.5.7/wagtail_fedit/adapters/block.py
--rw-rw-rw-   0        0        0     8779 2024-05-18 12:37:14.000000 wagtail_fedit-1.5.7/wagtail_fedit/adapters/field.py
--rw-rw-rw-   0        0        0     2305 2024-04-25 18:28:58.000000 wagtail_fedit-1.5.7/wagtail_fedit/adapters/funcs.py
--rw-rw-rw-   0        0        0     2755 2024-04-25 18:28:49.000000 wagtail_fedit-1.5.7/wagtail_fedit/adapters/misc.py
--rw-rw-rw-   0        0        0     5607 2024-05-07 18:13:59.000000 wagtail_fedit-1.5.7/wagtail_fedit/adapters/models.py
--rw-rw-rw-   0        0        0     1595 2024-04-18 20:22:37.000000 wagtail_fedit-1.5.7/wagtail_fedit/adapters/registry.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.7/wagtail_fedit/apps.py
--rw-rw-rw-   0        0        0     1354 2024-04-25 09:55:56.000000 wagtail_fedit-1.5.7/wagtail_fedit/errors.py
-drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.220364 wagtail_fedit-1.5.7/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0      215 2024-04-23 13:02:23.000000 wagtail_fedit-1.5.7/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.7/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     3269 2024-04-23 13:28:56.000000 wagtail_fedit-1.5.7/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0     4617 2024-04-21 02:08:33.000000 wagtail_fedit-1.5.7/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.174210 wagtail_fedit-1.5.7/wagtail_fedit/locale/
-drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.174210 wagtail_fedit-1.5.7/wagtail_fedit/locale/nl/
-drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.221365 wagtail_fedit-1.5.7/wagtail_fedit/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     7262 2024-04-23 15:50:58.000000 wagtail_fedit-1.5.7/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    15296 2024-04-25 14:19:13.000000 wagtail_fedit-1.5.7/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.222364 wagtail_fedit-1.5.7/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.7/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.223363 wagtail_fedit-1.5.7/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.7/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.7/wagtail_fedit/models.py
--rw-rw-rw-   0        0        0     1626 2024-04-25 13:40:59.000000 wagtail_fedit-1.5.7/wagtail_fedit/settings.py
-drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.176549 wagtail_fedit-1.5.7/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.177549 wagtail_fedit-1.5.7/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.226364 wagtail_fedit-1.5.7/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     5818 2024-05-18 12:31:35.000000 wagtail_fedit-1.5.7/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     5011 2024-05-18 15:36:53.000000 wagtail_fedit-1.5.7/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0     1249 2024-05-18 12:55:22.000000 wagtail_fedit-1.5.7/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.227365 wagtail_fedit-1.5.7/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    55265 2024-05-18 15:44:13.000000 wagtail_fedit-1.5.7/wagtail_fedit/static/wagtail_fedit/js/edit.js
-drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.228366 wagtail_fedit-1.5.7/wagtail_fedit/static/wagtail_fedit/js/licenses/
--rw-rw-rw-   0        0        0     1091 2024-04-23 15:39:19.000000 wagtail_fedit-1.5.7/wagtail_fedit/static/wagtail_fedit/js/licenses/TIPPY.LICENSE
-drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.178548 wagtail_fedit-1.5.7/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.229810 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/
--rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
-drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.232059 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.234060 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      929 2024-04-23 15:23:24.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
--rw-rw-rw-   0        0        0      991 2024-04-23 15:27:54.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
--rw-rw-rw-   0        0        0      601 2024-05-17 08:51:23.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
--rw-rw-rw-   0        0        0      378 2024-05-18 11:23:40.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/content/editable_dom_positioned_adapter.html
-drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.242571 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
--rw-rw-rw-   0        0        0     3699 2024-04-20 21:55:10.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
--rw-rw-rw-   0        0        0      266 2024-04-21 21:15:09.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler.html
--rw-rw-rw-   0        0        0      265 2024-04-21 21:23:24.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler_form.html
--rw-rw-rw-   0        0        0      770 2024-05-18 12:22:37.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
--rw-rw-rw-   0        0        0      455 2024-04-21 00:11:35.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
--rw-rw-rw-   0        0        0      345 2024-05-18 12:28:53.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
--rw-rw-rw-   0        0        0      397 2024-05-18 12:21:43.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe_dom_positioned.html
--rw-rw-rw-   0        0        0     5537 2024-05-18 12:20:21.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      549 2024-05-18 15:36:09.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/editor/field.html
-drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.248567 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/icons/
--rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
--rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
--rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
--rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
--rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
-drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.249750 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.251749 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
--rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
--rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.252750 wagtail_fedit-1.5.7/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.7/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.253750 wagtail_fedit-1.5.7/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.7/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    13170 2024-05-17 09:10:29.000000 wagtail_fedit-1.5.7/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0    10373 2024-05-17 09:10:26.000000 wagtail_fedit-1.5.7/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.254751 wagtail_fedit-1.5.7/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.259778 wagtail_fedit-1.5.7/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/core/apps.py
--rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/core/context_processors.py
-drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.262784 wagtail_fedit-1.5.7/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0    12115 2024-04-20 22:33:35.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      509 2024-04-21 18:41:55.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/core/migrations/0002_basicmodel_related_field.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     6047 2024-04-23 13:09:46.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.270295 wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     8962 2024-04-25 13:24:28.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0    28117 2024-04-25 18:07:06.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/test_adapters.py
--rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/test_generic.py
--rw-rw-rw-   0        0        0     4865 2024-04-23 14:23:09.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/test_model_edit.py
--rw-rw-rw-   0        0        0     1574 2024-04-20 20:49:12.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0     9545 2024-04-20 21:54:40.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/test_submit.py
--rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.275295 wagtail_fedit-1.5.7/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3660 2024-05-18 16:08:35.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/testapp/settings.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.7/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     2220 2024-04-23 14:21:34.000000 wagtail_fedit-1.5.7/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0     1196 2024-04-23 17:25:08.000000 wagtail_fedit-1.5.7/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    18093 2024-05-17 08:53:56.000000 wagtail_fedit-1.5.7/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.279809 wagtail_fedit-1.5.7/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      215 2024-04-23 17:24:50.000000 wagtail_fedit-1.5.7/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     8593 2024-05-17 08:17:48.000000 wagtail_fedit-1.5.7/wagtail_fedit/views/adapters.py
--rw-rw-rw-   0        0        0    17778 2024-04-25 09:19:32.000000 wagtail_fedit-1.5.7/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0     2239 2024-04-25 09:52:47.000000 wagtail_fedit-1.5.7/wagtail_fedit/views/mixins.py
-drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.286909 wagtail_fedit-1.5.7/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      184 2024-04-16 10:03:02.000000 wagtail_fedit-1.5.7/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     1907 2024-05-13 18:26:02.000000 wagtail_fedit-1.5.7/wagtail_fedit/wagtail_hooks/action_menu.py
--rw-rw-rw-   0        0        0     2446 2024-05-07 21:59:49.000000 wagtail_fedit-1.5.7/wagtail_fedit/wagtail_hooks/adapter_hooks.py
--rw-rw-rw-   0        0        0      500 2024-05-18 12:38:10.000000 wagtail_fedit-1.5.7/wagtail_fedit/wagtail_hooks/adapter_registry.py
--rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.7/wagtail_fedit/wagtail_hooks/icons.py
--rw-rw-rw-   0        0        0     3100 2024-05-07 18:11:10.000000 wagtail_fedit-1.5.7/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.7/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     7637 2024-04-23 20:17:24.000000 wagtail_fedit-1.5.7/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-05-18 16:17:52.208195 wagtail_fedit-1.5.7/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0     3010 2024-05-18 16:17:52.000000 wagtail_fedit-1.5.7/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4579 2024-05-18 16:17:52.000000 wagtail_fedit-1.5.7/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 16:17:52.000000 wagtail_fedit-1.5.7/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-05-18 16:17:52.000000 wagtail_fedit-1.5.7/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-18 16:17:52.000000 wagtail_fedit-1.5.7/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 10:25:28.263002 wagtail_fedit-1.5.8/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.8/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     3010 2024-05-20 10:25:28.264004 wagtail_fedit-1.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1812 2024-04-28 14:18:11.000000 wagtail_fedit-1.5.8/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.8/pyproject.toml
+-rw-rw-rw-   0        0        0     1186 2024-05-20 10:25:28.265000 wagtail_fedit-1.5.8/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:25:28.167065 wagtail_fedit-1.5.8/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.8/wagtail_fedit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:25:28.182221 wagtail_fedit-1.5.8/wagtail_fedit/adapters/
+-rw-rw-rw-   0        0        0      455 2024-05-18 21:36:58.000000 wagtail_fedit-1.5.8/wagtail_fedit/adapters/__init__.py
+-rw-rw-rw-   0        0        0    15622 2024-05-19 22:05:36.000000 wagtail_fedit-1.5.8/wagtail_fedit/adapters/base.py
+-rw-rw-rw-   0        0        0    10645 2024-05-20 10:04:42.000000 wagtail_fedit-1.5.8/wagtail_fedit/adapters/block.py
+-rw-rw-rw-   0        0        0     8946 2024-05-19 22:04:41.000000 wagtail_fedit-1.5.8/wagtail_fedit/adapters/field.py
+-rw-rw-rw-   0        0        0     2305 2024-04-25 18:28:58.000000 wagtail_fedit-1.5.8/wagtail_fedit/adapters/funcs.py
+-rw-rw-rw-   0        0        0     2755 2024-04-25 18:28:49.000000 wagtail_fedit-1.5.8/wagtail_fedit/adapters/misc.py
+-rw-rw-rw-   0        0        0     5665 2024-05-19 22:05:27.000000 wagtail_fedit-1.5.8/wagtail_fedit/adapters/models.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.8/wagtail_fedit/apps.py
+-rw-rw-rw-   0        0        0     1354 2024-04-25 09:55:56.000000 wagtail_fedit-1.5.8/wagtail_fedit/errors.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:25:28.184364 wagtail_fedit-1.5.8/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0      215 2024-04-23 13:02:23.000000 wagtail_fedit-1.5.8/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.8/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     3269 2024-04-23 13:28:56.000000 wagtail_fedit-1.5.8/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0     5612 2024-05-18 18:03:06.000000 wagtail_fedit-1.5.8/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:25:28.138780 wagtail_fedit-1.5.8/wagtail_fedit/locale/
+drwxrwxrwx   0        0        0        0 2024-05-20 10:25:28.138780 wagtail_fedit-1.5.8/wagtail_fedit/locale/nl/
+drwxrwxrwx   0        0        0        0 2024-05-20 10:25:28.185484 wagtail_fedit-1.5.8/wagtail_fedit/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     9614 2024-05-19 22:55:13.000000 wagtail_fedit-1.5.8/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    16810 2024-05-19 22:55:04.000000 wagtail_fedit-1.5.8/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-05-20 10:25:28.186485 wagtail_fedit-1.5.8/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.8/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:25:28.187485 wagtail_fedit-1.5.8/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.8/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.8/wagtail_fedit/models.py
+-rw-rw-rw-   0        0        0     1451 2024-05-18 21:38:18.000000 wagtail_fedit-1.5.8/wagtail_fedit/registry.py
+-rw-rw-rw-   0        0        0     1626 2024-04-25 13:40:59.000000 wagtail_fedit-1.5.8/wagtail_fedit/settings.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:25:28.140927 wagtail_fedit-1.5.8/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-05-20 10:25:28.141926 wagtail_fedit-1.5.8/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-05-20 10:25:28.191018 wagtail_fedit-1.5.8/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     5862 2024-05-18 21:44:47.000000 wagtail_fedit-1.5.8/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     4997 2024-05-18 21:47:34.000000 wagtail_fedit-1.5.8/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0     1249 2024-05-18 12:55:22.000000 wagtail_fedit-1.5.8/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-05-20 10:25:28.192409 wagtail_fedit-1.5.8/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    56720 2024-05-20 10:24:52.000000 wagtail_fedit-1.5.8/wagtail_fedit/static/wagtail_fedit/js/edit.js
+drwxrwxrwx   0        0        0        0 2024-05-20 10:25:28.193417 wagtail_fedit-1.5.8/wagtail_fedit/static/wagtail_fedit/js/licenses/
+-rw-rw-rw-   0        0        0     1091 2024-04-23 15:39:19.000000 wagtail_fedit-1.5.8/wagtail_fedit/static/wagtail_fedit/js/licenses/TIPPY.LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-20 10:25:28.142925 wagtail_fedit-1.5.8/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-05-20 10:25:28.194424 wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/
+-rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
+drwxrwxrwx   0        0        0        0 2024-05-20 10:25:28.196418 wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-05-20 10:25:28.199931 wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      929 2024-04-23 15:23:24.000000 wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
+-rw-rw-rw-   0        0        0      991 2024-04-23 15:27:54.000000 wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
+-rw-rw-rw-   0        0        0      742 2024-05-19 21:41:44.000000 wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/content/buttons/move_down.html
+-rw-rw-rw-   0        0        0      738 2024-05-19 21:41:46.000000 wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/content/buttons/move_up.html
+-rw-rw-rw-   0        0        0      601 2024-05-17 08:51:23.000000 wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
+-rw-rw-rw-   0        0        0      378 2024-05-18 11:23:40.000000 wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/content/editable_dom_positioned_adapter.html
+drwxrwxrwx   0        0        0        0 2024-05-20 10:25:28.211130 wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
+-rw-rw-rw-   0        0        0     3699 2024-04-20 21:55:10.000000 wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
+-rw-rw-rw-   0        0        0      266 2024-04-21 21:15:09.000000 wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler.html
+-rw-rw-rw-   0        0        0      265 2024-04-21 21:23:24.000000 wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler_form.html
+-rw-rw-rw-   0        0        0      786 2024-05-18 21:59:44.000000 wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
+-rw-rw-rw-   0        0        0      455 2024-04-21 00:11:35.000000 wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
+-rw-rw-rw-   0        0        0      345 2024-05-18 12:28:53.000000 wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
+-rw-rw-rw-   0        0        0      397 2024-05-18 21:49:55.000000 wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe_dom_positioned.html
+-rw-rw-rw-   0        0        0     5537 2024-05-18 12:20:21.000000 wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      549 2024-05-18 15:36:09.000000 wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+drwxrwxrwx   0        0        0        0 2024-05-20 10:25:28.215743 wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/icons/
+-rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
+-rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
+-rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
+-rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
+-rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
+drwxrwxrwx   0        0        0        0 2024-05-20 10:25:28.217742 wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-05-20 10:25:28.219250 wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+-rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
+-rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-05-20 10:25:28.220257 wagtail_fedit-1.5.8/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.8/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:25:28.223691 wagtail_fedit-1.5.8/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.8/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13210 2024-05-18 21:38:53.000000 wagtail_fedit-1.5.8/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10414 2024-05-18 21:38:48.000000 wagtail_fedit-1.5.8/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:25:28.224692 wagtail_fedit-1.5.8/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.8/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:25:28.229204 wagtail_fedit-1.5.8/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.8/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.8/wagtail_fedit/test/core/apps.py
+-rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.8/wagtail_fedit/test/core/context_processors.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:25:28.232212 wagtail_fedit-1.5.8/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0    12115 2024-04-20 22:33:35.000000 wagtail_fedit-1.5.8/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      509 2024-04-21 18:41:55.000000 wagtail_fedit-1.5.8/wagtail_fedit/test/core/migrations/0002_basicmodel_related_field.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.8/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     6047 2024-04-23 13:09:46.000000 wagtail_fedit-1.5.8/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:25:28.241521 wagtail_fedit-1.5.8/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.8/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     8962 2024-04-25 13:24:28.000000 wagtail_fedit-1.5.8/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0    28222 2024-05-19 20:29:16.000000 wagtail_fedit-1.5.8/wagtail_fedit/test/core/tests/test_adapters.py
+-rw-rw-rw-   0        0        0     4352 2024-05-19 20:28:32.000000 wagtail_fedit-1.5.8/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     7376 2024-05-19 20:53:17.000000 wagtail_fedit-1.5.8/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.8/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.8/wagtail_fedit/test/core/tests/test_generic.py
+-rw-rw-rw-   0        0        0     4865 2024-04-23 14:23:09.000000 wagtail_fedit-1.5.8/wagtail_fedit/test/core/tests/test_model_edit.py
+-rw-rw-rw-   0        0        0     1574 2024-04-20 20:49:12.000000 wagtail_fedit-1.5.8/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0     9545 2024-04-20 21:54:40.000000 wagtail_fedit-1.5.8/wagtail_fedit/test/core/tests/test_submit.py
+-rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.8/wagtail_fedit/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:25:28.247521 wagtail_fedit-1.5.8/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.8/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.8/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3660 2024-05-18 16:08:35.000000 wagtail_fedit-1.5.8/wagtail_fedit/test/testapp/settings.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.8/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.8/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     2220 2024-04-23 14:21:34.000000 wagtail_fedit-1.5.8/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0     1131 2024-05-18 22:43:51.000000 wagtail_fedit-1.5.8/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    18837 2024-05-19 22:26:15.000000 wagtail_fedit-1.5.8/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:25:28.253287 wagtail_fedit-1.5.8/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      215 2024-04-23 17:24:50.000000 wagtail_fedit-1.5.8/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     9078 2024-05-19 20:23:42.000000 wagtail_fedit-1.5.8/wagtail_fedit/views/adapters.py
+-rw-rw-rw-   0        0        0    17734 2024-05-20 09:37:43.000000 wagtail_fedit-1.5.8/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     2239 2024-04-25 09:52:47.000000 wagtail_fedit-1.5.8/wagtail_fedit/views/mixins.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:25:28.262003 wagtail_fedit-1.5.8/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      155 2024-05-18 18:02:59.000000 wagtail_fedit-1.5.8/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     1907 2024-05-13 18:26:02.000000 wagtail_fedit-1.5.8/wagtail_fedit/wagtail_hooks/action_menu.py
+-rw-rw-rw-   0        0        0     2446 2024-05-07 21:59:49.000000 wagtail_fedit-1.5.8/wagtail_fedit/wagtail_hooks/adapter_hooks.py
+-rw-rw-rw-   0        0        0     1173 2024-05-18 21:36:35.000000 wagtail_fedit-1.5.8/wagtail_fedit/wagtail_hooks/adapters.py
+-rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.8/wagtail_fedit/wagtail_hooks/icons.py
+-rw-rw-rw-   0        0        0     4017 2024-05-19 22:47:30.000000 wagtail_fedit-1.5.8/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0     7637 2024-04-23 20:17:24.000000 wagtail_fedit-1.5.8/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:25:28.174065 wagtail_fedit-1.5.8/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0     3010 2024-05-20 10:25:28.000000 wagtail_fedit-1.5.8/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4662 2024-05-20 10:25:28.000000 wagtail_fedit-1.5.8/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 10:25:28.000000 wagtail_fedit-1.5.8/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-20 10:25:28.000000 wagtail_fedit-1.5.8/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-20 10:25:28.000000 wagtail_fedit-1.5.8/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.5.7/LICENSE` & `wagtail_fedit-1.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/PKG-INFO` & `wagtail_fedit-1.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.5.7
+Version: 1.5.8
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `wagtail_fedit-1.5.7/README.md` & `wagtail_fedit-1.5.8/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/setup.cfg` & `wagtail_fedit-1.5.8/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 352e  ..version = 1.5.
-00000030: 370d 0a64 6573 6372 6970 7469 6f6e 203d  7..description =
+00000030: 380d 0a64 6573 6372 6970 7469 6f6e 203d  8..description =
 00000040: 2046 726f 6e74 656e 6420 6564 6974 696e   Frontend editin
 00000050: 6720 666f 7220 796f 7572 2057 6167 7461  g for your Wagta
 00000060: 696c 2073 6974 650d 0a6c 6f6e 675f 6465  il site..long_de
 00000070: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
 00000080: 3a20 5245 4144 4d45 2e6d 640d 0a6c 6f6e  : README.md..lon
 00000090: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
 000000a0: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
```

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/adapters/base.py` & `wagtail_fedit-1.5.8/wagtail_fedit/adapters/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,24 +11,28 @@
 )
 from django.core.signing import (
     Signer,
 )
 from django.http import (
     HttpRequest,
 )
+from wagtail import hooks
 from ..settings import (
     SIGN_SHARED_CONTEXT,
     SHARE_WITH_SESSIONS,
     USE_ADAPTER_SESSION_ID,
     TRACK_LOCALES,
 )
 from ..utils import (
     FeditIFrameMixin,
     wrap_adapter,
 )
+from ..hooks import (
+    REGISTER_ADAPTER_URLS,
+)
 
 if TYPE_CHECKING:
     from ..toolbar import (
         FeditToolbarComponent,
     )
 
 import json, base64, uuid
@@ -221,14 +225,21 @@
             self.field_name     = field_name
             self.meta_field     = object._meta.get_field(field_name)
         else:
             self.field_name     = None
             self.meta_field     = None
 
     @classmethod
+    def on_register(cls, registry):
+        """
+        Called when the adapter is registered.
+        """
+        pass
+
+    @classmethod
     def get_usage_string(cls) -> str:
         """
         Return a string which describes how to use the adapter.
         """
         s = []
         for keyword in cls.keywords:
             s.append(str(keyword))
@@ -350,14 +361,17 @@
         """
         return [
             self.model._meta.app_label,
             self.model._meta.model_name,
             self.object.pk,
             self.field_name,
         ]
+    
+    def wrapped_context(self) -> dict:
+        return {}
 
     def get_element_id(self) -> str:
         """
         Return a unique identifier for the elements on the frontend.
         """
         return content_id_from_parts(
             *self.get_element_id_parts(),
@@ -400,15 +414,15 @@
     def render_content(self, parent_context: dict = None) -> str:
         """
         Render the content for the field.
         This should NOT include the wagtail-fedit wrapper.
         """
         raise NotImplementedError
     
-    def encode_shared_context(self) -> dict:
+    def encode_shared_context(self) -> str:
         """
         Encode a dictionary to a string.
         This will be passed as a GET parameter to the iFrame.
         Make sure the data is not too large.
         """
         if not self.kwargs:
             return ""
@@ -456,25 +470,40 @@
         
         try:
             return Base85_json_loads(context)
         except json.JSONDecodeError:
             pass
         return {}
     
-    
-class BlockFieldReplacementAdapter(BaseAdapter):
-    js_constructor = "wagtail_fedit.editors.BlockFieldEditor"
+        
+class URLMixin:
+    @classmethod
+    def on_register(cls, registry):
+        """
+        Called when the adapter is registered.
+        """
+        @hooks.register(REGISTER_ADAPTER_URLS)
+        def register_admin_urls():
+            return cls.get_admin_urls()
+        
+    @classmethod
+    def get_admin_urls(self) -> list:
+        """
+        Return a list of admin URLs for the adapter.
+        """
+        
+        return []
 
+class BlockFieldReplacementAdapter(BaseAdapter):
     def get_response_data(self, parent_context = None):
         data = super().get_response_data(parent_context)
         data["html"] = wrap_adapter(
             request=self.request,
             adapter=self,
             context=parent_context,
             run_context_processors=True
         )
         return data
 
 class DomPositionedMixin(BaseAdapter):
     template_name = "wagtail_fedit/editor/adapter_iframe_dom_positioned.html"
     editable_template_name  = "wagtail_fedit/content/editable_dom_positioned_adapter.html"
-    js_constructor = "wagtail_fedit.editors.DomPositionedBlockFieldEditor"
```

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/adapters/block.py` & `wagtail_fedit-1.5.8/wagtail_fedit/adapters/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,190 +1,172 @@
-from django.db import models
-from django.utils import translation
 from django.utils.translation import gettext_lazy as _
-from django.utils.functional import cached_property
 from django.http import HttpRequest
+from django.utils import translation
 
 from wagtail.log_actions import log
-from wagtail.blocks import (
-    StreamValue,
-)
 from wagtail.models import (
-    RevisionMixin,
+    Page, RevisionMixin
+)
+from wagtail.admin.panels import (
+    page_utils,
+    model_utils,
+    TabbedInterface,
 )
 
 from .base import (
+    VARIABLES,
+    Keyword,
     BlockFieldReplacementAdapter,
-    DomPositionedMixin,
     AdapterError,
-    Keyword,
-    VARIABLES,
 )
 from ..forms import (
-    blocks as block_forms,
+    PossibleRevisionFormMixin,
+)
+from ..utils import (
+    get_model_string,
 )
-from .. import utils
 from wagtail.admin.admin_url_finder import (
     AdminURLFinder,
 )
 from ..toolbar import (
     FeditAdapterComponent,
     FeditAdapterAdminLinkButton,
 )
 
 
-
-class BlockAdapter(BlockFieldReplacementAdapter):
+class ModelAdapter(BlockFieldReplacementAdapter):
     """
-    An adapter for editing Wagtail blocks.
-    This will render the block and replace it on the frontend
+    An adapter for editing any model.
+    This will render the model and replace it on the frontend
     on successful form submission.
     """
-    identifier = "block"
-    usage_description = "This adapter is used to edit a block of a streamfield."
+    template_name = "wagtail_fedit/editor/adapter_edit_handler.html"
+    identifier = "model"
+    field_required = False
+    js_constructor = "wagtail_fedit.editors.FieldEditor"
+    usage_description = _("This adapter is used for directly editing a model instance.")
     keywords = BlockFieldReplacementAdapter.keywords + (
-        Keyword("block",
-            help_text="the block instance to edit. This can be a regular block instance or a BoundBlock.",
-            type_hint="blocks.Block"
+        Keyword(
+            "admin",
+            absolute=True,
+            help_text="If passed; the adapter will add a quick-link to the Wagtail Admin for this model.",
         ),
-        Keyword("block_id",
+        Keyword(
+            "render_method",
             optional=True,
-            help_text="the ID of the block to edit, required if block is not a BoundBlock.",
-            type_hint="str"
-        ),
-        Keyword("admin",
-            absolute=True,
-            help_text="if passed; the adapter will add a quick- link to the Wagtail Admin for this block."
+            default="render_as_content",
+            help_text="The method to call on the object to render it as content. Default is 'render_as_content'.",
         ),
     )
 
-    def __init__(self, object: models.Model, field_name: str, request: HttpRequest, **kwargs):
+    def __init__(self, object, field_name: str, request: HttpRequest, **kwargs):
         super().__init__(object, field_name, request, **kwargs)
-
-        self.block = self.kwargs.pop("block", None)
-        if self.block:
-            if not hasattr(self.block, "id") and not self.kwargs["block_id"]:
-                raise AdapterError("Invalid block type, block must have an `id` attribute or provide a `block_id`")
-            
-            if hasattr(self.block, "id"):
-                self.kwargs["block_id"] = self.block.id
-
+        if isinstance(self.object, Page):
+            self.edit_handler = page_utils._get_page_edit_handler(
+                self.object.__class__,
+            )
         else:
-            block_id = self.kwargs["block_id"]
-            if block_id is None:
-                raise AdapterError("Block ID is required")
-            
-            self.streamfield: StreamValue = getattr(self.object, self.field_name)
-            result = utils.find_block(block_id, self.streamfield)
-            if not result:
-                raise AdapterError("Block not found; did you provide the correct block ID?")
-            
-            self.block, _ = result
-
-    @cached_property
-    def tooltip(self) -> str:
-        return self.get_header_title()
+            self.edit_handler = model_utils.get_edit_handler(
+                self.object.__class__,
+            )
 
     def get_admin_url(self) -> str:
         finder = AdminURLFinder(self.request.user)
-        url = finder.get_edit_url(self.object)
-        hash = f"#block-{self.kwargs['block_id']}-section"
-        return f"{url}{hash}"
+        return finder.get_edit_url(self.object)
 
     def get_toolbar_buttons(self) -> list[FeditAdapterComponent]:
         buttons = super().get_toolbar_buttons()
         if not self.kwargs["admin"]:
             return buttons
         
         buttons.append(FeditAdapterAdminLinkButton(
             self.request, self,
         ))
         return buttons
 
-    def get_header_title(self):
-
-        model_string = getattr(self.object, "get_admin_display_title", None)
-        if model_string:
-            model_string = model_string()
-        else:
-            model_string = getattr(self.object, "title", str(self.object))
 
-        return _("Edit block %(block_label)s for %(model_name)s '%(model_string)s'") % {
-            "block_label": self.block.block.label,
-            "model_name": self.model._meta.verbose_name,
-            "model_string": model_string,
-        }
-    
-    def get_element_id(self) -> str:
-        return f"block-{self.kwargs['block_id']}-section"
-    
     def get_form_attrs(self) -> dict:
-
-        size = getattr(self.block.block.meta, VARIABLES.PY_SIZE_VAR, None)
-        if size:
-            return super().get_form_attrs() | {
-                VARIABLES.FORM_SIZE_VAR: size,
-            }
-        
-        return {}
+        attrs = super().get_form_attrs()
+        if isinstance(self.edit_handler, TabbedInterface):
+            attrs[VARIABLES.FORM_SIZE_VAR] = "full"
+        elif len(self.edit_handler.children) > 4:
+            attrs[VARIABLES.FORM_SIZE_VAR] = "large"
+        return attrs
     
-    def check_permissions(self):
-        return super().check_permissions() and getattr(
-            self.block.block.meta, "feditable", True
+    def get_form_context(self, **kwargs):
+        context = super().get_form_context(**kwargs)
+        bound_panel = self.edit_handler.get_bound_panel(
+            instance=self.object, request=self.request, form=kwargs["form"],
         )
+        context["edit_handler"] = bound_panel
+        return context
 
-    def get_form(self):
-
-        self.form_class = block_forms.get_block_form_class(self.block.block)
+    @property
+    def form_class(self):
+        cls = self.edit_handler.get_form_class()
+        class RevisionModelForm(PossibleRevisionFormMixin, cls):
+            pass
+        return RevisionModelForm
 
-        if self.request.method == "POST":
-            form = self.form_class(self.request.POST, block=self.block, parent_instance=self.object, request=self.request)
-        else:
-            form = self.form_class(block=self.block, parent_instance=self.object, request=self.request)
-        return form
-    
-    def form_valid(self, form: block_forms.BlockEditForm):
-        self.block = form.save()
+    def form_valid(self, form):
+        self.object = form.save()
 
         extra_log_kwargs = {}
         if isinstance(self.object, RevisionMixin):
             extra_log_kwargs["revision"] = self.object.latest_revision
 
         with translation.override(None):
             log(
                 instance=self.object,
-                action="wagtail_fedit.edit_block",
+                action="wagtail_fedit.edit_model",
                 user=self.request.user,
-                title=self.get_header_title(),
                 data={
-                    "block_id": self.kwargs["block_id"],
-                    "field_name": self.field_name,
-                    "model_id": self.object.pk,
-                    "model_name": self.object._meta.model_name,
-                    "app_label": self.object._meta.app_label,
-                    "verbose_field_name": str(self.meta_field.verbose_name),
-                    "block_label": str(self.block.block.label),
+                    "model_verbose": self.object._meta.verbose_name,
                 },
-                content_changed=True,
+                content_changed=form.has_changed(),
                 **extra_log_kwargs,
             )
 
-    @classmethod
-    def render_from_kwargs(cls, context, **kwargs):
-        if "block" not in kwargs:
-            raise AdapterError("Block is required")
-        
-        block = kwargs.pop("block")
-        if not hasattr(block, "render"):
-            raise AdapterError("Invalid block type, missing render method")
-        
-        return block.render(context)
+    def get_form(self):
+        if self.request.method == "POST":
+            form = self.form_class(self.request.POST, for_user=self.request.user, instance=self.object, request=self.request)
+        else:
+            form = self.form_class(for_user=self.request.user, instance=self.object, request=self.request)
+        return form
+
+    def get_header_title(self):
+        instance_string = get_model_string(self.object)
+        return _("Edit model %(type)s '%(instance_string)s'") % {
+            "type": self.object._meta.verbose_name,
+            "instance_string": instance_string,
+        }
+    
+    def get_help_text(self):
+        return None
+          
+    def get_element_id(self) -> str:
+        m = self.model
+        return f"model-{m._meta.app_label}-{m._meta.model_name}-{self.object.pk}"
+
+    def form_valid(self, form):
+        self.object = form.save()
 
-    def render_content(self, parent_context: dict = None) -> str:
-        parent_context = parent_context or {}
+    def render_content(self, parent_context=None):
         if hasattr(parent_context, "flatten"):
             parent_context = parent_context.flatten()
 
-        return self.block.render(parent_context)
-    
-class DomPositionedBlockAdapter(DomPositionedMixin, BlockAdapter):
-    identifier = "dom-block"
+        method_name = self.kwargs["render_method"]
+        if not hasattr(self.object, method_name):
+            raise AdapterError(
+                "Object '%s' does not have any method named '%s'" % (
+                    self.object.__class__.__name__,
+                    method_name,
+                )
+            )
+        method = getattr(
+            self.object,
+            method_name
+        )
+        return method(
+            request=self.request,
+            context=parent_context,
+        )
```

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/adapters/field.py` & `wagtail_fedit-1.5.8/wagtail_fedit/adapters/field.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 class FieldAdapter(BlockFieldReplacementAdapter):
     """
     An adapter for editing any model field.
     This will render the field and replace it on the frontend
     on successful form submission.
     """
     identifier = "field"
+    js_constructor = "wagtail_fedit.editors.FieldEditor"
 
     def __init__(self, object, field_name: str, request: HttpRequest, **kwargs):
         super().__init__(object, field_name, request, **kwargs)
 
         self.original_object = object
         self.initial_field_value = self.field_value
 
@@ -221,7 +222,9 @@
             self.meta_field,
             parent_context,
         )
 
 
 class DomPositionedFieldAdapter(DomPositionedMixin, FieldAdapter):
     identifier = "dom-field"
+    js_constructor = "wagtail_fedit.editors.DomPositionedFieldEditor"
+    keywords = FieldAdapter.keywords
```

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/adapters/funcs.py` & `wagtail_fedit-1.5.8/wagtail_fedit/adapters/funcs.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/adapters/misc.py` & `wagtail_fedit-1.5.8/wagtail_fedit/adapters/misc.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/adapters/registry.py` & `wagtail_fedit-1.5.8/wagtail_fedit/registry.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,44 @@
-from typing import Type
-from .base import BaseAdapter
+from typing import Type, TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from .adapters.base import BaseAdapter
 
 
 class RegistryLookUpError(Exception):
     pass
 
 class DuplicateAdapterError(Exception):
     pass
 
-class AdapterSubclassError(TypeError):
-    pass
-
 
 class AdapterRegistry:
     def __init__(self):
-        self.adapters: dict[str, Type[BaseAdapter]] = {}
+        self.adapters: dict[str, Type["BaseAdapter"]] = {}
 
-    def __getitem__(self, identifier: str) -> Type[BaseAdapter]:
+    def __getitem__(self, identifier: str) -> Type["BaseAdapter"]:
         """
         Retrieve an adapter by its identifier or raise a RegistryLookUpError if not found.
         """
         try:
             return self.adapters[identifier]
         except KeyError:
             raise RegistryLookUpError(f"No adapter found with identifier '{identifier}'.")
 
-    def register(self, adapter_class: Type[BaseAdapter]):
+    def register(self, adapter_class: Type["BaseAdapter"]):
         """
         Register an adapter class with the registry.
         """
-        if isinstance(adapter_class, BaseAdapter):
-            raise AdapterSubclassError(f"{adapter_class.__class__.__name__} must be a subclass of BaseAdapter; got instance.")
-        
         if adapter_class.identifier in self.adapters:
             raise DuplicateAdapterError(f"An adapter with identifier '{adapter_class.identifier}' is already registered.")
 
         self.adapters[adapter_class.identifier] = adapter_class
 
+        adapter_class.on_register(self)
+
     def unregister(self, identifier):
         """
         Unregister an adapter by its identifier.
         """
         if identifier not in self.adapters:
             raise RegistryLookUpError(f"No adapter found with identifier '{identifier}'.")
```

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/errors.py` & `wagtail_fedit-1.5.8/wagtail_fedit/errors.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.5.8/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.5.8/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/hooks.py` & `wagtail_fedit-1.5.8/wagtail_fedit/hooks.py`

 * *Files 20% similar despite different names*

```diff
@@ -162,7 +162,43 @@
 ```python
 for hook in hooks.get_hooks(ACTION_MENU_ITEM_IS_SHOWN):
     result = hook(context, instance)
     if result is not None:
         return result # <- bool
 ```
 """
+
+REGISTER_ADAPTER_CLASS = prefix("register_adapter_class")
+"""
+### wagtail_fedit.register_adapter_class
+Register an adapter class with the adapter registry.
+
+Example of how this hook is used in wagtail_hooks.py:
+
+```python
+@hooks.register(REGISTER_ADAPTER_CLASS)
+def register_adapter_class(registry):
+    registry.register(FieldAdapter)
+    registry.register(DomPositionedFieldAdapter)
+    registry.register(BlockAdapter)
+    registry.register(DomPositionedBlockAdapter)
+    registry.register(ModelAdapter)
+    registry.register(BackgroundImageFieldAdapter)
+```
+"""
+
+REGISTER_ADAPTER_URLS = prefix("register_adapter_urls")
+"""
+### wagtail_fedit.register_adapter_urls
+Register the adapter URLs.
+Used internally by the URLMixin class.
+
+Example of how this hook is used in wagtail_hooks.py:
+
+```python
+@hooks.register(REGISTER_ADAPTER_URLS)
+def register_adapter_urls():
+    return [
+        path("my-view/", views.MyView.as_view(), name="my_view")
+    ]
+```
+"""
```

#### html2text {}

```diff
@@ -48,8 +48,20 @@
 if field.related_model in [Page, Image, Document]: return True return False ```
 """ ACTION_MENU_ITEM_IS_SHOWN = prefix("action_menu_item_is_shown") """ ###
 wagtail_fedit.action_menu_item_is_shown Decide if the action menu item should
 be shown for the given instance. Return None if you cannot decide, False if you
 want to hide the item, and True if you want to show the item. Example of how
 this hook is called: ```python for hook in hooks.get_hooks
 (ACTION_MENU_ITEM_IS_SHOWN): result = hook(context, instance) if result is not
-None: return result # <- bool ``` """
+None: return result # <- bool ``` """ REGISTER_ADAPTER_CLASS = prefix
+("register_adapter_class") """ ### wagtail_fedit.register_adapter_class
+Register an adapter class with the adapter registry. Example of how this hook
+is used in wagtail_hooks.py: ```python @hooks.register(REGISTER_ADAPTER_CLASS)
+def register_adapter_class(registry): registry.register(FieldAdapter)
+registry.register(DomPositionedFieldAdapter) registry.register(BlockAdapter)
+registry.register(DomPositionedBlockAdapter) registry.register(ModelAdapter)
+registry.register(BackgroundImageFieldAdapter) ``` """ REGISTER_ADAPTER_URLS =
+prefix("register_adapter_urls") """ ### wagtail_fedit.register_adapter_urls
+Register the adapter URLs. Used internally by the URLMixin class. Example of
+how this hook is used in wagtail_hooks.py: ```python @hooks.register
+(REGISTER_ADAPTER_URLS) def register_adapter_urls(): return [ path("my-view/",
+views.MyView.as_view(), name="my_view") ] ``` """
```

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo` & `wagtail_fedit-1.5.8/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo`

 * *Files 20% similar despite different names*

#### msgunfmt {}

```diff
@@ -10,17 +10,23 @@
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "A block was changed from the frontend"
 msgstr "Een blok is gewijzigd vanaf de frontend"
 
+msgid "A block was moved from the frontend"
+msgstr "Een blok is verplaatst vanaf de frontend"
+
 msgid "A field was changed from the frontend"
 msgstr "Een veld is gewijzigd vanaf de frontend"
 
+msgid "A model was changed from the frontend"
+msgstr "Een model is gewijzigd vanaf de frontend"
+
 msgid "About cancelling workflows"
 msgstr "Over het annuleren van workflows"
 
 msgid "About publishing"
 msgstr "Over publiceren"
 
 msgid "About submitting for moderation"
@@ -28,36 +34,48 @@
 
 msgid "About unpublishing"
 msgstr "Over depubliceren"
 
 msgid "Action"
 msgstr "Actie"
 
+msgid "Adapter ID"
+msgstr "Adapter-ID"
+
 msgid "Are you sure you want to continue?"
 msgstr "Weet u zeker dat u wilt doorgaan?"
 
 msgid "Block Changed (Frontend)"
 msgstr "Blok gewijzigd (Frontend)"
 
+msgid "Block Moved (Frontend)"
+msgstr "Blok verplaatst (Frontend)"
+
 msgid "Cancel"
 msgstr "Annuleren"
 
 msgid "Cancel Workflow"
 msgstr "Workflow annuleren"
 
 msgid ""
 "Cancelling the workflow for this object will remove it from the moderation "
 "process."
 msgstr ""
 "Het annuleren van de workflow voor dit object verwijdert het uit het "
 "moderatieproces."
 
+msgid "Cancelling workflow for {} \"{}\""
+msgstr "Workflow annuleren voor {} \"{}\""
+
 msgid "Changed '%(field)s' from '%(old)s' to '%(new)s' (Frontend)"
 msgstr "Gewijzigd '%(field)s' van '%(old)s' naar '%(new)s' (Frontend)"
 
+msgid "Changed '%(model)s' (Frontend)"
+msgstr "Gewijzigd '%(model)s' (Frontend)"
+
 msgid ""
 "Changed block \"%(block)s\" on field \"%(field)s\" (%(block_id)s, Frontend)"
 msgstr ""
 "Blok \"%(block)s\" gewijzigd op veld \"%(field)s\" (%(block_id)s, Frontend)"
 
 msgid ""
 "Changed related '%(related)s' instance '%(instance)s' on field "
@@ -95,42 +113,82 @@
 
 msgid "Edit field '%(field_name)s' for %(model_name)s '%(model_string)s'"
 msgstr "Bewerk veld %(field_name)s voor %(model_name)s' %(model_string)s'"
 
 msgid "Edit in Wagtail Admin"
 msgstr "Bewerk in Wagtail Admin"
 
-msgid "Edit model '%(instance_string)s'"
-msgstr "Bewerk model '%(instance_string)s'"
+msgid "Edit model %(type)s '%(instance_string)s'"
+msgstr "Bewerk model %(type)s '%(instance_string)s'"
 
 msgid "Edit model '%(instance_string)s' for %(model_name)s '%(model_string)s'"
 msgstr ""
 "Bewerk model %(instance_string)s voor %(model_name)s '%(model_string)s'"
 
 msgid "Field Changed (Frontend)"
 msgstr "Veld gewijzigd (Frontend)"
 
+msgid "Field name"
+msgstr "Veldnaam"
+
 msgid "Frontend Edit"
 msgstr "Bewerk op frontend"
 
 msgid "Frontend Editing"
 msgstr "Bewerken op frontend"
 
 msgid "Invalid action specified: {}"
 msgstr "Ongeldige actie opgegeven: {}"
 
+msgid "Invalid {}"
+msgstr "Ongeldige {}"
+
 msgid "Locked"
 msgstr "Vergrendeld"
 
+msgid "Model"
+msgstr "Model"
+
+msgid "Model Changed (Frontend)"
+msgstr "Model gewijzigd (Frontend)"
+
+msgid "Model not found"
+msgstr "Model niet gevonden"
+
+msgid "Model {} does not inherit from {}"
+msgstr "Model {} erft niet van {}"
+
+msgid "Move block down"
+msgstr "Verplaats blok omlaag"
+
+msgid "Move block up"
+msgstr "Verplaats blok omhoog"
+
+msgid ""
+"Moved block \"%(block)s\" on field \"%(field)s\" %(direction)s "
+"(%(block_id)s, Frontend)"
+msgstr ""
+"Blok \"%(block)s\" verplaatst op veld \"%(field)s\" %(direction)s "
+"(%(block_id)s, Frontend)"
+
+msgid "Moved block on field (Frontend)"
+msgstr "Blok verplaatst op veld (Frontend)"
+
 msgid "No Publishing Required"
 msgstr "Geen publicatie vereist"
 
 msgid "No action specified"
 msgstr "Geen actie opgegeven"
 
+msgid "No workflow state found"
+msgstr "Geen workflowstatus gevonden"
+
+msgid "Object has no unpublished changes"
+msgstr "Object heeft geen ongepubliceerde wijzigingen"
+
 msgid "Publish"
 msgstr "Publiceren"
 
 msgid "Publishing Required"
 msgstr "Publicatie vereist"
 
 msgid "Publishing related object required."
@@ -165,41 +223,44 @@
 msgid "Submitting {} \"{}\" for moderation"
 msgstr "Indienen van {} \"{}\" voor moderatie"
 
 msgid ""
 "That means that any changes you make will be immediately visible to everyone."
 msgstr ""
 "Dit betekent dat alle wijzigingen die u aanbrengt, onmiddellijk zichtbaar "
-"zijnvoor iedereen."
+"zijn voor iedereen."
 
 msgid "That means that it will no longer be visible to anyone."
 msgstr "Dat betekent dat het niet langer zichtbaar is voor iedereen."
 
 msgid "The object you are editing does not support drafts."
 msgstr "Het object dat u bewerkt ondersteunt geen concepten."
 
 msgid "The object you are editing supports drafts."
 msgstr "Het object dat u bewerkt ondersteunt concepten."
 
+msgid "This adapter is used for directly editing a model instance."
+msgstr "Deze adapter wordt gebruikt voor het direct bewerken van een model."
+
 msgid ""
 "This object has more changes. <a href=\"%(view_more_url)s\">View all changes."
 "</a>"
 msgstr ""
 "Dit object heeft meer wijzigingen. <a href=\"%(view_more_url)s\">Bekijk alle "
 "wijzigingen.</a>"
 
 msgid "This object is locked"
 msgstr "Dit object is vergrendeld"
 
+msgid "This object is locked - it cannot be acted upon."
+msgstr "Dit object is vergrendeld - het kan niet worden bewerkt."
+
 msgid "This object is locked and cannot be edited."
 msgstr "Dit object is vergrendeld en kan niet worden bewerkt."
 
-msgid "This object is locked. It cannot be acted upon."
-msgstr "Dit object is vergrendeld. Er kan niet op worden gereageerd."
-
 msgid "This object is not live"
 msgstr "Dit object is niet live"
 
 msgid "Unpublish"
 msgstr "Depubliceren"
 
 msgid "Unpublishing this object will make it invisible to users on the site."
@@ -208,14 +269,17 @@
 
 msgid "Unpublishing {} \"{}\""
 msgstr "Depubliceren van {} \"{}\""
 
 msgid "User"
 msgstr "Gebruiker"
 
+msgid "User does not have permission to {}"
+msgstr "Gebruiker heeft geen toestemming om {}"
+
 msgid "Validation Errors"
 msgstr "Validatiefouten"
 
 msgid "View Live Page"
 msgstr "Bekijk live pagina"
 
 msgid "View in Wagtail admin"
@@ -235,14 +299,17 @@
 msgid "You can always choose to submit it for moderation again."
 msgstr ""
 "Je kunt er altijd voor kiezen om het opnieuw in te dienen voor moderatie."
 
 msgid "You can always choose to unpublish it."
 msgstr "U kunt er altijd voor kiezen om het te depubliceren."
 
+msgid "You do not have permission to view this page."
+msgstr "U heeft geen toestemming om deze pagina te bekijken."
+
 msgid ""
 "You must publish %(model)s and the related object of type "
 "%(related_verbose_name)s (%(related_model)s) to make any changes visible."
 msgstr ""
 "U moet %(model)s en het gerelateerde object van het type "
 "%(related_verbose_name)s (%(related_model)s) publiceren om wijzigingen "
 "zichtbaar te maken."
@@ -252,7 +319,43 @@
 
 msgid ""
 "You must publish the related object of type %(type)s (%(model)s) to make any "
 "changes visible."
 msgstr ""
 "U moet het gerelateerde object van het type %(type)s (%(model)s) publiceren "
 "om wijzigingen zichtbaar te maken."
+
+msgid "cancel the workflow"
+msgstr "workflow te annuleren"
+
+msgid "down"
+msgstr "omlaag"
+
+msgid "edit this field"
+msgstr "bewerken van dit veld"
+
+msgid "field name"
+msgstr "veldnaam"
+
+msgid "for object {}"
+msgstr "voor object {}"
+
+msgid "model provided"
+msgstr "model verstrekt"
+
+msgid "publish"
+msgstr "publiceren"
+
+msgid "submit for moderation"
+msgstr "indienen voor moderatie"
+
+msgid "unpublish"
+msgstr "depubliceren"
+
+msgid "up"
+msgstr "omhoog"
+
+msgid "view this page"
+msgstr "Bekijk deze pagina"
+
+msgid "{} is required"
+msgstr "{} is vereist"
```

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/locale/nl/LC_MESSAGES/django.po` & `wagtail_fedit-1.5.8/wagtail_fedit/locale/nl/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,73 +4,74 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-25 12:49+0200\n"
+"POT-Creation-Date: 2024-05-20 00:52+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: .\tester\wagtail_fedit\adapters\block.py:110
+#: .\tester\wagtail_fedit\adapters\block.py:235
 #, python-format
 msgid "Edit block %(block_label)s for %(model_name)s '%(model_string)s'"
 msgstr "Bewerk blok %(block_label)s voor %(model_name)s '%(model_string)s'"
 
-#: .\tester\wagtail_fedit\adapters\field.py:72
+#: .\tester\wagtail_fedit\adapters\field.py:74
 #, python-format
 msgid "Edit model '%(instance_string)s' for %(model_name)s '%(model_string)s'"
 msgstr ""
 "Bewerk model %(instance_string)s voor %(model_name)s '%(model_string)s'"
 
-#: .\tester\wagtail_fedit\adapters\field.py:78
+#: .\tester\wagtail_fedit\adapters\field.py:80
 #, python-format
 msgid "Edit field '%(field_name)s' for %(model_name)s '%(model_string)s'"
 msgstr "Bewerk veld %(field_name)s voor %(model_name)s' %(model_string)s'"
 
-#: .\tester\wagtail_fedit\adapters\field.py:92
+#: .\tester\wagtail_fedit\adapters\field.py:94
 #, python-format
 msgid ""
 "You must publish %(model)s and the related object of type "
 "%(related_verbose_name)s (%(related_model)s) to make any changes visible."
 msgstr ""
 "U moet %(model)s en het gerelateerde object van het type "
 "%(related_verbose_name)s (%(related_model)s) publiceren om wijzigingen "
 "zichtbaar te maken."
 
-#: .\tester\wagtail_fedit\adapters\field.py:116
+#: .\tester\wagtail_fedit\adapters\field.py:118
 msgid "Publishing related object required."
 msgstr "Publicatie van gerelateerd object vereist."
 
-#: .\tester\wagtail_fedit\adapters\field.py:117
-#: .\tester\wagtail_fedit\utils.py:71
+#: .\tester\wagtail_fedit\adapters\field.py:119
+#: .\tester\wagtail_fedit\utils.py:86
 msgid "The object you are editing supports drafts."
 msgstr "Het object dat u bewerkt ondersteunt concepten."
 
-#: .\tester\wagtail_fedit\adapters\field.py:118
+#: .\tester\wagtail_fedit\adapters\field.py:120
 #, python-format
 msgid ""
 "You must publish the related object of type %(type)s (%(model)s) to make any "
 "changes visible."
 msgstr ""
 "U moet het gerelateerde object van het type %(type)s (%(model)s) publiceren "
 "om wijzigingen zichtbaar te maken."
 
-#: .\tester\wagtail_fedit\adapters\models.py:41
+#: .\tester\wagtail_fedit\adapters\models.py:46
 msgid "This adapter is used for directly editing a model instance."
 msgstr "Deze adapter wordt gebruikt voor het direct bewerken van een model."
 
-#: .\tester\wagtail_fedit\adapters\models.py:108
+#: .\tester\wagtail_fedit\adapters\models.py:138
+#, python-format
 msgid "Edit model %(type)s '%(instance_string)s'"
 msgstr "Bewerk model %(type)s '%(instance_string)s'"
 
 #: .\tester\wagtail_fedit\errors.py:22
 msgid "You do not have permission to view this page."
 msgstr "U heeft geen toestemming om deze pagina te bekijken."
 
@@ -122,14 +123,22 @@
 msgid "{} is required"
 msgstr "{} is vereist"
 
 #: .\tester\wagtail_fedit\templates\wagtail_fedit\content\buttons\admin_link.html:1
 msgid "View in Wagtail admin"
 msgstr "Bekijk in Wagtail admin"
 
+#: .\tester\wagtail_fedit\templates\wagtail_fedit\content\buttons\move_down.html:1
+msgid "Move block down"
+msgstr "Verplaats blok omlaag"
+
+#: .\tester\wagtail_fedit\templates\wagtail_fedit\content\buttons\move_up.html:1
+msgid "Move block up"
+msgstr "Verplaats blok omhoog"
+
 #: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\action_confirm.html:32
 msgid "Are you sure you want to continue?"
 msgstr "Weet u zeker dat u wilt doorgaan?"
 
 #: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\action_confirm.html:45
 msgid "Cancel"
 msgstr "Annuleren"
@@ -163,41 +172,41 @@
 msgid ""
 "This object has more changes. <a href=\"%(view_more_url)s\">View all changes."
 "</a>"
 msgstr ""
 "Dit object heeft meer wijzigingen. <a href=\"%(view_more_url)s\">Bekijk alle "
 "wijzigingen.</a>"
 
-#: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\base_iframe.html:55
+#: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\base_iframe.html:59
 msgid "Locked"
 msgstr "Vergrendeld"
 
-#: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\base_iframe.html:59
+#: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\base_iframe.html:63
 msgid "This object is locked"
 msgstr "Dit object is vergrendeld"
 
-#: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\base_iframe.html:60
+#: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\base_iframe.html:64
 msgid "You are still able to edit this object."
 msgstr "U kunt dit object nog steeds bewerken."
 
-#: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\base_iframe.html:68
+#: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\base_iframe.html:73
 msgid "This object is locked and cannot be edited."
 msgstr "Dit object is vergrendeld en kan niet worden bewerkt."
 
-#: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\base_iframe.html:90
+#: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\base_iframe.html:96
 msgid "Edit in Wagtail Admin"
 msgstr "Bewerk in Wagtail Admin"
 
-#: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\base_iframe.html:94
-#: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\base_iframe.html:95
+#: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\base_iframe.html:100
+#: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\base_iframe.html:101
 msgid "Save"
 msgstr "Opslaan"
 
-#: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\base_iframe.html:101
-#: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\base_iframe.html:102
+#: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\base_iframe.html:107
+#: .\tester\wagtail_fedit\templates\wagtail_fedit\editor\base_iframe.html:108
 msgid "Close"
 msgstr "Sluiten"
 
 #: .\tester\wagtail_fedit\templates\wagtail_fedit\userbar\item_fedit.html:11
 msgid "Frontend Editing"
 msgstr "Bewerken op frontend"
 
@@ -205,68 +214,68 @@
 msgid "View Live Page"
 msgstr "Bekijk live pagina"
 
 #: .\tester\wagtail_fedit\templates\wagtail_fedit\userbar\publish\item_fedit_publishing.html:17
 msgid "Revision Management"
 msgstr "Revisiebeheer"
 
-#: .\tester\wagtail_fedit\utils.py:68
-#: .\tester\wagtail_fedit\views\adapters.py:49
+#: .\tester\wagtail_fedit\utils.py:83
+#: .\tester\wagtail_fedit\views\adapters.py:52
 msgid "Validation Errors"
 msgstr "Validatiefouten"
 
-#: .\tester\wagtail_fedit\utils.py:70
+#: .\tester\wagtail_fedit\utils.py:85
 msgid "Publishing Required"
 msgstr "Publicatie vereist"
 
-#: .\tester\wagtail_fedit\utils.py:72
+#: .\tester\wagtail_fedit\utils.py:87
 #, python-format
 msgid "You must publish %(model)s to make any changes visible."
 msgstr "U moet %(model)s publiceren om wijzigingen zichtbaar te maken."
 
-#: .\tester\wagtail_fedit\utils.py:74
+#: .\tester\wagtail_fedit\utils.py:89
 msgid "No Publishing Required"
 msgstr "Geen publicatie vereist"
 
-#: .\tester\wagtail_fedit\utils.py:75
+#: .\tester\wagtail_fedit\utils.py:90
 msgid "The object you are editing does not support drafts."
 msgstr "Het object dat u bewerkt ondersteunt geen concepten."
 
-#: .\tester\wagtail_fedit\utils.py:76
+#: .\tester\wagtail_fedit\utils.py:91
 msgid ""
 "You are not required to publish this object to make this change visible."
 msgstr ""
 "U hoeft dit object niet te publiceren om deze wijziging zichtbaar te maken."
 
-#: .\tester\wagtail_fedit\utils.py:90
+#: .\tester\wagtail_fedit\utils.py:105
 #, python-format
 msgid "Edit %(type)s '%(model)s'"
 msgstr "Bewerk %(type)s '%(model)s'"
 
-#: .\tester\wagtail_fedit\views\adapters.py:66
+#: .\tester\wagtail_fedit\views\adapters.py:69
 msgid "Adapter ID"
 msgstr "Adapter-ID"
 
-#: .\tester\wagtail_fedit\views\adapters.py:76
+#: .\tester\wagtail_fedit\views\adapters.py:79
 msgid "Model"
 msgstr "Model"
 
-#: .\tester\wagtail_fedit\views\adapters.py:83
+#: .\tester\wagtail_fedit\views\adapters.py:86
 msgid "view this page"
 msgstr "Bekijk deze pagina"
 
-#: .\tester\wagtail_fedit\views\adapters.py:101
+#: .\tester\wagtail_fedit\views\adapters.py:104
 msgid "Field name"
 msgstr "Veldnaam"
 
-#: .\tester\wagtail_fedit\views\adapters.py:109
+#: .\tester\wagtail_fedit\views\adapters.py:112
 msgid "field name"
 msgstr "veldnaam"
 
-#: .\tester\wagtail_fedit\views\adapters.py:135
+#: .\tester\wagtail_fedit\views\adapters.py:138
 msgid "edit this field"
 msgstr "bewerken van dit veld"
 
 #: .\tester\wagtail_fedit\views\editable.py:251
 #: .\tester\wagtail_fedit\wagtail_hooks\userbar.py:53
 msgid "Publish"
 msgstr "Publiceren"
@@ -285,15 +294,15 @@
 "Publicatie van dit object maakt het zichtbaar voor gebruikers op de site."
 
 #: .\tester\wagtail_fedit\views\editable.py:263
 msgid ""
 "That means that any changes you make will be immediately visible to everyone."
 msgstr ""
 "Dit betekent dat alle wijzigingen die u aanbrengt, onmiddellijk zichtbaar "
-"zijnvoor iedereen."
+"zijn voor iedereen."
 
 #: .\tester\wagtail_fedit\views\editable.py:267
 msgid "You can always choose to unpublish it."
 msgstr "U kunt er altijd voor kiezen om het te depubliceren."
 
 #: .\tester\wagtail_fedit\views\editable.py:337
 msgid "publish"
@@ -425,29 +434,67 @@
 msgid "Changed '%(field)s' from '%(old)s' to '%(new)s' (Frontend)"
 msgstr "Gewijzigd '%(field)s' van '%(old)s' naar '%(new)s' (Frontend)"
 
 #: .\tester\wagtail_fedit\wagtail_hooks\log_actions.py:49
 msgid "Edit Field"
 msgstr "Bewerk veld"
 
+#: .\tester\wagtail_fedit\wagtail_hooks\log_actions.py:53
+msgid "Model Changed (Frontend)"
+msgstr "Model gewijzigd (Frontend)"
+
 #: .\tester\wagtail_fedit\wagtail_hooks\log_actions.py:54
+msgid "A model was changed from the frontend"
+msgstr "Een model is gewijzigd vanaf de frontend"
+
+#: .\tester\wagtail_fedit\wagtail_hooks\log_actions.py:62
+msgid "Changed '%(model)s' (Frontend)"
+msgstr "Gewijzigd '%(model)s' (Frontend)"
+
+#: .\tester\wagtail_fedit\wagtail_hooks\log_actions.py:68
 msgid "Block Changed (Frontend)"
 msgstr "Blok gewijzigd (Frontend)"
 
-#: .\tester\wagtail_fedit\wagtail_hooks\log_actions.py:55
+#: .\tester\wagtail_fedit\wagtail_hooks\log_actions.py:69
 msgid "A block was changed from the frontend"
 msgstr "Een blok is gewijzigd vanaf de frontend"
 
-#: .\tester\wagtail_fedit\wagtail_hooks\log_actions.py:68
+#: .\tester\wagtail_fedit\wagtail_hooks\log_actions.py:82
 #, python-format
 msgid ""
 "Changed block \"%(block)s\" on field \"%(field)s\" (%(block_id)s, Frontend)"
 msgstr ""
 "Blok \"%(block)s\" gewijzigd op veld \"%(field)s\" (%(block_id)s, Frontend)"
 
+#: .\tester\wagtail_fedit\wagtail_hooks\log_actions.py:90
+msgid "Block Moved (Frontend)"
+msgstr "Blok verplaatst (Frontend)"
+
+#: .\tester\wagtail_fedit\wagtail_hooks\log_actions.py:91
+msgid "A block was moved from the frontend"
+msgstr "Een blok is verplaatst vanaf de frontend"
+
+#: .\tester\wagtail_fedit\wagtail_hooks\log_actions.py:103
+msgid "Moved block on field (Frontend)"
+msgstr "Blok verplaatst op veld (Frontend)"
+
+#: .\tester\wagtail_fedit\wagtail_hooks\log_actions.py:105
+msgid ""
+"Moved block \"%(block)s\" on field \"%(field)s\" %(direction)s "
+"(%(block_id)s, Frontend)"
+msgstr ""
+"Blok \"%(block)s\" verplaatst op veld \"%(field)s\" %(direction)s "
+"(%(block_id)s, Frontend)"
+
+msgid "up"
+msgstr "omhoog"
+
+msgid "down"
+msgstr "omlaag"
+
 #~ msgid "Edit block"
 #~ msgstr "Bewerk blok"
 
 #~ msgid "Block Validation Errors"
 #~ msgstr "Blokvalidatiefouten"
 
 #~ msgid "Submit for Moderation"
```

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/models.py` & `wagtail_fedit-1.5.8/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/settings.py` & `wagtail_fedit-1.5.8/wagtail_fedit/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.5.8/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files 2% similar despite different names*

```diff
@@ -182,14 +182,16 @@
     }
 }
 .wagtail-fedit-modal-wrapper iframe,
 .wagtail-fedit-adapter-wrapper iframe {
     width: 100%;
     height: 100%;
     border: none;
+    z-index: 300;
+    position: relative;
     flex: 1;
 }
 .wagtail-fedit-modal-wrapper .wagtail-fedit-close-button {
     position: absolute;
     right: 0;
     top: 0;
     text-align: center;
```

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.5.8/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,14 @@
     height: 100%;
     gap: 1em;
 }
 .wagtail-fedit-form-wrapper #wagtail-fedit-form {
     display: flex;
     flex-direction: column;
     justify-content: space-between;
-    flex: 1;
 }
 .wagtail-fedit-form-wrapper #wagtail-fedit-form .field > input
 .wagtail-fedit-form-wrapper #wagtail-fedit-form .field > * > input {
     margin-bottom: 0.5em;
 }
 .wagtail-fedit-form-wrapper .wagtail-fedit-form {
     display: flex;
```

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.5.8/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/static/wagtail_fedit/js/edit.js` & `wagtail_fedit-1.5.8/wagtail_fedit/static/wagtail_fedit/js/edit.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -371,27 +371,27 @@
                     n = n.parentNode
                 }
                 return null
             }(t) || n
         }
         var T = "top",
             A = "bottom",
-            C = "right",
-            S = "left",
+            S = "right",
+            C = "left",
             D = "auto",
-            M = [T, A, C, S],
-            R = "start",
-            j = "end",
-            I = "viewport",
-            k = "popper",
+            M = [T, A, S, C],
+            I = "start",
+            k = "end",
+            R = "viewport",
+            j = "popper",
             P = M.reduce((function(e, t) {
-                return e.concat([t + "-" + R, t + "-" + j])
+                return e.concat([t + "-" + I, t + "-" + k])
             }), []),
             H = [].concat(M, [D]).reduce((function(e, t) {
-                return e.concat([t, t + "-" + R, t + "-" + j])
+                return e.concat([t, t + "-" + I, t + "-" + k])
             }), []),
             N = ["beforeRead", "read", "afterRead", "beforeMain", "main", "afterMain", "beforeWrite", "write", "afterWrite"];
 
         function W(e) {
             var t = new Map,
                 n = new Set,
                 i = [];
@@ -412,22 +412,22 @@
         }
         var B = {
             placement: "bottom",
             modifiers: [],
             strategy: "absolute"
         };
 
-        function _() {
+        function F() {
             for (var e = arguments.length, t = new Array(e), n = 0; n < e; n++) t[n] = arguments[n];
             return !t.some((function(e) {
                 return !(e && "function" == typeof e.getBoundingClientRect)
             }))
         }
 
-        function F(e) {
+        function q(e) {
             void 0 === e && (e = {});
             var n = e,
                 i = n.defaultModifiers,
                 r = void 0 === i ? [] : i,
                 o = n.defaultOptions,
                 a = void 0 === o ? B : o;
             return function(e, n, i) {
@@ -489,15 +489,15 @@
                             })), p.update()
                         },
                         forceUpdate: function() {
                             if (!d) {
                                 var e = c.elements,
                                     t = e.reference,
                                     n = e.popper;
-                                if (_(t, n)) {
+                                if (F(t, n)) {
                                     c.rects = {
                                         reference: g(t, L(n), "fixed" === c.options.strategy),
                                         popper: w(n)
                                     }, c.reset = !1, c.placement = c.options.placement, c.orderedModifiers.forEach((function(e) {
                                         return c.modifiersData[e.name] = Object.assign({}, e.data)
                                     }));
                                     for (var i = 0; i < c.orderedModifiers.length; i++)
@@ -528,27 +528,27 @@
                                 }))
                             }))), s
                         }),
                         destroy: function() {
                             u(), d = !0
                         }
                     };
-                if (!_(e, n)) return p;
+                if (!F(e, n)) return p;
 
                 function u() {
                     l.forEach((function(e) {
                         return e()
                     })), l = []
                 }
                 return p.setOptions(i).then((function(e) {
                     !d && i.onFirstUpdate && i.onFirstUpdate(e)
                 })), p
             }
         }
-        var q = {
+        var _ = {
             passive: !0
         };
         const V = {
             name: "eventListeners",
             enabled: !0,
             phase: "write",
             fn: function() {},
@@ -559,43 +559,43 @@
                     o = r.scroll,
                     a = void 0 === o || o,
                     s = r.resize,
                     c = void 0 === s || s,
                     l = e(n.elements.popper),
                     d = [].concat(n.scrollParents.reference, n.scrollParents.popper);
                 return a && d.forEach((function(e) {
-                        e.addEventListener("scroll", i.update, q)
-                    })), c && l.addEventListener("resize", i.update, q),
+                        e.addEventListener("scroll", i.update, _)
+                    })), c && l.addEventListener("resize", i.update, _),
                     function() {
                         a && d.forEach((function(e) {
-                            e.removeEventListener("scroll", i.update, q)
-                        })), c && l.removeEventListener("resize", i.update, q)
+                            e.removeEventListener("scroll", i.update, _)
+                        })), c && l.removeEventListener("resize", i.update, _)
                     }
             },
             data: {}
         };
 
-        function U(e) {
+        function $(e) {
             return e.split("-")[0]
         }
 
-        function $(e) {
+        function U(e) {
             return e.split("-")[1]
         }
 
         function z(e) {
             return ["top", "bottom"].indexOf(e) >= 0 ? "x" : "y"
         }
 
         function X(e) {
             var t, n = e.reference,
                 i = e.element,
                 r = e.placement,
-                o = r ? U(r) : null,
-                a = r ? $(r) : null,
+                o = r ? $(r) : null,
+                a = r ? U(r) : null,
                 s = n.x + n.width / 2 - i.width / 2,
                 c = n.y + n.height / 2 - i.height / 2;
             switch (o) {
                 case T:
                     t = {
                         x: s,
                         y: n.y - i.height
@@ -603,21 +603,21 @@
                     break;
                 case A:
                     t = {
                         x: s,
                         y: n.y + n.height
                     };
                     break;
-                case C:
+                case S:
                     t = {
                         x: n.x + n.width,
                         y: c
                     };
                     break;
-                case S:
+                case C:
                     t = {
                         x: n.x - i.width,
                         y: c
                     };
                     break;
                 default:
                     t = {
@@ -625,31 +625,31 @@
                         y: n.y
                     }
             }
             var l = o ? z(o) : null;
             if (null != l) {
                 var d = "y" === l ? "height" : "width";
                 switch (a) {
-                    case R:
+                    case I:
                         t[l] = t[l] - (n[d] / 2 - i[d] / 2);
                         break;
-                    case j:
+                    case k:
                         t[l] = t[l] + (n[d] / 2 - i[d] / 2)
                 }
             }
             return t
         }
         var Y = {
             top: "auto",
             right: "auto",
             bottom: "auto",
             left: "auto"
         };
 
-        function G(t) {
+        function J(t) {
             var n, i = t.popper,
                 r = t.popperRect,
                 o = t.placement,
                 a = t.variation,
                 c = t.offsets,
                 l = t.position,
                 d = t.gpuAcceleration,
@@ -666,22 +666,22 @@
                 }) : {
                     x: g,
                     y
                 };
             g = b.x, y = b.y;
             var E = c.hasOwnProperty("x"),
                 x = c.hasOwnProperty("y"),
-                O = S,
+                O = C,
                 D = T,
                 M = window;
             if (p) {
-                var R = L(i),
-                    I = "clientHeight",
-                    k = "clientWidth";
-                R === e(i) && "static" !== m(R = f(i)).position && "absolute" === l && (I = "scrollHeight", k = "scrollWidth"), (o === T || (o === S || o === C) && a === j) && (D = A, y -= (h && R === M && M.visualViewport ? M.visualViewport.height : R[I]) - r.height, y *= d ? 1 : -1), o !== S && (o !== T && o !== A || a !== j) || (O = C, g -= (h && R === M && M.visualViewport ? M.visualViewport.width : R[k]) - r.width, g *= d ? 1 : -1)
+                var I = L(i),
+                    R = "clientHeight",
+                    j = "clientWidth";
+                I === e(i) && "static" !== m(I = f(i)).position && "absolute" === l && (R = "scrollHeight", j = "scrollWidth"), (o === T || (o === C || o === S) && a === k) && (D = A, y -= (h && I === M && M.visualViewport ? M.visualViewport.height : I[R]) - r.height, y *= d ? 1 : -1), o !== C && (o !== T && o !== A || a !== k) || (O = S, g -= (h && I === M && M.visualViewport ? M.visualViewport.width : I[j]) - r.width, g *= d ? 1 : -1)
             }
             var P, H = Object.assign({
                     position: l
                 }, p && Y),
                 N = !0 === u ? function(e, t) {
                     var n = e.x,
                         i = e.y,
@@ -695,41 +695,41 @@
                     y
                 }, e(i)) : {
                     x: g,
                     y
                 };
             return g = N.x, y = N.y, d ? Object.assign({}, H, ((P = {})[D] = x ? "0" : "", P[O] = E ? "0" : "", P.transform = (M.devicePixelRatio || 1) <= 1 ? "translate(" + g + "px, " + y + "px)" : "translate3d(" + g + "px, " + y + "px, 0)", P)) : Object.assign({}, H, ((n = {})[D] = x ? y + "px" : "", n[O] = E ? g + "px" : "", n.transform = "", n))
         }
-        const J = {
+        const G = {
                 name: "computeStyles",
                 enabled: !0,
                 phase: "beforeWrite",
                 fn: function(e) {
                     var t = e.state,
                         n = e.options,
                         i = n.gpuAcceleration,
                         r = void 0 === i || i,
                         o = n.adaptive,
                         a = void 0 === o || o,
                         s = n.roundOffsets,
                         c = void 0 === s || s,
                         l = {
-                            placement: U(t.placement),
-                            variation: $(t.placement),
+                            placement: $(t.placement),
+                            variation: U(t.placement),
                             popper: t.elements.popper,
                             popperRect: t.rects.popper,
                             gpuAcceleration: r,
                             isFixed: "fixed" === t.options.strategy
                         };
-                    null != t.modifiersData.popperOffsets && (t.styles.popper = Object.assign({}, t.styles.popper, G(Object.assign({}, l, {
+                    null != t.modifiersData.popperOffsets && (t.styles.popper = Object.assign({}, t.styles.popper, J(Object.assign({}, l, {
                         offsets: t.modifiersData.popperOffsets,
                         position: t.options.strategy,
                         adaptive: a,
                         roundOffsets: c
-                    })))), null != t.modifiersData.arrow && (t.styles.arrow = Object.assign({}, t.styles.arrow, G(Object.assign({}, l, {
+                    })))), null != t.modifiersData.arrow && (t.styles.arrow = Object.assign({}, t.styles.arrow, J(Object.assign({}, l, {
                         offsets: t.modifiersData.arrow,
                         position: "absolute",
                         adaptive: !1,
                         roundOffsets: c
                     })))), t.attributes.popper = Object.assign({}, t.attributes.popper, {
                         "data-popper-placement": t.placement
                     })
@@ -791,22 +791,22 @@
                     var t = e.state,
                         n = e.options,
                         i = e.name,
                         r = n.offset,
                         o = void 0 === r ? [0, 0] : r,
                         a = H.reduce((function(e, n) {
                             return e[n] = function(e, t, n) {
-                                var i = U(e),
-                                    r = [S, T].indexOf(i) >= 0 ? -1 : 1,
+                                var i = $(e),
+                                    r = [C, T].indexOf(i) >= 0 ? -1 : 1,
                                     o = "function" == typeof n ? n(Object.assign({}, t, {
                                         placement: e
                                     })) : n,
                                     a = o[0],
                                     s = o[1];
-                                return a = a || 0, s = (s || 0) * r, [S, C].indexOf(i) >= 0 ? {
+                                return a = a || 0, s = (s || 0) * r, [C, S].indexOf(i) >= 0 ? {
                                     x: s,
                                     y: a
                                 } : {
                                     x: a,
                                     y: s
                                 }
                             }(n, t.rects, o), e
@@ -859,15 +859,15 @@
                 top: e.y,
                 right: e.x + e.width,
                 bottom: e.y + e.height
             })
         }
 
         function oe(n, i, r) {
-            return i === I ? re(function(t, n) {
+            return i === R ? re(function(t, n) {
                 var i = e(t),
                     r = f(t),
                     o = i.visualViewport,
                     a = r.clientWidth,
                     s = r.clientHeight,
                     c = 0,
                     d = 0;
@@ -923,25 +923,25 @@
                 s = r.placement,
                 c = void 0 === s ? e.placement : s,
                 l = r.strategy,
                 p = void 0 === l ? e.strategy : l,
                 h = r.boundary,
                 v = void 0 === h ? "clippingParents" : h,
                 g = r.rootBoundary,
-                w = void 0 === g ? I : g,
+                w = void 0 === g ? R : g,
                 b = r.elementContext,
-                x = void 0 === b ? k : b,
+                x = void 0 === b ? j : b,
                 O = r.altBoundary,
-                S = void 0 !== O && O,
+                C = void 0 !== O && O,
                 D = r.padding,
-                R = void 0 === D ? 0 : D,
-                j = ae("number" != typeof R ? R : se(R, M)),
-                P = x === k ? "reference" : k,
+                I = void 0 === D ? 0 : D,
+                k = ae("number" != typeof I ? I : se(I, M)),
+                P = x === j ? "reference" : j,
                 H = e.rects.popper,
-                N = e.elements[S ? P : x],
+                N = e.elements[C ? P : x],
                 W = function(e, n, r, s) {
                     var c = "clippingParents" === n ? function(e) {
                             var n = E(y(e)),
                                 r = ["absolute", "fixed"].indexOf(m(e).position) >= 0 && i(e) ? L(e) : e;
                             return t(r) ? n.filter((function(e) {
                                 return t(e) && ie(e, r) && "body" !== u(e)
                             })) : []
@@ -951,114 +951,114 @@
                         p = l.reduce((function(t, n) {
                             var i = oe(e, n, s);
                             return t.top = o(i.top, t.top), t.right = a(i.right, t.right), t.bottom = a(i.bottom, t.bottom), t.left = o(i.left, t.left), t
                         }), oe(e, d, s));
                     return p.width = p.right - p.left, p.height = p.bottom - p.top, p.x = p.left, p.y = p.top, p
                 }(t(N) ? N : N.contextElement || f(e.elements.popper), v, w, p),
                 B = d(e.elements.reference),
-                _ = X({
+                F = X({
                     reference: B,
                     element: H,
                     strategy: "absolute",
                     placement: c
                 }),
-                F = re(Object.assign({}, H, _)),
-                q = x === k ? F : B,
+                q = re(Object.assign({}, H, F)),
+                _ = x === j ? q : B,
                 V = {
-                    top: W.top - q.top + j.top,
-                    bottom: q.bottom - W.bottom + j.bottom,
-                    left: W.left - q.left + j.left,
-                    right: q.right - W.right + j.right
+                    top: W.top - _.top + k.top,
+                    bottom: _.bottom - W.bottom + k.bottom,
+                    left: W.left - _.left + k.left,
+                    right: _.right - W.right + k.right
                 },
-                U = e.modifiersData.offset;
-            if (x === k && U) {
-                var $ = U[c];
+                $ = e.modifiersData.offset;
+            if (x === j && $) {
+                var U = $[c];
                 Object.keys(V).forEach((function(e) {
-                    var t = [C, A].indexOf(e) >= 0 ? 1 : -1,
+                    var t = [S, A].indexOf(e) >= 0 ? 1 : -1,
                         n = [T, A].indexOf(e) >= 0 ? "y" : "x";
-                    V[e] += $[n] * t
+                    V[e] += U[n] * t
                 }))
             }
             return V
         }
         const le = {
             name: "flip",
             enabled: !0,
             phase: "main",
             fn: function(e) {
                 var t = e.state,
                     n = e.options,
                     i = e.name;
                 if (!t.modifiersData[i]._skip) {
-                    for (var r = n.mainAxis, o = void 0 === r || r, a = n.altAxis, s = void 0 === a || a, c = n.fallbackPlacements, l = n.padding, d = n.boundary, p = n.rootBoundary, u = n.altBoundary, f = n.flipVariations, h = void 0 === f || f, m = n.allowedAutoPlacements, v = t.options.placement, g = U(v), w = c || (g !== v && h ? function(e) {
-                            if (U(e) === D) return [];
+                    for (var r = n.mainAxis, o = void 0 === r || r, a = n.altAxis, s = void 0 === a || a, c = n.fallbackPlacements, l = n.padding, d = n.boundary, p = n.rootBoundary, u = n.altBoundary, f = n.flipVariations, h = void 0 === f || f, m = n.allowedAutoPlacements, v = t.options.placement, g = $(v), w = c || (g !== v && h ? function(e) {
+                            if ($(e) === D) return [];
                             var t = ee(e);
                             return [ne(e), t, ne(t)]
                         }(v) : [ee(v)]), y = [v].concat(w).reduce((function(e, n) {
-                            return e.concat(U(n) === D ? function(e, t) {
+                            return e.concat($(n) === D ? function(e, t) {
                                 void 0 === t && (t = {});
                                 var n = t,
                                     i = n.placement,
                                     r = n.boundary,
                                     o = n.rootBoundary,
                                     a = n.padding,
                                     s = n.flipVariations,
                                     c = n.allowedAutoPlacements,
                                     l = void 0 === c ? H : c,
-                                    d = $(i),
+                                    d = U(i),
                                     p = d ? s ? P : P.filter((function(e) {
-                                        return $(e) === d
+                                        return U(e) === d
                                     })) : M,
                                     u = p.filter((function(e) {
                                         return l.indexOf(e) >= 0
                                     }));
                                 0 === u.length && (u = p);
                                 var f = u.reduce((function(t, n) {
                                     return t[n] = ce(e, {
                                         placement: n,
                                         boundary: r,
                                         rootBoundary: o,
                                         padding: a
-                                    })[U(n)], t
+                                    })[$(n)], t
                                 }), {});
                                 return Object.keys(f).sort((function(e, t) {
                                     return f[e] - f[t]
                                 }))
                             }(t, {
                                 placement: n,
                                 boundary: d,
                                 rootBoundary: p,
                                 padding: l,
                                 flipVariations: h,
                                 allowedAutoPlacements: m
                             }) : n)
-                        }), []), b = t.rects.reference, E = t.rects.popper, x = new Map, O = !0, L = y[0], j = 0; j < y.length; j++) {
-                        var I = y[j],
-                            k = U(I),
-                            N = $(I) === R,
-                            W = [T, A].indexOf(k) >= 0,
+                        }), []), b = t.rects.reference, E = t.rects.popper, x = new Map, O = !0, L = y[0], k = 0; k < y.length; k++) {
+                        var R = y[k],
+                            j = $(R),
+                            N = U(R) === I,
+                            W = [T, A].indexOf(j) >= 0,
                             B = W ? "width" : "height",
-                            _ = ce(t, {
-                                placement: I,
+                            F = ce(t, {
+                                placement: R,
                                 boundary: d,
                                 rootBoundary: p,
                                 altBoundary: u,
                                 padding: l
                             }),
-                            F = W ? N ? C : S : N ? A : T;
-                        b[B] > E[B] && (F = ee(F));
-                        var q = ee(F),
+                            q = W ? N ? S : C : N ? A : T;
+                        b[B] > E[B] && (q = ee(q));
+                        var _ = ee(q),
                             V = [];
-                        if (o && V.push(_[k] <= 0), s && V.push(_[F] <= 0, _[q] <= 0), V.every((function(e) {
+                        if (o && V.push(F[j] <= 0), s && V.push(F[q] <= 0, F[_] <= 0), V.every((function(e) {
                                 return e
                             }))) {
-                            L = I, O = !1;
+                            L = R, O = !1;
                             break
                         }
-                        x.set(I, V)
+                        x.set(R, V)
                     }
                     if (O)
                         for (var z = function(e) {
                                 var t = y.find((function(t) {
                                     var n = x.get(t);
                                     if (n) return n.slice(0, e).every((function(e) {
                                         return e
@@ -1100,82 +1100,82 @@
                         g = void 0 === v ? 0 : v,
                         y = ce(t, {
                             boundary: d,
                             rootBoundary: p,
                             padding: f,
                             altBoundary: u
                         }),
-                        b = U(t.placement),
-                        E = $(t.placement),
+                        b = $(t.placement),
+                        E = U(t.placement),
                         x = !E,
                         O = z(b),
                         D = "x" === O ? "y" : "x",
                         M = t.modifiersData.popperOffsets,
-                        j = t.rects.reference,
-                        I = t.rects.popper,
-                        k = "function" == typeof g ? g(Object.assign({}, t.rects, {
+                        k = t.rects.reference,
+                        R = t.rects.popper,
+                        j = "function" == typeof g ? g(Object.assign({}, t.rects, {
                             placement: t.placement
                         })) : g,
-                        P = "number" == typeof k ? {
-                            mainAxis: k,
-                            altAxis: k
+                        P = "number" == typeof j ? {
+                            mainAxis: j,
+                            altAxis: j
                         } : Object.assign({
                             mainAxis: 0,
                             altAxis: 0
-                        }, k),
+                        }, j),
                         H = t.modifiersData.offset ? t.modifiersData.offset[t.placement] : null,
                         N = {
                             x: 0,
                             y: 0
                         };
                     if (M) {
                         if (s) {
-                            var W, B = "y" === O ? T : S,
-                                _ = "y" === O ? A : C,
-                                F = "y" === O ? "height" : "width",
-                                q = M[O],
-                                V = q + y[B],
-                                X = q - y[_],
-                                Y = m ? -I[F] / 2 : 0,
-                                G = E === R ? j[F] : I[F],
-                                J = E === R ? -I[F] : -j[F],
+                            var W, B = "y" === O ? T : C,
+                                F = "y" === O ? A : S,
+                                q = "y" === O ? "height" : "width",
+                                _ = M[O],
+                                V = _ + y[B],
+                                X = _ - y[F],
+                                Y = m ? -R[q] / 2 : 0,
+                                J = E === I ? k[q] : R[q],
+                                G = E === I ? -R[q] : -k[q],
                                 K = t.elements.arrow,
                                 Q = m && K ? w(K) : {
                                     width: 0,
                                     height: 0
                                 },
                                 Z = t.modifiersData["arrow#persistent"] ? t.modifiersData["arrow#persistent"].padding : {
                                     top: 0,
                                     right: 0,
                                     bottom: 0,
                                     left: 0
                                 },
                                 ee = Z[B],
-                                te = Z[_],
-                                ne = de(0, j[F], Q[F]),
-                                ie = x ? j[F] / 2 - Y - ne - ee - P.mainAxis : G - ne - ee - P.mainAxis,
-                                re = x ? -j[F] / 2 + Y + ne + te + P.mainAxis : J + ne + te + P.mainAxis,
+                                te = Z[F],
+                                ne = de(0, k[q], Q[q]),
+                                ie = x ? k[q] / 2 - Y - ne - ee - P.mainAxis : J - ne - ee - P.mainAxis,
+                                re = x ? -k[q] / 2 + Y + ne + te + P.mainAxis : G + ne + te + P.mainAxis,
                                 oe = t.elements.arrow && L(t.elements.arrow),
                                 ae = oe ? "y" === O ? oe.clientTop || 0 : oe.clientLeft || 0 : 0,
                                 se = null != (W = null == H ? void 0 : H[O]) ? W : 0,
-                                le = q + re - se,
-                                pe = de(m ? a(V, q + ie - se - ae) : V, q, m ? o(X, le) : X);
-                            M[O] = pe, N[O] = pe - q
+                                le = _ + re - se,
+                                pe = de(m ? a(V, _ + ie - se - ae) : V, _, m ? o(X, le) : X);
+                            M[O] = pe, N[O] = pe - _
                         }
                         if (l) {
-                            var ue, fe = "x" === O ? T : S,
-                                he = "x" === O ? A : C,
+                            var ue, fe = "x" === O ? T : C,
+                                he = "x" === O ? A : S,
                                 me = M[D],
                                 ve = "y" === D ? "height" : "width",
                                 ge = me + y[fe],
                                 we = me - y[he],
-                                ye = -1 !== [T, S].indexOf(b),
+                                ye = -1 !== [T, C].indexOf(b),
                                 be = null != (ue = null == H ? void 0 : H[D]) ? ue : 0,
-                                Ee = ye ? ge : me - j[ve] - I[ve] - be + P.altAxis,
-                                xe = ye ? me + j[ve] + I[ve] - be - P.altAxis : we,
+                                Ee = ye ? ge : me - k[ve] - R[ve] - be + P.altAxis,
+                                xe = ye ? me + k[ve] + R[ve] - be - P.altAxis : we,
                                 Oe = m && ye ? function(e, t, n) {
                                     var i = de(e, t, n);
                                     return i > n ? n : i
                                 }(Ee, me, xe) : de(m ? Ee : ge, me, m ? xe : we);
                             M[D] = Oe, N[D] = Oe - me
                         }
                         t.modifiersData[i] = N
@@ -1189,26 +1189,26 @@
                 phase: "main",
                 fn: function(e) {
                     var t, n = e.state,
                         i = e.name,
                         r = e.options,
                         o = n.elements.arrow,
                         a = n.modifiersData.popperOffsets,
-                        s = U(n.placement),
+                        s = $(n.placement),
                         c = z(s),
-                        l = [S, C].indexOf(s) >= 0 ? "height" : "width";
+                        l = [C, S].indexOf(s) >= 0 ? "height" : "width";
                     if (o && a) {
                         var d = function(e, t) {
                                 return ae("number" != typeof(e = "function" == typeof e ? e(Object.assign({}, t.rects, {
                                     placement: t.placement
                                 })) : e) ? e : se(e, M))
                             }(r.padding, n),
                             p = w(o),
-                            u = "y" === c ? T : S,
-                            f = "y" === c ? A : C,
+                            u = "y" === c ? T : C,
+                            f = "y" === c ? A : S,
                             h = n.rects.reference[l] + n.rects.reference[c] - a[c] - n.rects.popper[l],
                             m = a[c] - n.rects.reference[c],
                             v = L(o),
                             g = v ? "y" === c ? v.clientHeight || 0 : v.clientWidth || 0 : 0,
                             y = h / 2 - m / 2,
                             b = d[u],
                             E = g - p[l] - d[f],
@@ -1237,19 +1237,19 @@
                 right: e.right - t.width + n.x,
                 bottom: e.bottom - t.height + n.y,
                 left: e.left - t.width - n.x
             }
         }
 
         function he(e) {
-            return [T, C, A, S].some((function(t) {
+            return [T, S, A, C].some((function(t) {
                 return e[t] >= 0
             }))
         }
-        var me = F({
+        var me = q({
                 defaultModifiers: [V, {
                     name: "popperOffsets",
                     enabled: !0,
                     phase: "read",
                     fn: function(e) {
                         var t = e.state,
                             n = e.name;
@@ -1257,15 +1257,15 @@
                             reference: t.rects.reference,
                             element: t.rects.popper,
                             strategy: "absolute",
                             placement: t.placement
                         })
                     },
                     data: {}
-                }, J, K, Q, le, pe, ue, {
+                }, G, K, Q, le, pe, ue, {
                     name: "hide",
                     enabled: !0,
                     phase: "main",
                     requiresIfExists: ["preventOverflow"],
                     fn: function(e) {
                         var t = e.state,
                             n = e.name,
@@ -1332,51 +1332,51 @@
             var n
         }
 
         function Ae(e) {
             return [].concat(e)
         }
 
-        function Ce(e, t) {
+        function Se(e, t) {
             -1 === e.indexOf(t) && e.push(t)
         }
 
-        function Se(e) {
+        function Ce(e) {
             return [].slice.call(e)
         }
 
         function De(e) {
             return Object.keys(e).reduce((function(t, n) {
                 return void 0 !== e[n] && (t[n] = e[n]), t
             }), {})
         }
 
         function Me() {
             return document.createElement("div")
         }
 
-        function Re(e) {
+        function Ie(e) {
             return ["Element", "Fragment"].some((function(t) {
                 return Oe(e, t)
             }))
         }
 
-        function je(e, t) {
+        function ke(e, t) {
             e.forEach((function(e) {
                 e && (e.style.transitionDuration = t + "ms")
             }))
         }
 
-        function Ie(e, t) {
+        function Re(e, t) {
             e.forEach((function(e) {
                 e && e.setAttribute("data-state", t)
             }))
         }
 
-        function ke(e, t, n) {
+        function je(e, t, n) {
             var i = t + "EventListener";
             ["transitionend", "webkitTransitionEnd"].forEach((function(t) {
                 e[i](t, n)
             }))
         }
 
         function Pe(e, t) {
@@ -1397,23 +1397,23 @@
         }
 
         function Be() {
             var e = performance.now();
             e - Ne < 20 && (He.isTouch = !1, document.removeEventListener("mousemove", Be)), Ne = e
         }
 
-        function _e() {
+        function Fe() {
             var e, t = document.activeElement;
             if ((e = t) && e._tippy && e._tippy.reference === e) {
                 var n = t._tippy;
                 t.blur && !n.state.isVisible && t.blur()
             }
         }
-        var Fe = !("undefined" == typeof window || "undefined" == typeof document || !window.msCrypto),
-            qe = Object.assign({
+        var qe = !("undefined" == typeof window || "undefined" == typeof document || !window.msCrypto),
+            _e = Object.assign({
                 appendTo: Ee,
                 aria: {
                     content: "auto",
                     expanded: "auto"
                 },
                 delay: 0,
                 duration: [300, 250],
@@ -1457,68 +1457,68 @@
                 content: "",
                 inertia: !1,
                 maxWidth: 350,
                 role: "tooltip",
                 theme: "",
                 zIndex: 9999
             }),
-            Ve = Object.keys(qe);
+            Ve = Object.keys(_e);
 
-        function Ue(e) {
+        function $e(e) {
             var t = (e.plugins || []).reduce((function(t, n) {
                 var i, r = n.name,
                     o = n.defaultValue;
-                return r && (t[r] = void 0 !== e[r] ? e[r] : null != (i = qe[r]) ? i : o), t
+                return r && (t[r] = void 0 !== e[r] ? e[r] : null != (i = _e[r]) ? i : o), t
             }), {});
             return Object.assign({}, e, t)
         }
 
-        function $e(e, t) {
+        function Ue(e, t) {
             var n = Object.assign({}, t, {
                 content: Le(t.content, [e])
             }, t.ignoreAttributes ? {} : function(e, t) {
-                return (t ? Object.keys(Ue(Object.assign({}, qe, {
+                return (t ? Object.keys($e(Object.assign({}, _e, {
                     plugins: t
                 }))) : Ve).reduce((function(t, n) {
                     var i = (e.getAttribute("data-tippy-" + n) || "").trim();
                     if (!i) return t;
                     if ("content" === n) t[n] = i;
                     else try {
                         t[n] = JSON.parse(i)
                     } catch (e) {
                         t[n] = i
                     }
                     return t
                 }), {})
             }(e, t.plugins));
-            return n.aria = Object.assign({}, qe.aria, n.aria), n.aria = {
+            return n.aria = Object.assign({}, _e.aria, n.aria), n.aria = {
                 expanded: "auto" === n.aria.expanded ? t.interactive : n.aria.expanded,
                 content: "auto" === n.aria.content ? t.interactive ? null : "describedby" : n.aria.content
             }, n
         }
         var ze = function() {
             return "innerHTML"
         };
 
         function Xe(e, t) {
             e[ze()] = t
         }
 
         function Ye(e) {
             var t = Me();
-            return !0 === e ? t.className = we : (t.className = ye, Re(e) ? t.appendChild(e) : Xe(t, e)), t
+            return !0 === e ? t.className = we : (t.className = ye, Ie(e) ? t.appendChild(e) : Xe(t, e)), t
         }
 
-        function Ge(e, t) {
-            Re(t.content) ? (Xe(e, ""), e.appendChild(t.content)) : "function" != typeof t.content && (t.allowHTML ? Xe(e, t.content) : e.textContent = t.content)
+        function Je(e, t) {
+            Ie(t.content) ? (Xe(e, ""), e.appendChild(t.content)) : "function" != typeof t.content && (t.allowHTML ? Xe(e, t.content) : e.textContent = t.content)
         }
 
-        function Je(e) {
+        function Ge(e) {
             var t = e.firstElementChild,
-                n = Se(t.children);
+                n = Ce(t.children);
             return {
                 box: t,
                 content: n.find((function(e) {
                     return e.classList.contains(ve)
                 })),
                 arrow: n.find((function(e) {
                     return e.classList.contains(we) || e.classList.contains(ye)
@@ -1532,32 +1532,32 @@
         function Ke(e) {
             var t = Me(),
                 n = Me();
             n.className = "tippy-box", n.setAttribute("data-state", "hidden"), n.setAttribute("tabindex", "-1");
             var i = Me();
 
             function r(n, i) {
-                var r = Je(t),
+                var r = Ge(t),
                     o = r.box,
                     a = r.content,
                     s = r.arrow;
-                i.theme ? o.setAttribute("data-theme", i.theme) : o.removeAttribute("data-theme"), "string" == typeof i.animation ? o.setAttribute("data-animation", i.animation) : o.removeAttribute("data-animation"), i.inertia ? o.setAttribute("data-inertia", "") : o.removeAttribute("data-inertia"), o.style.maxWidth = "number" == typeof i.maxWidth ? i.maxWidth + "px" : i.maxWidth, i.role ? o.setAttribute("role", i.role) : o.removeAttribute("role"), n.content === i.content && n.allowHTML === i.allowHTML || Ge(a, e.props), i.arrow ? s ? n.arrow !== i.arrow && (o.removeChild(s), o.appendChild(Ye(i.arrow))) : o.appendChild(Ye(i.arrow)) : s && o.removeChild(s)
+                i.theme ? o.setAttribute("data-theme", i.theme) : o.removeAttribute("data-theme"), "string" == typeof i.animation ? o.setAttribute("data-animation", i.animation) : o.removeAttribute("data-animation"), i.inertia ? o.setAttribute("data-inertia", "") : o.removeAttribute("data-inertia"), o.style.maxWidth = "number" == typeof i.maxWidth ? i.maxWidth + "px" : i.maxWidth, i.role ? o.setAttribute("role", i.role) : o.removeAttribute("role"), n.content === i.content && n.allowHTML === i.allowHTML || Je(a, e.props), i.arrow ? s ? n.arrow !== i.arrow && (o.removeChild(s), o.appendChild(Ye(i.arrow))) : o.appendChild(Ye(i.arrow)) : s && o.removeChild(s)
             }
-            return i.className = ve, i.setAttribute("data-state", "hidden"), Ge(i, e.props), t.appendChild(n), n.appendChild(i), r(e.props, e.props), {
+            return i.className = ve, i.setAttribute("data-state", "hidden"), Je(i, e.props), t.appendChild(n), n.appendChild(i), r(e.props, e.props), {
                 popper: t,
                 onUpdate: r
             }
         }
         Ke.$$tippy = !0;
         var Qe = 1,
             Ze = [],
             et = [];
 
         function tt(e, t) {
-            var n, i, r, o, a, s, c, l, d = $e(e, Object.assign({}, qe, Ue(De(t)))),
+            var n, i, r, o, a, s, c, l, d = Ue(e, Object.assign({}, _e, $e(De(t)))),
                 p = !1,
                 u = !1,
                 f = !1,
                 h = !1,
                 m = [],
                 v = Te(X, d.interactiveDebounce),
                 g = Qe++,
@@ -1579,158 +1579,158 @@
                     },
                     plugins: w,
                     clearDelayTimeouts: function() {
                         clearTimeout(n), clearTimeout(i), cancelAnimationFrame(r)
                     },
                     setProps: function(t) {
                         if (!y.state.isDestroyed) {
-                            I("onBeforeUpdate", [y, t]), $();
+                            R("onBeforeUpdate", [y, t]), U();
                             var n = y.props,
-                                i = $e(e, Object.assign({}, n, De(t), {
+                                i = Ue(e, Object.assign({}, n, De(t), {
                                     ignoreAttributes: !0
                                 }));
-                            y.props = i, U(), n.interactiveDebounce !== i.interactiveDebounce && (H(), v = Te(X, i.interactiveDebounce)), n.triggerTarget && !i.triggerTarget ? Ae(n.triggerTarget).forEach((function(e) {
+                            y.props = i, $(), n.interactiveDebounce !== i.interactiveDebounce && (H(), v = Te(X, i.interactiveDebounce)), n.triggerTarget && !i.triggerTarget ? Ae(n.triggerTarget).forEach((function(e) {
                                 e.removeAttribute("aria-expanded")
-                            })) : i.triggerTarget && e.removeAttribute("aria-expanded"), P(), j(), x && x(n, i), y.popperInstance && (K(), Z().forEach((function(e) {
+                            })) : i.triggerTarget && e.removeAttribute("aria-expanded"), P(), k(), x && x(n, i), y.popperInstance && (K(), Z().forEach((function(e) {
                                 requestAnimationFrame(e._tippy.popperInstance.forceUpdate)
-                            }))), I("onAfterUpdate", [y, t])
+                            }))), R("onAfterUpdate", [y, t])
                         }
                     },
                     setContent: function(e) {
                         y.setProps({
                             content: e
                         })
                     },
                     show: function() {
                         var e = y.state.isVisible,
                             t = y.state.isDestroyed,
                             n = !y.state.isEnabled,
                             i = He.isTouch && !y.props.touch,
-                            r = xe(y.props.duration, 0, qe.duration);
-                        if (!(e || t || n || i || S().hasAttribute("disabled") || (I("onShow", [y], !1), !1 === y.props.onShow(y)))) {
-                            if (y.state.isVisible = !0, C() && (E.style.visibility = "visible"), j(), _(), y.state.isMounted || (E.style.transition = "none"), C()) {
+                            r = xe(y.props.duration, 0, _e.duration);
+                        if (!(e || t || n || i || C().hasAttribute("disabled") || (R("onShow", [y], !1), !1 === y.props.onShow(y)))) {
+                            if (y.state.isVisible = !0, S() && (E.style.visibility = "visible"), k(), F(), y.state.isMounted || (E.style.transition = "none"), S()) {
                                 var o = M();
-                                je([o.box, o.content], 0)
+                                ke([o.box, o.content], 0)
                             }
                             var a, c, l;
                             s = function() {
                                 var e;
                                 if (y.state.isVisible && !h) {
-                                    if (h = !0, E.offsetHeight, E.style.transition = y.props.moveTransition, C() && y.props.animation) {
+                                    if (h = !0, E.offsetHeight, E.style.transition = y.props.moveTransition, S() && y.props.animation) {
                                         var t = M(),
                                             n = t.box,
                                             i = t.content;
-                                        je([n, i], r), Ie([n, i], "visible")
+                                        ke([n, i], r), Re([n, i], "visible")
                                     }
-                                    k(), P(), Ce(et, y), null == (e = y.popperInstance) || e.forceUpdate(), I("onMount", [y]), y.props.animation && C() && function(e, t) {
-                                        q(e, (function() {
-                                            y.state.isShown = !0, I("onShown", [y])
+                                    j(), P(), Se(et, y), null == (e = y.popperInstance) || e.forceUpdate(), R("onMount", [y]), y.props.animation && S() && function(e, t) {
+                                        _(e, (function() {
+                                            y.state.isShown = !0, R("onShown", [y])
                                         }))
                                     }(r)
                                 }
-                            }, c = y.props.appendTo, l = S(), (a = y.props.interactive && c === Ee || "parent" === c ? l.parentNode : Le(c, [l])).contains(E) || a.appendChild(E), y.state.isMounted = !0, K()
+                            }, c = y.props.appendTo, l = C(), (a = y.props.interactive && c === Ee || "parent" === c ? l.parentNode : Le(c, [l])).contains(E) || a.appendChild(E), y.state.isMounted = !0, K()
                         }
                     },
                     hide: function() {
                         var e = !y.state.isVisible,
                             t = y.state.isDestroyed,
                             n = !y.state.isEnabled,
-                            i = xe(y.props.duration, 1, qe.duration);
-                        if (!(e || t || n) && (I("onHide", [y], !1), !1 !== y.props.onHide(y))) {
-                            if (y.state.isVisible = !1, y.state.isShown = !1, h = !1, p = !1, C() && (E.style.visibility = "hidden"), H(), F(), j(!0), C()) {
+                            i = xe(y.props.duration, 1, _e.duration);
+                        if (!(e || t || n) && (R("onHide", [y], !1), !1 !== y.props.onHide(y))) {
+                            if (y.state.isVisible = !1, y.state.isShown = !1, h = !1, p = !1, S() && (E.style.visibility = "hidden"), H(), q(), k(!0), S()) {
                                 var r = M(),
                                     o = r.box,
                                     a = r.content;
-                                y.props.animation && (je([o, a], i), Ie([o, a], "hidden"))
+                                y.props.animation && (ke([o, a], i), Re([o, a], "hidden"))
                             }
-                            k(), P(), y.props.animation ? C() && function(e, t) {
-                                q(e, (function() {
+                            j(), P(), y.props.animation ? S() && function(e, t) {
+                                _(e, (function() {
                                     !y.state.isVisible && E.parentNode && E.parentNode.contains(E) && t()
                                 }))
                             }(i, y.unmount) : y.unmount()
                         }
                     },
                     hideWithInteractivity: function(e) {
-                        D().addEventListener("mousemove", v), Ce(Ze, v), v(e)
+                        D().addEventListener("mousemove", v), Se(Ze, v), v(e)
                     },
                     enable: function() {
                         y.state.isEnabled = !0
                     },
                     disable: function() {
                         y.hide(), y.state.isEnabled = !1
                     },
                     unmount: function() {
                         y.state.isVisible && y.hide(), y.state.isMounted && (Q(), Z().forEach((function(e) {
                             e._tippy.unmount()
                         })), E.parentNode && E.parentNode.removeChild(E), et = et.filter((function(e) {
                             return e !== y
-                        })), y.state.isMounted = !1, I("onHidden", [y]))
+                        })), y.state.isMounted = !1, R("onHidden", [y]))
                     },
                     destroy: function() {
-                        y.state.isDestroyed || (y.clearDelayTimeouts(), y.unmount(), $(), delete e._tippy, y.state.isDestroyed = !0, I("onDestroy", [y]))
+                        y.state.isDestroyed || (y.clearDelayTimeouts(), y.unmount(), U(), delete e._tippy, y.state.isDestroyed = !0, R("onDestroy", [y]))
                     }
                 };
             if (!d.render) return y;
             var b = d.render(y),
                 E = b.popper,
                 x = b.onUpdate;
             E.setAttribute("data-tippy-root", ""), E.id = "tippy-" + y.id, y.popper = E, e._tippy = y, E._tippy = y;
             var O = w.map((function(e) {
                     return e.fn(y)
                 })),
                 L = e.hasAttribute("aria-expanded");
-            return U(), P(), j(), I("onCreate", [y]), d.showOnCreate && ee(), E.addEventListener("mouseenter", (function() {
+            return $(), P(), k(), R("onCreate", [y]), d.showOnCreate && ee(), E.addEventListener("mouseenter", (function() {
                 y.props.interactive && y.state.isVisible && y.clearDelayTimeouts()
             })), E.addEventListener("mouseleave", (function() {
                 y.props.interactive && y.props.trigger.indexOf("mouseenter") >= 0 && D().addEventListener("mousemove", v)
             })), y;
 
             function T() {
                 var e = y.props.touch;
                 return Array.isArray(e) ? e : [e, 0]
             }
 
             function A() {
                 return "hold" === T()[0]
             }
 
-            function C() {
+            function S() {
                 var e;
                 return !(null == (e = y.props.render) || !e.$$tippy)
             }
 
-            function S() {
+            function C() {
                 return c || e
             }
 
             function D() {
-                var e, t, n = S().parentNode;
+                var e, t, n = C().parentNode;
                 return n ? null != (t = Ae(n)[0]) && null != (e = t.ownerDocument) && e.body ? t.ownerDocument : document : document
             }
 
             function M() {
-                return Je(E)
+                return Ge(E)
             }
 
-            function R(e) {
-                return y.state.isMounted && !y.state.isVisible || He.isTouch || o && "focus" === o.type ? 0 : xe(y.props.delay, e ? 0 : 1, qe.delay)
+            function I(e) {
+                return y.state.isMounted && !y.state.isVisible || He.isTouch || o && "focus" === o.type ? 0 : xe(y.props.delay, e ? 0 : 1, _e.delay)
             }
 
-            function j(e) {
+            function k(e) {
                 void 0 === e && (e = !1), E.style.pointerEvents = y.props.interactive && !e ? "" : "none", E.style.zIndex = "" + y.props.zIndex
             }
 
-            function I(e, t, n) {
+            function R(e, t, n) {
                 var i;
                 void 0 === n && (n = !0), O.forEach((function(n) {
                     n[e] && n[e].apply(n, t)
                 })), n && (i = y.props)[e].apply(i, t)
             }
 
-            function k() {
+            function j() {
                 var t = y.props.aria;
                 if (t.content) {
                     var n = "aria-" + t.content,
                         i = E.id;
                     Ae(y.props.triggerTarget || e).forEach((function(e) {
                         var t = e.getAttribute(n);
                         if (y.state.isVisible) e.setAttribute(n, t ? t + " " + i : i);
@@ -1740,15 +1740,15 @@
                         }
                     }))
                 }
             }
 
             function P() {
                 !L && y.props.aria.expanded && Ae(y.props.triggerTarget || e).forEach((function(e) {
-                    y.props.interactive ? e.setAttribute("aria-expanded", y.state.isVisible && e === S() ? "true" : "false") : e.removeAttribute("aria-expanded")
+                    y.props.interactive ? e.setAttribute("aria-expanded", y.state.isVisible && e === C() ? "true" : "false") : e.removeAttribute("aria-expanded")
                 }))
             }
 
             function H() {
                 D().removeEventListener("mousemove", v), Ze = Ze.filter((function(e) {
                     return e !== v
                 }))
@@ -1759,104 +1759,104 @@
                     var n = t.composedPath && t.composedPath()[0] || t.target;
                     if (!y.props.interactive || !Pe(E, n)) {
                         if (Ae(y.props.triggerTarget || e).some((function(e) {
                                 return Pe(e, n)
                             }))) {
                             if (He.isTouch) return;
                             if (y.state.isVisible && y.props.trigger.indexOf("click") >= 0) return
-                        } else I("onClickOutside", [y, t]);
+                        } else R("onClickOutside", [y, t]);
                         !0 === y.props.hideOnClick && (y.clearDelayTimeouts(), y.hide(), u = !0, setTimeout((function() {
                             u = !1
-                        })), y.state.isMounted || F())
+                        })), y.state.isMounted || q())
                     }
                 }
             }
 
             function W() {
                 f = !0
             }
 
             function B() {
                 f = !1
             }
 
-            function _() {
+            function F() {
                 var e = D();
                 e.addEventListener("mousedown", N, !0), e.addEventListener("touchend", N, be), e.addEventListener("touchstart", B, be), e.addEventListener("touchmove", W, be)
             }
 
-            function F() {
+            function q() {
                 var e = D();
                 e.removeEventListener("mousedown", N, !0), e.removeEventListener("touchend", N, be), e.removeEventListener("touchstart", B, be), e.removeEventListener("touchmove", W, be)
             }
 
-            function q(e, t) {
+            function _(e, t) {
                 var n = M().box;
 
                 function i(e) {
-                    e.target === n && (ke(n, "remove", i), t())
+                    e.target === n && (je(n, "remove", i), t())
                 }
                 if (0 === e) return t();
-                ke(n, "remove", a), ke(n, "add", i), a = i
+                je(n, "remove", a), je(n, "add", i), a = i
             }
 
             function V(t, n, i) {
                 void 0 === i && (i = !1), Ae(y.props.triggerTarget || e).forEach((function(e) {
                     e.addEventListener(t, n, i), m.push({
                         node: e,
                         eventType: t,
                         handler: n,
                         options: i
                     })
                 }))
             }
 
-            function U() {
+            function $() {
                 var e;
                 A() && (V("touchstart", z, {
                     passive: !0
                 }), V("touchend", Y, {
                     passive: !0
                 })), (e = y.props.trigger, e.split(/\s+/).filter(Boolean)).forEach((function(e) {
                     if ("manual" !== e) switch (V(e, z), e) {
                         case "mouseenter":
                             V("mouseleave", Y);
                             break;
                         case "focus":
-                            V(Fe ? "focusout" : "blur", G);
+                            V(qe ? "focusout" : "blur", J);
                             break;
                         case "focusin":
-                            V("focusout", G)
+                            V("focusout", J)
                     }
                 }))
             }
 
-            function $() {
+            function U() {
                 m.forEach((function(e) {
                     var t = e.node,
                         n = e.eventType,
                         i = e.handler,
                         r = e.options;
                     t.removeEventListener(n, i, r)
                 })), m = []
             }
 
             function z(e) {
                 var t, n = !1;
-                if (y.state.isEnabled && !J(e) && !u) {
+                if (y.state.isEnabled && !G(e) && !u) {
                     var i = "focus" === (null == (t = o) ? void 0 : t.type);
                     o = e, c = e.currentTarget, P(), !y.state.isVisible && Oe(e, "MouseEvent") && Ze.forEach((function(t) {
                         return t(e)
                     })), "click" === e.type && (y.props.trigger.indexOf("mouseenter") < 0 || p) && !1 !== y.props.hideOnClick && y.state.isVisible ? n = !0 : ee(e), "click" === e.type && (p = !n), n && !i && te(e)
                 }
             }
 
             function X(e) {
                 var t = e.target,
-                    n = S().contains(t) || E.contains(t);
+                    n = C().contains(t) || E.contains(t);
                 if ("mousemove" !== e.type || !n) {
                     var i = Z().concat(E).map((function(e) {
                         var t, n = null == (t = e._tippy.popperInstance) ? void 0 : t.state;
                         return n ? {
                             popperRect: e.getBoundingClientRect(),
                             popperState: n,
                             props: d
@@ -1883,37 +1883,37 @@
                             return u || f || h || m
                         }))
                     })(i, e) && (H(), te(e))
                 }
             }
 
             function Y(e) {
-                J(e) || y.props.trigger.indexOf("click") >= 0 && p || (y.props.interactive ? y.hideWithInteractivity(e) : te(e))
+                G(e) || y.props.trigger.indexOf("click") >= 0 && p || (y.props.interactive ? y.hideWithInteractivity(e) : te(e))
             }
 
-            function G(e) {
-                y.props.trigger.indexOf("focusin") < 0 && e.target !== S() || y.props.interactive && e.relatedTarget && E.contains(e.relatedTarget) || te(e)
+            function J(e) {
+                y.props.trigger.indexOf("focusin") < 0 && e.target !== C() || y.props.interactive && e.relatedTarget && E.contains(e.relatedTarget) || te(e)
             }
 
-            function J(e) {
+            function G(e) {
                 return !!He.isTouch && A() !== e.type.indexOf("touch") >= 0
             }
 
             function K() {
                 Q();
                 var t = y.props,
                     n = t.popperOptions,
                     i = t.placement,
                     r = t.offset,
                     o = t.getReferenceClientRect,
                     a = t.moveTransition,
-                    c = C() ? Je(E).arrow : null,
+                    c = S() ? Ge(E).arrow : null,
                     l = o ? {
                         getBoundingClientRect: o,
-                        contextElement: o.contextElement || S()
+                        contextElement: o.contextElement || C()
                     } : e,
                     d = [{
                         name: "offset",
                         options: {
                             offset: r
                         }
                     }, {
@@ -1939,23 +1939,23 @@
                     }, {
                         name: "$$tippy",
                         enabled: !0,
                         phase: "beforeWrite",
                         requires: ["computeStyles"],
                         fn: function(e) {
                             var t = e.state;
-                            if (C()) {
+                            if (S()) {
                                 var n = M().box;
                                 ["placement", "reference-hidden", "escaped"].forEach((function(e) {
                                     "placement" === e ? n.setAttribute("data-placement", t.placement) : t.attributes.popper["data-popper-" + e] ? n.setAttribute("data-" + e, "") : n.removeAttribute("data-" + e)
                                 })), t.attributes.popper = {}
                             }
                         }
                     }];
-                C() && c && d.push({
+                S() && c && d.push({
                     name: "arrow",
                     options: {
                         element: c,
                         padding: 3
                     }
                 }), d.push.apply(d, (null == n ? void 0 : n.modifiers) || []), y.popperInstance = me(l, E, Object.assign({}, n, {
                     placement: i,
@@ -1965,60 +1965,60 @@
             }
 
             function Q() {
                 y.popperInstance && (y.popperInstance.destroy(), y.popperInstance = null)
             }
 
             function Z() {
-                return Se(E.querySelectorAll("[data-tippy-root]"))
+                return Ce(E.querySelectorAll("[data-tippy-root]"))
             }
 
             function ee(e) {
-                y.clearDelayTimeouts(), e && I("onTrigger", [y, e]), _();
-                var t = R(!0),
+                y.clearDelayTimeouts(), e && R("onTrigger", [y, e]), F();
+                var t = I(!0),
                     i = T(),
                     r = i[0],
                     o = i[1];
                 He.isTouch && "hold" === r && o && (t = o), t ? n = setTimeout((function() {
                     y.show()
                 }), t) : y.show()
             }
 
             function te(e) {
-                if (y.clearDelayTimeouts(), I("onUntrigger", [y, e]), y.state.isVisible) {
+                if (y.clearDelayTimeouts(), R("onUntrigger", [y, e]), y.state.isVisible) {
                     if (!(y.props.trigger.indexOf("mouseenter") >= 0 && y.props.trigger.indexOf("click") >= 0 && ["mouseleave", "mousemove"].indexOf(e.type) >= 0 && p)) {
-                        var t = R(!1);
+                        var t = I(!1);
                         t ? i = setTimeout((function() {
                             y.state.isVisible && y.hide()
                         }), t) : r = requestAnimationFrame((function() {
                             y.hide()
                         }))
                     }
-                } else F()
+                } else q()
             }
         }
 
         function nt(e, t) {
             void 0 === t && (t = {});
-            var n = qe.plugins.concat(t.plugins || []);
-            document.addEventListener("touchstart", We, be), window.addEventListener("blur", _e);
+            var n = _e.plugins.concat(t.plugins || []);
+            document.addEventListener("touchstart", We, be), window.addEventListener("blur", Fe);
             var i, r = Object.assign({}, t, {
                     plugins: n
                 }),
-                o = (i = e, Re(i) ? [i] : function(e) {
+                o = (i = e, Ie(i) ? [i] : function(e) {
                     return Oe(e, "NodeList")
-                }(i) ? Se(i) : Array.isArray(i) ? i : Se(document.querySelectorAll(i))).reduce((function(e, t) {
+                }(i) ? Ce(i) : Array.isArray(i) ? i : Ce(document.querySelectorAll(i))).reduce((function(e, t) {
                     var n = t && tt(t, r);
                     return n && e.push(n), e
                 }), []);
-            return Re(e) ? o[0] : o
+            return Ie(e) ? o[0] : o
         }
-        nt.defaultProps = qe, nt.setDefaultProps = function(e) {
+        nt.defaultProps = _e, nt.setDefaultProps = function(e) {
             Object.keys(e).forEach((function(t) {
-                qe[t] = e[t]
+                _e[t] = e[t]
             }))
         }, nt.currentInput = He, Object.assign({}, K, {
             effect: function(e) {
                 var t = e.state,
                     n = {
                         popper: {
                             position: t.options.strategy,
@@ -2091,20 +2091,28 @@
                 for (let e = 0; e < r.length; e++) {
                     const t = r[e];
                     "true" == t.dataset.tooltip && (new wt(t), delete t.dataset.tooltip)
                 }
             }
         }
 
-        function Et(e) {
+        function Et() {
+            let e = window.location.href,
+                t = window.scrollY,
+                n = window.scrollX,
+                i = new URL(e);
+            i.searchParams.set("scrollY", `${t}`), i.searchParams.set("scrollX", `${n}`), window.location.href = i.toString()
+        }
+
+        function xt(e) {
             if (!e) return;
             const t = new URL(e.href);
             window.scrollY > 100 && t.searchParams.set("scrollY", `${window.scrollY}`), window.scrollX > 100 && t.searchParams.set("scrollX", `${window.scrollX}`), e.href = t.toString()
         }
-        class xt {
+        class Ot {
             constructor(e) {
                 this.editor = e
             }
             openEditor() {
                 this.editor.openEditor()
             }
             closeEditor() {
@@ -2128,37 +2136,85 @@
                         const r = i.firstElementChild;
                         return r.classList.add("wagtail-fedit-initialized"), n.parentNode.insertBefore(r, n), n.parentNode.removeChild(n), this.editor.wrapperElement = r, this.editor.initNewEditors(), this.editor.init(), t(r), n
                     };
                     if ("string" != typeof e) return "function" == typeof e ? (this.editor.wrapperElement.editorAPI = this, void e(i)) : void 0;
                     i(e)
                 }))
             }
+            fetch(e, t, n) {
+                return i = this, r = void 0, a = function*() {
+                    let i = new Headers;
+                    return i.append("X-Requested-With", "XMLHttpRequest"), i.append("X-CSRFToken", function(e) {
+                        let t = null;
+                        if (document.cookie && "" !== document.cookie) {
+                            const n = document.cookie.split(";");
+                            for (let i = 0; i < n.length; i++) {
+                                const r = n[i].trim();
+                                if (r.substring(0, 10) === e + "=") {
+                                    t = decodeURIComponent(r.substring(10));
+                                    break
+                                }
+                            }
+                        }
+                        return t
+                    }("csrftoken")), fetch(e, {
+                        method: t,
+                        headers: i,
+                        body: JSON.stringify(n)
+                    }).then((e => e.json()))
+                }, new((o = void 0) || (o = Promise))((function(e, t) {
+                    function n(e) {
+                        try {
+                            c(a.next(e))
+                        } catch (e) {
+                            t(e)
+                        }
+                    }
+
+                    function s(e) {
+                        try {
+                            c(a.throw(e))
+                        } catch (e) {
+                            t(e)
+                        }
+                    }
+
+                    function c(t) {
+                        var i;
+                        t.done ? e(t.value) : (i = t.value, i instanceof o ? i : new o((function(e) {
+                            e(i)
+                        }))).then(n, s)
+                    }
+                    c((a = a.apply(i, r || [])).next())
+                }));
+                var i, r, o, a
+            }
             refetch() {
                 return this.editor.refetch()
             }
             execRelated(e) {
                 for (const t of this.editor.relatedWrappers) e(t.editorAPI)
             }
         }
-        const Ot = "wagtail-fedit-modal",
-            Lt = `\n<div class="${Ot}-wrapper">\n    <div class="${Ot}" id="${Ot}-__ID__-modal">\n    </div>\n</div>`;
-        class Tt {
+        const Lt = "wagtail-fedit-modal",
+            Tt = `\n<div class="${Lt}-wrapper">\n    <div class="${Lt}" id="${Lt}-__ID__-modal">\n    </div>\n</div>`;
+        class At {
             constructor(e) {
-                this.options = e, this.modalHtml = Lt.replace("__ID__", this.options.modalId)
+                this.options = e, this.modalHtml = Tt.replace("__ID__", this.options.modalId)
             }
             static get modalWrapper() {
-                var e = document.querySelector(`#${Ot}-wrapper`);
-                return e || ((e = document.createElement("div")).id = `${Ot}-wrapper`, e.classList.add(`${Ot}-wrapper`), document.body.appendChild(e), e)
+                var e = document.querySelector(`#${Lt}-wrapper`);
+                return e || ((e = document.createElement("div")).id = `${Lt}-wrapper`, e.classList.add(`${Lt}-wrapper`), document.body.appendChild(e), e)
             }
             get wrapper() {
                 return this.constructor.modalWrapper
             }
             get modal() {
-                var e = this.wrapper.querySelector(`.${Ot}`);
-                e && e.id !== `${Ot}-${this.options.modalId}-modal` && (e.remove(), e = null), e || (e = this.buildModal());
+                var e = this.wrapper.querySelector(`.${Lt}`);
+                e && e.id !== `${Lt}-${this.options.modalId}-modal` && (e.remove(), e = null), e || (e = this.buildModal());
                 var t = e;
                 return t.modal = this, t
             }
             get innerHTML() {
                 return this.modal.innerHTML
             }
             set innerHTML(e) {
@@ -2171,16 +2227,16 @@
                 return this.modal.classList
             }
             get children() {
                 return this.modal.children
             }
             buildModal() {
                 var e = this.wrapper,
-                    t = e.querySelector(`.${Ot}`);
-                return t || (e.innerHTML = this.modalHtml, t = e.querySelector(`.${Ot}`)), t.modal || (t.modal = this), t
+                    t = e.querySelector(`.${Lt}`);
+                return t || (e.innerHTML = this.modalHtml, t = e.querySelector(`.${Lt}`)), t.modal || (t.modal = this), t
             }
             addClass(e) {
                 this.modal.classList.add(e)
             }
             removeClass(e) {
                 this.modal.classList.remove(e)
             }
@@ -2210,15 +2266,15 @@
             addEventListener(e, t) {
                 this.modal.addEventListener(e, t)
             }
             removeEventListener(e, t) {
                 this.modal.removeEventListener(e, t)
             }
         }
-        class At {
+        class St {
             constructor(e) {
                 this.executeOnloadImmediately = !1;
                 const {
                     id: t,
                     className: n,
                     srcdoc: i = null,
                     url: r = null,
@@ -2248,15 +2304,15 @@
                 return null === (e = this.document) || void 0 === e ? void 0 : e.querySelector("#wagtail-fedit-form")
             }
             get formWrapper() {
                 var e;
                 return null === (e = this.document) || void 0 === e ? void 0 : e.querySelector(".wagtail-fedit-form-wrapper")
             }
             destroy() {
-                this.iframe.remove()
+                this.iframe.remove(), this.resizeInterval && (clearInterval(this.resizeInterval), delete this.resizeInterval)
             }
             update(e, t) {
                 this.srcdoc = t, this.url = e, this._renderFrame(this.url, this.srcdoc, (({
                     newFrame: e
                 }) => {
                     this.iframe.remove(), this.iframe = e, this.onLoad({
                         newFrame: e
@@ -2266,37 +2322,41 @@
             render() {
                 return this.iframe || (this.iframe = this._renderFrame(this.url, this.srcdoc, this.onLoad)), this.iframe
             }
             _renderFrame(e, t, n, i = (() => {})) {
                 const r = document.createElement("iframe");
                 return t ? r.srcdoc = t : r.src = e, r.id = this.id, r.className = this.className, r.onload = () => {
                     if (!this.formElement) return void i();
-                    let e, t = this.formElement,
-                        o = t.scrollHeight;
-                    this.onResize && this.onResize(0, o), this.onResize && (e = setInterval((() => {
-                        t ? o !== t.scrollHeight && (this.onResize(o, t.scrollHeight), o = t.scrollHeight) : clearInterval(e)
+                    let e = this.formElement,
+                        t = e.scrollHeight;
+                    this.onResize && this.onResize(0, t), this.resizeInterval && clearInterval(this.resizeInterval), this.onResize && (this.resizeInterval = setInterval((() => {
+                        if (e) try {
+                            t !== e.scrollHeight && (this.onResize(t, e.scrollHeight), t = e.scrollHeight)
+                        } catch (e) {
+                            clearInterval(this.resizeInterval), console.error(e), i()
+                        } else clearInterval(this.resizeInterval)
                     }), 25));
-                    const a = this.document.querySelector(".wagtail-fedit-cancel-button");
-                    a && a.addEventListener("click", (() => {
-                        clearInterval(e), this.onCancel()
+                    const o = this.document.querySelector(".wagtail-fedit-cancel-button");
+                    o && o.addEventListener("click", (() => {
+                        clearInterval(this.resizeInterval), this.onCancel()
                     })), "complete" === this.document.readyState || this.executeOnloadImmediately ? n({
                         newFrame: r
                     }) : r.contentWindow.addEventListener("DOMContentLoaded", (() => {
                         n({
                             newFrame: r
                         })
                     }))
                 }, r.onerror = () => {
                     i()
                 }, r
             }
         }
         class Ct extends EventTarget {
             constructor(e) {
-                super(), this.api = new xt(this), this.initialTitle = document.title, this.wrapperElement = e, this.sharedContext = null, this.editBtn = null, this.iframe = null, this.init(), window.location.hash === `#${this.wrapperElement.id}` && (this.openEditor(), this.focus())
+                super(), this.api = new Ot(this), this.initialTitle = document.title, this.wrapperElement = e, this.sharedContext = null, this.editBtn = null, this.iframe = null, this.init(), window.location.hash === `#${this.wrapperElement.id}` && (this.openEditor(), this.focus())
             }
             get editUrl() {
                 return this.wrapperElement.dataset.editUrl
             }
             get refetchUrl() {
                 return this.wrapperElement.dataset.refetchUrl
             }
@@ -2341,50 +2401,42 @@
                 bt(this.wrapperElement)
             }
             focus() {
                 this.wrapperElement.focus()
             }
             refetch() {
                 return new Promise(((e, t) => {
-                    fetch(this.getRefetchUrl()).then((e => e.json())).then((t => {
+                    fetch(this.refetchUrl).then((e => e.json())).then((t => {
                         t.success ? (this.onResponse(t), e(t)) : console.error("Errors rendering response, failed to refetch", t)
                     })).catch((e => {
                         console.error("Failed to refetch", e), t(e)
                     }))
                 }))
             }
             onResponse(e) {
                 throw new Error("onResponse not implemented, cannot call super")
             }
-            getEditUrl() {
-                const e = new URL(window.location.href);
-                return e.pathname = this.editUrl, this.sharedContext && e.searchParams.set("shared_context", this.sharedContext), e.toString()
-            }
-            getRefetchUrl() {
-                const e = new URL(window.location.href);
-                return e.pathname = this.refetchUrl, this.sharedContext && e.searchParams.set("shared_context", this.sharedContext), e.toString()
-            }
             get frameOptions() {
                 return {}
             }
             openIframe(e, t) {
-                this.iframe || (this.iframe = new At(Object.assign(Object.assign({
-                    url: this.getEditUrl(),
+                this.iframe || (this.iframe = new St(Object.assign(Object.assign({
+                    url: this.editUrl,
                     id: "wagtail-fedit-iframe",
                     className: null,
                     executeOnloadImmediately: !0
                 }, this.frameOptions), {
                     onLoad: () => {
                         const t = e => {
                             e.preventDefault();
                             const n = new FormData(this.iframe.formElement);
                             this.executeEvent(window.wagtailFedit.EVENTS.SUBMIT, {
                                 element: this.wrapperElement,
                                 formData: n
-                            }), fetch(this.getEditUrl(), {
+                            }), fetch(this.editUrl, {
                                 method: "POST",
                                 body: n
                             }).then((e => e.json())).then((e => {
                                 if (!e.success) {
                                     console.error("Errors rendering response", e);
                                     let n = document.createElement("div");
                                     n.innerHTML = e.html, this.iframe.mainElement.innerHTML = n.querySelector("#main").innerHTML, this.iframe.formElement.onsubmit = t;
@@ -2423,15 +2475,15 @@
                     },
                     onCancel: () => {
                         this.closeEditor()
                     }
                 })), e.appendChild(this.iframe.element)), t(this.iframe)
             }
             openEditor() {
-                this.modal || (this.modal = new Tt({
+                this.modal || (this.modal = new At({
                     modalId: this.wrapperElement.id
                 })), this.opened = !0, this.openIframe(this.modal, (e => {
                     const t = document.createElement("button");
                     t.innerHTML = "&times;", t.classList.add("wagtail-fedit-close-button"), t.addEventListener("click", this.closeEditor.bind(this)), this.modal.appendChild(t), this.executeEvent(window.wagtailFedit.EVENTS.EDITOR_OPEN, {
                         iframe: this.iframe,
                         modal: this.modal
                     }), this.modal.openModal()
@@ -2446,15 +2498,15 @@
                 }), t.editor = this, t.api = this.api, e.startsWith(`${window.wagtailFedit.NAMESPACE}:`) || (e = `${window.wagtailFedit.NAMESPACE}:${e}`);
                 const n = new CustomEvent(e, {
                     detail: t
                 });
                 super.dispatchEvent(n), this.wrapperElement.dispatchEvent(n), document.dispatchEvent(n)
             }
         }
-        class St {
+        class Dt {
             constructor(e) {
                 this.publishButton = e, this.publishButtonsWrapper = e.parentElement.querySelector(".wagtail-fedit-form-buttons"), this.publishButtonsWrapper.querySelectorAll(".wagtail-fedit-userbar-button"), this.init()
             }
             init() {
                 this.publishButton.addEventListener("click", (e => {
                     this.publishButtonsWrapper.classList.contains("open") ? this.publishButtonsWrapper.animate([{
                         opacity: 1,
@@ -2478,30 +2530,30 @@
                         easing: "ease-in-out"
                     }).onfinish = () => {
                         this.publishButtonsWrapper.classList.add("open")
                     })
                 }))
             }
         }
-        class Dt extends Ct {
+        class Mt extends Ct {
             static get funcMap() {
                 return window
             }
             onResponse(e) {
                 const t = e.func.name,
                     n = e.func.target;
                 if (!t || !n) return void console.error("Invalid response", e);
                 const i = document.querySelector(n);
                 if (!i) return void console.error("Target element not found", n);
                 const r = this.constructor.funcMap[t];
                 if (r) return r(i, e);
                 console.error("Function not found", t)
             }
         }
-        class Mt extends Ct {
+        class It extends Ct {
             onResponse(e) {
                 return this.api.updateHtml((t => {
                     this.wrapperElement.animate([{
                         opacity: 1
                     }, {
                         opacity: 0
                     }], {
@@ -2522,15 +2574,63 @@
                             n.style.opacity = "1"
                         }
                     }
                 }))
             }
         }
 
-        function Rt() {
+        function kt(e) {
+            return class extends e {
+                constructor(...e) {
+                    super(...e);
+                    let t = this.wrapperElement.querySelectorAll("[data-direction]");
+                    for (let e = 0; e < t.length; e++) {
+                        let n = t[e],
+                            i = n.dataset.url;
+                        n.addEventListener("click", (e => {
+                            e.preventDefault(), this.api.fetch(i, "POST", {}).then((e => {
+                                e.success ? Et() : e.error ? alert("Failed to move block: " + e.error) : alert("Failed to move block")
+                            })).catch((e => {
+                                console.error("Failed to move block", e), alert("Failed to move block")
+                            }))
+                        }))
+                    }
+                }
+            }
+        }
+        class Rt extends(kt(It)) {}
+        class jt extends It {
+            get buttonsElement() {
+                return this.wrapperElement.querySelector(".wagtail-fedit-buttons")
+            }
+            get formElement() {
+                return this.wrapperElement.querySelector(".wagtail-fedit-adapter-form")
+            }
+            get contentElement() {
+                return this.wrapperElement.querySelector(".wagtail-fedit-adapter-content")
+            }
+            get frameOptions() {
+                return {
+                    onResize: (e, t) => {
+                        this.iframe.element.style.height = `${t}px`
+                    }
+                }
+            }
+            openEditor() {
+                this.openIframe(this.formElement, (e => {
+                    this.contentElement.style.display = "none"
+                }))
+            }
+            closeEditor() {
+                this.opened = !1, window.history.pushState(null, this.initialTitle, window.location.href.split("#")[0]), document.title = this.initialTitle, this.contentElement.style.display = "block", this.iframe.destroy(), this.executeEvent(window.wagtailFedit.EVENTS.EDITOR_CLOSE), delete this.iframe
+            }
+        }
+        class Pt extends(kt(jt)) {}
+
+        function Ht() {
             bt(), new MutationObserver((e => {
                 for (const t of e)
                     for (let e = 0; e < t.addedNodes.length; e++) {
                         const n = t.addedNodes[e];
                         1 === n.nodeType && bt(n)
                     }
             })).observe(document.body, {
@@ -2546,63 +2646,40 @@
                 const e = i.shadowRoot.querySelector("#wagtail-fedit-editor-button"),
                     t = i.shadowRoot.querySelector("#wagtail-fedit-live-button"),
                     n = i.shadowRoot.querySelector("#wagtail-fedit-publish-menu");
                 if (e || t) {
                     let n;
                     window.addEventListener("scroll", (() => {
                         n && clearTimeout(n), n = setTimeout((() => {
-                            Et(e), Et(t);
+                            xt(e), xt(t);
                             const n = new URL(window.location.href);
                             n.searchParams.set("scrollY", `${window.scrollY}`), n.searchParams.set("scrollX", `${window.scrollX}`), window.history.replaceState(null, "", n.toString())
                         }), 50)
                     }))
                 }
-                n && new St(n)
+                n && new Dt(n)
             }
         }
         window.wagtailFedit = {
             NAMESPACE: "wagtail-fedit",
             EVENTS: {
                 SUBMIT: "wagtail-fedit:submit",
                 CHANGE: "wagtail-fedit:change",
                 EDITOR_OPEN: "wagtail-fedit:editorOpen",
                 EDITOR_LOAD: "wagtail-fedit:editorLoad",
                 EDITOR_CLOSE: "wagtail-fedit:editorClose",
                 SUBMIT_ERROR: "wagtail-fedit:submitError"
             },
             editors: {
-                "wagtail_fedit.editors.BaseFuncEditor": Dt,
-                "wagtail_fedit.editors.BlockFieldEditor": Mt,
-                "wagtail_fedit.editors.DomPositionedBlockFieldEditor": class extends Mt {
-                    get buttonsElement() {
-                        return this.wrapperElement.querySelector(".wagtail-fedit-buttons")
-                    }
-                    get formElement() {
-                        return this.wrapperElement.querySelector(".wagtail-fedit-adapter-form")
-                    }
-                    get contentElement() {
-                        return this.wrapperElement.querySelector(".wagtail-fedit-adapter-content")
-                    }
-                    get frameOptions() {
-                        return {
-                            onResize: (e, t) => {
-                                this.iframe.element.style.height = `${t}px`
-                            }
-                        }
-                    }
-                    openEditor() {
-                        this.openIframe(this.formElement, (e => {
-                            this.contentElement.style.display = "none"
-                        }))
-                    }
-                    closeEditor() {
-                        this.opened = !1, window.history.pushState(null, this.initialTitle, window.location.href.split("#")[0]), document.title = this.initialTitle, this.contentElement.style.display = "block", this.iframe.destroy(), delete this.iframe, this.executeEvent(window.wagtailFedit.EVENTS.EDITOR_CLOSE)
-                    }
-                },
-                "wagtail_fedit.editors.WagtailFeditFuncEditor": class extends Dt {
+                "wagtail_fedit.editors.BaseFuncEditor": Mt,
+                "wagtail_fedit.editors.FieldEditor": It,
+                "wagtail_fedit.editors.BlockEditor": Rt,
+                "wagtail_fedit.editors.DomPositionedFieldEditor": jt,
+                "wagtail_fedit.editors.DomPositionedBlockEditor": Pt,
+                "wagtail_fedit.editors.WagtailFeditFuncEditor": class extends Mt {
                     static get funcMap() {
                         return window.wagtailFedit.funcs
                     }
                 }
             },
             funcs: {
                 "wagtail_fedit.funcs.backgroundImageFunc": function(e, t) {
@@ -2613,10 +2690,10 @@
             },
             register: function(e, t) {
                 this.editors[e] = t
             },
             registerFunc: function(e, t) {
                 this.funcs[e] = t
             }
-        }, "loading" === document.readyState ? document.addEventListener("DOMContentLoaded", Rt) : Rt()
+        }, "loading" === document.readyState ? document.addEventListener("DOMContentLoaded", Ht) : Ht()
     })()
 })();
```

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/static/wagtail_fedit/js/licenses/TIPPY.LICENSE` & `wagtail_fedit-1.5.8/wagtail_fedit/static/wagtail_fedit/js/licenses/TIPPY.LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html` & `wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html` & `wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html` & `wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html` & `wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html` & `wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html` & `wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {% load i18n wagtailadmin_tags %}
-<form id="wagtail-fedit-form" data-edit-form action="{{ edit_url }}" method="post" {% for k, v in form_attrs.items %}{{ k }}="{{ v|safe }}" {% endfor %}>
+<form id="wagtail-fedit-form" class="w-panel" data-edit-form action="{{ edit_url }}" method="post" {% for k, v in form_attrs.items %}{{ k }}="{{ v|safe }}" {% endfor %}>
     {% csrf_token %}
     {% block form %}
         {% fragment as panel_content %}
             <div class="wagtail-fedit-form">
                 {% for field in form %}
                     {% include "./field.html" %}
                 {% endfor %}
```

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/editor/field.html` & `wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/editor/field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg` & `wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg` & `wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg` & `wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg` & `wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.5.8/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.5.8/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,42 +1,42 @@
 magic:    0xa70d0d0a
-moddate:  0x021f4766 (Fri May 17 09:10:26 2024 UTC)
-files sz: 10373
+moddate:  0xe81f4966 (Sat May 18 21:38:48 2024 UTC)
+files sz: 10414
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 11
    flags     : 0
    code
       0x9700640064016c006d015a016d025a020100640064026c036d045a046d
       055a056d065a060100640064036c076d085a080100640064046c096d0a5a
       0a6d0b5a0b6d0c5a0c0100640064056c0d6d0e5a0e0100640064066c0f6d
       105a100100640064076c116d125a120100640064086c136d145a14010064
       0064096c156d165a166d175a1701006400640a6c185a18640b640c6c196d
-      1a5a1a0100640b640d6c1b6d1c5a1c6d1d5a1d6d1e5a1e6d1f5a1f010064
-      0b640e6c206d215a216d225a226d235a236d245a246d255a256d265a266d
-      275a276d285a286d295a290100640b640f6c146d2a5a2a6d2b5a2b010002
-      0065046a2c0000000000000000a6000000ab0000000000000000005a2d64
-      105a2e64115a2f641265306413650864146530641565306608641684045a
-      31020047006417840064186505a6030000ab0300000000000000005a3265
-      2da03300000000000000000000000000000000000000006527ac19a60100
-      00ab010000000000000000641a650a641b650b6604641c8404a6000000ab
-      0000000000000000005a34652da035000000000000000000000000000000
-      0000000000641dac1ea6010000ab01000000000000000064136508641f65
-      1e64156530660664208404a6000000ab0000000000000000005a36652da0
-      37000000000000000000000000000000000000000064216422641dac23a6
-      030000ab03000000000000000064156538660264248404a6000000ab0000
-      000000000000005a39652da0350000000000000000000000000000000000
-      00000064256426ac27a6020000ab02000000000000000064316428653064
-      156530660464298405a6000000ab0000000000000000005a3a652da03500
-      00000000000000000000000000000000000000641d642aac27a6020000ab
-      020000000000000000642b6502641565306604642c8404a6000000ab0000
-      000000000000005a3b6432641a650a642d653c6530190000000000000000
-      00642e653c653019000000000000000000642f653c653019000000000000
-      00000064156538660a643084055a3d640a5300
+      1a5a1a0100640b640d6c1b6d1c5a1c6d1d5a1d0100640b640e6c1e6d1e5a
+      1f6d205a200100640b640f6c216d225a226d235a236d245a246d255a256d
+      265a266d275a276d285a286d295a296d2a5a2a0100640b64106c146d2b5a
+      2b6d2c5a2c0100020065046a2d0000000000000000a6000000ab00000000
+      00000000005a2e64115a2f64125a30641365316414650864156531641665
+      316608641784045a32020047006418840064196505a6030000ab03000000
+      00000000005a33652ea03400000000000000000000000000000000000000
+      006528ac1aa6010000ab010000000000000000641b650a641c650b660464
+      1d8404a6000000ab0000000000000000005a35652ea03600000000000000
+      00000000000000000000000000641eac1fa6010000ab0100000000000000
+      00641465086420651c64166531660664218404a6000000ab000000000000
+      0000005a37652ea038000000000000000000000000000000000000000064
+      226423641eac24a6030000ab030000000000000000641665396602642584
+      04a6000000ab0000000000000000005a3a652ea036000000000000000000
+      000000000000000000000064266427ac28a6020000ab0200000000000000
+      00643264296531641665316604642a8405a6000000ab0000000000000000
+      005a3b652ea0360000000000000000000000000000000000000000641e64
+      2bac28a6020000ab020000000000000000642c6502641665316604642d84
+      04a6000000ab0000000000000000005a3c6433641b650a642e653d653119
+      000000000000000000642f653d6531190000000000000000006430653d65
+      311900000000000000000064166539660a643184055a3e640a5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('Type', 'Any'))
                  6 IMPORT_NAME              0 (typing)
                  8 IMPORT_FROM              1 (Type)
                 10 STORE_NAME               1 (Type)
@@ -119,323 +119,329 @@
                144 LOAD_CONST              12 (('TIPPY_ENABLED',))
                146 IMPORT_NAME             25 (settings)
                148 IMPORT_FROM             26 (TIPPY_ENABLED)
                150 STORE_NAME              26 (TIPPY_ENABLED)
                152 POP_TOP
    
     27         154 LOAD_CONST              11 (2)
-               156 LOAD_CONST              13 (('adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError'))
+               156 LOAD_CONST              13 (('BaseAdapter', 'AdapterError'))
                158 IMPORT_NAME             27 (adapters)
-               160 IMPORT_FROM             28 (adapter_registry)
-               162 STORE_NAME              28 (adapter_registry)
-               164 IMPORT_FROM             29 (RegistryLookUpError)
-               166 STORE_NAME              29 (RegistryLookUpError)
-               168 IMPORT_FROM             30 (BaseAdapter)
-               170 STORE_NAME              30 (BaseAdapter)
-               172 IMPORT_FROM             31 (AdapterError)
-               174 STORE_NAME              31 (AdapterError)
-               176 POP_TOP
-   
-    33         178 LOAD_CONST              11 (2)
-               180 LOAD_CONST              14 (('wrap_adapter', 'with_userbar_model', 'base_adapter_context', '_flatten_context', '_can_edit', 'FEDIT_PREVIEW_VAR', 'TEMPLATE_TAG_NAME', 'FIELD_TEMPLATE_VAR', 'INSTANCE_TEMPLATE_VAR'))
-               182 IMPORT_NAME             32 (utils)
-               184 IMPORT_FROM             33 (wrap_adapter)
-               186 STORE_NAME              33 (wrap_adapter)
-               188 IMPORT_FROM             34 (with_userbar_model)
-               190 STORE_NAME              34 (with_userbar_model)
-               192 IMPORT_FROM             35 (base_adapter_context)
-               194 STORE_NAME              35 (base_adapter_context)
-               196 IMPORT_FROM             36 (_flatten_context)
-               198 STORE_NAME              36 (_flatten_context)
-               200 IMPORT_FROM             37 (_can_edit)
-               202 STORE_NAME              37 (_can_edit)
-               204 IMPORT_FROM             38 (FEDIT_PREVIEW_VAR)
-               206 STORE_NAME              38 (FEDIT_PREVIEW_VAR)
-               208 IMPORT_FROM             39 (TEMPLATE_TAG_NAME)
-               210 STORE_NAME              39 (TEMPLATE_TAG_NAME)
-               212 IMPORT_FROM             40 (FIELD_TEMPLATE_VAR)
-               214 STORE_NAME              40 (FIELD_TEMPLATE_VAR)
-               216 IMPORT_FROM             41 (INSTANCE_TEMPLATE_VAR)
-               218 STORE_NAME              41 (INSTANCE_TEMPLATE_VAR)
-               220 POP_TOP
-   
-    45         222 LOAD_CONST              11 (2)
-               224 LOAD_CONST              15 (('REGISTER_CSS', 'REGISTER_JS'))
-               226 IMPORT_NAME             20 (hooks)
-               228 IMPORT_FROM             42 (REGISTER_CSS)
-               230 STORE_NAME              42 (REGISTER_CSS)
-               232 IMPORT_FROM             43 (REGISTER_JS)
-               234 STORE_NAME              43 (REGISTER_JS)
-               236 POP_TOP
-   
-    51         238 PUSH_NULL
-               240 LOAD_NAME                4 (library)
-               242 LOAD_ATTR               44 (Library)
-               252 PRECALL                  0
-               256 CALL                     0
-               266 STORE_NAME              45 (register)
-   
-    54         268 LOAD_CONST              16 ('Field name is not available in the context for %(object)s.')
-               270 STORE_NAME              46 (WARNING_FIELD_NAME_NOT_AVAILABLE)
-   
-    55         272 LOAD_CONST              17 ('Model instance is not available in the context for %(object)s.')
-               274 STORE_NAME              47 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
-   
-    58         276 LOAD_CONST              18 ('var')
-               278 LOAD_NAME               48 (str)
-               280 LOAD_CONST              19 ('context')
-               282 LOAD_NAME                8 (Context)
-               284 LOAD_CONST              20 ('value')
-               286 LOAD_NAME               48 (str)
-               288 LOAD_CONST              21 ('return')
-               290 LOAD_NAME               48 (str)
-               292 BUILD_TUPLE              8
-               294 LOAD_CONST              22 (<code object as_var, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 58>)
-               296 MAKE_FUNCTION            4 (annotations)
-               298 STORE_NAME              49 (as_var)
-   
-    65         300 PUSH_NULL
-               302 LOAD_BUILD_CLASS
-               304 LOAD_CONST              23 (<code object AdapterNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 65>)
-               306 MAKE_FUNCTION            0
-               308 LOAD_CONST              24 ('AdapterNode')
-               310 LOAD_NAME                5 (Node)
-               312 PRECALL                  3
-               316 CALL                     3
-               326 STORE_NAME              50 (AdapterNode)
-   
-   174         328 LOAD_NAME               45 (register)
-               330 LOAD_METHOD             51 (tag)
-               352 LOAD_NAME               39 (TEMPLATE_TAG_NAME)
-               354 KW_NAMES                25
-               356 PRECALL                  1
-               360 CALL                     1
-   
-   175         370 LOAD_CONST              26 ('parser')
-               372 LOAD_NAME               10 (Parser)
-               374 LOAD_CONST              27 ('token')
-               376 LOAD_NAME               11 (Token)
-               378 BUILD_TUPLE              4
-               380 LOAD_CONST              28 (<code object do_render_fedit, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 174>)
-               382 MAKE_FUNCTION            4 (annotations)
-   
-   174         384 PRECALL                  0
-               388 CALL                     0
-   
-   175         398 STORE_NAME              52 (do_render_fedit)
-   
-   230         400 LOAD_NAME               45 (register)
-               402 LOAD_METHOD             53 (simple_tag)
-               424 LOAD_CONST              29 (True)
-               426 KW_NAMES                30
-               428 PRECALL                  1
-               432 CALL                     1
-   
-   231         442 LOAD_CONST              19 ('context')
-               444 LOAD_NAME                8 (Context)
-               446 LOAD_CONST              31 ('adapter')
-               448 LOAD_NAME               30 (BaseAdapter)
-               450 LOAD_CONST              21 ('return')
-               452 LOAD_NAME               48 (str)
-               454 BUILD_TUPLE              6
-               456 LOAD_CONST              32 (<code object render_adapter, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 230>)
-               458 MAKE_FUNCTION            4 (annotations)
-   
-   230         460 PRECALL                  0
-               464 CALL                     0
-   
-   231         474 STORE_NAME              54 (render_adapter)
-   
-   257         476 LOAD_NAME               45 (register)
-               478 LOAD_METHOD             55 (inclusion_tag)
-               500 LOAD_CONST              33 ('wagtail_fedit/_hook_output.html')
-               502 LOAD_CONST              34 ('fedit_scripts')
-               504 LOAD_CONST              29 (True)
-               506 KW_NAMES                35
-               508 PRECALL                  3
-               512 CALL                     3
-   
-   258         522 LOAD_CONST              21 ('return')
-               524 LOAD_NAME               56 (dict)
-               526 BUILD_TUPLE              2
-               528 LOAD_CONST              36 (<code object static_hook_output, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 257>)
-               530 MAKE_FUNCTION            4 (annotations)
-   
-   257         532 PRECALL                  0
-               536 CALL                     0
-   
-   258         546 STORE_NAME              57 (static_hook_output)
-   
-   287         548 LOAD_NAME               45 (register)
-               550 LOAD_METHOD             53 (simple_tag)
-               572 LOAD_CONST              37 (False)
-               574 LOAD_CONST              38 ('tooltip')
-               576 KW_NAMES                39
-               578 PRECALL                  2
-               582 CALL                     2
-   
-   288         592 LOAD_CONST              49 ((None,))
-               594 LOAD_CONST              40 ('wrapping')
-               596 LOAD_NAME               48 (str)
-               598 LOAD_CONST              21 ('return')
-               600 LOAD_NAME               48 (str)
-               602 BUILD_TUPLE              4
-               604 LOAD_CONST              41 (<code object tooltip, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 287>)
-               606 MAKE_FUNCTION            5 (defaults, annotations)
-   
-   287         608 PRECALL                  0
-               612 CALL                     0
-   
-   288         622 STORE_NAME              58 (tooltip)
-   
-   306         624 LOAD_NAME               45 (register)
-               626 LOAD_METHOD             53 (simple_tag)
-               648 LOAD_CONST              29 (True)
-               650 LOAD_CONST              42 ('fedit_userbar')
-               652 KW_NAMES                39
-               654 PRECALL                  2
-               658 CALL                     2
-   
-   307         668 LOAD_CONST              43 ('model')
-               670 LOAD_NAME                2 (Any)
-               672 LOAD_CONST              21 ('return')
-               674 LOAD_NAME               48 (str)
-               676 BUILD_TUPLE              4
-               678 LOAD_CONST              44 (<code object do_with_userbar_model, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 306>)
-               680 MAKE_FUNCTION            4 (annotations)
-   
-   306         682 PRECALL                  0
-               686 CALL                     0
-   
-   307         696 STORE_NAME              59 (do_with_userbar_model)
-   
-   314         698 LOAD_CONST              50 ((None, None))
-               700 LOAD_CONST              26 ('parser')
-               702 LOAD_NAME               10 (Parser)
-               704 LOAD_CONST              45 ('tokens')
-               706 LOAD_NAME               60 (list)
-               708 LOAD_NAME               48 (str)
-               710 BINARY_SUBSCR
-               720 LOAD_CONST              46 ('kwarg_list')
-               722 LOAD_NAME               60 (list)
-               724 LOAD_NAME               48 (str)
-               726 BINARY_SUBSCR
-               736 LOAD_CONST              47 ('absolute_tokens')
-               738 LOAD_NAME               60 (list)
-               740 LOAD_NAME               48 (str)
-               742 BINARY_SUBSCR
-               752 LOAD_CONST              21 ('return')
-               754 LOAD_NAME               56 (dict)
-               756 BUILD_TUPLE             10
-               758 LOAD_CONST              48 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 314>)
-               760 MAKE_FUNCTION            5 (defaults, annotations)
-               762 STORE_NAME              61 (get_kwargs)
-               764 LOAD_CONST              10 (None)
-               766 RETURN_VALUE
+               160 IMPORT_FROM             28 (BaseAdapter)
+               162 STORE_NAME              28 (BaseAdapter)
+               164 IMPORT_FROM             29 (AdapterError)
+               166 STORE_NAME              29 (AdapterError)
+               168 POP_TOP
+   
+    31         170 LOAD_CONST              11 (2)
+               172 LOAD_CONST              14 (('registry', 'RegistryLookUpError'))
+               174 IMPORT_NAME             30 (registry)
+               176 IMPORT_FROM             30 (registry)
+               178 STORE_NAME              31 (adapter_registry)
+               180 IMPORT_FROM             32 (RegistryLookUpError)
+               182 STORE_NAME              32 (RegistryLookUpError)
+               184 POP_TOP
+   
+    35         186 LOAD_CONST              11 (2)
+               188 LOAD_CONST              15 (('wrap_adapter', 'with_userbar_model', 'base_adapter_context', '_flatten_context', '_can_edit', 'FEDIT_PREVIEW_VAR', 'TEMPLATE_TAG_NAME', 'FIELD_TEMPLATE_VAR', 'INSTANCE_TEMPLATE_VAR'))
+               190 IMPORT_NAME             33 (utils)
+               192 IMPORT_FROM             34 (wrap_adapter)
+               194 STORE_NAME              34 (wrap_adapter)
+               196 IMPORT_FROM             35 (with_userbar_model)
+               198 STORE_NAME              35 (with_userbar_model)
+               200 IMPORT_FROM             36 (base_adapter_context)
+               202 STORE_NAME              36 (base_adapter_context)
+               204 IMPORT_FROM             37 (_flatten_context)
+               206 STORE_NAME              37 (_flatten_context)
+               208 IMPORT_FROM             38 (_can_edit)
+               210 STORE_NAME              38 (_can_edit)
+               212 IMPORT_FROM             39 (FEDIT_PREVIEW_VAR)
+               214 STORE_NAME              39 (FEDIT_PREVIEW_VAR)
+               216 IMPORT_FROM             40 (TEMPLATE_TAG_NAME)
+               218 STORE_NAME              40 (TEMPLATE_TAG_NAME)
+               220 IMPORT_FROM             41 (FIELD_TEMPLATE_VAR)
+               222 STORE_NAME              41 (FIELD_TEMPLATE_VAR)
+               224 IMPORT_FROM             42 (INSTANCE_TEMPLATE_VAR)
+               226 STORE_NAME              42 (INSTANCE_TEMPLATE_VAR)
+               228 POP_TOP
+   
+    47         230 LOAD_CONST              11 (2)
+               232 LOAD_CONST              16 (('REGISTER_CSS', 'REGISTER_JS'))
+               234 IMPORT_NAME             20 (hooks)
+               236 IMPORT_FROM             43 (REGISTER_CSS)
+               238 STORE_NAME              43 (REGISTER_CSS)
+               240 IMPORT_FROM             44 (REGISTER_JS)
+               242 STORE_NAME              44 (REGISTER_JS)
+               244 POP_TOP
+   
+    53         246 PUSH_NULL
+               248 LOAD_NAME                4 (library)
+               250 LOAD_ATTR               45 (Library)
+               260 PRECALL                  0
+               264 CALL                     0
+               274 STORE_NAME              46 (register)
+   
+    56         276 LOAD_CONST              17 ('Field name is not available in the context for %(object)s.')
+               278 STORE_NAME              47 (WARNING_FIELD_NAME_NOT_AVAILABLE)
+   
+    57         280 LOAD_CONST              18 ('Model instance is not available in the context for %(object)s.')
+               282 STORE_NAME              48 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
+   
+    60         284 LOAD_CONST              19 ('var')
+               286 LOAD_NAME               49 (str)
+               288 LOAD_CONST              20 ('context')
+               290 LOAD_NAME                8 (Context)
+               292 LOAD_CONST              21 ('value')
+               294 LOAD_NAME               49 (str)
+               296 LOAD_CONST              22 ('return')
+               298 LOAD_NAME               49 (str)
+               300 BUILD_TUPLE              8
+               302 LOAD_CONST              23 (<code object as_var, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 60>)
+               304 MAKE_FUNCTION            4 (annotations)
+               306 STORE_NAME              50 (as_var)
+   
+    67         308 PUSH_NULL
+               310 LOAD_BUILD_CLASS
+               312 LOAD_CONST              24 (<code object AdapterNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 67>)
+               314 MAKE_FUNCTION            0
+               316 LOAD_CONST              25 ('AdapterNode')
+               318 LOAD_NAME                5 (Node)
+               320 PRECALL                  3
+               324 CALL                     3
+               334 STORE_NAME              51 (AdapterNode)
+   
+   176         336 LOAD_NAME               46 (register)
+               338 LOAD_METHOD             52 (tag)
+               360 LOAD_NAME               40 (TEMPLATE_TAG_NAME)
+               362 KW_NAMES                26
+               364 PRECALL                  1
+               368 CALL                     1
+   
+   177         378 LOAD_CONST              27 ('parser')
+               380 LOAD_NAME               10 (Parser)
+               382 LOAD_CONST              28 ('token')
+               384 LOAD_NAME               11 (Token)
+               386 BUILD_TUPLE              4
+               388 LOAD_CONST              29 (<code object do_render_fedit, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 176>)
+               390 MAKE_FUNCTION            4 (annotations)
+   
+   176         392 PRECALL                  0
+               396 CALL                     0
+   
+   177         406 STORE_NAME              53 (do_render_fedit)
+   
+   232         408 LOAD_NAME               46 (register)
+               410 LOAD_METHOD             54 (simple_tag)
+               432 LOAD_CONST              30 (True)
+               434 KW_NAMES                31
+               436 PRECALL                  1
+               440 CALL                     1
+   
+   233         450 LOAD_CONST              20 ('context')
+               452 LOAD_NAME                8 (Context)
+               454 LOAD_CONST              32 ('adapter')
+               456 LOAD_NAME               28 (BaseAdapter)
+               458 LOAD_CONST              22 ('return')
+               460 LOAD_NAME               49 (str)
+               462 BUILD_TUPLE              6
+               464 LOAD_CONST              33 (<code object render_adapter, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 232>)
+               466 MAKE_FUNCTION            4 (annotations)
+   
+   232         468 PRECALL                  0
+               472 CALL                     0
+   
+   233         482 STORE_NAME              55 (render_adapter)
+   
+   259         484 LOAD_NAME               46 (register)
+               486 LOAD_METHOD             56 (inclusion_tag)
+               508 LOAD_CONST              34 ('wagtail_fedit/_hook_output.html')
+               510 LOAD_CONST              35 ('fedit_scripts')
+               512 LOAD_CONST              30 (True)
+               514 KW_NAMES                36
+               516 PRECALL                  3
+               520 CALL                     3
+   
+   260         530 LOAD_CONST              22 ('return')
+               532 LOAD_NAME               57 (dict)
+               534 BUILD_TUPLE              2
+               536 LOAD_CONST              37 (<code object static_hook_output, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 259>)
+               538 MAKE_FUNCTION            4 (annotations)
+   
+   259         540 PRECALL                  0
+               544 CALL                     0
+   
+   260         554 STORE_NAME              58 (static_hook_output)
+   
+   289         556 LOAD_NAME               46 (register)
+               558 LOAD_METHOD             54 (simple_tag)
+               580 LOAD_CONST              38 (False)
+               582 LOAD_CONST              39 ('tooltip')
+               584 KW_NAMES                40
+               586 PRECALL                  2
+               590 CALL                     2
+   
+   290         600 LOAD_CONST              50 ((None,))
+               602 LOAD_CONST              41 ('wrapping')
+               604 LOAD_NAME               49 (str)
+               606 LOAD_CONST              22 ('return')
+               608 LOAD_NAME               49 (str)
+               610 BUILD_TUPLE              4
+               612 LOAD_CONST              42 (<code object tooltip, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 289>)
+               614 MAKE_FUNCTION            5 (defaults, annotations)
+   
+   289         616 PRECALL                  0
+               620 CALL                     0
+   
+   290         630 STORE_NAME              59 (tooltip)
+   
+   308         632 LOAD_NAME               46 (register)
+               634 LOAD_METHOD             54 (simple_tag)
+               656 LOAD_CONST              30 (True)
+               658 LOAD_CONST              43 ('fedit_userbar')
+               660 KW_NAMES                40
+               662 PRECALL                  2
+               666 CALL                     2
+   
+   309         676 LOAD_CONST              44 ('model')
+               678 LOAD_NAME                2 (Any)
+               680 LOAD_CONST              22 ('return')
+               682 LOAD_NAME               49 (str)
+               684 BUILD_TUPLE              4
+               686 LOAD_CONST              45 (<code object do_with_userbar_model, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 308>)
+               688 MAKE_FUNCTION            4 (annotations)
+   
+   308         690 PRECALL                  0
+               694 CALL                     0
+   
+   309         704 STORE_NAME              60 (do_with_userbar_model)
+   
+   316         706 LOAD_CONST              51 ((None, None))
+               708 LOAD_CONST              27 ('parser')
+               710 LOAD_NAME               10 (Parser)
+               712 LOAD_CONST              46 ('tokens')
+               714 LOAD_NAME               61 (list)
+               716 LOAD_NAME               49 (str)
+               718 BINARY_SUBSCR
+               728 LOAD_CONST              47 ('kwarg_list')
+               730 LOAD_NAME               61 (list)
+               732 LOAD_NAME               49 (str)
+               734 BINARY_SUBSCR
+               744 LOAD_CONST              48 ('absolute_tokens')
+               746 LOAD_NAME               61 (list)
+               748 LOAD_NAME               49 (str)
+               750 BINARY_SUBSCR
+               760 LOAD_CONST              22 ('return')
+               762 LOAD_NAME               57 (dict)
+               764 BUILD_TUPLE             10
+               766 LOAD_CONST              49 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 316>)
+               768 MAKE_FUNCTION            5 (defaults, annotations)
+               770 STORE_NAME              62 (get_kwargs)
+               772 LOAD_CONST              10 (None)
+               774 RETURN_VALUE
    consts
       0
       ('Type', 'Any')
       ('library', 'Node', 'TemplateSyntaxError')
       ('Context',)
       ('Parser', 'Token', 'FilterExpression')
       ('escape',)
       ('mark_safe',)
       ('signing',)
       ('hooks',)
       ('Page', 'PAGE_TEMPLATE_VAR')
       None
       2
       ('TIPPY_ENABLED',)
-      ('adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError')
+      ('BaseAdapter', 'AdapterError')
+      ('registry', 'RegistryLookUpError')
       ('wrap_adapter', 'with_userbar_model', 'base_adapter_context', '_flatten_context', '_can_edit', 'FEDIT_PREVIEW_VAR', 'TEMPLATE_TAG_NAME', 'FIELD_TEMPLATE_VAR', 'INSTANCE_TEMPLATE_VAR')
       ('REGISTER_CSS', 'REGISTER_JS')
       'Field name is not available in the context for %(object)s.'
       'Model instance is not available in the context for %(object)s.'
       'var'
       'context'
       'value'
       'return'
       code
          argcount  : 3
          nlocals   : 3
          stacksize : 3
          flags     : 3
          code 0x97007c0073027c0253007c027c017c003c00000064015300
-          58           0 RESUME                   0
+          60           0 RESUME                   0
          
-          59           2 LOAD_FAST                0 (var)
+          61           2 LOAD_FAST                0 (var)
                        4 POP_JUMP_FORWARD_IF_TRUE     2 (to 10)
          
-          60           6 LOAD_FAST                2 (value)
+          62           6 LOAD_FAST                2 (value)
                        8 RETURN_VALUE
          
-          62     >>   10 LOAD_FAST                2 (value)
+          64     >>   10 LOAD_FAST                2 (value)
                       12 LOAD_FAST                1 (context)
                       14 LOAD_FAST                0 (var)
                       16 STORE_SUBSCR
          
-          63          20 LOAD_CONST               1 ('')
+          65          20 LOAD_CONST               1 ('')
                       22 RETURN_VALUE
          consts
             None
             ''
          names      ()
          varnames   ('var', 'context', 'value')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'as_var'
-         firstlineno 58
+         firstlineno 60
          lnotab 0x0201040104020a01
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 9
          flags     : 0
          code
             0x970065005a0164005a02020065036a040000000000000000a6000000ab
             0000000000000000005a0564096402650665071900000000000000000064
             03650864046509650a190000000000000000006405650a6608640684055a
             0b640784005a0c640884005a0d64015300
-          65           0 RESUME                   0
+          67           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdapterNode')
                        8 STORE_NAME               2 (__qualname__)
          
-          66          10 PUSH_NULL
+          68          10 PUSH_NULL
                       12 LOAD_NAME                3 (signing)
                       14 LOAD_ATTR                4 (TimestampSigner)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_NAME               5 (signer)
          
-          68          40 LOAD_CONST               9 ((None,))
+          70          40 LOAD_CONST               9 ((None,))
                       42 LOAD_CONST               2 ('adapter')
                       44 LOAD_NAME                6 (Type)
                       46 LOAD_NAME                7 (BaseAdapter)
                       48 BINARY_SUBSCR
                       58 LOAD_CONST               3 ('model')
                       60 LOAD_NAME                8 (FilterExpression)
                       62 LOAD_CONST               4 ('getters')
                       64 LOAD_NAME                9 (list)
                       66 LOAD_NAME               10 (str)
                       68 BINARY_SUBSCR
                       78 LOAD_CONST               5 ('as_var')
                       80 LOAD_NAME               10 (str)
                       82 BUILD_TUPLE              8
-                      84 LOAD_CONST               6 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 68>)
+                      84 LOAD_CONST               6 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 70>)
                       86 MAKE_FUNCTION            5 (defaults, annotations)
                       88 STORE_NAME              11 (__init__)
          
-          75          90 LOAD_CONST               7 (<code object _resolve_expressions, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 75>)
+          77          90 LOAD_CONST               7 (<code object _resolve_expressions, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 77>)
                       92 MAKE_FUNCTION            0
                       94 STORE_NAME              12 (_resolve_expressions)
          
-          85          96 LOAD_CONST               8 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 85>)
+          87          96 LOAD_CONST               8 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 87>)
                       98 MAKE_FUNCTION            0
                      100 STORE_NAME              13 (render)
                      102 LOAD_CONST               1 (None)
                      104 RETURN_VALUE
          consts
             'AdapterNode'
             None
@@ -448,46 +454,46 @@
                nlocals   : 6
                stacksize : 2
                flags     : 11
                code
                   0x97007c017c005f0000000000000000007c027c005f0100000000000000
                   007c037c005f0200000000000000007c057c005f0300000000000000007c
                   047c005f04000000000000000064005300
-                68           0 RESUME                   0
+                70           0 RESUME                   0
                
-                69           2 LOAD_FAST                1 (adapter)
+                71           2 LOAD_FAST                1 (adapter)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (adapter)
                
-                70          16 LOAD_FAST                2 (model)
+                72          16 LOAD_FAST                2 (model)
                             18 LOAD_FAST                0 (self)
                             20 STORE_ATTR               1 (model)
                
-                71          30 LOAD_FAST                3 (getters)
+                73          30 LOAD_FAST                3 (getters)
                             32 LOAD_FAST                0 (self)
                             34 STORE_ATTR               2 (getters)
                
-                72          44 LOAD_FAST                5 (kwargs)
+                74          44 LOAD_FAST                5 (kwargs)
                             46 LOAD_FAST                0 (self)
                             48 STORE_ATTR               3 (kwargs)
                
-                73          58 LOAD_FAST                4 (as_var)
+                75          58 LOAD_FAST                4 (as_var)
                             60 LOAD_FAST                0 (self)
                             62 STORE_ATTR               4 (as_var)
                             72 LOAD_CONST               0 (None)
                             74 RETURN_VALUE
                consts
                   None
                names      ('adapter', 'model', 'getters', 'kwargs', 'as_var')
                varnames   ('self', 'adapter', 'model', 'getters', 'as_var', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       '__init__'
-               firstlineno 68
+               firstlineno 70
                lnotab 0x02010e010e010e010e01
             code
                argcount  : 3
                nlocals   : 6
                stacksize : 5
                flags     : 11
                code
@@ -495,70 +501,70 @@
                   00ab00000000000000000044005d325c0200007d047d0574030000000000
                   00000000007c05740400000000000000000000a6020000ab020000000000
                   00000072187c05a00300000000000000000000000000000000000000007c
                   01a6010000ab0100000000000000007c037c043c0000008c337403000000
                   000000000000007c02740400000000000000000000a6020000ab02000000
                   000000000072157c02a00300000000000000000000000000000000000000
                   007c01a6010000ab0100000000000000007d027c027c0366025300
-                75           0 RESUME                   0
+                77           0 RESUME                   0
                
-                76           2 LOAD_FAST                3 (kwargs)
+                78           2 LOAD_FAST                3 (kwargs)
                              4 LOAD_METHOD              0 (items)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 GET_ITER
                        >>   42 FOR_ITER                50 (to 144)
                             44 UNPACK_SEQUENCE          2
                             48 STORE_FAST               4 (k)
                             50 STORE_FAST               5 (v)
                
-                77          52 LOAD_GLOBAL              3 (NULL + isinstance)
+                79          52 LOAD_GLOBAL              3 (NULL + isinstance)
                             64 LOAD_FAST                5 (v)
                             66 LOAD_GLOBAL              4 (FilterExpression)
                             78 PRECALL                  2
                             82 CALL                     2
                             92 POP_JUMP_FORWARD_IF_FALSE    24 (to 142)
                
-                78          94 LOAD_FAST                5 (v)
+                80          94 LOAD_FAST                5 (v)
                             96 LOAD_METHOD              3 (resolve)
                            118 LOAD_FAST                1 (context)
                            120 PRECALL                  1
                            124 CALL                     1
                            134 LOAD_FAST                3 (kwargs)
                            136 LOAD_FAST                4 (k)
                            138 STORE_SUBSCR
                        >>  142 JUMP_BACKWARD           51 (to 42)
                
-                80     >>  144 LOAD_GLOBAL              3 (NULL + isinstance)
+                82     >>  144 LOAD_GLOBAL              3 (NULL + isinstance)
                            156 LOAD_FAST                2 (model)
                            158 LOAD_GLOBAL              4 (FilterExpression)
                            170 PRECALL                  2
                            174 CALL                     2
                            184 POP_JUMP_FORWARD_IF_FALSE    21 (to 228)
                
-                81         186 LOAD_FAST                2 (model)
+                83         186 LOAD_FAST                2 (model)
                            188 LOAD_METHOD              3 (resolve)
                            210 LOAD_FAST                1 (context)
                            212 PRECALL                  1
                            216 CALL                     1
                            226 STORE_FAST               2 (model)
                
-                83     >>  228 LOAD_FAST                2 (model)
+                85     >>  228 LOAD_FAST                2 (model)
                            230 LOAD_FAST                3 (kwargs)
                            232 BUILD_TUPLE              2
                            234 RETURN_VALUE
                consts
                   None
                names      ('items', 'isinstance', 'FilterExpression', 'resolve')
                varnames   ('self', 'context', 'model', 'kwargs', 'k', 'v')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       '_resolve_expressions'
-               firstlineno 75
+               firstlineno 77
                lnotab 0x020132012a0132022a012a02
             code
                argcount  : 2
                nlocals   : 13
                stacksize : 9
                flags     : 3
                code
@@ -598,342 +604,342 @@
                   000000ab00000000000000000072247437000000000000000000007c0a7c
                   06a6020000ab02000000000000000072147439000000000000000000007c
                   0a7c0b7c016407ac08a6040000ab0400000000000000007d0c6e24743b00
                   0000000000000000007c01a6010000ab01000000000000000001007c0ba0
                   1e00000000000000000000000000000000000000007c01a6010000ab0100
                   000000000000007d0c741d000000000000000000007c006a0e0000000000
                   0000007c017c0ca6030000ab0300000000000000005300
-                85           0 RESUME                   0
+                87           0 RESUME                   0
                
-                86           2 LOAD_FAST                0 (self)
+                88           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (model)
                             14 STORE_FAST               2 (model)
                
-                87          16 LOAD_FAST                0 (self)
+                89          16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (getters)
                             28 STORE_FAST               3 (getters)
                
-                89          30 PUSH_NULL
+                91          30 PUSH_NULL
                             32 LOAD_FAST                0 (self)
                             34 LOAD_ATTR                2 (_resolve_expressions)
                
-                90          44 LOAD_FAST                1 (context)
+                92          44 LOAD_FAST                1 (context)
                             46 LOAD_FAST                2 (model)
                
-                89          48 BUILD_TUPLE              2
+                91          48 BUILD_TUPLE              2
                             50 BUILD_MAP                0
                
-                90          52 LOAD_FAST                0 (self)
+                92          52 LOAD_FAST                0 (self)
                             54 LOAD_ATTR                3 (kwargs)
                
-                89          64 DICT_MERGE               1
+                91          64 DICT_MERGE               1
                             66 CALL_FUNCTION_EX         1
                             68 UNPACK_SEQUENCE          2
                             72 STORE_FAST               2 (model)
                             74 STORE_FAST               4 (kwargs)
                
-                93          76 LOAD_GLOBAL              8 (FIELD_TEMPLATE_VAR)
+                95          76 LOAD_GLOBAL              8 (FIELD_TEMPLATE_VAR)
                             88 LOAD_FAST                1 (context)
                             90 CONTAINS_OP              0
                             92 POP_JUMP_FORWARD_IF_FALSE    51 (to 196)
                
-                94          94 LOAD_GLOBAL             10 (INSTANCE_TEMPLATE_VAR)
+                96          94 LOAD_GLOBAL             10 (INSTANCE_TEMPLATE_VAR)
                            106 LOAD_FAST                1 (context)
                            108 CONTAINS_OP              0
                            110 POP_JUMP_FORWARD_IF_FALSE    42 (to 196)
                
-                95         112 LOAD_FAST                2 (model)
+                97         112 LOAD_FAST                2 (model)
                
-                94         114 POP_JUMP_FORWARD_IF_TRUE    40 (to 196)
+                96         114 POP_JUMP_FORWARD_IF_TRUE    40 (to 196)
                
-                95         116 LOAD_FAST                0 (self)
+                97         116 LOAD_FAST                0 (self)
                            118 LOAD_ATTR                6 (adapter)
                            128 LOAD_ATTR                7 (field_required)
                
-                94         138 POP_JUMP_FORWARD_IF_FALSE    28 (to 196)
+                96         138 POP_JUMP_FORWARD_IF_FALSE    28 (to 196)
                
-                97         140 LOAD_FAST                1 (context)
+                99         140 LOAD_FAST                1 (context)
                            142 LOAD_GLOBAL              8 (FIELD_TEMPLATE_VAR)
                            154 BINARY_SUBSCR
                            164 STORE_FAST               5 (field_name)
                
-                98         166 LOAD_FAST                1 (context)
+               100         166 LOAD_FAST                1 (context)
                            168 LOAD_GLOBAL             10 (INSTANCE_TEMPLATE_VAR)
                            180 BINARY_SUBSCR
                            190 STORE_FAST               6 (obj)
                            192 EXTENDED_ARG             1
                            194 JUMP_FORWARD           328 (to 852)
                
-               100     >>  196 LOAD_FAST                2 (model)
+               102     >>  196 LOAD_FAST                2 (model)
                            198 POP_JUMP_FORWARD_IF_TRUE    38 (to 276)
                
-               101         200 LOAD_GLOBAL             10 (INSTANCE_TEMPLATE_VAR)
+               103         200 LOAD_GLOBAL             10 (INSTANCE_TEMPLATE_VAR)
                            212 LOAD_FAST                1 (context)
                            214 CONTAINS_OP              0
                            216 POP_JUMP_FORWARD_IF_FALSE    29 (to 276)
                
-               102         218 LOAD_FAST                0 (self)
+               104         218 LOAD_FAST                0 (self)
                            220 LOAD_ATTR                6 (adapter)
                            230 LOAD_ATTR                7 (field_required)
                
-               101         240 POP_JUMP_FORWARD_IF_TRUE    17 (to 276)
+               103         240 POP_JUMP_FORWARD_IF_TRUE    17 (to 276)
                
-               103         242 LOAD_FAST                1 (context)
+               105         242 LOAD_FAST                1 (context)
                            244 LOAD_GLOBAL             10 (INSTANCE_TEMPLATE_VAR)
                            256 BINARY_SUBSCR
                            266 STORE_FAST               6 (obj)
                
-               104         268 LOAD_CONST               0 (None)
+               106         268 LOAD_CONST               0 (None)
                            270 STORE_FAST               5 (field_name)
                            272 EXTENDED_ARG             1
                            274 JUMP_FORWARD           288 (to 852)
                
-               108     >>  276 LOAD_FAST                2 (model)
+               110     >>  276 LOAD_FAST                2 (model)
                            278 POP_JUMP_FORWARD_IF_TRUE   152 (to 584)
                
-               109         280 LOAD_GLOBAL             17 (NULL + warnings)
+               111         280 LOAD_GLOBAL             17 (NULL + warnings)
                            292 LOAD_ATTR                9 (warn)
                
-               110         302 LOAD_GLOBAL             20 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
+               112         302 LOAD_GLOBAL             20 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
                
-               111         314 LOAD_CONST               1 ('object')
+               113         314 LOAD_CONST               1 ('object')
                            316 LOAD_FAST                0 (self)
                            318 LOAD_ATTR                6 (adapter)
                            328 LOAD_ATTR               11 (__name__)
                
-               110         338 BUILD_MAP                1
+               112         338 BUILD_MAP                1
                            340 BINARY_OP                6 (%)
                
-               113         344 LOAD_GLOBAL             24 (RuntimeWarning)
+               115         344 LOAD_GLOBAL             24 (RuntimeWarning)
                
-               109         356 PRECALL                  2
+               111         356 PRECALL                  2
                            360 CALL                     2
                            370 POP_TOP
                
-               116         372 LOAD_FAST                1 (context)
+               118         372 LOAD_FAST                1 (context)
                            374 LOAD_METHOD             13 (flatten)
                            396 PRECALL                  0
                            400 CALL                     0
                            410 STORE_FAST               1 (context)
                
-               118         412 NOP
+               120         412 NOP
                
-               119         414 LOAD_GLOBAL             29 (NULL + as_var)
+               121         414 LOAD_GLOBAL             29 (NULL + as_var)
                            426 LOAD_FAST                0 (self)
                            428 LOAD_ATTR               14 (as_var)
                            438 LOAD_FAST                1 (context)
                            440 PUSH_NULL
                            442 LOAD_FAST                0 (self)
                            444 LOAD_ATTR                6 (adapter)
                            454 LOAD_ATTR               15 (render_from_kwargs)
                
-               120         464 LOAD_FAST                1 (context)
+               122         464 LOAD_FAST                1 (context)
                
-               119         466 BUILD_TUPLE              1
+               121         466 BUILD_TUPLE              1
                            468 BUILD_MAP                0
                
-               120         470 LOAD_FAST                4 (kwargs)
+               122         470 LOAD_FAST                4 (kwargs)
                
-               119         472 DICT_MERGE               1
+               121         472 DICT_MERGE               1
                            474 CALL_FUNCTION_EX         1
                            476 PRECALL                  3
                            480 CALL                     3
                            490 RETURN_VALUE
                        >>  492 PUSH_EXC_INFO
                
-               122         494 LOAD_GLOBAL             32 (AdapterError)
+               124         494 LOAD_GLOBAL             32 (AdapterError)
                            506 CHECK_EXC_MATCH
                            508 POP_JUMP_FORWARD_IF_FALSE    33 (to 576)
                            510 STORE_FAST               7 (e)
                
-               123         512 LOAD_GLOBAL             35 (NULL + TemplateSyntaxError)
+               125         512 LOAD_GLOBAL             35 (NULL + TemplateSyntaxError)
                            524 LOAD_GLOBAL             37 (NULL + str)
                            536 LOAD_FAST                7 (e)
                            538 PRECALL                  1
                            542 CALL                     1
                            552 PRECALL                  1
                            556 CALL                     1
                            566 RAISE_VARARGS            1
                        >>  568 LOAD_CONST               0 (None)
                            570 STORE_FAST               7 (e)
                            572 DELETE_FAST              7 (e)
                            574 RERAISE                  1
                
-               122     >>  576 RERAISE                  0
+               124     >>  576 RERAISE                  0
                        >>  578 COPY                     3
                            580 POP_EXCEPT
                            582 RERAISE                  1
                
-               125     >>  584 LOAD_CONST               0 (None)
+               127     >>  584 LOAD_CONST               0 (None)
                            586 STORE_FAST               5 (field_name)
                
-               126         588 LOAD_FAST                2 (model)
+               128         588 LOAD_FAST                2 (model)
                            590 STORE_FAST               6 (obj)
                
-               127         592 LOAD_FAST                3 (getters)
+               129         592 LOAD_FAST                3 (getters)
                            594 POP_JUMP_FORWARD_IF_FALSE   128 (to 852)
                
-               128         596 LOAD_FAST                3 (getters)
+               130         596 LOAD_FAST                3 (getters)
                            598 LOAD_GLOBAL             39 (NULL + len)
                            610 LOAD_FAST                3 (getters)
                            612 PRECALL                  1
                            616 CALL                     1
                            626 LOAD_CONST               2 (1)
                            628 BINARY_OP               10 (-)
                            632 BINARY_SUBSCR
                            642 STORE_FAST               5 (field_name)
                
-               130         644 LOAD_GLOBAL             41 (NULL + range)
+               132         644 LOAD_GLOBAL             41 (NULL + range)
                            656 LOAD_GLOBAL             39 (NULL + len)
                            668 LOAD_FAST                3 (getters)
                            670 PRECALL                  1
                            674 CALL                     1
                            684 LOAD_CONST               2 (1)
                            686 BINARY_OP               10 (-)
                            690 PRECALL                  1
                            694 CALL                     1
                            704 GET_ITER
                        >>  706 FOR_ITER                72 (to 852)
                            708 STORE_FAST               8 (i)
                
-               131         710 LOAD_FAST                3 (getters)
+               133         710 LOAD_FAST                3 (getters)
                            712 LOAD_FAST                8 (i)
                            714 BINARY_SUBSCR
                            724 STORE_FAST               9 (getter)
                
-               132         726 NOP
+               134         726 NOP
                
-               133         728 LOAD_GLOBAL             43 (NULL + getattr)
+               135         728 LOAD_GLOBAL             43 (NULL + getattr)
                            740 LOAD_FAST                6 (obj)
                            742 LOAD_FAST                9 (getter)
                            744 PRECALL                  2
                            748 CALL                     2
                            758 STORE_FAST               6 (obj)
                            760 JUMP_BACKWARD           28 (to 706)
                        >>  762 PUSH_EXC_INFO
                
-               134         764 LOAD_GLOBAL             44 (AttributeError)
+               136         764 LOAD_GLOBAL             44 (AttributeError)
                            776 CHECK_EXC_MATCH
                            778 POP_JUMP_FORWARD_IF_FALSE    32 (to 844)
                            780 POP_TOP
                
-               135         782 LOAD_GLOBAL             35 (NULL + TemplateSyntaxError)
+               137         782 LOAD_GLOBAL             35 (NULL + TemplateSyntaxError)
                            794 LOAD_CONST               3 ('Object ')
                            796 LOAD_FAST                2 (model)
                            798 LOAD_ATTR               23 (__class__)
                            808 LOAD_ATTR               11 (__name__)
                            818 FORMAT_VALUE             0
                            820 LOAD_CONST               4 (' does not have attribute ')
                            822 LOAD_FAST                9 (getter)
                            824 FORMAT_VALUE             0
                            826 BUILD_STRING             4
                            828 PRECALL                  1
                            832 CALL                     1
                            842 RAISE_VARARGS            1
                
-               134     >>  844 RERAISE                  0
+               136     >>  844 RERAISE                  0
                        >>  846 COPY                     3
                            848 POP_EXCEPT
                            850 RERAISE                  1
                
-               138     >>  852 LOAD_FAST                1 (context)
+               140     >>  852 LOAD_FAST                1 (context)
                            854 LOAD_METHOD             24 (get)
                            876 LOAD_CONST               5 ('request')
                            878 PRECALL                  1
                            882 CALL                     1
                            892 STORE_FAST              10 (request)
                
-               139         894 PUSH_NULL
+               141         894 PUSH_NULL
                            896 LOAD_FAST                0 (self)
                            898 LOAD_ATTR                6 (adapter)
                            908 LOAD_CONST               9 (())
                
-               140         910 LOAD_FAST                6 (obj)
+               142         910 LOAD_FAST                6 (obj)
                
-               141         912 LOAD_FAST                5 (field_name)
+               143         912 LOAD_FAST                5 (field_name)
                
-               142         914 LOAD_FAST               10 (request)
+               144         914 LOAD_FAST               10 (request)
                
-               139         916 LOAD_CONST               6 (('object', 'field_name', 'request'))
+               141         916 LOAD_CONST               6 (('object', 'field_name', 'request'))
                            918 BUILD_CONST_KEY_MAP      3
                
-               143         920 LOAD_FAST                4 (kwargs)
+               145         920 LOAD_FAST                4 (kwargs)
                
-               139         922 DICT_MERGE               1
+               141         922 DICT_MERGE               1
                            924 CALL_FUNCTION_EX         1
                            926 STORE_FAST              11 (adapter)
                
-               146         928 LOAD_GLOBAL             51 (NULL + base_adapter_context)
+               148         928 LOAD_GLOBAL             51 (NULL + base_adapter_context)
                
-               147         940 LOAD_FAST               11 (adapter)
+               149         940 LOAD_FAST               11 (adapter)
                
-               148         942 LOAD_FAST                1 (context)
+               150         942 LOAD_FAST                1 (context)
                
-               146         944 PRECALL                  2
+               148         944 PRECALL                  2
                            948 CALL                     2
                            958 STORE_FAST               1 (context)
                
-               151         960 LOAD_CONST               0 (None)
+               153         960 LOAD_CONST               0 (None)
                            962 STORE_FAST              12 (content)
                
-               152         964 LOAD_FAST               11 (adapter)
+               154         964 LOAD_FAST               11 (adapter)
                            966 LOAD_METHOD             26 (check_permissions)
                            988 PRECALL                  0
                            992 CALL                     0
                           1002 POP_JUMP_FORWARD_IF_FALSE    36 (to 1076)
                
-               153        1004 LOAD_GLOBAL             55 (NULL + _can_edit)
+               155        1004 LOAD_GLOBAL             55 (NULL + _can_edit)
                           1016 LOAD_FAST               10 (request)
                           1018 LOAD_FAST                6 (obj)
                           1020 PRECALL                  2
                           1024 CALL                     2
                
-               152        1034 POP_JUMP_FORWARD_IF_FALSE    20 (to 1076)
+               154        1034 POP_JUMP_FORWARD_IF_FALSE    20 (to 1076)
                
-               154        1036 LOAD_GLOBAL             57 (NULL + wrap_adapter)
+               156        1036 LOAD_GLOBAL             57 (NULL + wrap_adapter)
                
-               155        1048 LOAD_FAST               10 (request)
+               157        1048 LOAD_FAST               10 (request)
                
-               156        1050 LOAD_FAST               11 (adapter)
+               158        1050 LOAD_FAST               11 (adapter)
                
-               157        1052 LOAD_FAST                1 (context)
+               159        1052 LOAD_FAST                1 (context)
                
-               158        1054 LOAD_CONST               7 (False)
+               160        1054 LOAD_CONST               7 (False)
                
-               154        1056 KW_NAMES                 8
+               156        1056 KW_NAMES                 8
                           1058 PRECALL                  4
                           1062 CALL                     4
                           1072 STORE_FAST              12 (content)
                           1074 JUMP_FORWARD            36 (to 1148)
                
-               162     >> 1076 LOAD_GLOBAL             59 (NULL + _flatten_context)
+               164     >> 1076 LOAD_GLOBAL             59 (NULL + _flatten_context)
                           1088 LOAD_FAST                1 (context)
                           1090 PRECALL                  1
                           1094 CALL                     1
                           1104 POP_TOP
                
-               163        1106 LOAD_FAST               11 (adapter)
+               165        1106 LOAD_FAST               11 (adapter)
                           1108 LOAD_METHOD             30 (render_content)
                
-               164        1130 LOAD_FAST                1 (context)
+               166        1130 LOAD_FAST                1 (context)
                
-               163        1132 PRECALL                  1
+               165        1132 PRECALL                  1
                           1136 CALL                     1
                           1146 STORE_FAST              12 (content)
                
-               167     >> 1148 LOAD_GLOBAL             29 (NULL + as_var)
+               169     >> 1148 LOAD_GLOBAL             29 (NULL + as_var)
                
-               168        1160 LOAD_FAST                0 (self)
+               170        1160 LOAD_FAST                0 (self)
                           1162 LOAD_ATTR               14 (as_var)
                
-               169        1172 LOAD_FAST                1 (context)
+               171        1172 LOAD_FAST                1 (context)
                
-               170        1174 LOAD_FAST               12 (content)
+               172        1174 LOAD_FAST               12 (content)
                
-               167        1176 PRECALL                  3
+               169        1176 PRECALL                  3
                           1180 CALL                     3
                           1190 RETURN_VALUE
                ExceptionTable:
                  414 to 488 -> 492 [0]
                  492 to 510 -> 578 [1] lasti
                  512 to 566 -> 568 [1] lasti
                  568 to 576 -> 578 [1] lasti
@@ -952,30 +958,30 @@
                   ()
                names      ('model', 'getters', '_resolve_expressions', 'kwargs', 'FIELD_TEMPLATE_VAR', 'INSTANCE_TEMPLATE_VAR', 'adapter', 'field_required', 'warnings', 'warn', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', '__name__', 'RuntimeWarning', 'flatten', 'as_var', 'render_from_kwargs', 'AdapterError', 'TemplateSyntaxError', 'str', 'len', 'range', 'getattr', 'AttributeError', '__class__', 'get', 'base_adapter_context', 'check_permissions', '_can_edit', 'wrap_adapter', '_flatten_context', 'render_content')
                varnames   ('self', 'context', 'model', 'getters', 'kwargs', 'field_name', 'obj', 'e', 'i', 'getter', 'request', 'adapter', 'content')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       'render'
-               firstlineno 85
+               firstlineno 87
                lnotab
                   0x02010e010e020e0104ff04010cff0c041201120102ff020116ff02031a
                   011e020401120116ff02021a010804040116010c0118ff06030cfc100728
                   020201320102ff040102ff1603120140ff08030401040104013002420110
                   010201240112013eff08042a0110010201020102fd040402fc06070c0102
                   0102fe1005040128011eff02020c0102010201020102fc14081e01180102
                   ff10040c010c01020102fd
             (None,)
          names      ('__name__', '__module__', '__qualname__', 'signing', 'TimestampSigner', 'signer', 'Type', 'BaseAdapter', 'FilterExpression', 'list', 'str', '__init__', '_resolve_expressions', 'render')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'AdapterNode'
-         firstlineno 65
+         firstlineno 67
          lnotab 0x0a011e023207060a
       'AdapterNode'
       ('name',)
       'parser'
       'token'
       code
          argcount  : 2
@@ -1009,216 +1015,216 @@
             01000000000000000064097a0a0000a6010000ab0100000000000000007d
             097c02a0010000000000000000000000000000000000000000740d000000
             000000000000007c02a6010000ab01000000000000000064097a0a0000a6
             010000ab01000000000000000001007413000000000000000000007c007c
             027c056a0a00000000000000007c056a0b0000000000000000a6040000ab
             0400000000000000007d0a741900000000000000000000640c7c057c067c
             077c09640b9c047c0aa4018e015300
-         174           0 RESUME                   0
+         176           0 RESUME                   0
          
-         177           2 LOAD_FAST                1 (token)
+         179           2 LOAD_FAST                1 (token)
                        4 LOAD_METHOD              0 (split_contents)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               2 (tokens)
          
-         179          42 LOAD_FAST                2 (tokens)
+         181          42 LOAD_FAST                2 (tokens)
                       44 LOAD_METHOD              1 (pop)
                       66 LOAD_CONST               1 (0)
                       68 PRECALL                  1
                       72 CALL                     1
                       82 STORE_FAST               3 (_)
          
-         180          84 LOAD_FAST                2 (tokens)
+         182          84 LOAD_FAST                2 (tokens)
                       86 LOAD_METHOD              1 (pop)
                      108 LOAD_CONST               1 (0)
                      110 PRECALL                  1
                      114 CALL                     1
                      124 STORE_FAST               4 (adapter_id)
          
-         182         126 NOP
+         184         126 NOP
          
-         183         128 LOAD_GLOBAL              4 (adapter_registry)
+         185         128 LOAD_GLOBAL              4 (adapter_registry)
                      140 LOAD_FAST                4 (adapter_id)
                      142 BINARY_SUBSCR
                      152 STORE_FAST               5 (adapter)
                      154 JUMP_FORWARD            33 (to 222)
                  >>  156 PUSH_EXC_INFO
          
-         184         158 LOAD_GLOBAL              6 (RegistryLookUpError)
+         186         158 LOAD_GLOBAL              6 (RegistryLookUpError)
                      170 CHECK_EXC_MATCH
                      172 POP_JUMP_FORWARD_IF_FALSE    20 (to 214)
                      174 POP_TOP
          
-         185         176 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
+         187         176 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
                      188 LOAD_CONST               2 ("No adapter found with identifier '")
                      190 LOAD_FAST                4 (adapter_id)
                      192 FORMAT_VALUE             0
                      194 LOAD_CONST               3 ("'")
                      196 BUILD_STRING             3
                      198 PRECALL                  1
                      202 CALL                     1
                      212 RAISE_VARARGS            1
          
-         184     >>  214 RERAISE                  0
+         186     >>  214 RERAISE                  0
                  >>  216 COPY                     3
                      218 POP_EXCEPT
                      220 RERAISE                  1
          
-         187     >>  222 LOAD_CONST               4 ((None, None))
+         189     >>  222 LOAD_CONST               4 ((None, None))
                      224 UNPACK_SEQUENCE          2
                      228 STORE_FAST               6 (model)
                      230 STORE_FAST               7 (model_tokens)
          
-         188         232 LOAD_FAST                2 (tokens)
+         190         232 LOAD_FAST                2 (tokens)
                      234 POP_JUMP_FORWARD_IF_FALSE   173 (to 582)
          
-         189         236 LOAD_FAST                2 (tokens)
+         191         236 LOAD_FAST                2 (tokens)
                      238 LOAD_METHOD              1 (pop)
                      260 LOAD_CONST               1 (0)
                      262 PRECALL                  1
                      266 CALL                     1
                      276 STORE_FAST               8 (model__field)
          
-         190         278 LOAD_FAST                8 (model__field)
+         192         278 LOAD_FAST                8 (model__field)
                      280 LOAD_METHOD              5 (split)
                      302 LOAD_CONST               5 ('.')
                      304 PRECALL                  1
                      308 CALL                     1
                      318 STORE_FAST               7 (model_tokens)
          
-         194         320 LOAD_GLOBAL             13 (NULL + len)
+         196         320 LOAD_GLOBAL             13 (NULL + len)
                      332 LOAD_FAST                7 (model_tokens)
                      334 PRECALL                  1
                      338 CALL                     1
                      348 LOAD_CONST               6 (2)
                      350 COMPARE_OP               0 (<)
                      356 POP_JUMP_FORWARD_IF_FALSE    34 (to 426)
          
-         195         358 LOAD_FAST                7 (model_tokens)
+         197         358 LOAD_FAST                7 (model_tokens)
                      360 LOAD_CONST               1 (0)
                      362 BINARY_SUBSCR
                      372 LOAD_CONST               7 ('from_context')
                      374 COMPARE_OP               3 (!=)
                      380 POP_JUMP_FORWARD_IF_FALSE    22 (to 426)
                      382 LOAD_FAST                5 (adapter)
                      384 LOAD_ATTR                7 (field_required)
                      394 POP_JUMP_FORWARD_IF_FALSE    15 (to 426)
          
-         196         396 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
+         198         396 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
          
-         197         408 LOAD_CONST               8 ("Model and field name are required: 'mymodel.myfield' or 'from_context'")
+         199         408 LOAD_CONST               8 ("Model and field name are required: 'mymodel.myfield' or 'from_context'")
          
-         196         410 PRECALL                  1
+         198         410 PRECALL                  1
                      414 CALL                     1
                      424 RAISE_VARARGS            1
          
-         201     >>  426 LOAD_GLOBAL             13 (NULL + len)
+         203     >>  426 LOAD_GLOBAL             13 (NULL + len)
                      438 LOAD_FAST                7 (model_tokens)
                      440 PRECALL                  1
                      444 CALL                     1
                      454 LOAD_CONST               9 (1)
                      456 COMPARE_OP               4 (>)
                      462 POP_JUMP_FORWARD_IF_TRUE    19 (to 502)
          
-         202         464 LOAD_FAST                7 (model_tokens)
+         204         464 LOAD_FAST                7 (model_tokens)
                      466 LOAD_CONST               1 (0)
                      468 BINARY_SUBSCR
                      478 LOAD_CONST               7 ('from_context')
                      480 COMPARE_OP               3 (!=)
                      486 POP_JUMP_FORWARD_IF_FALSE    47 (to 582)
                      488 LOAD_FAST                5 (adapter)
                      490 LOAD_ATTR                7 (field_required)
                      500 POP_JUMP_FORWARD_IF_TRUE    40 (to 582)
          
-         207     >>  502 LOAD_FAST                0 (parser)
+         209     >>  502 LOAD_FAST                0 (parser)
                      504 LOAD_METHOD              8 (compile_filter)
                      526 LOAD_FAST                7 (model_tokens)
                      528 LOAD_METHOD              1 (pop)
                      550 LOAD_CONST               1 (0)
                      552 PRECALL                  1
                      556 CALL                     1
                      566 PRECALL                  1
                      570 CALL                     1
                      580 STORE_FAST               6 (model)
          
-         209     >>  582 LOAD_CONST               0 (None)
+         211     >>  582 LOAD_CONST               0 (None)
                      584 STORE_FAST               9 (as_var)
          
-         210         586 LOAD_FAST                2 (tokens)
+         212         586 LOAD_FAST                2 (tokens)
                      588 POP_JUMP_FORWARD_IF_FALSE   102 (to 794)
                      590 LOAD_FAST                2 (tokens)
                      592 LOAD_GLOBAL             13 (NULL + len)
                      604 LOAD_FAST                2 (tokens)
                      606 PRECALL                  1
                      610 CALL                     1
                      620 LOAD_CONST               6 (2)
                      622 BINARY_OP               10 (-)
                      626 BINARY_SUBSCR
                      636 LOAD_CONST              10 ('as')
                      638 COMPARE_OP               2 (==)
                      644 POP_JUMP_FORWARD_IF_FALSE    74 (to 794)
          
-         211         646 LOAD_FAST                2 (tokens)
+         213         646 LOAD_FAST                2 (tokens)
                      648 LOAD_METHOD              1 (pop)
                      670 LOAD_GLOBAL             13 (NULL + len)
                      682 LOAD_FAST                2 (tokens)
                      684 PRECALL                  1
                      688 CALL                     1
                      698 LOAD_CONST               9 (1)
                      700 BINARY_OP               10 (-)
                      704 PRECALL                  1
                      708 CALL                     1
                      718 STORE_FAST               9 (as_var)
          
-         212         720 LOAD_FAST                2 (tokens)
+         214         720 LOAD_FAST                2 (tokens)
                      722 LOAD_METHOD              1 (pop)
                      744 LOAD_GLOBAL             13 (NULL + len)
                      756 LOAD_FAST                2 (tokens)
                      758 PRECALL                  1
                      762 CALL                     1
                      772 LOAD_CONST               9 (1)
                      774 BINARY_OP               10 (-)
                      778 PRECALL                  1
                      782 CALL                     1
                      792 POP_TOP
          
-         214     >>  794 LOAD_GLOBAL             19 (NULL + get_kwargs)
+         216     >>  794 LOAD_GLOBAL             19 (NULL + get_kwargs)
          
-         215         806 LOAD_FAST                0 (parser)
+         217         806 LOAD_FAST                0 (parser)
          
-         216         808 LOAD_FAST                2 (tokens)
+         218         808 LOAD_FAST                2 (tokens)
          
-         217         810 LOAD_FAST                5 (adapter)
+         219         810 LOAD_FAST                5 (adapter)
                      812 LOAD_ATTR               10 (required_kwargs)
          
-         218         822 LOAD_FAST                5 (adapter)
+         220         822 LOAD_FAST                5 (adapter)
                      824 LOAD_ATTR               11 (absolute_tokens)
          
-         214         834 PRECALL                  4
+         216         834 PRECALL                  4
                      838 CALL                     4
                      848 STORE_FAST              10 (kwargs)
          
-         221         850 LOAD_GLOBAL             25 (NULL + AdapterNode)
+         223         850 LOAD_GLOBAL             25 (NULL + AdapterNode)
                      862 LOAD_CONST              12 (())
          
-         222         864 LOAD_FAST                5 (adapter)
+         224         864 LOAD_FAST                5 (adapter)
          
-         223         866 LOAD_FAST                6 (model)
+         225         866 LOAD_FAST                6 (model)
          
-         224         868 LOAD_FAST                7 (model_tokens)
+         226         868 LOAD_FAST                7 (model_tokens)
          
-         225         870 LOAD_FAST                9 (as_var)
+         227         870 LOAD_FAST                9 (as_var)
          
-         221         872 LOAD_CONST              11 (('adapter', 'model', 'getters', 'as_var'))
+         223         872 LOAD_CONST              11 (('adapter', 'model', 'getters', 'as_var'))
                      874 BUILD_CONST_KEY_MAP      4
          
-         226         876 LOAD_FAST               10 (kwargs)
+         228         876 LOAD_FAST               10 (kwargs)
          
-         221         878 DICT_MERGE               1
+         223         878 DICT_MERGE               1
                      880 CALL_FUNCTION_EX         1
                      882 RETURN_VALUE
          ExceptionTable:
            128 to 152 -> 156 [0]
            156 to 214 -> 216 [1] lasti
          consts
             None
@@ -1236,15 +1242,15 @@
             ()
          names      ('split_contents', 'pop', 'adapter_registry', 'RegistryLookUpError', 'TemplateSyntaxError', 'split', 'len', 'field_required', 'compile_filter', 'get_kwargs', 'required_kwargs', 'absolute_tokens', 'AdapterNode')
          varnames   ('parser', 'token', 'tokens', '_', 'adapter_id', 'adapter', 'model', 'model_tokens', 'model__field', 'as_var', 'kwargs')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'do_render_fedit'
-         firstlineno 174
+         firstlineno 176
          lnotab
             0x020328022a012a0202011e01120126ff08030a0104012a012a04260126
             010c0102ff100526012605500204013c014a014a020c01020102010c010c
             fc10070e0102010201020102fc040502fb
       True
       ('takes_context',)
       'adapter'
@@ -1257,81 +1263,81 @@
             0x970069007d0264017c00760072087c006401190000000000000000007d
             027401000000000000000000007c00a6010000ab0100000000000000007d
             007401000000000000000000007c02a6010000ab0100000000000000007d
             0264017c00760072037c0064013d007c00a0010000000000000000000000
             0000000000000000007c02a6010000ab01000000000000000001007c01a0
             0200000000000000000000000000000000000000007c00a6010000ab0100
             000000000000005300
-         230           0 RESUME                   0
+         232           0 RESUME                   0
          
-         232           2 BUILD_MAP                0
+         234           2 BUILD_MAP                0
                        4 STORE_FAST               2 (adapter_context)
          
-         235           6 LOAD_CONST               1 ('adapter_context')
+         237           6 LOAD_CONST               1 ('adapter_context')
                        8 LOAD_FAST                0 (context)
                       10 CONTAINS_OP              0
                       12 POP_JUMP_FORWARD_IF_FALSE     8 (to 30)
          
-         236          14 LOAD_FAST                0 (context)
+         238          14 LOAD_FAST                0 (context)
                       16 LOAD_CONST               1 ('adapter_context')
                       18 BINARY_SUBSCR
                       28 STORE_FAST               2 (adapter_context)
          
-         238     >>   30 LOAD_GLOBAL              1 (NULL + _flatten_context)
+         240     >>   30 LOAD_GLOBAL              1 (NULL + _flatten_context)
          
-         239          42 LOAD_FAST                0 (context)
+         241          42 LOAD_FAST                0 (context)
          
-         238          44 PRECALL                  1
+         240          44 PRECALL                  1
                       48 CALL                     1
                       58 STORE_FAST               0 (context)
          
-         241          60 LOAD_GLOBAL              1 (NULL + _flatten_context)
+         243          60 LOAD_GLOBAL              1 (NULL + _flatten_context)
          
-         242          72 LOAD_FAST                2 (adapter_context)
+         244          72 LOAD_FAST                2 (adapter_context)
          
-         241          74 PRECALL                  1
+         243          74 PRECALL                  1
                       78 CALL                     1
                       88 STORE_FAST               2 (adapter_context)
          
-         245          90 LOAD_CONST               1 ('adapter_context')
+         247          90 LOAD_CONST               1 ('adapter_context')
                       92 LOAD_FAST                0 (context)
                       94 CONTAINS_OP              0
                       96 POP_JUMP_FORWARD_IF_FALSE     3 (to 104)
          
-         246          98 LOAD_FAST                0 (context)
+         248          98 LOAD_FAST                0 (context)
                      100 LOAD_CONST               1 ('adapter_context')
                      102 DELETE_SUBSCR
          
-         248     >>  104 LOAD_FAST                0 (context)
+         250     >>  104 LOAD_FAST                0 (context)
                      106 LOAD_METHOD              1 (update)
          
-         249         128 LOAD_FAST                2 (adapter_context)
+         251         128 LOAD_FAST                2 (adapter_context)
          
-         248         130 PRECALL                  1
+         250         130 PRECALL                  1
                      134 CALL                     1
                      144 POP_TOP
          
-         252         146 LOAD_FAST                1 (adapter)
+         254         146 LOAD_FAST                1 (adapter)
                      148 LOAD_METHOD              2 (render_content)
          
-         253         170 LOAD_FAST                0 (context)
+         255         170 LOAD_FAST                0 (context)
          
-         252         172 PRECALL                  1
+         254         172 PRECALL                  1
                      176 CALL                     1
                      186 RETURN_VALUE
          consts
             None
             'adapter_context'
          names      ('_flatten_context', 'update', 'render_content')
          varnames   ('context', 'adapter', 'adapter_context')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'render_adapter'
-         firstlineno 230
+         firstlineno 232
          lnotab
             0x02020403080110020c0102ff10030c0102ff100408010602180102ff10
             04180102ff
       'wagtail_fedit/_hook_output.html'
       'fedit_scripts'
       ('name', 'takes_context')
       code
@@ -1350,107 +1356,107 @@
             00530067007d04740f000000000000000000006a0800000000000000007c
             03a6010000ab01000000000000000044005d417d0502007c057c02a60100
             00ab0100000000000000007d067413000000000000000000007c06741400
             0000000000000000007416000000000000000000006602a6020000ab0200
             0000000000000073037c0667017d067c04a00c0000000000000000000000
             0000000000000000007c06a6010000ab01000000000000000001008c4264
             067c0469015300
-         257           0 RESUME                   0
+         259           0 RESUME                   0
          
-         259           2 LOAD_FAST                1 (css_or_js)
+         261           2 LOAD_FAST                1 (css_or_js)
                        4 LOAD_METHOD              0 (lower)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               1 (css_or_js)
          
-         261          42 LOAD_FAST                1 (css_or_js)
+         263          42 LOAD_FAST                1 (css_or_js)
                       44 LOAD_CONST               1 (('css', 'js'))
                       46 CONTAINS_OP              1
                       48 POP_JUMP_FORWARD_IF_FALSE    15 (to 80)
          
-         262          50 LOAD_GLOBAL              3 (NULL + ValueError)
+         264          50 LOAD_GLOBAL              3 (NULL + ValueError)
                       62 LOAD_CONST               2 ("Invalid argument, must be 'css' or 'js'")
                       64 PRECALL                  1
                       68 CALL                     1
                       78 RAISE_VARARGS            1
          
-         264     >>   80 LOAD_FAST                0 (context)
+         266     >>   80 LOAD_FAST                0 (context)
                       82 LOAD_METHOD              2 (get)
                      104 LOAD_CONST               3 ('request')
                      106 PRECALL                  1
                      110 CALL                     1
                      120 STORE_FAST               2 (request)
          
-         266         122 LOAD_FAST                1 (css_or_js)
+         268         122 LOAD_FAST                1 (css_or_js)
                      124 LOAD_CONST               4 ('css')
                      126 COMPARE_OP               2 (==)
                      132 POP_JUMP_FORWARD_IF_FALSE     8 (to 150)
          
-         267         134 LOAD_GLOBAL              6 (REGISTER_CSS)
+         269         134 LOAD_GLOBAL              6 (REGISTER_CSS)
                      146 STORE_FAST               3 (hook_name)
                      148 JUMP_FORWARD             7 (to 164)
          
-         269     >>  150 LOAD_GLOBAL              8 (REGISTER_JS)
+         271     >>  150 LOAD_GLOBAL              8 (REGISTER_JS)
                      162 STORE_FAST               3 (hook_name)
          
-         271     >>  164 LOAD_GLOBAL             11 (NULL + getattr)
+         273     >>  164 LOAD_GLOBAL             11 (NULL + getattr)
                      176 LOAD_FAST                2 (request)
                      178 LOAD_GLOBAL             12 (FEDIT_PREVIEW_VAR)
                      190 LOAD_CONST               5 (False)
                      192 PRECALL                  3
                      196 CALL                     3
                      206 POP_JUMP_FORWARD_IF_TRUE     2 (to 212)
          
-         272         208 BUILD_MAP                0
+         274         208 BUILD_MAP                0
                      210 RETURN_VALUE
          
-         274     >>  212 BUILD_LIST               0
+         276     >>  212 BUILD_LIST               0
                      214 STORE_FAST               4 (files)
          
-         275         216 LOAD_GLOBAL             15 (NULL + hooks)
+         277         216 LOAD_GLOBAL             15 (NULL + hooks)
                      228 LOAD_ATTR                8 (get_hooks)
                      238 LOAD_FAST                3 (hook_name)
                      240 PRECALL                  1
                      244 CALL                     1
                      254 GET_ITER
                  >>  256 FOR_ITER                65 (to 388)
                      258 STORE_FAST               5 (hook)
          
-         276         260 PUSH_NULL
+         278         260 PUSH_NULL
                      262 LOAD_FAST                5 (hook)
                      264 LOAD_FAST                2 (request)
                      266 PRECALL                  1
                      270 CALL                     1
                      280 STORE_FAST               6 (ret)
          
-         278         282 LOAD_GLOBAL             19 (NULL + isinstance)
+         280         282 LOAD_GLOBAL             19 (NULL + isinstance)
                      294 LOAD_FAST                6 (ret)
                      296 LOAD_GLOBAL             20 (list)
                      308 LOAD_GLOBAL             22 (tuple)
                      320 BUILD_TUPLE              2
                      322 PRECALL                  2
                      326 CALL                     2
                      336 POP_JUMP_FORWARD_IF_TRUE     3 (to 344)
          
-         279         338 LOAD_FAST                6 (ret)
+         281         338 LOAD_FAST                6 (ret)
                      340 BUILD_LIST               1
                      342 STORE_FAST               6 (ret)
          
-         281     >>  344 LOAD_FAST                4 (files)
+         283     >>  344 LOAD_FAST                4 (files)
                      346 LOAD_METHOD             12 (extend)
                      368 LOAD_FAST                6 (ret)
                      370 PRECALL                  1
                      374 CALL                     1
                      384 POP_TOP
                      386 JUMP_BACKWARD           66 (to 256)
          
-         284     >>  388 LOAD_CONST               6 ('hook_output')
+         286     >>  388 LOAD_CONST               6 ('hook_output')
                      390 LOAD_FAST                4 (files)
          
-         283         392 BUILD_MAP                1
+         285         392 BUILD_MAP                1
                      394 RETURN_VALUE
          consts
             None
             ('css', 'js')
             "Invalid argument, must be 'css' or 'js'"
             'request'
             'css'
@@ -1458,15 +1464,15 @@
             'hook_output'
          names      ('lower', 'ValueError', 'get', 'REGISTER_CSS', 'REGISTER_JS', 'getattr', 'FEDIT_PREVIEW_VAR', 'hooks', 'get_hooks', 'isinstance', 'list', 'tuple', 'extend')
          varnames   ('context', 'css_or_js', 'request', 'hook_name', 'files', 'hook', 'ret')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'static_hook_output'
-         firstlineno 257
+         firstlineno 259
          lnotab
             0x0202280208011e022a020c0110020e022c01040204012c011602380106
             022c0304ff
       False
       'tooltip'
       ('takes_context', 'name')
       'wrapping'
@@ -1482,43 +1488,43 @@
             02000000000000000000000000000000000000000064047c049b00640574
             07000000000000000000007c05a6010000ab0100000000000000009b0064
             069d05a6010000ab01000000000000000001008c2f6407a0040000000000
             0000000000000000000000000000007c03a6010000ab0100000000000000
             007d067c01730f740b000000000000000000007c06a6010000ab01000000
             00000000005300740b0000000000000000000064087c069b0064097c019b
             00640a9d05a6010000ab0100000000000000005300
-         287           0 RESUME                   0
+         289           0 RESUME                   0
          
-         290           2 LOAD_GLOBAL              0 (TIPPY_ENABLED)
+         292           2 LOAD_GLOBAL              0 (TIPPY_ENABLED)
                       14 POP_JUMP_FORWARD_IF_TRUE     2 (to 20)
          
-         291          16 LOAD_CONST               1 ('')
+         293          16 LOAD_CONST               1 ('')
                       18 RETURN_VALUE
          
-         293     >>   20 LOAD_FAST                0 (content)
+         295     >>   20 LOAD_FAST                0 (content)
                       22 LOAD_FAST                2 (kwargs)
                       24 LOAD_CONST               2 ('content')
                       26 STORE_SUBSCR
          
-         295          30 LOAD_CONST               3 ("data-tooltip='true'")
+         297          30 LOAD_CONST               3 ("data-tooltip='true'")
          
-         294          32 BUILD_LIST               1
+         296          32 BUILD_LIST               1
                       34 STORE_FAST               3 (s)
          
-         297          36 LOAD_FAST                2 (kwargs)
+         299          36 LOAD_FAST                2 (kwargs)
                       38 LOAD_METHOD              1 (items)
                       60 PRECALL                  0
                       64 CALL                     0
                       74 GET_ITER
                  >>   76 FOR_ITER                46 (to 170)
                       78 UNPACK_SEQUENCE          2
                       82 STORE_FAST               4 (key)
                       84 STORE_FAST               5 (value)
          
-         298          86 LOAD_FAST                3 (s)
+         300          86 LOAD_FAST                3 (s)
                       88 LOAD_METHOD              2 (append)
                      110 LOAD_CONST               4 ('data-tooltip-')
                      112 LOAD_FAST                4 (key)
                      114 FORMAT_VALUE             0
                      116 LOAD_CONST               5 ("='")
                      118 LOAD_GLOBAL              7 (NULL + escape)
                      130 LOAD_FAST                5 (value)
@@ -1528,31 +1534,31 @@
                      148 LOAD_CONST               6 ("'")
                      150 BUILD_STRING             5
                      152 PRECALL                  1
                      156 CALL                     1
                      166 POP_TOP
                      168 JUMP_BACKWARD           47 (to 76)
          
-         299     >>  170 LOAD_CONST               7 (' ')
+         301     >>  170 LOAD_CONST               7 (' ')
                      172 LOAD_METHOD              4 (join)
                      194 LOAD_FAST                3 (s)
                      196 PRECALL                  1
                      200 CALL                     1
                      210 STORE_FAST               6 (attrs)
          
-         301         212 LOAD_FAST                1 (wrapping)
+         303         212 LOAD_FAST                1 (wrapping)
                      214 POP_JUMP_FORWARD_IF_TRUE    15 (to 246)
          
-         302         216 LOAD_GLOBAL             11 (NULL + mark_safe)
+         304         216 LOAD_GLOBAL             11 (NULL + mark_safe)
                      228 LOAD_FAST                6 (attrs)
                      230 PRECALL                  1
                      234 CALL                     1
                      244 RETURN_VALUE
          
-         304     >>  246 LOAD_GLOBAL             11 (NULL + mark_safe)
+         306     >>  246 LOAD_GLOBAL             11 (NULL + mark_safe)
                      258 LOAD_CONST               8 ('<span ')
                      260 LOAD_FAST                6 (attrs)
                      262 FORMAT_VALUE             0
                      264 LOAD_CONST               9 ('>')
                      266 LOAD_FAST                1 (wrapping)
                      268 FORMAT_VALUE             0
                      270 LOAD_CONST              10 ('</span>')
@@ -1574,76 +1580,76 @@
             '</span>'
          names      ('TIPPY_ENABLED', 'items', 'append', 'escape', 'join', 'mark_safe')
          varnames   ('content', 'wrapping', 'kwargs', 's', 'key', 'value', 'attrs')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'tooltip'
-         firstlineno 287
+         firstlineno 289
          lnotab 0x02030e0104020a0202ff0403320154012a0204011e02
       'fedit_userbar'
       'model'
       code
          argcount  : 2
          nlocals   : 2
          stacksize : 4
          flags     : 3
          code
             0x970064017c00760072197401000000000000000000007c006401190000
             000000000000007c01a6020000ab0200000000000000007c0064013c0000
             007402000000000000000000007c007600721b7c00740200000000000000
             000000190000000000000000007c016b0300000000720a7c017c00740200
             0000000000000000003c00000064025300
-         306           0 RESUME                   0
+         308           0 RESUME                   0
          
-         308           2 LOAD_CONST               1 ('request')
+         310           2 LOAD_CONST               1 ('request')
                        4 LOAD_FAST                0 (context)
                        6 CONTAINS_OP              0
                        8 POP_JUMP_FORWARD_IF_FALSE    25 (to 60)
          
-         309          10 LOAD_GLOBAL              1 (NULL + with_userbar_model)
+         311          10 LOAD_GLOBAL              1 (NULL + with_userbar_model)
                       22 LOAD_FAST                0 (context)
                       24 LOAD_CONST               1 ('request')
                       26 BINARY_SUBSCR
                       36 LOAD_FAST                1 (model)
                       38 PRECALL                  2
                       42 CALL                     2
                       52 LOAD_FAST                0 (context)
                       54 LOAD_CONST               1 ('request')
                       56 STORE_SUBSCR
          
-         310     >>   60 LOAD_GLOBAL              2 (PAGE_TEMPLATE_VAR)
+         312     >>   60 LOAD_GLOBAL              2 (PAGE_TEMPLATE_VAR)
                       72 LOAD_FAST                0 (context)
                       74 CONTAINS_OP              0
                       76 POP_JUMP_FORWARD_IF_FALSE    27 (to 132)
                       78 LOAD_FAST                0 (context)
                       80 LOAD_GLOBAL              2 (PAGE_TEMPLATE_VAR)
                       92 BINARY_SUBSCR
                      102 LOAD_FAST                1 (model)
                      104 COMPARE_OP               3 (!=)
                      110 POP_JUMP_FORWARD_IF_FALSE    10 (to 132)
          
-         311         112 LOAD_FAST                1 (model)
+         313         112 LOAD_FAST                1 (model)
                      114 LOAD_FAST                0 (context)
                      116 LOAD_GLOBAL              2 (PAGE_TEMPLATE_VAR)
                      128 STORE_SUBSCR
          
-         312     >>  132 LOAD_CONST               2 ('')
+         314     >>  132 LOAD_CONST               2 ('')
                      134 RETURN_VALUE
          consts
             None
             'request'
             ''
          names      ('with_userbar_model', 'PAGE_TEMPLATE_VAR')
          varnames   ('context', 'model')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'do_with_userbar_model'
-         firstlineno 306
+         firstlineno 308
          lnotab 0x02020801320134011401
       'tokens'
       'kwarg_list'
       'absolute_tokens'
       code
          argcount  : 4
          nlocals   : 11
@@ -1670,212 +1676,212 @@
             0000007d0a7c0a7c057c093c0000008cd37c086404190000000000000000
             007d097c097c0376007213740d0000000000000000000064077c099b0064
             089d03a6010000ab01000000000000000082017c00a00500000000000000
             000000000000000000000000007c08640319000000000000000000a60100
             00ab0100000000000000007c057c093c00000064057d0490018c147c0244
             005d187d097c097c0576017212740d0000000000000000000064097c099b
             009d02a6010000ab01000000000000000082018c197c055300
-         314           0 RESUME                   0
+         316           0 RESUME                   0
          
-         315           2 LOAD_CONST               1 (False)
+         317           2 LOAD_CONST               1 (False)
                        4 STORE_FAST               4 (had_kwargs)
          
-         316           6 BUILD_MAP                0
+         318           6 BUILD_MAP                0
                        8 STORE_FAST               5 (kwargs)
          
-         318          10 LOAD_FAST                2 (kwarg_list)
+         320          10 LOAD_FAST                2 (kwarg_list)
                       12 POP_JUMP_FORWARD_IF_TRUE    14 (to 42)
          
-         319          14 LOAD_GLOBAL              1 (NULL + tuple)
+         321          14 LOAD_GLOBAL              1 (NULL + tuple)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               2 (kwarg_list)
          
-         321     >>   42 LOAD_FAST                3 (absolute_tokens)
+         323     >>   42 LOAD_FAST                3 (absolute_tokens)
                       44 POP_JUMP_FORWARD_IF_TRUE    14 (to 74)
          
-         322          46 LOAD_GLOBAL              1 (NULL + tuple)
+         324          46 LOAD_GLOBAL              1 (NULL + tuple)
                       58 PRECALL                  0
                       62 CALL                     0
                       72 STORE_FAST               3 (absolute_tokens)
          
-         324     >>   74 LOAD_GLOBAL              3 (NULL + enumerate)
+         326     >>   74 LOAD_GLOBAL              3 (NULL + enumerate)
                       86 LOAD_FAST                1 (tokens)
                       88 PRECALL                  1
                       92 CALL                     1
                      102 GET_ITER
                  >>  104 EXTENDED_ARG             1
                      106 FOR_ITER               274 (to 656)
                      108 UNPACK_SEQUENCE          2
                      112 STORE_FAST               6 (i)
                      114 STORE_FAST               7 (token)
          
-         325         116 LOAD_FAST                7 (token)
+         327         116 LOAD_FAST                7 (token)
                      118 LOAD_METHOD              2 (split)
                      140 LOAD_CONST               2 ('=')
                      142 PRECALL                  1
                      146 CALL                     1
                      156 STORE_FAST               8 (split)
          
-         326         158 LOAD_GLOBAL              7 (NULL + len)
+         328         158 LOAD_GLOBAL              7 (NULL + len)
                      170 LOAD_FAST                8 (split)
                      172 PRECALL                  1
                      176 CALL                     1
                      186 LOAD_CONST               3 (1)
                      188 COMPARE_OP               2 (==)
                      194 POP_JUMP_FORWARD_IF_FALSE    89 (to 374)
                      196 LOAD_GLOBAL              7 (NULL + len)
                      208 LOAD_FAST                2 (kwarg_list)
                      210 PRECALL                  1
                      214 CALL                     1
                      224 LOAD_FAST                6 (i)
                      226 COMPARE_OP               4 (>)
                      232 POP_JUMP_FORWARD_IF_FALSE    70 (to 374)
          
-         327         234 LOAD_FAST                8 (split)
+         329         234 LOAD_FAST                8 (split)
                      236 LOAD_CONST               4 (0)
                      238 BINARY_SUBSCR
                      248 LOAD_FAST                3 (absolute_tokens)
                      250 CONTAINS_OP              0
                      252 POP_JUMP_FORWARD_IF_FALSE    12 (to 278)
          
-         328         254 LOAD_CONST               5 (True)
+         330         254 LOAD_CONST               5 (True)
                      256 LOAD_FAST                5 (kwargs)
                      258 LOAD_FAST                8 (split)
                      260 LOAD_CONST               4 (0)
                      262 BINARY_SUBSCR
                      272 STORE_SUBSCR
          
-         329         276 JUMP_BACKWARD           87 (to 104)
+         331         276 JUMP_BACKWARD           87 (to 104)
          
-         331     >>  278 LOAD_FAST                4 (had_kwargs)
+         333     >>  278 LOAD_FAST                4 (had_kwargs)
                      280 POP_JUMP_FORWARD_IF_FALSE    15 (to 312)
          
-         332         282 LOAD_GLOBAL              9 (NULL + ValueError)
+         334         282 LOAD_GLOBAL              9 (NULL + ValueError)
                      294 LOAD_CONST               6 ('Unexpected positional argument after keyword argument')
                      296 PRECALL                  1
                      300 CALL                     1
                      310 RAISE_VARARGS            1
          
-         334     >>  312 LOAD_FAST                0 (parser)
+         336     >>  312 LOAD_FAST                0 (parser)
                      314 LOAD_METHOD              5 (compile_filter)
                      336 LOAD_FAST                7 (token)
                      338 PRECALL                  1
                      342 CALL                     1
                      352 LOAD_FAST                5 (kwargs)
                      354 LOAD_FAST                2 (kwarg_list)
                      356 LOAD_FAST                6 (i)
                      358 BINARY_SUBSCR
                      368 STORE_SUBSCR
                      372 JUMP_BACKWARD          135 (to 104)
          
-         335     >>  374 LOAD_GLOBAL              7 (NULL + len)
+         337     >>  374 LOAD_GLOBAL              7 (NULL + len)
                      386 LOAD_FAST                8 (split)
                      388 PRECALL                  1
                      392 CALL                     1
                      402 LOAD_CONST               3 (1)
                      404 COMPARE_OP               2 (==)
                      410 POP_JUMP_FORWARD_IF_FALSE    57 (to 526)
          
-         336         412 LOAD_FAST                8 (split)
+         338         412 LOAD_FAST                8 (split)
                      414 LOAD_CONST               4 (0)
                      416 BINARY_SUBSCR
                      426 LOAD_FAST                3 (absolute_tokens)
                      428 CONTAINS_OP              0
                      430 POP_JUMP_FORWARD_IF_FALSE    12 (to 456)
          
-         337         432 LOAD_CONST               5 (True)
+         339         432 LOAD_CONST               5 (True)
                      434 LOAD_FAST                5 (kwargs)
                      436 LOAD_FAST                8 (split)
                      438 LOAD_CONST               4 (0)
                      440 BINARY_SUBSCR
                      450 STORE_SUBSCR
          
-         338         454 JUMP_BACKWARD          176 (to 104)
+         340         454 JUMP_BACKWARD          176 (to 104)
          
-         340     >>  456 LOAD_FAST                8 (split)
+         342     >>  456 LOAD_FAST                8 (split)
                      458 LOAD_CONST               4 (0)
                      460 BINARY_SUBSCR
                      470 STORE_FAST               9 (key)
          
-         341         472 LOAD_FAST                0 (parser)
+         343         472 LOAD_FAST                0 (parser)
                      474 LOAD_METHOD              5 (compile_filter)
                      496 LOAD_FAST                9 (key)
                      498 PRECALL                  1
                      502 CALL                     1
                      512 STORE_FAST              10 (value)
          
-         342         514 LOAD_FAST               10 (value)
+         344         514 LOAD_FAST               10 (value)
                      516 LOAD_FAST                5 (kwargs)
                      518 LOAD_FAST                9 (key)
                      520 STORE_SUBSCR
                      524 JUMP_BACKWARD          211 (to 104)
          
-         344     >>  526 LOAD_FAST                8 (split)
+         346     >>  526 LOAD_FAST                8 (split)
                      528 LOAD_CONST               4 (0)
                      530 BINARY_SUBSCR
                      540 STORE_FAST               9 (key)
          
-         347         542 LOAD_FAST                9 (key)
+         349         542 LOAD_FAST                9 (key)
                      544 LOAD_FAST                3 (absolute_tokens)
                      546 CONTAINS_OP              0
                      548 POP_JUMP_FORWARD_IF_FALSE    19 (to 588)
          
-         348         550 LOAD_GLOBAL             13 (NULL + TemplateSyntaxError)
+         350         550 LOAD_GLOBAL             13 (NULL + TemplateSyntaxError)
          
-         349         562 LOAD_CONST               7 ('Keyword argument ')
+         351         562 LOAD_CONST               7 ('Keyword argument ')
                      564 LOAD_FAST                9 (key)
                      566 FORMAT_VALUE             0
                      568 LOAD_CONST               8 (' cannot be resolved; it can only be used as an absolute argument.')
                      570 BUILD_STRING             3
          
-         348         572 PRECALL                  1
+         350         572 PRECALL                  1
                      576 CALL                     1
                      586 RAISE_VARARGS            1
          
-         353     >>  588 LOAD_FAST                0 (parser)
+         355     >>  588 LOAD_FAST                0 (parser)
                      590 LOAD_METHOD              5 (compile_filter)
                      612 LOAD_FAST                8 (split)
                      614 LOAD_CONST               3 (1)
                      616 BINARY_SUBSCR
                      626 PRECALL                  1
                      630 CALL                     1
                      640 LOAD_FAST                5 (kwargs)
                      642 LOAD_FAST                9 (key)
                      644 STORE_SUBSCR
          
-         354         648 LOAD_CONST               5 (True)
+         356         648 LOAD_CONST               5 (True)
                      650 STORE_FAST               4 (had_kwargs)
                      652 EXTENDED_ARG             1
                      654 JUMP_BACKWARD          276 (to 104)
          
-         356     >>  656 LOAD_FAST                2 (kwarg_list)
+         358     >>  656 LOAD_FAST                2 (kwarg_list)
                      658 GET_ITER
                  >>  660 FOR_ITER                24 (to 710)
                      662 STORE_FAST               9 (key)
          
-         357         664 LOAD_FAST                9 (key)
+         359         664 LOAD_FAST                9 (key)
                      666 LOAD_FAST                5 (kwargs)
                      668 CONTAINS_OP              1
                      670 POP_JUMP_FORWARD_IF_FALSE    18 (to 708)
          
-         358         672 LOAD_GLOBAL             13 (NULL + TemplateSyntaxError)
+         360         672 LOAD_GLOBAL             13 (NULL + TemplateSyntaxError)
          
-         359         684 LOAD_CONST               9 ('Missing required keyword argument ')
+         361         684 LOAD_CONST               9 ('Missing required keyword argument ')
                      686 LOAD_FAST                9 (key)
                      688 FORMAT_VALUE             0
                      690 BUILD_STRING             2
          
-         358         692 PRECALL                  1
+         360         692 PRECALL                  1
                      696 CALL                     1
                      706 RAISE_VARARGS            1
          
-         357     >>  708 JUMP_BACKWARD           25 (to 660)
+         359     >>  708 JUMP_BACKWARD           25 (to 660)
          
-         362     >>  710 LOAD_FAST                5 (kwargs)
+         364     >>  710 LOAD_FAST                5 (kwargs)
                      712 RETURN_VALUE
          consts
             None
             False
             '='
             1
             0
@@ -1886,25 +1892,25 @@
             'Missing required keyword argument '
          names      ('tuple', 'enumerate', 'split', 'len', 'ValueError', 'compile_filter', 'TemplateSyntaxError')
          varnames   ('parser', 'tokens', 'kwarg_list', 'absolute_tokens', 'had_kwargs', 'kwargs', 'i', 'token', 'split', 'key', 'value')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'get_kwargs'
-         firstlineno 314
+         firstlineno 316
          lnotab
             0x02010401040204011c0204011c022a012a014c0114011601020204011e
             023e01260114011601020210012a010c02100308010c010aff10053c0108
             02080108010c0108ff10ff0205
       (None,)
       (None, None)
-   names      ('typing', 'Type', 'Any', 'django.template', 'library', 'Node', 'TemplateSyntaxError', 'django.template.context', 'Context', 'django.template.base', 'Parser', 'Token', 'FilterExpression', 'django.utils.html', 'escape', 'django.utils.safestring', 'mark_safe', 'django.core', 'signing', 'wagtail', 'hooks', 'wagtail.models', 'Page', 'PAGE_TEMPLATE_VAR', 'warnings', 'settings', 'TIPPY_ENABLED', 'adapters', 'adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError', 'utils', 'wrap_adapter', 'with_userbar_model', 'base_adapter_context', '_flatten_context', '_can_edit', 'FEDIT_PREVIEW_VAR', 'TEMPLATE_TAG_NAME', 'FIELD_TEMPLATE_VAR', 'INSTANCE_TEMPLATE_VAR', 'REGISTER_CSS', 'REGISTER_JS', 'Library', 'register', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'str', 'as_var', 'AdapterNode', 'tag', 'do_render_fedit', 'simple_tag', 'render_adapter', 'inclusion_tag', 'dict', 'static_hook_output', 'tooltip', 'do_with_userbar_model', 'list', 'get_kwargs')
+   names      ('typing', 'Type', 'Any', 'django.template', 'library', 'Node', 'TemplateSyntaxError', 'django.template.context', 'Context', 'django.template.base', 'Parser', 'Token', 'FilterExpression', 'django.utils.html', 'escape', 'django.utils.safestring', 'mark_safe', 'django.core', 'signing', 'wagtail', 'hooks', 'wagtail.models', 'Page', 'PAGE_TEMPLATE_VAR', 'warnings', 'settings', 'TIPPY_ENABLED', 'adapters', 'BaseAdapter', 'AdapterError', 'registry', 'adapter_registry', 'RegistryLookUpError', 'utils', 'wrap_adapter', 'with_userbar_model', 'base_adapter_context', '_flatten_context', '_can_edit', 'FEDIT_PREVIEW_VAR', 'TEMPLATE_TAG_NAME', 'FIELD_TEMPLATE_VAR', 'INSTANCE_TEMPLATE_VAR', 'REGISTER_CSS', 'REGISTER_JS', 'Library', 'register', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'str', 'as_var', 'AdapterNode', 'tag', 'do_render_fedit', 'simple_tag', 'render_adapter', 'inclusion_tag', 'dict', 'static_hook_output', 'tooltip', 'do_with_userbar_model', 'list', 'get_kwargs')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff0201100114030c0314040c010c010c020c01100508020c0318062c
-      0c10061e030401040318071c6d2a010eff0e0102372a0112ff0e01021a2e
-      010aff0e01021d2c0110ff0e0102122c010eff0e010207
+      0x00ff0201100114030c0314040c010c010c020c01100508020c03100410
+      042c0c10061e030401040318071c6d2a010eff0e0102372a0112ff0e0102
+      1a2e010aff0e01021d2c0110ff0e0102122c010eff0e010207
```

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.5.8/wagtail_fedit/templatetags/fedit.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,19 +21,21 @@
 
 import warnings
 
 from ..settings import (
     TIPPY_ENABLED,
 )
 from ..adapters import (
-    adapter_registry,
-    RegistryLookUpError,
     BaseAdapter,
     AdapterError,
 )
+from ..registry import (
+    registry as adapter_registry,
+    RegistryLookUpError,
+)
 from ..utils import (
     wrap_adapter,
     with_userbar_model,
     base_adapter_context,
     _flatten_context,
     _can_edit,
     FEDIT_PREVIEW_VAR,
```

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.5.8/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.5.8/wagtail_fedit/test/core/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.5.8/wagtail_fedit/test/core/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/test_adapters.py` & `wagtail_fedit-1.5.8/wagtail_fedit/test/core/tests/test_adapters.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 from django.template import (
     Context, Template,
     TemplateSyntaxError,
 )
 from wagtail_fedit.adapters import (
     Keyword,
     BaseAdapter,
-    adapter_registry,
     BlockAdapter,
     FieldAdapter,
     ModelAdapter,
 )
+from wagtail_fedit.registry import (
+    registry as adapter_registry,
+)
 from wagtail_fedit.adapters.base import (
     BlockFieldReplacementAdapter,
 )
 from wagtail_fedit.utils import (
     FEDIT_PREVIEW_VAR,
     FIELD_TEMPLATE_VAR,
     INSTANCE_TEMPLATE_VAR,
@@ -633,15 +635,15 @@
         )
         request.user = self.admin_user
         setattr(
             request,
             FEDIT_PREVIEW_VAR,
             True,
         )
-        block_value, _ = block
+        block_value, _, parent, idx = block
         template = Template(
             "{% load fedit %}"
             f"{{% fedit test_block object.content block=block block_id=block_id id='{id}' %}}"
         )
 
         context = {
             "object": self.basic_model,
@@ -670,15 +672,15 @@
 
         request.user = self.admin_user
         setattr(
             request,
             FEDIT_PREVIEW_VAR,
             True,
         )
-        block_value, _ = block
+        block_value, _, parent, idx = block
         template = Template(
             "{% load fedit %}"
             f"{{% fedit test_block object.content block=block block_id=block_id id='{id}' as test %}}"
             "{{ test }}"
         )
 
         context = {
@@ -706,15 +708,15 @@
         )
         request.user = self.admin_user
         setattr(
             request,
             FEDIT_PREVIEW_VAR,
             True,
         )
-        block_value, _ = block
+        block_value, _, parent, idx = block
         template = Template(
             "{% load fedit %}"
             f"{{% fedit test_block from_context block=block block_id=block_id id='{id}' %}}"
         )
 
         context = {
             "object": self.basic_model,
@@ -739,15 +741,15 @@
         block = find_block(self.BLOCK_ID, streamfield)
         request = self.request_factory.get(
             self.get_editable_url(
                 self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
             )
         )
         request.user = self.admin_user
-        block_value, _ = block
+        block_value, _, parent, idx = block
         template = Template(
             "{% load fedit %}"
             f"{{% fedit test_block from_context block=block block_id=block_id id='{id}' %}}"
         )
 
         context = {
             "object": self.basic_model,
```

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.5.8/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             
             if isinstance(model, RevisionMixin):
                 self.assertEqual(model.revisions.count(), 0)
             else:
                 with self.assertRaises(AttributeError):
                     model.revisions.count()
 
-            bound, _ = find_block(block_id=self.BLOCK_ID, field=model.content)
+            bound, _, _, _ = find_block(block_id=self.BLOCK_ID, field=model.content)
             initial_content = bound.value["link"]["text"]
 
             response = self.client.post(
                 self.get_block_url(
                     self.BLOCK_ID,
                     "content",
                     model._meta.app_label,
@@ -46,15 +46,15 @@
                 self.assertEqual(model.revisions.count(), 1)
                 chk = model.latest_revision.as_object()
             else:
                 with self.assertRaises(AttributeError):
                     model.revisions.count()
                 chk = model
 
-            bound, contentpath = find_block(block_id=self.BLOCK_ID, field=chk.content)
+            bound, contentpath, parent, idx = find_block(block_id=self.BLOCK_ID, field=chk.content)
             self.assertEqual(bound.value["link"]["text"], f"{initial_content} test case {i + 1}",
                 msg=f"Block: {bound.block} does not contain the expected value: {initial_content} test case {i + 1}"
             )
 
     def test_unauthorized_unchanged(self):
         self.client.force_login(self.regular_user)
         
@@ -87,15 +87,15 @@
                 chk = model
 
             self.assertEqual(chk.content.get_prep_value(), initial_content.get_prep_value())
 
     def test_lock_unchanged(self):
         self.client.force_login(self.other_admin_user)
         initial_content = self.lock_model.content
-        initial_bound, _ = find_block(block_id=self.BLOCK_ID, field=self.lock_model.content)
+        initial_bound, _, parent, idx = find_block(block_id=self.BLOCK_ID, field=self.lock_model.content)
 
         response = self.client.post(
             self.get_block_url(
                 self.BLOCK_ID,
                 "content",
                 self.lock_model._meta.app_label,
                 self.lock_model._meta.model_name,
```

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.5.8/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from django.test import TestCase
 from wagtail import blocks
 from wagtail_fedit import forms as block_forms
 from wagtail_fedit import utils
+import copy
 from .base import TEST_BLOCK_DATA
 from ..models import (
     HeadingComponent,
     FlatMenuComponent
 )
 
 import uuid
@@ -49,32 +50,66 @@
 
 class TestBlocks(TestCase):
     def setUp(self) -> None:
         self.stream_block = blocks.StreamBlock([
             ("heading_component", HeadingComponent()),
             ("flat_menu_component", FlatMenuComponent())
         ])
-        self.stream_value = self.stream_block.to_python(TEST_BLOCK_DATA)
+        self.stream_value = self.stream_block.to_python(copy.deepcopy(TEST_BLOCK_DATA))
 
     def test_find_block(self):
-        block, contentpath = utils.find_block("d543a6bf-34dc-4365-a3fa-d302561930ae", self.stream_value)
+        block, contentpath, parent, idx = utils.find_block("d543a6bf-34dc-4365-a3fa-d302561930ae", self.stream_value)
         self.assertEqual(block.value["heading"], "AWESOME!!")
         self.assertEqual(block.value["subheading"], "RIGHT?!")
 
-        block, contentpath = utils.find_block("a98a19c6-2ead-4e69-9ea2-3158c7e82976", self.stream_value)
+        block, contentpath, parent, idx = utils.find_block("a98a19c6-2ead-4e69-9ea2-3158c7e82976", self.stream_value)
         self.assertEqual(block.value["link"]["text"], "Test Item 3")
         self.assertEqual(contentpath, ["3e9144fd-5fa5-47f8-917e-8fe87c15da01", "items", "a98a19c6-2ead-4e69-9ea2-3158c7e82976"])
 
         item = self.stream_block.get_block_by_content_path(self.stream_value, contentpath)
         self.assertEqual(item.value["link"]["text"], "Test Item 3")
 
-        block, contentpath = utils.find_block("invalid-id", self.stream_value)
+        block, contentpath, parent, idx = utils.find_block("invalid-id", self.stream_value)
         self.assertIsNone(block)
         self.assertEqual(contentpath, [])
 
+    def test_find_block_parent(self):
+        block, contentpath, parent, idx = utils.find_block("d543a6bf-34dc-4365-a3fa-d302561930ae", self.stream_value)
+        self.assertEqual(parent, self.stream_value)
+
+        block, contentpath, parent, idx = utils.find_block("a98a19c6-2ead-4e69-9ea2-3158c7e82976", self.stream_value)
+        self.assertEqual(idx, 2)
+        self.assertEqual(parent[idx].value["link"]["text"], "Test Item 3")
+    
+    def test_move_block_down(self):
+        block, contentpath, parent, idx = utils.find_block("a98a19c6-2ead-4e69-9ea2-3158c7e82976", self.stream_value)
+        self.assertEqual(idx, 2)
+        self.assertEqual(parent[idx].value["link"]["text"], "Test Item 3")
+
+        if idx < len(parent) - 1:
+            parent[idx], parent[idx + 1] = parent[idx + 1], parent[idx]
+        else:
+            self.fail("Block is already at the bottom")
+
+        self.assertEqual(parent[idx].value["link"]["text"], "Test Item 4")
+        self.assertEqual(parent[idx + 1].value["link"]["text"], "Test Item 3")
+
+    def test_move_block_up(self):
+        block, contentpath, parent, idx = utils.find_block("a98a19c6-2ead-4e69-9ea2-3158c7e82976", self.stream_value)
+        self.assertEqual(idx, 2)
+        self.assertEqual(parent[idx].value["link"]["text"], "Test Item 3")
+
+        if idx > 0:
+            parent[idx], parent[idx - 1] = parent[idx - 1], parent[idx]
+        else:
+            self.fail("Block is already at the top")
+
+        self.assertEqual(parent[idx].value["link"]["text"], "Test Item 2")
+        self.assertEqual(parent[idx - 1].value["link"]["text"], "Test Item 3")
+
     def test_get_form_class(self):
         block = utils.find_block("d543a6bf-34dc-4365-a3fa-d302561930ae", self.stream_value)[0]
         form_class = block_forms.get_block_form_class(block.block)
         self.assertIsNotNone(form_class)
 
         VALID_DATA = {
             "value-heading": "New Heading",
```

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.5.8/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/test_generic.py` & `wagtail_fedit-1.5.8/wagtail_fedit/test/core/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/test_model_edit.py` & `wagtail_fedit-1.5.8/wagtail_fedit/test/core/tests/test_model_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.5.8/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/test/core/tests/test_submit.py` & `wagtail_fedit-1.5.8/wagtail_fedit/test/core/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.5.8/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/test/testapp/settings.py` & `wagtail_fedit-1.5.8/wagtail_fedit/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.5.8/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.5.8/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/urls.py` & `wagtail_fedit-1.5.8/wagtail_fedit/urls.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 urlpatterns = []
 
 adapter_based_views = (
     ("edit", views.EditAdapterView),
     ("refetch", views.AdapterRefetchView),
 )
-
+ 
 for name, view in adapter_based_views:
     view.url_name = f"wagtail_fedit:{name}"
-    view.url_pattern = f"{name}/<str:adapter_id>/<str:app_label>/<str:model_name>/<str:model_id>/<str:field_name>/"
+    view.url_pattern = view.prefix_url_path(name)
     urlpatterns.append(
         path(view.url_pattern, view.as_view(), name=name)
     )
     view.url_pattern = f"{name}/<str:adapter_id>/<str:app_label>/<str:model_name>/<str:model_id>/"
     urlpatterns.append(
         path(view.url_pattern, view.as_view(), name=name)
     )
```

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/utils.py` & `wagtail_fedit-1.5.8/wagtail_fedit/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -195,36 +195,36 @@
     if not isinstance(field, StreamValue) and not hasattr(field, "__iter__"):
         field = [field]
 
     # Adjust for ListValue to get the iterable bound_blocks.
     if isinstance(field, ListValue):
         field = field.bound_blocks
 
-    for block in field:
+    for idx, block in enumerate(field):
         # Determine the block's name only if needed to avoid premature addition to contentpath.
         block_name = get_block_path(block)
         
         if getattr(block, "id", None) == block_id:
             # Append the block name here as it directly leads to the target.
-            return block, contentpath + [block_name]
+            return block, contentpath + [block_name], field, idx
         
         # Prepare to check children without altering the current path yet.
         if isinstance(block.value, blocks.StructValue):
-            for _, value in block.value.bound_blocks.items():
-                found, found_path = find_block(block_id, value, contentpath + [block_name])
+            for value in block.value.bound_blocks.values():
+                found, found_path, parent, block_index = find_block(block_id, value, contentpath + [block_name])
                 if found:
-                    return found, found_path
+                    return found, found_path, parent, block_index
 
         elif isinstance(block.value, (StreamValue, StreamValue.StreamChild, ListValue)):
-            found, found_path = find_block(block_id, block.value, contentpath + [block_name])
+            found, found_path, parent, block_index = find_block(block_id, block.value, contentpath + [block_name])
             if found:
-                return found, found_path
+                return found, found_path, parent, block_index
 
     # Return None and the current path if no block is found at this level.
-    return None, contentpath
+    return None, contentpath, field, -1
 
 
 
 _renderer_map = {}
 _field_renderer_map = {}
 _looked_for_renderers = False
 
@@ -489,58 +489,79 @@
 
     context[FIELD_TEMPLATE_VAR]    = adapter.field_name
     context[INSTANCE_TEMPLATE_VAR] = adapter.object
     context[ADAPTER_TEMPLATE_VAR]  = adapter
 
     return context
 
+def shared_context_url(shared_context: str, base_url: str, hash: str = None, **kwargs) -> str:
+    """
+    Append the shared context to a URL.
+    """
+    kwargs["shared_context"] = shared_context
+    encoded = urlencode(kwargs)
+    url = f"{base_url}?{encoded}"
+    if hash:
+        url = f"{url}#{hash}"
+    return url
+
+def get_reverse_kwargs(adapter: "BaseAdapter") -> dict:
+    reverse_kwargs = {
+        "adapter_id": adapter.identifier,
+        "app_label":  adapter.object._meta.app_label,
+        "model_name": adapter.object._meta.model_name,
+        "model_id":   adapter.object.pk,
+    }
+
+    if adapter.field_name is not None:
+        reverse_kwargs["field_name"] = adapter.field_name
+
+    return reverse_kwargs
 
 def wrap_adapter(request: HttpRequest, adapter: "BaseAdapter", context: dict, run_context_processors: bool = False) -> str:
     if not context:
         context = {}
 
+    shared = adapter.encode_shared_context()
+    adapter.shared_context_string = shared
+
     items: list[FeditAdapterComponent] = [
         *adapter.get_toolbar_buttons(),
         FeditAdapterEditButton(request, adapter),
     ]
 
     for hook in hooks.get_hooks(CONSTRUCT_ADAPTER_TOOLBAR):
         hook(items=items, adapter=adapter)
 
     items = [item.render() for item in items]
     items = list(filter(None, items))
 
-    reverse_kwargs = {
-        "adapter_id": adapter.identifier,
-        "app_label":  adapter.object._meta.app_label,
-        "model_name": adapter.object._meta.model_name,
-        "model_id":   adapter.object.pk,
-    }
-
-    if adapter.field_name is not None:
-        reverse_kwargs["field_name"] = adapter.field_name
-
-    shared = adapter.encode_shared_context()
     js_constructor = adapter.get_js_constructor()
+
+    reverse_kwargs = get_reverse_kwargs(adapter)
+    edit_url = shared_context_url(shared, reverse(
+        "wagtail_fedit:edit",
+        kwargs=reverse_kwargs,
+    ))
     
+    refetch_url = shared_context_url(shared, reverse(
+        "wagtail_fedit:refetch",
+        kwargs=reverse_kwargs,
+    ))
+
     return render_to_string(
         adapter.get_editable_template_names(),
         {
+            **adapter.wrapped_context(),
             "identifier": adapter.identifier,
             "adapter": adapter,
             "buttons": items,
             "shared": shared,
             "unique_id": adapter.get_element_id(),
             "js_constructor": js_constructor,
             "shared_context": adapter.kwargs,
             "adapter_context": context,
-            "edit_url": reverse(
-                "wagtail_fedit:edit",
-                kwargs=reverse_kwargs,
-            ),
-            "refetch_url": reverse(
-                "wagtail_fedit:refetch",
-                kwargs=reverse_kwargs,
-            ),
+            "edit_url": edit_url,
+            "refetch_url": refetch_url,
         },
         request=request if run_context_processors else None,
     )
```

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/views/adapters.py` & `wagtail_fedit-1.5.8/wagtail_fedit/views/adapters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any
+from typing import Any, TYPE_CHECKING
 from django.apps import apps
 from django.utils.translation import gettext as _
 from django.utils.decorators import method_decorator
 from django.template.loader import render_to_string
 from django.views.decorators.clickjacking import (
     xframe_options_sameorigin,
 )
@@ -20,17 +20,19 @@
     PAGE_TEMPLATE_VAR,
     Page,
 )
 from wagtail.admin.views.generic import (
     WagtailAdminTemplateMixin,
 )
 
-from ..adapters import (
-    adapter_registry,
-    BaseAdapter,
+if TYPE_CHECKING:
+    from ..adapters import BaseAdapter
+
+from ..registry import (
+    registry as adapter_registry,
     RegistryLookUpError,
 )
 from ..utils import (
     FeditPermissionCheck,
     FeditIFrameMixin,
     FEDIT_PREVIEW_VAR,
     base_adapter_context,
@@ -56,15 +58,15 @@
             model_name: str = None,
             model_id:   Any = None,
             field_name: str = None,
         ) -> None:
 
         # Fetch the adapter class from the registry
         try:
-            self.adapter_class: BaseAdapter = adapter_registry[adapter_id]
+            self.adapter_class: "BaseAdapter" = adapter_registry[adapter_id]
         except RegistryLookUpError:
             return HttpResponseBadRequest(
                 INVALID.format(
                     _("Adapter ID")
                 )
             )
 
@@ -119,15 +121,15 @@
                 self.instance,
                 field_name,
                 shared_context_str,
             )
         else:
             self.shared_context = {}
 
-        self.adapter: BaseAdapter = self.adapter_class(
+        self.adapter: "BaseAdapter" = self.adapter_class(
             request=request,
             object=self.instance,
             field_name=field_name,
             **self.shared_context,
         )
 
         if not self.adapter.check_permissions():
@@ -152,14 +154,26 @@
             adapter_id=adapter_id,
             field_name=field_name,
             app_label=app_label,
             model_name=model_name,
             model_id=model_id,
         )
     
+    @classmethod
+    def prefix_url_path(cls, name: str, *suffix: str) -> str:
+        suffix_url = ""
+        
+        if suffix:
+            suffix_url = f"{'/'.join(suffix)}"
+        
+        if suffix_url and not suffix_url.endswith("/"):
+            suffix_url += "/"
+
+        return f"{name}/<str:adapter_id>/<str:app_label>/<str:model_name>/<str:model_id>/<str:field_name>/{suffix_url}"
+    
     @property
     def template_name(self):
         return self.adapter.get_template_names()
     
     def render_to_response(self, context: dict[str, Any], success: bool = True, extra: dict = None, **response_kwargs: Any) -> HttpResponse:
         if not extra:
             extra = {}
```

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.5.8/wagtail_fedit/views/editable.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,16 +83,15 @@
             return self.error_response
 
         if not self.has_perms(request, self.object):
             return HttpResponseForbidden(NO_PERMISSION_VIEW)
 
         if issubclass(self.model, RevisionMixin) and self.object.latest_revision_id:
             instance: RevisionMixin  = self.object
-            revision: RevisionMixin = instance.latest_revision
-            self.object = revision.as_object()
+            self.object = instance.get_latest_revision_as_object()
             self.is_preview = True
         else:
             self.is_preview = False
 
         try:
             self.checks(request, self.object)
         except ValueError as e:
```

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/views/mixins.py` & `wagtail_fedit-1.5.8/wagtail_fedit/views/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/wagtail_hooks/action_menu.py` & `wagtail_fedit-1.5.8/wagtail_fedit/wagtail_hooks/action_menu.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/wagtail_hooks/adapter_hooks.py` & `wagtail_fedit-1.5.8/wagtail_fedit/wagtail_hooks/adapter_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.5.8/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files 14% similar despite different names*

```diff
@@ -79,8 +79,33 @@
             if not all([key in data for key in self.must]):
                 return self.label
 
             return _("Changed block \"%(block)s\" on field \"%(field)s\" (%(block_id)s, Frontend)") % {
                 "block": gettext(data["block_label"]),
                 "field": gettext(data["verbose_field_name"]),
                 "block_id": data["block_id"],
-            }
+            }
+        
+    @actions.register_action("wagtail_fedit.move_block")
+    class BlockMovedFormatter(LogFormatter):
+        label = _("Block Moved (Frontend)")
+        message = _("A block was moved from the frontend")
+        must = [
+            "field_name",
+            "block_label",
+            "block_id",
+            "direction",
+        ]
+
+        def format_message(self, log_entry):
+            data = log_entry.data
+
+            if not all([key in data for key in self.must]):
+                return _("Moved block on field (Frontend)")
+
+            return _("Moved block \"%(block)s\" on field \"%(field)s\" %(direction)s (%(block_id)s, Frontend)") % {
+                "block": gettext(data["block_label"]),
+                "field": gettext(data["field_name"]),
+                "direction": gettext(data["direction"]),
+                "block_id": data["block_id"],
+            }
+
```

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.5.8/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.5.8/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-fedit
-Version: 1.5.7
+Version: 1.5.8
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `wagtail_fedit-1.5.7/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.5.8/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 setup.cfg
 setup.py
 wagtail_fedit/__init__.py
 wagtail_fedit/apps.py
 wagtail_fedit/errors.py
 wagtail_fedit/hooks.py
 wagtail_fedit/models.py
+wagtail_fedit/registry.py
 wagtail_fedit/settings.py
 wagtail_fedit/toolbar.py
 wagtail_fedit/urls.py
 wagtail_fedit/utils.py
 wagtail_fedit.egg-info/PKG-INFO
 wagtail_fedit.egg-info/SOURCES.txt
 wagtail_fedit.egg-info/dependency_links.txt
@@ -21,15 +22,14 @@
 wagtail_fedit/adapters/__init__.py
 wagtail_fedit/adapters/base.py
 wagtail_fedit/adapters/block.py
 wagtail_fedit/adapters/field.py
 wagtail_fedit/adapters/funcs.py
 wagtail_fedit/adapters/misc.py
 wagtail_fedit/adapters/models.py
-wagtail_fedit/adapters/registry.py
 wagtail_fedit/forms/__init__.py
 wagtail_fedit/forms/blocks.py
 wagtail_fedit/forms/fields.py
 wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
 wagtail_fedit/locale/nl/LC_MESSAGES/django.po
 wagtail_fedit/migrations/__init__.py
 wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
@@ -39,14 +39,16 @@
 wagtail_fedit/static/wagtail_fedit/js/edit.js
 wagtail_fedit/static/wagtail_fedit/js/licenses/TIPPY.LICENSE
 wagtail_fedit/templates/wagtail_fedit/_hook_output.html
 wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
 wagtail_fedit/templates/wagtail_fedit/content/editable_dom_positioned_adapter.html
 wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
 wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
+wagtail_fedit/templates/wagtail_fedit/content/buttons/move_down.html
+wagtail_fedit/templates/wagtail_fedit/content/buttons/move_up.html
 wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
 wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
 wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler.html
 wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler_form.html
 wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
 wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
 wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
@@ -93,12 +95,11 @@
 wagtail_fedit/views/__init__.py
 wagtail_fedit/views/adapters.py
 wagtail_fedit/views/editable.py
 wagtail_fedit/views/mixins.py
 wagtail_fedit/wagtail_hooks/__init__.py
 wagtail_fedit/wagtail_hooks/action_menu.py
 wagtail_fedit/wagtail_hooks/adapter_hooks.py
-wagtail_fedit/wagtail_hooks/adapter_registry.py
+wagtail_fedit/wagtail_hooks/adapters.py
 wagtail_fedit/wagtail_hooks/icons.py
 wagtail_fedit/wagtail_hooks/log_actions.py
-wagtail_fedit/wagtail_hooks/urls.py
 wagtail_fedit/wagtail_hooks/userbar.py
```

