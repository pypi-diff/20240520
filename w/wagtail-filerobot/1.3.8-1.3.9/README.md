# Comparing `tmp/wagtail-filerobot-1.3.8.tar.gz` & `tmp/wagtail_filerobot-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-filerobot-1.3.8.tar", last modified: Tue Mar 19 22:35:57 2024, max compression
+gzip compressed data, was "wagtail_filerobot-1.3.9.tar", last modified: Mon May 20 09:53:16 2024, max compression
```

## Comparing `wagtail-filerobot-1.3.8.tar` & `wagtail_filerobot-1.3.9.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 22:35:57.386622 wagtail-filerobot-1.3.8/
--rw-rw-rw-   0        0        0    18429 2024-03-13 17:17:38.000000 wagtail-filerobot-1.3.8/LICENSE
--rw-rw-rw-   0        0        0      237 2024-03-13 17:20:48.000000 wagtail-filerobot-1.3.8/MANIFEST.in
--rw-rw-rw-   0        0        0     8816 2024-03-19 22:35:57.386622 wagtail-filerobot-1.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     7637 2024-03-19 22:35:21.000000 wagtail-filerobot-1.3.8/README.md
-drwxrwxrwx   0        0        0        0 2024-03-19 22:35:57.339547 wagtail-filerobot-1.3.8/filerobot/
--rw-rw-rw-   0        0        0      553 2024-03-19 22:35:54.000000 wagtail-filerobot-1.3.8/filerobot/__init__.py
--rw-rw-rw-   0        0        0       66 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/admin.py
--rw-rw-rw-   0        0        0      213 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/apps.py
--rw-rw-rw-   0        0        0     2991 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/blocks.py
--rw-rw-rw-   0        0        0     1244 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/constants.py
--rw-rw-rw-   0        0        0     8816 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/fields.py
--rw-rw-rw-   0        0        0     1414 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/forms.py
-drwxrwxrwx   0        0        0        0 2024-03-19 22:35:57.306752 wagtail-filerobot-1.3.8/filerobot/locale/
-drwxrwxrwx   0        0        0        0 2024-03-19 22:35:57.312803 wagtail-filerobot-1.3.8/filerobot/locale/nl/
-drwxrwxrwx   0        0        0        0 2024-03-19 22:35:57.339547 wagtail-filerobot-1.3.8/filerobot/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     6165 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    11417 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/locale/nl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-03-19 22:35:57.339547 wagtail-filerobot-1.3.8/filerobot/migrations/
--rw-rw-rw-   0        0        0     1002 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      438 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/migrations/0002_alter_designstate_options.py
--rw-rw-rw-   0        0        0        0 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 22:35:57.339547 wagtail-filerobot-1.3.8/filerobot/migrations/__pycache__/
--rw-rw-rw-   0        0        0     1628 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/migrations/__pycache__/0001_initial.cpython-311.pyc
--rw-rw-rw-   0        0        0      863 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/migrations/__pycache__/0002_alter_designstate_options.cpython-311.pyc
--rw-rw-rw-   0        0        0      228 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     1353 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/models.py
--rw-rw-rw-   0        0        0     1493 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/signals.py
-drwxrwxrwx   0        0        0        0 2024-03-19 22:35:57.312803 wagtail-filerobot-1.3.8/filerobot/static/
-drwxrwxrwx   0        0        0        0 2024-03-19 22:35:57.314474 wagtail-filerobot-1.3.8/filerobot/static/filerobot/
-drwxrwxrwx   0        0        0        0 2024-03-19 22:35:57.339547 wagtail-filerobot-1.3.8/filerobot/static/filerobot/css/
--rw-rw-rw-   0        0        0      141 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/static/filerobot/css/filerobot.css
--rw-rw-rw-   0        0        0     8475 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/static/filerobot/css/filerobot_widget.css
-drwxrwxrwx   0        0        0        0 2024-03-19 22:35:57.339547 wagtail-filerobot-1.3.8/filerobot/static/filerobot/js/
--rw-rw-rw-   0        0        0     1066 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/static/filerobot/js/LICENSE.txt
--rw-rw-rw-   0        0        0    73481 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/static/filerobot/js/README.md
--rw-rw-rw-   0        0        0    13213 2024-03-19 22:22:39.000000 wagtail-filerobot-1.3.8/filerobot/static/filerobot/js/file_robot_widget.js
--rw-rw-rw-   0        0        0     3108 2024-03-19 22:22:32.000000 wagtail-filerobot-1.3.8/filerobot/static/filerobot/js/file_robot_widget_controller.js
--rw-rw-rw-   0        0        0   905179 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/static/filerobot/js/filerobot.js
-drwxrwxrwx   0        0        0        0 2024-03-19 22:35:57.314474 wagtail-filerobot-1.3.8/filerobot/templates/
-drwxrwxrwx   0        0        0        0 2024-03-19 22:35:57.314474 wagtail-filerobot-1.3.8/filerobot/templates/filerobot/
-drwxrwxrwx   0        0        0        0 2024-03-19 22:35:57.339547 wagtail-filerobot-1.3.8/filerobot/templates/filerobot/blocks/
--rw-rw-rw-   0        0        0      219 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/templates/filerobot/blocks/filerobot.html
-drwxrwxrwx   0        0        0        0 2024-03-19 22:35:57.339547 wagtail-filerobot-1.3.8/filerobot/templates/filerobot/widgets/
--rw-rw-rw-   0        0        0      744 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/templates/filerobot/widgets/file_robot_widget.html
-drwxrwxrwx   0        0        0        0 2024-03-19 22:35:57.354563 wagtail-filerobot-1.3.8/filerobot/templatetags/
-drwxrwxrwx   0        0        0        0 2024-03-19 22:35:57.354563 wagtail-filerobot-1.3.8/filerobot/templatetags/__pycache__/
--rw-rw-rw-   0        0        0     6602 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/templatetags/__pycache__/filerobot.cpython-311.pyc
--rw-rw-rw-   0        0        0     5513 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/templatetags/filerobot.py
--rw-rw-rw-   0        0        0       63 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/tests.py
-drwxrwxrwx   0        0        0        0 2024-03-19 22:35:57.354563 wagtail-filerobot-1.3.8/filerobot/utils/
--rw-rw-rw-   0        0        0       79 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/utils/__init__.py
--rw-rw-rw-   0        0        0     4642 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/utils/casing.py
--rw-rw-rw-   0        0        0      579 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/utils/dictionary.py
--rw-rw-rw-   0        0        0     4008 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/value.py
-drwxrwxrwx   0        0        0        0 2024-03-19 22:35:57.354563 wagtail-filerobot-1.3.8/filerobot/views/
--rw-rw-rw-   0        0        0       40 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/views/__init__.py
--rw-rw-rw-   0        0        0     3800 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/views/image_chooser.py
--rw-rw-rw-   0        0        0     2635 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/views/utils.py
--rw-rw-rw-   0        0        0     6290 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/views/widget.py
--rw-rw-rw-   0        0        0     4788 2024-03-19 22:25:58.000000 wagtail-filerobot-1.3.8/filerobot/wagtail_hooks.py
-drwxrwxrwx   0        0        0        0 2024-03-19 22:35:57.354563 wagtail-filerobot-1.3.8/filerobot/widgets/
--rw-rw-rw-   0        0        0       71 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/widgets/__init__.py
--rw-rw-rw-   0        0        0     9980 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/widgets/filerobot.py
--rw-rw-rw-   0        0        0     7312 2024-03-19 22:19:18.000000 wagtail-filerobot-1.3.8/filerobot/widgets/obj.py
--rw-rw-rw-   0        0        0       90 2024-03-13 17:17:38.000000 wagtail-filerobot-1.3.8/pyproject.toml
--rw-rw-rw-   0        0        0     1132 2024-03-19 22:35:57.389049 wagtail-filerobot-1.3.8/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-03-13 17:17:38.000000 wagtail-filerobot-1.3.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-19 22:35:57.354563 wagtail-filerobot-1.3.8/tests/
--rw-rw-rw-   0        0        0        0 2024-03-13 17:17:38.000000 wagtail-filerobot-1.3.8/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 22:35:57.354563 wagtail-filerobot-1.3.8/tests/testapp/
--rw-rw-rw-   0        0        0        0 2024-03-13 17:17:38.000000 wagtail-filerobot-1.3.8/tests/testapp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 22:35:57.354563 wagtail-filerobot-1.3.8/tests/testapp/core/
--rw-rw-rw-   0        0        0        0 2024-03-13 17:17:38.000000 wagtail-filerobot-1.3.8/tests/testapp/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 22:35:57.354563 wagtail-filerobot-1.3.8/tests/testapp/core/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-13 17:17:38.000000 wagtail-filerobot-1.3.8/tests/testapp/core/migrations/__init__.py
--rw-rw-rw-   0        0        0      151 2024-03-13 17:17:38.000000 wagtail-filerobot-1.3.8/tests/testapp/core/tests.py
--rw-rw-rw-   0        0        0      685 2024-03-13 17:17:38.000000 wagtail-filerobot-1.3.8/tests/testapp/manage.py
-drwxrwxrwx   0        0        0        0 2024-03-19 22:35:57.354563 wagtail-filerobot-1.3.8/tests/testapp/testapp/
--rw-rw-rw-   0        0        0        0 2024-03-13 17:17:38.000000 wagtail-filerobot-1.3.8/tests/testapp/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-03-13 17:17:38.000000 wagtail-filerobot-1.3.8/tests/testapp/testapp/asgi.py
--rw-rw-rw-   0        0        0     3521 2024-03-13 17:17:38.000000 wagtail-filerobot-1.3.8/tests/testapp/testapp/settings.py
--rw-rw-rw-   0        0        0      785 2024-03-13 17:17:38.000000 wagtail-filerobot-1.3.8/tests/testapp/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-03-13 17:17:38.000000 wagtail-filerobot-1.3.8/tests/testapp/testapp/wsgi.py
-drwxrwxrwx   0        0        0        0 2024-03-19 22:35:57.386622 wagtail-filerobot-1.3.8/wagtail_filerobot.egg-info/
--rw-rw-rw-   0        0        0     8816 2024-03-19 22:35:57.000000 wagtail-filerobot-1.3.8/wagtail_filerobot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2077 2024-03-19 22:35:57.000000 wagtail-filerobot-1.3.8/wagtail_filerobot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 22:35:57.000000 wagtail-filerobot-1.3.8/wagtail_filerobot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-03-19 22:35:57.000000 wagtail-filerobot-1.3.8/wagtail_filerobot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-03-19 22:35:57.000000 wagtail-filerobot-1.3.8/wagtail_filerobot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 09:53:16.804514 wagtail_filerobot-1.3.9/
+-rw-rw-rw-   0        0        0    18429 2024-03-13 17:17:38.000000 wagtail_filerobot-1.3.9/LICENSE
+-rw-rw-rw-   0        0        0      237 2024-03-13 17:20:48.000000 wagtail_filerobot-1.3.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     8816 2024-05-20 09:53:16.803513 wagtail_filerobot-1.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     7637 2024-03-19 22:35:21.000000 wagtail_filerobot-1.3.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 09:53:16.746159 wagtail_filerobot-1.3.9/filerobot/
+-rw-rw-rw-   0        0        0      553 2024-03-19 22:35:54.000000 wagtail_filerobot-1.3.9/filerobot/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-03-19 22:19:18.000000 wagtail_filerobot-1.3.9/filerobot/admin.py
+-rw-rw-rw-   0        0        0      213 2024-03-19 22:19:18.000000 wagtail_filerobot-1.3.9/filerobot/apps.py
+-rw-rw-rw-   0        0        0     2991 2024-03-19 22:19:18.000000 wagtail_filerobot-1.3.9/filerobot/blocks.py
+-rw-rw-rw-   0        0        0     1244 2024-03-19 22:19:18.000000 wagtail_filerobot-1.3.9/filerobot/constants.py
+-rw-rw-rw-   0        0        0     8816 2024-03-19 22:19:18.000000 wagtail_filerobot-1.3.9/filerobot/fields.py
+-rw-rw-rw-   0        0        0     1414 2024-03-19 22:19:18.000000 wagtail_filerobot-1.3.9/filerobot/forms.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:53:16.715640 wagtail_filerobot-1.3.9/filerobot/locale/
+drwxrwxrwx   0        0        0        0 2024-05-20 09:53:16.716604 wagtail_filerobot-1.3.9/filerobot/locale/nl/
+drwxrwxrwx   0        0        0        0 2024-05-20 09:53:16.748788 wagtail_filerobot-1.3.9/filerobot/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     6165 2024-03-19 22:19:18.000000 wagtail_filerobot-1.3.9/filerobot/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    11417 2024-03-19 22:19:18.000000 wagtail_filerobot-1.3.9/filerobot/locale/nl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-05-20 09:53:16.752452 wagtail_filerobot-1.3.9/filerobot/migrations/
+-rw-rw-rw-   0        0        0     1002 2024-03-19 22:19:18.000000 wagtail_filerobot-1.3.9/filerobot/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      438 2024-03-19 22:19:18.000000 wagtail_filerobot-1.3.9/filerobot/migrations/0002_alter_designstate_options.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 22:19:18.000000 wagtail_filerobot-1.3.9/filerobot/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:53:16.757516 wagtail_filerobot-1.3.9/filerobot/migrations/__pycache__/
+-rw-rw-rw-   0        0        0     1628 2024-03-19 22:19:18.000000 wagtail_filerobot-1.3.9/filerobot/migrations/__pycache__/0001_initial.cpython-311.pyc
+-rw-rw-rw-   0        0        0      863 2024-03-19 22:19:18.000000 wagtail_filerobot-1.3.9/filerobot/migrations/__pycache__/0002_alter_designstate_options.cpython-311.pyc
+-rw-rw-rw-   0        0        0      228 2024-03-19 22:19:18.000000 wagtail_filerobot-1.3.9/filerobot/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1353 2024-03-19 22:19:18.000000 wagtail_filerobot-1.3.9/filerobot/models.py
+-rw-rw-rw-   0        0        0     1493 2024-03-19 22:19:18.000000 wagtail_filerobot-1.3.9/filerobot/signals.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:53:16.717610 wagtail_filerobot-1.3.9/filerobot/static/
+drwxrwxrwx   0        0        0        0 2024-05-20 09:53:16.718610 wagtail_filerobot-1.3.9/filerobot/static/filerobot/
+drwxrwxrwx   0        0        0        0 2024-05-20 09:53:16.757516 wagtail_filerobot-1.3.9/filerobot/static/filerobot/css/
+-rw-rw-rw-   0        0        0      147 2024-03-31 15:57:18.000000 wagtail_filerobot-1.3.9/filerobot/static/filerobot/css/filerobot.css
+-rw-rw-rw-   0        0        0     8475 2024-03-19 22:19:18.000000 wagtail_filerobot-1.3.9/filerobot/static/filerobot/css/filerobot_widget.css
+drwxrwxrwx   0        0        0        0 2024-05-20 09:53:16.763888 wagtail_filerobot-1.3.9/filerobot/static/filerobot/js/
+-rw-rw-rw-   0        0        0     1066 2024-03-19 22:19:18.000000 wagtail_filerobot-1.3.9/filerobot/static/filerobot/js/LICENSE.txt
+-rw-rw-rw-   0        0        0    73481 2024-03-19 22:19:18.000000 wagtail_filerobot-1.3.9/filerobot/static/filerobot/js/README.md
+-rw-rw-rw-   0        0        0    13213 2024-03-19 22:22:39.000000 wagtail_filerobot-1.3.9/filerobot/static/filerobot/js/file_robot_widget.js
+-rw-rw-rw-   0        0        0     3108 2024-03-19 22:22:32.000000 wagtail_filerobot-1.3.9/filerobot/static/filerobot/js/file_robot_widget_controller.js
+-rw-rw-rw-   0        0        0   905179 2024-03-19 22:19:18.000000 wagtail_filerobot-1.3.9/filerobot/static/filerobot/js/filerobot.js
+drwxrwxrwx   0        0        0        0 2024-05-20 09:53:16.719718 wagtail_filerobot-1.3.9/filerobot/templates/
+drwxrwxrwx   0        0        0        0 2024-05-20 09:53:16.720720 wagtail_filerobot-1.3.9/filerobot/templates/filerobot/
+drwxrwxrwx   0        0        0        0 2024-05-20 09:53:16.765887 wagtail_filerobot-1.3.9/filerobot/templates/filerobot/blocks/
+-rw-rw-rw-   0        0        0      219 2024-03-19 22:19:18.000000 wagtail_filerobot-1.3.9/filerobot/templates/filerobot/blocks/filerobot.html
+drwxrwxrwx   0        0        0        0 2024-05-20 09:53:16.767887 wagtail_filerobot-1.3.9/filerobot/templates/filerobot/widgets/
+-rw-rw-rw-   0        0        0      744 2024-03-19 22:19:18.000000 wagtail_filerobot-1.3.9/filerobot/templates/filerobot/widgets/file_robot_widget.html
+drwxrwxrwx   0        0        0        0 2024-05-20 09:53:16.769746 wagtail_filerobot-1.3.9/filerobot/templatetags/
+drwxrwxrwx   0        0        0        0 2024-05-20 09:53:16.771182 wagtail_filerobot-1.3.9/filerobot/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0     6602 2024-03-19 22:19:18.000000 wagtail_filerobot-1.3.9/filerobot/templatetags/__pycache__/filerobot.cpython-311.pyc
+-rw-rw-rw-   0        0        0     5513 2024-03-19 22:19:18.000000 wagtail_filerobot-1.3.9/filerobot/templatetags/filerobot.py
+-rw-rw-rw-   0        0        0       63 2024-03-19 22:19:18.000000 wagtail_filerobot-1.3.9/filerobot/tests.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:53:16.772995 wagtail_filerobot-1.3.9/filerobot/utils/
+-rw-rw-rw-   0        0        0       79 2024-03-19 22:19:18.000000 wagtail_filerobot-1.3.9/filerobot/utils/__init__.py
+-rw-rw-rw-   0        0        0     4642 2024-03-19 22:19:18.000000 wagtail_filerobot-1.3.9/filerobot/utils/casing.py
+-rw-rw-rw-   0        0        0      579 2024-03-19 22:19:18.000000 wagtail_filerobot-1.3.9/filerobot/utils/dictionary.py
+-rw-rw-rw-   0        0        0     4073 2024-05-20 09:50:39.000000 wagtail_filerobot-1.3.9/filerobot/value.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:53:16.772995 wagtail_filerobot-1.3.9/filerobot/views/
+-rw-rw-rw-   0        0        0       40 2024-03-19 22:19:18.000000 wagtail_filerobot-1.3.9/filerobot/views/__init__.py
+-rw-rw-rw-   0        0        0     3800 2024-03-19 22:19:18.000000 wagtail_filerobot-1.3.9/filerobot/views/image_chooser.py
+-rw-rw-rw-   0        0        0     2635 2024-03-19 22:19:18.000000 wagtail_filerobot-1.3.9/filerobot/views/utils.py
+-rw-rw-rw-   0        0        0     6290 2024-03-19 22:19:18.000000 wagtail_filerobot-1.3.9/filerobot/views/widget.py
+-rw-rw-rw-   0        0        0     4788 2024-03-19 22:25:58.000000 wagtail_filerobot-1.3.9/filerobot/wagtail_hooks.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:53:16.782013 wagtail_filerobot-1.3.9/filerobot/widgets/
+-rw-rw-rw-   0        0        0       71 2024-03-19 22:19:18.000000 wagtail_filerobot-1.3.9/filerobot/widgets/__init__.py
+-rw-rw-rw-   0        0        0     9980 2024-03-19 22:19:18.000000 wagtail_filerobot-1.3.9/filerobot/widgets/filerobot.py
+-rw-rw-rw-   0        0        0     7312 2024-03-19 22:19:18.000000 wagtail_filerobot-1.3.9/filerobot/widgets/obj.py
+-rw-rw-rw-   0        0        0       90 2024-03-13 17:17:38.000000 wagtail_filerobot-1.3.9/pyproject.toml
+-rw-rw-rw-   0        0        0     1132 2024-05-20 09:53:16.805513 wagtail_filerobot-1.3.9/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-03-13 17:17:38.000000 wagtail_filerobot-1.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:53:16.783014 wagtail_filerobot-1.3.9/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-13 17:17:38.000000 wagtail_filerobot-1.3.9/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:53:16.785220 wagtail_filerobot-1.3.9/tests/testapp/
+-rw-rw-rw-   0        0        0        0 2024-03-13 17:17:38.000000 wagtail_filerobot-1.3.9/tests/testapp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:53:16.787380 wagtail_filerobot-1.3.9/tests/testapp/core/
+-rw-rw-rw-   0        0        0        0 2024-03-13 17:17:38.000000 wagtail_filerobot-1.3.9/tests/testapp/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:53:16.789757 wagtail_filerobot-1.3.9/tests/testapp/core/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-13 17:17:38.000000 wagtail_filerobot-1.3.9/tests/testapp/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0      151 2024-03-13 17:17:38.000000 wagtail_filerobot-1.3.9/tests/testapp/core/tests.py
+-rw-rw-rw-   0        0        0      685 2024-03-13 17:17:38.000000 wagtail_filerobot-1.3.9/tests/testapp/manage.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:53:16.795305 wagtail_filerobot-1.3.9/tests/testapp/testapp/
+-rw-rw-rw-   0        0        0        0 2024-03-13 17:17:38.000000 wagtail_filerobot-1.3.9/tests/testapp/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-03-13 17:17:38.000000 wagtail_filerobot-1.3.9/tests/testapp/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3521 2024-03-13 17:17:38.000000 wagtail_filerobot-1.3.9/tests/testapp/testapp/settings.py
+-rw-rw-rw-   0        0        0      785 2024-03-13 17:17:38.000000 wagtail_filerobot-1.3.9/tests/testapp/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-03-13 17:17:38.000000 wagtail_filerobot-1.3.9/tests/testapp/testapp/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:53:16.802505 wagtail_filerobot-1.3.9/wagtail_filerobot.egg-info/
+-rw-rw-rw-   0        0        0     8816 2024-05-20 09:53:16.000000 wagtail_filerobot-1.3.9/wagtail_filerobot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2077 2024-05-20 09:53:16.000000 wagtail_filerobot-1.3.9/wagtail_filerobot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 09:53:16.000000 wagtail_filerobot-1.3.9/wagtail_filerobot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-20 09:53:16.000000 wagtail_filerobot-1.3.9/wagtail_filerobot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-20 09:53:16.000000 wagtail_filerobot-1.3.9/wagtail_filerobot.egg-info/top_level.txt
```

### Comparing `wagtail-filerobot-1.3.8/LICENSE` & `wagtail_filerobot-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-filerobot-1.3.8/PKG-INFO` & `wagtail_filerobot-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-filerobot
-Version: 1.3.8
+Version: 1.3.9
 Summary: A filerobot image editing widget for Wagtail Image fields.
 Home-page: https://github.com/Nigel2392/wagtail-filerobot
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `wagtail-filerobot-1.3.8/README.md` & `wagtail_filerobot-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-filerobot-1.3.8/filerobot/__init__.py` & `wagtail_filerobot-1.3.9/filerobot/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtail-filerobot-1.3.8/filerobot/blocks.py` & `wagtail_filerobot-1.3.9/filerobot/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-filerobot-1.3.8/filerobot/constants.py` & `wagtail_filerobot-1.3.9/filerobot/constants.py`

 * *Files identical despite different names*

