# Comparing `tmp/aa_ledger-0.3.6.tar.gz` & `tmp/aa_ledger-0.3.7.tar.gz`

## Comparing `aa_ledger-0.3.6.tar` & `aa_ledger-0.3.7.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/__init__.py
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/admin.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/app_settings.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/apps.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/auth_hooks.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/decorators.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/errors.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/hooks.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/providers.py
--rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/tasks.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/urls.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/api/__init__.py
--rw-r--r--   0        0        0     7185 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/api/helpers.py
--rw-r--r--   0        0        0    21348 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/api/ledgermanager.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/api/schema.py
--rw-r--r--   0        0        0    16190 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/api/templatemanager.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/api/character/__init__.py
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/api/character/ledger.py
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/api/character/template.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/api/corporation/__init__.py
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/api/corporation/ledger.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/api/corporation/template.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/managers/charaudit_manager.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/managers/corpaudit_manager.py
--rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/managers/general_manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/migrations/__init__.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/models/__init__.py
--rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/models/characteraudit.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/models/corporationaudit.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/models/events.py
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/models/general.py
--rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/static/ledger/css/billboards_dark.css
--rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/static/ledger/css/cards.css
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/static/ledger/css/custom.css
--rw-r--r--   0        0        0   236145 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/static/ledger/guides/ledger-1.png
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/static/ledger/guides/ledger-2.png
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/static/ledger/guides/ledger-3.png
--rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/static/ledger/images/Spinner-1s-64px-dark.gif
--rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/static/ledger/images/Spinner-1s-64px-light.gif
--rw-r--r--   0        0        0    22096 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/static/ledger/js/charledger.js
--rw-r--r--   0        0        0    18853 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/static/ledger/js/corpledger.js
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/static/ledger/js/img.js
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/task_helpers/__init__.py
--rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/task_helpers/char_helpers.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/task_helpers/core_helpers.py
--rw-r--r--   0        0        0     8398 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/task_helpers/corp_helpers.py
--rw-r--r--   0        0        0     8434 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/task_helpers/etag_helpers.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/templates/ledger/base.html
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/templates/ledger/error.html
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/templates/ledger/bundles/ledger-css.html
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/templates/ledger/ledger/base.html
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/templates/ledger/ledger/index.html
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/templates/ledger/ledger/menu.html
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/templates/ledger/ledger/charledger/char_ledger.html
--rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/templates/ledger/ledger/charledger/month.html
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/templates/ledger/ledger/charledger/year.html
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/templates/ledger/ledger/corpledger/corp_ledger.html
--rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/templates/ledger/ledger/corpledger/month.html
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/templates/ledger/ledger/corpledger/year.html
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/templates/ledger/modals/modal-full.html
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/templates/ledger/modals/modal-xl.html
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/templates/ledger/modals/modal.html
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/templates/ledger/modals/modal_dialog.html
--rw-r--r--   0        0        0    17674 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/templates/ledger/modals/pve/view_character_content.html
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/view_helpers/__init__.py
--rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/view_helpers/core.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/views/__init__.py
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/views/pve.py
--rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/views/character/char_audit.py
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/views/corporation/corp_audit.py
--rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/views/corporation/corp_events.py
--rw-r--r--   0        0        0     8919 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/ledger/views/corporation/corp_tax.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/LICENSE
--rw-r--r--   0        0        0     5523 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/README.md
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     8278 2020-02-02 00:00:00.000000 aa_ledger-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/__init__.py
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/admin.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/app_settings.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/apps.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/auth_hooks.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/decorators.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/errors.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/hooks.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/providers.py
+-rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/tasks.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/urls.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/api/__init__.py
+-rw-r--r--   0        0        0     7185 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/api/helpers.py
+-rw-r--r--   0        0        0    21348 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/api/ledgermanager.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/api/schema.py
+-rw-r--r--   0        0        0    16190 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/api/templatemanager.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/api/character/__init__.py
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/api/character/ledger.py
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/api/character/template.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/api/corporation/__init__.py
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/api/corporation/ledger.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/api/corporation/template.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/managers/charaudit_manager.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/managers/corpaudit_manager.py
+-rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/managers/general_manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/migrations/__init__.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/models/__init__.py
+-rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/models/characteraudit.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/models/corporationaudit.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/models/events.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/models/general.py
+-rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/static/ledger/css/billboards_dark.css
+-rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/static/ledger/css/cards.css
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/static/ledger/css/custom.css
+-rw-r--r--   0        0        0   236145 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/static/ledger/guides/ledger-1.png
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/static/ledger/guides/ledger-2.png
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/static/ledger/guides/ledger-3.png
+-rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/static/ledger/images/Spinner-1s-64px-dark.gif
+-rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/static/ledger/images/Spinner-1s-64px-light.gif
+-rw-r--r--   0        0        0    22096 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/static/ledger/js/charledger.js
+-rw-r--r--   0        0        0    18853 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/static/ledger/js/corpledger.js
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/static/ledger/js/img.js
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/task_helpers/__init__.py
+-rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/task_helpers/char_helpers.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/task_helpers/core_helpers.py
+-rw-r--r--   0        0        0     8398 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/task_helpers/corp_helpers.py
+-rw-r--r--   0        0        0     8434 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/task_helpers/etag_helpers.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/templates/ledger/base.html
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/templates/ledger/error.html
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/templates/ledger/bundles/ledger-css.html
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/templates/ledger/ledger/base.html
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/templates/ledger/ledger/index.html
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/templates/ledger/ledger/menu.html
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/templates/ledger/ledger/charledger/char_ledger.html
+-rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/templates/ledger/ledger/charledger/month.html
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/templates/ledger/ledger/charledger/year.html
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/templates/ledger/ledger/corpledger/corp_ledger.html
+-rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/templates/ledger/ledger/corpledger/month.html
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/templates/ledger/ledger/corpledger/year.html
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/templates/ledger/modals/modal-full.html
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/templates/ledger/modals/modal-xl.html
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/templates/ledger/modals/modal.html
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/templates/ledger/modals/modal_dialog.html
+-rw-r--r--   0        0        0    17674 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/templates/ledger/modals/pve/view_character_content.html
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/view_helpers/__init__.py
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/view_helpers/core.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/views/__init__.py
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/views/pve.py
+-rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/views/character/char_audit.py
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/views/corporation/corp_audit.py
+-rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/views/corporation/corp_events.py
+-rw-r--r--   0        0        0     8919 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/ledger/views/corporation/corp_tax.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/LICENSE
+-rw-r--r--   0        0        0     5523 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/README.md
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     8312 2020-02-02 00:00:00.000000 aa_ledger-0.3.7/PKG-INFO
```

### Comparing `aa_ledger-0.3.6/ledger/admin.py` & `aa_ledger-0.3.7/ledger/admin.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/app_settings.py` & `aa_ledger-0.3.7/ledger/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/auth_hooks.py` & `aa_ledger-0.3.7/ledger/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/decorators.py` & `aa_ledger-0.3.7/ledger/decorators.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/hooks.py` & `aa_ledger-0.3.7/ledger/hooks.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/tasks.py` & `aa_ledger-0.3.7/ledger/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/urls.py` & `aa_ledger-0.3.7/ledger/urls.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/api/__init__.py` & `aa_ledger-0.3.7/ledger/api/__init__.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/api/helpers.py` & `aa_ledger-0.3.7/ledger/api/helpers.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/api/ledgermanager.py` & `aa_ledger-0.3.7/ledger/api/ledgermanager.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/api/schema.py` & `aa_ledger-0.3.7/ledger/api/schema.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/api/templatemanager.py` & `aa_ledger-0.3.7/ledger/api/templatemanager.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/api/character/ledger.py` & `aa_ledger-0.3.7/ledger/api/character/ledger.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/api/character/template.py` & `aa_ledger-0.3.7/ledger/api/character/template.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/api/corporation/ledger.py` & `aa_ledger-0.3.7/ledger/api/corporation/ledger.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/api/corporation/template.py` & `aa_ledger-0.3.7/ledger/api/corporation/template.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/managers/charaudit_manager.py` & `aa_ledger-0.3.7/ledger/managers/charaudit_manager.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/managers/corpaudit_manager.py` & `aa_ledger-0.3.7/ledger/managers/corpaudit_manager.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/managers/general_manager.py` & `aa_ledger-0.3.7/ledger/managers/general_manager.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/models/characteraudit.py` & `aa_ledger-0.3.7/ledger/models/characteraudit.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/models/corporationaudit.py` & `aa_ledger-0.3.7/ledger/models/corporationaudit.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/models/events.py` & `aa_ledger-0.3.7/ledger/models/events.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/models/general.py` & `aa_ledger-0.3.7/ledger/models/general.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/static/ledger/css/billboards_dark.css` & `aa_ledger-0.3.7/ledger/static/ledger/css/billboards_dark.css`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/static/ledger/css/cards.css` & `aa_ledger-0.3.7/ledger/static/ledger/css/cards.css`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/static/ledger/css/custom.css` & `aa_ledger-0.3.7/ledger/static/ledger/css/custom.css`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/static/ledger/guides/ledger-1.png` & `aa_ledger-0.3.7/ledger/static/ledger/guides/ledger-1.png`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/static/ledger/guides/ledger-2.png` & `aa_ledger-0.3.7/ledger/static/ledger/guides/ledger-2.png`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/static/ledger/guides/ledger-3.png` & `aa_ledger-0.3.7/ledger/static/ledger/guides/ledger-3.png`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/static/ledger/images/Spinner-1s-64px-dark.gif` & `aa_ledger-0.3.7/ledger/static/ledger/images/Spinner-1s-64px-dark.gif`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/static/ledger/images/Spinner-1s-64px-light.gif` & `aa_ledger-0.3.7/ledger/static/ledger/images/Spinner-1s-64px-light.gif`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/static/ledger/js/charledger.js` & `aa_ledger-0.3.7/ledger/static/ledger/js/charledger.js`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/static/ledger/js/corpledger.js` & `aa_ledger-0.3.7/ledger/static/ledger/js/corpledger.js`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/static/ledger/js/img.js` & `aa_ledger-0.3.7/ledger/static/ledger/js/img.js`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/task_helpers/char_helpers.py` & `aa_ledger-0.3.7/ledger/task_helpers/char_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/task_helpers/core_helpers.py` & `aa_ledger-0.3.7/ledger/task_helpers/core_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/task_helpers/corp_helpers.py` & `aa_ledger-0.3.7/ledger/task_helpers/corp_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/task_helpers/etag_helpers.py` & `aa_ledger-0.3.7/ledger/task_helpers/etag_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/templates/ledger/base.html` & `aa_ledger-0.3.7/ledger/templates/ledger/base.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/templates/ledger/error.html` & `aa_ledger-0.3.7/ledger/templates/ledger/error.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/templates/ledger/ledger/base.html` & `aa_ledger-0.3.7/ledger/templates/ledger/ledger/base.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/templates/ledger/ledger/index.html` & `aa_ledger-0.3.7/ledger/templates/ledger/ledger/index.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/templates/ledger/ledger/menu.html` & `aa_ledger-0.3.7/ledger/templates/ledger/ledger/menu.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/templates/ledger/ledger/charledger/char_ledger.html` & `aa_ledger-0.3.7/ledger/templates/ledger/ledger/charledger/char_ledger.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/templates/ledger/ledger/charledger/month.html` & `aa_ledger-0.3.7/ledger/templates/ledger/ledger/charledger/month.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/templates/ledger/ledger/charledger/year.html` & `aa_ledger-0.3.7/ledger/templates/ledger/ledger/charledger/year.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/templates/ledger/ledger/corpledger/corp_ledger.html` & `aa_ledger-0.3.7/ledger/templates/ledger/ledger/corpledger/corp_ledger.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/templates/ledger/ledger/corpledger/month.html` & `aa_ledger-0.3.7/ledger/templates/ledger/ledger/corpledger/month.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/templates/ledger/ledger/corpledger/year.html` & `aa_ledger-0.3.7/ledger/templates/ledger/ledger/corpledger/year.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/templates/ledger/modals/modal-full.html` & `aa_ledger-0.3.7/ledger/templates/ledger/modals/modal-full.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/templates/ledger/modals/modal-xl.html` & `aa_ledger-0.3.7/ledger/templates/ledger/modals/modal-xl.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/templates/ledger/modals/modal.html` & `aa_ledger-0.3.7/ledger/templates/ledger/modals/modal.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/templates/ledger/modals/modal_dialog.html` & `aa_ledger-0.3.7/ledger/templates/ledger/modals/modal_dialog.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/templates/ledger/modals/pve/view_character_content.html` & `aa_ledger-0.3.7/ledger/templates/ledger/modals/pve/view_character_content.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/view_helpers/core.py` & `aa_ledger-0.3.7/ledger/view_helpers/core.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/views/pve.py` & `aa_ledger-0.3.7/ledger/views/pve.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/views/character/char_audit.py` & `aa_ledger-0.3.7/ledger/views/character/char_audit.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/views/corporation/corp_audit.py` & `aa_ledger-0.3.7/ledger/views/corporation/corp_audit.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/views/corporation/corp_events.py` & `aa_ledger-0.3.7/ledger/views/corporation/corp_events.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/ledger/views/corporation/corp_tax.py` & `aa_ledger-0.3.7/ledger/views/corporation/corp_tax.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/LICENSE` & `aa_ledger-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/README.md` & `aa_ledger-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.6/pyproject.toml` & `aa_ledger-0.3.7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 build-backend = "hatchling.build"
 requires = [
     "hatchling",
 ]
 
 [project]
 name = "aa-ledger"
+description = "EVE Online - Character/Corporation Ledger"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [
     { name = "Geuthur", email = "devgeuthur@gmail.com" },
 ]
 requires-python = ">=3.8"
 classifiers = [
@@ -26,15 +27,14 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 ]
 dynamic = [
-    "description",
     "version",
 ]
 dependencies = [
     "allianceauth>=4",
     "allianceauth-app-utils>=1.19",
     "dacite",
     "django-eveuniverse>=1.3",
```

### Comparing `aa_ledger-0.3.6/PKG-INFO` & `aa_ledger-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.3
 Name: aa-ledger
-Version: 0.3.6
-Dynamic: Summary
+Version: 0.3.7
+Summary: EVE Online - Character/Corporation Ledger
 Project-URL: Changelog, https://github.com/Geuthur/aa-ledger/blob/master/CHANGELOG.md
 Project-URL: Homepage, https://github.com/Geuthur/aa-ledger
 Project-URL: Source, https://github.com/Geuthur/aa-ledger
 Project-URL: Tracker, https://github.com/Geuthur/aa-ledger/issues
 Author-email: Geuthur <devgeuthur@gmail.com>
 License: MIT License
```