### Comparing `wagtail-filerobot-1.3.8/filerobot/fields.py` & `wagtail_filerobot-1.3.9/filerobot/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail-filerobot-1.3.8/filerobot/forms.py` & `wagtail_filerobot-1.3.9/filerobot/forms.py`

 * *Files identical despite different names*

### Comparing `wagtail-filerobot-1.3.8/filerobot/locale/nl/LC_MESSAGES/django.mo` & `wagtail_filerobot-1.3.9/filerobot/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail-filerobot-1.3.8/filerobot/locale/nl/LC_MESSAGES/django.po` & `wagtail_filerobot-1.3.9/filerobot/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail-filerobot-1.3.8/filerobot/migrations/0001_initial.py` & `wagtail_filerobot-1.3.9/filerobot/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-filerobot-1.3.8/filerobot/migrations/__pycache__/0001_initial.cpython-311.pyc` & `wagtail_filerobot-1.3.9/filerobot/migrations/__pycache__/0001_initial.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail-filerobot-1.3.8/filerobot/migrations/__pycache__/0002_alter_designstate_options.cpython-311.pyc` & `wagtail_filerobot-1.3.9/filerobot/migrations/__pycache__/0002_alter_designstate_options.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail-filerobot-1.3.8/filerobot/models.py` & `wagtail_filerobot-1.3.9/filerobot/models.py`

 * *Files identical despite different names*

### Comparing `wagtail-filerobot-1.3.8/filerobot/signals.py` & `wagtail_filerobot-1.3.9/filerobot/signals.py`

 * *Files identical despite different names*

### Comparing `wagtail-filerobot-1.3.8/filerobot/static/filerobot/css/filerobot_widget.css` & `wagtail_filerobot-1.3.9/filerobot/static/filerobot/css/filerobot_widget.css`

 * *Files identical despite different names*

### Comparing `wagtail-filerobot-1.3.8/filerobot/static/filerobot/js/LICENSE.txt` & `wagtail_filerobot-1.3.9/filerobot/static/filerobot/js/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wagtail-filerobot-1.3.8/filerobot/static/filerobot/js/README.md` & `wagtail_filerobot-1.3.9/filerobot/static/filerobot/js/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-filerobot-1.3.8/filerobot/static/filerobot/js/file_robot_widget.js` & `wagtail_filerobot-1.3.9/filerobot/static/filerobot/js/file_robot_widget.js`

 * *Files identical despite different names*

### Comparing `wagtail-filerobot-1.3.8/filerobot/static/filerobot/js/file_robot_widget_controller.js` & `wagtail_filerobot-1.3.9/filerobot/static/filerobot/js/file_robot_widget_controller.js`

 * *Files identical despite different names*

### Comparing `wagtail-filerobot-1.3.8/filerobot/static/filerobot/js/filerobot.js` & `wagtail_filerobot-1.3.9/filerobot/static/filerobot/js/filerobot.js`

 * *Files identical despite different names*

### Comparing `wagtail-filerobot-1.3.8/filerobot/templates/filerobot/widgets/file_robot_widget.html` & `wagtail_filerobot-1.3.9/filerobot/templates/filerobot/widgets/file_robot_widget.html`

 * *Files identical despite different names*

### Comparing `wagtail-filerobot-1.3.8/filerobot/templatetags/__pycache__/filerobot.cpython-311.pyc` & `wagtail_filerobot-1.3.9/filerobot/templatetags/__pycache__/filerobot.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail-filerobot-1.3.8/filerobot/templatetags/filerobot.py` & `wagtail_filerobot-1.3.9/filerobot/templatetags/filerobot.py`

 * *Files identical despite different names*

### Comparing `wagtail-filerobot-1.3.8/filerobot/utils/casing.py` & `wagtail_filerobot-1.3.9/filerobot/utils/casing.py`

 * *Files identical despite different names*

### Comparing `wagtail-filerobot-1.3.8/filerobot/utils/dictionary.py` & `wagtail_filerobot-1.3.9/filerobot/utils/dictionary.py`

 * *Files identical despite different names*

### Comparing `wagtail-filerobot-1.3.8/filerobot/value.py` & `wagtail_filerobot-1.3.9/filerobot/value.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,17 @@
             
     def __str__(self):
         return str(self.image)
 
     def __bool__(self):
         return bool(self.image)
     
+    def __int__(self):
+        return int(self.image.pk)
+    
     def __getattr__(self, name):
         """
             Proxy all attribute access to the image object,
             except for the ones required by the block.
         """
         if name in self.__noproxy_fields__:
             return object.__getattribute__(self, name)
```

### Comparing `wagtail-filerobot-1.3.8/filerobot/views/image_chooser.py` & `wagtail_filerobot-1.3.9/filerobot/views/image_chooser.py`

 * *Files identical despite different names*

### Comparing `wagtail-filerobot-1.3.8/filerobot/views/utils.py` & `wagtail_filerobot-1.3.9/filerobot/views/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail-filerobot-1.3.8/filerobot/views/widget.py` & `wagtail_filerobot-1.3.9/filerobot/views/widget.py`

 * *Files identical despite different names*

### Comparing `wagtail-filerobot-1.3.8/filerobot/wagtail_hooks.py` & `wagtail_filerobot-1.3.9/filerobot/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail-filerobot-1.3.8/filerobot/widgets/filerobot.py` & `wagtail_filerobot-1.3.9/filerobot/widgets/filerobot.py`

 * *Files identical despite different names*

### Comparing `wagtail-filerobot-1.3.8/filerobot/widgets/obj.py` & `wagtail_filerobot-1.3.9/filerobot/widgets/obj.py`

 * *Files identical despite different names*

### Comparing `wagtail-filerobot-1.3.8/setup.cfg` & `wagtail_filerobot-1.3.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 2d66 696c 6572   = wagtail-filer
 00000020: 6f62 6f74 0d0a 7665 7273 696f 6e20 3d20  obot..version = 
-00000030: 312e 332e 380d 0a64 6573 6372 6970 7469  1.3.8..descripti
+00000030: 312e 332e 390d 0a64 6573 6372 6970 7469  1.3.9..descripti
 00000040: 6f6e 203d 2041 2066 696c 6572 6f62 6f74  on = A filerobot
 00000050: 2069 6d61 6765 2065 6469 7469 6e67 2077   image editing w
 00000060: 6964 6765 7420 666f 7220 5761 6774 6169  idget for Wagtai
 00000070: 6c20 496d 6167 6520 6669 656c 6473 2e0d  l Image fields..
 00000080: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
 00000090: 6e20 3d20 6669 6c65 3a20 5245 4144 4d45  n = file: README
 000000a0: 2e6d 640d 0a6c 6f6e 675f 6465 7363 7269  .md..long_descri
```

### Comparing `wagtail-filerobot-1.3.8/tests/testapp/manage.py` & `wagtail_filerobot-1.3.9/tests/testapp/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail-filerobot-1.3.8/tests/testapp/testapp/settings.py` & `wagtail_filerobot-1.3.9/tests/testapp/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail-filerobot-1.3.8/tests/testapp/testapp/urls.py` & `wagtail_filerobot-1.3.9/tests/testapp/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail-filerobot-1.3.8/wagtail_filerobot.egg-info/PKG-INFO` & `wagtail_filerobot-1.3.9/wagtail_filerobot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-filerobot
-Version: 1.3.8
+Version: 1.3.9
 Summary: A filerobot image editing widget for Wagtail Image fields.
 Home-page: https://github.com/Nigel2392/wagtail-filerobot
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `wagtail-filerobot-1.3.8/wagtail_filerobot.egg-info/SOURCES.txt` & `wagtail_filerobot-1.3.9/wagtail_filerobot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

