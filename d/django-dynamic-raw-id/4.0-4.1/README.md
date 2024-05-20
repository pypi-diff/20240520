# Comparing `tmp/django_dynamic_raw_id-4.0.tar.gz` & `tmp/django_dynamic_raw_id-4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_dynamic_raw_id-4.0.tar", max compression
+gzip compressed data, was "django_dynamic_raw_id-4.1.tar", max compression
```

## Comparing `django_dynamic_raw_id-4.0.tar` & `django_dynamic_raw_id-4.1.tar`

### file list

```diff
@@ -1,26 +1,30 @@
--rw-r--r--   0        0        0     1419 2024-04-21 14:54:27.874661 django_dynamic_raw_id-4.0/CHANGELOG.md
--rw-r--r--   0        0        0     1079 2024-04-21 11:05:58.530638 django_dynamic_raw_id-4.0/LICENSE
--rw-r--r--   0        0        0     5823 2024-04-21 11:06:52.721092 django_dynamic_raw_id-4.0/README.md
--rw-r--r--   0        0        0        0 2024-04-21 06:11:35.934369 django_dynamic_raw_id-4.0/dynamic_raw_id/__init__.py
--rw-r--r--   0        0        0     1414 2024-04-21 11:05:58.531938 django_dynamic_raw_id-4.0/dynamic_raw_id/admin.py
--rw-r--r--   0        0        0     2697 2024-04-21 11:05:58.532184 django_dynamic_raw_id-4.0/dynamic_raw_id/filters.py
--rw-r--r--   0        0        0     3401 2024-04-21 11:05:58.532485 django_dynamic_raw_id-4.0/dynamic_raw_id/static/dynamic_raw_id/js/dynamic_raw_id.js
--rw-r--r--   0        0        0      565 2024-04-21 06:11:35.934806 django_dynamic_raw_id-4.0/dynamic_raw_id/templates/dynamic_raw_id/admin/filters/dynamic_raw_id_filter.html
--rw-r--r--   0        0        0      847 2024-04-21 06:11:35.934881 django_dynamic_raw_id-4.0/dynamic_raw_id/templates/dynamic_raw_id/admin/widgets/dynamic_raw_id_field.html
--rw-r--r--   0        0        0       45 2024-04-21 06:11:35.934943 django_dynamic_raw_id-4.0/dynamic_raw_id/templates/dynamic_raw_id/label.html
--rw-r--r--   0        0        0      134 2024-04-21 06:11:35.934993 django_dynamic_raw_id-4.0/dynamic_raw_id/templates/dynamic_raw_id/multi_label.html
--rw-r--r--   0        0        0        0 2024-04-21 06:11:35.935046 django_dynamic_raw_id-4.0/dynamic_raw_id/tests/__init__.py
--rw-r--r--   0        0        0     5358 2024-04-21 13:53:50.169615 django_dynamic_raw_id-4.0/dynamic_raw_id/tests/test_integrity.py
--rw-r--r--   0        0        0     6359 2024-04-21 14:53:58.700862 django_dynamic_raw_id-4.0/dynamic_raw_id/tests/test_selenium.py
--rw-r--r--   0        0        0        0 2024-04-21 06:11:35.935234 django_dynamic_raw_id-4.0/dynamic_raw_id/tests/testapp/__init__.py
--rw-r--r--   0        0        0     1000 2024-04-21 11:05:58.533543 django_dynamic_raw_id-4.0/dynamic_raw_id/tests/testapp/admin.py
--rw-r--r--   0        0        0     5028 2024-04-21 11:05:58.533753 django_dynamic_raw_id-4.0/dynamic_raw_id/tests/testapp/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-04-21 06:11:35.935393 django_dynamic_raw_id-4.0/dynamic_raw_id/tests/testapp/migrations/__init__.py
--rw-r--r--   0        0        0     3722 2024-04-21 13:07:55.842214 django_dynamic_raw_id-4.0/dynamic_raw_id/tests/testapp/models.py
--rw-r--r--   0        0        0     1886 2024-04-21 11:05:58.534074 django_dynamic_raw_id-4.0/dynamic_raw_id/tests/testapp/settings.py
--rw-r--r--   0        0        0      194 2024-04-21 06:11:35.935552 django_dynamic_raw_id-4.0/dynamic_raw_id/tests/testapp/urls.py
--rw-r--r--   0        0        0      592 2024-04-21 11:05:58.534237 django_dynamic_raw_id-4.0/dynamic_raw_id/urls.py
--rw-r--r--   0        0        0     2896 2024-04-21 11:05:58.534472 django_dynamic_raw_id-4.0/dynamic_raw_id/views.py
--rw-r--r--   0        0        0     2907 2024-04-21 11:05:58.534753 django_dynamic_raw_id-4.0/dynamic_raw_id/widgets.py
--rw-r--r--   0        0        0     3100 2024-04-21 14:53:43.043206 django_dynamic_raw_id-4.0/pyproject.toml
--rw-r--r--   0        0        0     8437 1970-01-01 00:00:00.000000 django_dynamic_raw_id-4.0/PKG-INFO
+-rw-r--r--   0        0        0     1509 2024-05-20 06:04:15.108207 django_dynamic_raw_id-4.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1079 2024-04-21 11:05:58.530638 django_dynamic_raw_id-4.1/LICENSE
+-rw-r--r--   0        0        0     5553 2024-04-22 02:32:53.654759 django_dynamic_raw_id-4.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-21 06:11:35.934369 django_dynamic_raw_id-4.1/dynamic_raw_id/__init__.py
+-rw-r--r--   0        0        0     1440 2024-04-22 08:29:10.732335 django_dynamic_raw_id-4.1/dynamic_raw_id/admin.py
+-rw-r--r--   0        0        0     2711 2024-04-22 03:18:52.708852 django_dynamic_raw_id-4.1/dynamic_raw_id/filters.py
+-rw-r--r--   0        0        0     3358 2024-05-20 06:01:13.186162 django_dynamic_raw_id-4.1/dynamic_raw_id/static/dynamic_raw_id/js/dynamic_raw_id.js
+-rw-r--r--   0        0        0      565 2024-04-21 06:11:35.934806 django_dynamic_raw_id-4.1/dynamic_raw_id/templates/dynamic_raw_id/admin/filters/dynamic_raw_id_filter.html
+-rw-r--r--   0        0        0      847 2024-05-20 06:01:12.026862 django_dynamic_raw_id-4.1/dynamic_raw_id/templates/dynamic_raw_id/admin/widgets/dynamic_raw_id_field.html
+-rw-r--r--   0        0        0       45 2024-04-22 09:23:22.167898 django_dynamic_raw_id-4.1/dynamic_raw_id/templates/dynamic_raw_id/label.html
+-rw-r--r--   0        0        0      134 2024-04-21 06:11:35.934993 django_dynamic_raw_id-4.1/dynamic_raw_id/templates/dynamic_raw_id/multi_label.html
+-rw-r--r--   0        0        0        0 2024-04-21 06:11:35.935046 django_dynamic_raw_id-4.1/dynamic_raw_id/tests/__init__.py
+-rw-r--r--   0        0        0     2265 2024-04-21 15:23:59.581803 django_dynamic_raw_id-4.1/dynamic_raw_id/tests/conftest.py
+-rw-r--r--   0        0        0     2298 2024-04-22 09:21:46.504022 django_dynamic_raw_id-4.1/dynamic_raw_id/tests/test_admin.py
+-rw-r--r--   0        0        0     2800 2024-04-21 15:19:59.464452 django_dynamic_raw_id-4.1/dynamic_raw_id/tests/test_admin_changelist.py
+-rw-r--r--   0        0        0     2079 2024-04-22 02:04:48.803645 django_dynamic_raw_id-4.1/dynamic_raw_id/tests/test_admin_inlines.py
+-rw-r--r--   0        0        0     2065 2024-04-21 16:40:55.231612 django_dynamic_raw_id-4.1/dynamic_raw_id/tests/test_django_admin.py
+-rw-r--r--   0        0        0     5358 2024-05-20 06:01:13.187596 django_dynamic_raw_id-4.1/dynamic_raw_id/tests/test_integrity.py
+-rw-r--r--   0        0        0        0 2024-04-21 06:11:35.935234 django_dynamic_raw_id-4.1/dynamic_raw_id/tests/testapp/__init__.py
+-rw-r--r--   0        0        0     1493 2024-04-21 15:10:28.552381 django_dynamic_raw_id-4.1/dynamic_raw_id/tests/testapp/admin.py
+-rw-r--r--   0        0        0     7268 2024-04-21 15:12:37.438028 django_dynamic_raw_id-4.1/dynamic_raw_id/tests/testapp/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-21 06:11:35.935393 django_dynamic_raw_id-4.1/dynamic_raw_id/tests/testapp/migrations/__init__.py
+-rw-r--r--   0        0        0     4352 2024-04-21 15:12:34.561466 django_dynamic_raw_id-4.1/dynamic_raw_id/tests/testapp/models.py
+-rw-r--r--   0        0        0     1565 2024-04-22 03:38:38.905913 django_dynamic_raw_id-4.1/dynamic_raw_id/tests/testapp/settings.py
+-rw-r--r--   0        0        0      194 2024-04-21 06:11:35.935552 django_dynamic_raw_id-4.1/dynamic_raw_id/tests/testapp/urls.py
+-rw-r--r--   0        0        0      592 2024-05-20 06:01:13.188284 django_dynamic_raw_id-4.1/dynamic_raw_id/urls.py
+-rw-r--r--   0        0        0     2697 2024-05-20 06:01:13.188999 django_dynamic_raw_id-4.1/dynamic_raw_id/views.py
+-rw-r--r--   0        0        0     2001 2024-05-20 06:01:13.189968 django_dynamic_raw_id-4.1/dynamic_raw_id/widgets.py
+-rw-r--r--   0        0        0     3101 2024-05-20 06:14:18.861514 django_dynamic_raw_id-4.1/pyproject.toml
+-rw-r--r--   0        0        0     8257 1970-01-01 00:00:00.000000 django_dynamic_raw_id-4.1/PKG-INFO
```

### Comparing `django_dynamic_raw_id-4.0/CHANGELOG.md` & `django_dynamic_raw_id-4.1/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 # Changelog
 
+## v4.1 (2024-05-20)
+
+- Overall code cleanup.
+- Refactored tests. Now full test coverage.
+
 ## v4.0 (2024-04-21)
 
 - Django 4.2 compatibility and tests.
 - Django 5.0 compatibility and tests.
 - Requires Python 3.8 or up.
 - Switch package management to Poetry.
 
 ## v3.0 (2022-03-20)
 
 - Django 4.0 compatibility and tests.
 - Requires Django 3.2 or up.
 - Requires Python 3.7 or up.
-- *Note:* You may now need to change the order and put the dynamic-raw-id
+- _Note:_ You may now need to change the order and put the dynamic-raw-id
   include before the generic admin include. See Readme for details.
 
 ## v2.8 (2020-12-02)
 
 - Django 3.1 compatibility and tests.
 
 ## v2.7 (2020-05-02)
@@ -40,15 +45,15 @@
 
 - Fixes missing icons in Admin views.
 - Fixes missing JS handling when using a custom /admin/ url.
 
 ## v2.3 (2018-01-18)
 
 - BACKWARDS INCOMPATIBLE: Renamed the project to `django-dynamic-raw-id`.
-  to reflect what it's  actually doing.
+  to reflect what it's actually doing.
 - Fixed glass lookup icon in Django 1.10 and below.
 - Specific ordering of media asset loading.
 
 ## v1.2 (2018-01-17)
 
 - Multiple fixes and enhancements.
 - Full Selenium based testsuite.
```

### Comparing `django_dynamic_raw_id-4.0/LICENSE` & `django_dynamic_raw_id-4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_dynamic_raw_id-4.0/README.md` & `django_dynamic_raw_id-4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # django-dynamic-raw-id
 
 A Django admin raw_id_fields widget replacement that handles display of an object's
 string value on change and can be overridden via a template.
 
 See this example:
 
-<img src="https://d.pr/i/1kv7d.png" style="max-height: 500px;" alt="Screenshot of Django Admin"/>
+<img src="https://d.pr/i/1kv7d.png" style="max-height: 400px;" alt="Screenshot of Django Admin"/>
 
 ## Compatibility Matrix:
 
 | Py/Dj     | 3.8 | 3.9 | 3.10 | 3.11 | 3.12 |
 |-----------|-----|-----|------|------|------|
 | 3.2 (LTS) | ✓   | ✓   | ✓    | ✓    | ✓    |
 | 4.0       | ✓   | ✓   | ✓    | ✓    | ✓    |
@@ -23,15 +23,15 @@
 ## Rationale
 
 By default, Django’s admin loads all possible related instances into a select-box
 interface (`<select>`) for fields that are ForeignKey. This can result in long load
 times and unresponsive admin pages for models with thousands of instances, or with
 multiple ForeinKeys.
 
-The normal fix is to use Django's [ModelAdmin.raw_id_fields](https://docs.djangoproject.com/en/4.0/ref/contrib/admin/#django.contrib.admin.ModelAdmin.raw_id_fields),
+The normal fix is to use Django's [ModelAdmin.raw_id_fields][raw_id_docs],
 but by default it *only* shows the raw id of the related model instance, which is
 somewhat unhelpful.
 
 This package improves the user experience by providing the string representation or
 other customized text for the related instance, linked to that instance's admin
 change form, in addition to the raw id itself.
 
@@ -96,76 +96,61 @@
 
 The coolest feature of django-dynamic-raw-id is the ability to customize the output
 of the value displayed alongside the `DynamicRawIDWidget`. There is a basic
 implementation if all you want is your object's `__unicode__` value. To change
 the value displayed all you need to do is implement the correct template.
 
 django-dynamic-raw-id looks for this template
-structure `dynamic_raw_id/<app>/<model>.html``
+structure `dynamic_raw_id/<app>/<model>.html`
 and `dynamic_raw_id/<app>/multi_<model>.html` (for multi-value lookups).
 
 For instance, if I have a blog post with a `User` dynamic_raw_id field that I want
-display as `Firstname Lastname``, I would create the template
-``dynamic_raw_id/auth/user.html` with:
+display as `Firstname Lastname`, I would create the template
+`dynamic_raw_id/auth/user.html` with:
 
 ```html
 <span>{{ object.0.first_name }} {{ object.0.last_name }}</span>
 ```
 
-A custom admin URL prefix
-=========================
+### A custom admin URL prefix
 
 If you have your admin *and* the dynamic_raw_id scripts located on a different
-prefix than `/admin/dynamic_raw_id/` you need adjust the `DYNAMIC_RAW_ID_MOUNT_URL``
-JS variable.
+prefix than `/admin/dynamic_raw_id/` you need adjust the `DYNAMIC_RAW_ID_MOUNT_URL`
+Javascript variable.
 
 Example:
 
 ```python
-    # In case the app is setup at /foobar/dynamic_raw_id/
+# In case the app is setup at /foobar/dynamic_raw_id/
 path('foobar/dynamic_raw_id/', include('dynamic_raw_id.urls')),
 ```
 
 ```html
 
-<script>window.DYNAMIC_RAW_ID_MOUNT_URL = "{% url "
-admin:index
-" %}";</script>
+<script>window.DYNAMIC_RAW_ID_MOUNT_URL = "{% url 'admin:index' %}";</script>
 ```
 
-An ideal place is the admin `base_site.html` template. Full example:
+An ideal place is the admin `admin/base_site.html` template. Full example:
 
 ```html
-{% extends "admin/base.html" %}
-
-{% block title %}{{ title }} | {{ site_title|default:_('Django site admin') }}{% endblock %}
+{% extends "admin/base_site.html" %}
 
 {% block extrahead %}
-{{ block.super }}
-<script>
-  window.DYNAMIC_RAW_ID_MOUNT_URL = "{% url "
-  admin:index
-  " %}";
-</script>
-{% endblock %}
-
-{% block branding %}
-<h1 id="site-name"><a href="{% url 'admin:index' %}">{{ site_header|default:_('Django
-  administration') }}</a></h1>
+  {{ block.super }}
+  <script>
+    window.DYNAMIC_RAW_ID_MOUNT_URL = "{% url 'admin:index' %}";
+  </script>
 {% endblock %}
-
-{% block nav-global %}{% endblock %}
 ```
 
-Testing and Local Development
-=============================
+# Testing and Local Development
 
 The testsuite uses Selenium to do frontend tests, we require Firefox and
-[geckodriver](https://github.com/mozilla/geckodriver) to be installed. You can
-install geckodriver on OS X with Homebrew:
+[geckodriver][geckodriver] to be installed. You can install geckodriver on OS X with
+Homebrew:
 
 ```bash
 $ brew install geckodriver
 ```
 
 Run the testsuite in your local environment using:
 
@@ -197,7 +182,10 @@
 ```shell
 $ poetry shell
 
 $ django-admin migrate
 $ django-admin createsuperuser
 $ django-admin runserver
 ```
+
+[raw_id_docs]: https://docs.djangoproject.com/en/dev/ref/contrib/admin/#django.contrib.admin.ModelAdmin.raw_id_fields
+[geckodriver]: https://github.com/mozilla/geckodriver
```

### Comparing `django_dynamic_raw_id-4.0/dynamic_raw_id/admin.py` & `django_dynamic_raw_id-4.1/dynamic_raw_id/admin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 from django.contrib.admin.options import BaseModelAdmin
 
-from dynamic_raw_id.widgets import DynamicRawIDMultiIdWidget, DynamicRawIDWidget
+from .widgets import DynamicRawIDMultiIdWidget, DynamicRawIDWidget
 
 if TYPE_CHECKING:
-    from django.db.models.fields import Field as DbField
+    from django.db.models.fields import Field as DB_Field
     from django.forms.fields import Field as FormField
     from django.http import HttpRequest
 
 
 class DynamicRawIDMixin(BaseModelAdmin):
     dynamic_raw_id_fields = ()
 
     def formfield_for_foreignkey(
         self,
-        db_field: DbField,
+        db_field: DB_Field,
         request: HttpRequest | None = None,
         **kwargs: Any,
     ) -> FormField:
         if db_field.name in self.dynamic_raw_id_fields:
             rel = db_field.remote_field
             kwargs["widget"] = DynamicRawIDWidget(rel, self.admin_site)
+            kwargs["help_text"] = ""
             return db_field.formfield(**kwargs)
         return super().formfield_for_foreignkey(db_field, request, **kwargs)
 
     def formfield_for_manytomany(
         self,
-        db_field: DbField,
+        db_field: DB_Field,
         request: HttpRequest | None = None,
         **kwargs: Any,
     ) -> FormField:
         if db_field.name in self.dynamic_raw_id_fields:
             rel = db_field.remote_field
             kwargs["widget"] = DynamicRawIDMultiIdWidget(rel, self.admin_site)
             kwargs["help_text"] = ""
```

### Comparing `django_dynamic_raw_id-4.0/dynamic_raw_id/filters.py` & `django_dynamic_raw_id-4.1/dynamic_raw_id/filters.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 from django import forms
 from django.contrib import admin
 
-from dynamic_raw_id.widgets import DynamicRawIDWidget
+from .widgets import DynamicRawIDWidget
 
 if TYPE_CHECKING:
     from django.db.models import Field as DbField
     from django.db.models import Model, QuerySet
     from django.forms import Form
     from django.http import HttpRequest
 
@@ -52,15 +52,15 @@
         """Use GET param for lookup and form initialization."""
         self.lookup_kwarg = field_path
         super().__init__(field, request, params, model, model_admin, field_path)
         rel = field.remote_field
         self.form = self.get_form(request, rel, model_admin.admin_site)
 
     def choices(self, changelist: Any) -> list:
-        """Filter choices are not available."""
+        """Filter choices do not exist, since we choose the popup value."""
         return []
 
     def expected_parameters(self) -> str:
         """Return GET params for this filter."""
         return self.lookup_kwarg
 
     def get_form(
```

### Comparing `django_dynamic_raw_id-4.0/dynamic_raw_id/static/dynamic_raw_id/js/dynamic_raw_id.js` & `django_dynamic_raw_id-4.1/dynamic_raw_id/static/dynamic_raw_id/js/dynamic_raw_id.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -3,22 +3,23 @@
 /**
  * Overwrite Django's `dismissRelatedLookupPopup` to trigger
  * a change event on the value change, so dynamic_raw_id can
  * catch it and update the associated label.
  */
 if (!windowname_to_id) {
     function windowname_to_id(text) {
-        text = text.replace(/__dot__/g, '.');
-        text = text.replace(/__dash__/g, '-');
-        return text;
+        return text
+            .replace(/__dot__/g, '.')
+            .replace(/__dash__/g, '-')
+            .replace(/__\d+$/, '');
     }
 }
 
 function dismissRelatedLookupPopup(win, chosenId) {
-    const name = windowname_to_id(win.name).replace(/__\d+$/, '');
+    const name = windowname_to_id(win.name);
     const elem = document.getElementById(name);
     if (elem.className.indexOf('vManyToManyRawIdAdminField') !== -1 && elem.value) {
         elem.value += `,${chosenId}`;
     } else {
         elem.value = chosenId;
     }
     django.jQuery(elem).trigger('change');
@@ -81,22 +82,20 @@
             e.stopPropagation();
         });
 
         // Clear both the input field and the labels
         $('.dynamic_raw_id-clear-field').click(function() {
             const $this = $(this);
             $this
-                .parent()
-                .find('.vForeignKeyRawIdAdminField, .vManyToManyRawIdAdminField')
+                .closest('.vForeignKeyRawIdAdminField, .vManyToManyRawIdAdminField')
                 .val('')
                 .trigger('change');
 
             $this
-                .parent()
-                .find('.dynamic_raw_id_label')
+                .closest('.dynamic_raw_id_label')
                 .html('&nbsp;');
         });
 
         // Open up the pop up window and set the focus in the input field
         $('.dynamic_raw_id-related-lookup').click(function() {
             // Actual Django javascript function
             showRelatedObjectLookupPopup(this);
```

### Comparing `django_dynamic_raw_id-4.0/dynamic_raw_id/templates/dynamic_raw_id/admin/filters/dynamic_raw_id_filter.html` & `django_dynamic_raw_id-4.1/dynamic_raw_id/templates/dynamic_raw_id/admin/filters/dynamic_raw_id_filter.html`

 * *Files identical despite different names*

### Comparing `django_dynamic_raw_id-4.0/dynamic_raw_id/templates/dynamic_raw_id/admin/widgets/dynamic_raw_id_field.html` & `django_dynamic_raw_id-4.1/dynamic_raw_id/templates/dynamic_raw_id/admin/widgets/dynamic_raw_id_field.html`

 * *Files identical despite different names*

### Comparing `django_dynamic_raw_id-4.0/dynamic_raw_id/tests/test_integrity.py` & `django_dynamic_raw_id-4.1/dynamic_raw_id/tests/test_integrity.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_raw_id-4.0/dynamic_raw_id/tests/testapp/admin.py` & `django_dynamic_raw_id-4.1/dynamic_raw_id/tests/testapp/admin.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from dynamic_raw_id.admin import DynamicRawIDMixin
 from dynamic_raw_id.filters import DynamicRawIDFilter
 
 from . import models
 
 
 @admin.register(models.ModelToTest)
-class ModelToTestlAdmin(DynamicRawIDMixin, admin.ModelAdmin):
+class ModelToTestAdmin(DynamicRawIDMixin, admin.ModelAdmin):
     raw_id_fields = (
         "rawid_fk",
         "rawid_fk_limited",
         "rawid_many",
     )
     dynamic_raw_id_fields = (
         "dynamic_raw_id_fk",
@@ -25,10 +25,27 @@
         ("dynamic_raw_id_fk", DynamicRawIDFilter),
         ("dynamic_raw_id_fk_int_pk", DynamicRawIDFilter),
         ("dynamic_raw_id_fk_char_pk", DynamicRawIDFilter),
         ("dynamic_raw_id_fk_uuid_pk", DynamicRawIDFilter),
     )
 
 
+class ModelToTestInlineAdmin(DynamicRawIDMixin, admin.TabularInline):
+    model = models.ModelToTestInlines
+    dynamic_raw_id_fields = (
+        "dynamic_raw_id_fk",
+        "dynamic_raw_id_fk_limited",
+        "dynamic_raw_id_many",
+        "dynamic_raw_id_fk_int_pk",
+        "dynamic_raw_id_fk_char_pk",
+        "dynamic_raw_id_fk_uuid_pk",
+    )
+
+
+@admin.register(models.ModelToTestInlinesBase)
+class ModelToTestInlineBaseAdmin(admin.ModelAdmin):
+    inlines = (ModelToTestInlineAdmin,)
+
+
 admin.site.register(models.IntPrimaryKeyModel)
 admin.site.register(models.CharPrimaryKeyModel)
 admin.site.register(models.UUIDPrimaryKeyModel)
```

### Comparing `django_dynamic_raw_id-4.0/dynamic_raw_id/tests/testapp/migrations/0001_initial.py` & `django_dynamic_raw_id-4.1/dynamic_raw_id/tests/testapp/migrations/0001_initial.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Generated by Django 4.2.11 on 2024-04-21 05:22
+# Generated by Django 5.0.4 on 2024-04-21 15:12
 
+import django.db.models.deletion
 from django.conf import settings
 from django.db import migrations, models
-import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
@@ -31,20 +31,66 @@
                     models.IntegerField(
                         primary_key=True, serialize=False, verbose_name="Number"
                     ),
                 ),
             ],
         ),
         migrations.CreateModel(
+            name="ModelToTestInlinesBase",
+            fields=[
+                (
+                    "id",
+                    models.AutoField(
+                        auto_created=True,
+                        primary_key=True,
+                        serialize=False,
+                        verbose_name="ID",
+                    ),
+                ),
+            ],
+        ),
+        migrations.CreateModel(
             name="UUIDPrimaryKeyModel",
             fields=[
                 ("uuid", models.UUIDField(primary_key=True, serialize=False)),
             ],
         ),
         migrations.CreateModel(
+            name="ModelToTestInlines",
+            fields=[
+                (
+                    "id",
+                    models.AutoField(
+                        auto_created=True,
+                        primary_key=True,
+                        serialize=False,
+                        verbose_name="ID",
+                    ),
+                ),
+                (
+                    "dynamic_raw_id_fk",
+                    models.ForeignKey(
+                        blank=True,
+                        null=True,
+                        on_delete=django.db.models.deletion.CASCADE,
+                        related_name="inline_dynamic_raw_id_fk",
+                        to=settings.AUTH_USER_MODEL,
+                        verbose_name="Dynamic RawID ForeignKey",
+                    ),
+                ),
+                (
+                    "base",
+                    models.ForeignKey(
+                        on_delete=django.db.models.deletion.CASCADE,
+                        to="testapp.modeltotestinlinesbase",
+                    ),
+                ),
+            ],
+        ),
+        migrations.CreateModel(
             name="ModelToTest",
             fields=[
                 (
                     "id",
                     models.AutoField(
                         auto_created=True,
                         primary_key=True,
@@ -56,90 +102,99 @@
                     "dynamic_raw_id_fk",
                     models.ForeignKey(
                         blank=True,
                         null=True,
                         on_delete=django.db.models.deletion.CASCADE,
                         related_name="dynamic_raw_id_fk",
                         to=settings.AUTH_USER_MODEL,
+                        verbose_name="Dynamic RawID ForeignKey",
                     ),
                 ),
                 (
                     "dynamic_raw_id_fk_char_pk",
                     models.ForeignKey(
                         blank=True,
                         null=True,
                         on_delete=django.db.models.deletion.CASCADE,
                         related_name="dynamic_raw_id_fk_char_pk",
                         to="testapp.charprimarykeymodel",
+                        verbose_name="Dynamic RawID Custom Primary Key: Character Field",
                     ),
                 ),
                 (
                     "dynamic_raw_id_fk_int_pk",
                     models.ForeignKey(
                         blank=True,
                         null=True,
                         on_delete=django.db.models.deletion.CASCADE,
                         related_name="dynamic_raw_id_fk_int_pk",
                         to="testapp.intprimarykeymodel",
+                        verbose_name="Dynamic RawID Custom Primary Key: Integer Field",
                     ),
                 ),
                 (
                     "dynamic_raw_id_fk_limited",
                     models.ForeignKey(
                         blank=True,
                         limit_choices_to={"is_staff": True},
                         null=True,
                         on_delete=django.db.models.deletion.CASCADE,
                         related_name="dynamic_raw_id_fk_limited",
                         to=settings.AUTH_USER_MODEL,
-                    ),
-                ),
-                (
-                    "dynamic_raw_id_fk_uuid_pk",
-                    models.ForeignKey(
-                        blank=True,
-                        null=True,
-                        on_delete=django.db.models.deletion.CASCADE,
-                        related_name="dynamic_raw_id_fk_uuid_pk",
-                        to="testapp.uuidprimarykeymodel",
+                        verbose_name="Dynamic RawID ForeignKey with limited choices",
                     ),
                 ),
                 (
                     "dynamic_raw_id_many",
                     models.ManyToManyField(
                         blank=True,
                         related_name="dynamic_raw_id_many",
                         to=settings.AUTH_USER_MODEL,
+                        verbose_name="Dynamic RawID ManyToMany",
                     ),
                 ),
                 (
                     "rawid_fk",
                     models.ForeignKey(
                         blank=True,
                         null=True,
                         on_delete=django.db.models.deletion.CASCADE,
                         related_name="rawid_fk",
                         to=settings.AUTH_USER_MODEL,
+                        verbose_name="Regular RawID ForeignKey",
                     ),
                 ),
                 (
                     "rawid_fk_limited",
                     models.ForeignKey(
                         blank=True,
                         limit_choices_to={"is_staff": True},
                         null=True,
                         on_delete=django.db.models.deletion.CASCADE,
                         related_name="rawid_fk_limited",
                         to=settings.AUTH_USER_MODEL,
+                        verbose_name="Regular RawID ForeignKey with limited choices",
                     ),
                 ),
                 (
                     "rawid_many",
                     models.ManyToManyField(
                         blank=True,
                         related_name="rawid_many",
                         to=settings.AUTH_USER_MODEL,
+                        verbose_name="Regular RawID ManyToMany",
+                    ),
+                ),
+                (
+                    "dynamic_raw_id_fk_uuid_pk",
+                    models.ForeignKey(
+                        blank=True,
+                        null=True,
+                        on_delete=django.db.models.deletion.CASCADE,
+                        related_name="dynamic_raw_id_fk_uuid_pk",
+                        to="testapp.uuidprimarykeymodel",
+                        verbose_name="Dynamic RawID Custom Primary Key: UUID Field",
                     ),
                 ),
             ],
         ),
     ]
```

### Comparing `django_dynamic_raw_id-4.0/dynamic_raw_id/tests/testapp/models.py` & `django_dynamic_raw_id-4.1/dynamic_raw_id/tests/testapp/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -111,7 +111,29 @@
         if self.dynamic_raw_id_fk_int_pk:
             return str(self.dynamic_raw_id_fk_int_pk)
         if self.dynamic_raw_id_fk_char_pk:
             return str(self.dynamic_raw_id_fk_char_pk)
         if self.dynamic_raw_id_fk_uuid_pk:
             return str(self.dynamic_raw_id_fk_uuid_pk)
         return "Test Instance"
+
+
+# Test Inline Admin Model --------------------------------------------------------------
+class ModelToTestInlinesBase(models.Model):
+    def __str__(self) -> str:
+        return "Base Model with Inlines"
+
+
+class ModelToTestInlines(models.Model):
+    base = models.ForeignKey(ModelToTestInlinesBase, on_delete=models.CASCADE)
+
+    dynamic_raw_id_fk = models.ForeignKey(
+        "auth.User",
+        related_name="inline_dynamic_raw_id_fk",
+        blank=True,
+        null=True,
+        on_delete=models.CASCADE,
+        verbose_name="Dynamic RawID ForeignKey",
+    )
+
+    def __str__(self) -> str:
+        return "Inline Model"
```

### Comparing `django_dynamic_raw_id-4.0/dynamic_raw_id/tests/testapp/settings.py` & `django_dynamic_raw_id-4.1/dynamic_raw_id/tests/testapp/settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from tempfile import TemporaryDirectory
 
 DEBUG = True
 
 SECRET_KEY = "super-secret-dynamic_raw_id-key"  # noqa: S105 Hardcoded password
 
+
+ROOT_URLCONF = "dynamic_raw_id.tests.testapp.urls"
+
 DATABASES = {
     "default": {"ENGINE": "django.db.backends.sqlite3", "NAME": "testapp.db"},
 }
 
 DEFAULT_AUTO_FIELD = "django.db.models.AutoField"
 
 TEMPLATES = [
@@ -43,26 +46,14 @@
     "django.middleware.common.CommonMiddleware",
     "django.contrib.messages.middleware.MessageMiddleware",
 )
 
 
 STATIC_ROOT = TemporaryDirectory().name
 STATIC_URL = "/static/"
-ROOT_URLCONF = "dynamic_raw_id.tests.testapp.urls"
 
 STATICFILES_FINDERS = [
     "django.contrib.staticfiles.finders.FileSystemFinder",
     "django.contrib.staticfiles.finders.AppDirectoriesFinder",
 ]
 
-TEST_SETTINGS = {
-    "DEBUG": DEBUG,
-    "SECRET_KEY": SECRET_KEY,
-    "DATABASES": DATABASES,
-    "TEMPLATES": TEMPLATES,
-    "INSTALLED_APPS": INSTALLED_APPS,
-    "MIDDLEWARE": MIDDLEWARE,
-    "STATIC_ROOT": STATIC_ROOT,
-    "STATIC_URL": STATIC_URL,
-    "ROOT_URLCONF": ROOT_URLCONF,
-    "STATICFILES_FINDERS": STATICFILES_FINDERS,
-}
+USE_TZ = False
```

### Comparing `django_dynamic_raw_id-4.0/dynamic_raw_id/urls.py` & `django_dynamic_raw_id-4.1/dynamic_raw_id/urls.py`

 * *Files identical despite different names*

### Comparing `django_dynamic_raw_id-4.0/dynamic_raw_id/views.py` & `django_dynamic_raw_id-4.1/dynamic_raw_id/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 @user_passes_test(lambda u: u.is_staff)
 def label_view(  # noqa: PLR0913 Too Many arguments
     request: HttpRequest,
     app_name: str,
     model_name: str,
-    template_name: str = "",
+    template_name: str,
     multi: bool = False,
     template_object_name: str = "object",
 ) -> HttpResponse:
     # The list of to obtained objects is in GET.id. No need to resume if we
     # didn't get it.
     if not request.GET.get("id"):
         msg = "No list of objects given"
@@ -34,38 +34,37 @@
     # Make sure this model exists and the user has 'change' permission for it.
     # If he doesn't have this permission, Django would not display the
     # change_list in the popup, and the user was never able to select objects.
     try:
         model = apps.get_model(app_name, model_name)
     except LookupError:
         msg = f"Model {app_name}.{model_name} does not exist."
-        return HttpResponseBadRequest(settings.DEBUG and msg or "")
+        return HttpResponseBadRequest(msg)
 
-    # Check 'view' or 'change' permission depending on Django's version
+    # Check 'view' permission
     if not request.user.has_perm(f"{app_name}.view_{model_name}"):
         return HttpResponseForbidden()
 
     try:
         if multi:
             model_template = f"dynamic_raw_id/{app_name}/multi_{model_name}.html"
             objs = model.objects.filter(pk__in=object_list)
-            objects = []
-            for obj in objs:
-                change_url = reverse(
-                    f"admin:{app_name}_{model_name}_change", args=[obj.pk]
-                )
-                objects.append((obj, change_url))
+            objects = [
+                (obj, reverse(f"admin:{app_name}_{model_name}_change", args=[obj.pk]))
+                for obj in objs
+            ]
             extra_context = {template_object_name: objects}
         else:
             model_template = f"dynamic_raw_id/{app_name}/{model_name}.html"
             obj = model.objects.get(pk=object_list[0])
             change_url = reverse(f"admin:{app_name}_{model_name}_change", args=[obj.pk])
             extra_context = {template_object_name: (obj, change_url)}
+
     # most likely, the pk wasn't convertable
     except ValueError:
         msg = "ValueError during lookup"
-        return HttpResponseBadRequest(settings.DEBUG and msg or "")
+        return HttpResponseBadRequest(msg)
     except model.DoesNotExist:
         msg = "Model instance does not exist"
-        return HttpResponseBadRequest(settings.DEBUG and msg or "")
+        return HttpResponseBadRequest(msg)
 
     return render(request, (model_template, template_name), extra_context)
```

### Comparing `django_dynamic_raw_id-4.0/dynamic_raw_id/widgets.py` & `django_dynamic_raw_id-4.1/dynamic_raw_id/widgets.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,85 +1,57 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
+from urllib.parse import urlencode
 
 from django import forms
-from django.conf import settings
 from django.contrib.admin import widgets
-from django.core.exceptions import ImproperlyConfigured
 from django.urls import reverse
 from django.utils.encoding import force_str
 
 if TYPE_CHECKING:
     from django.forms.renderers import BaseRenderer
     from django.template import Context
 
 
-class DynamicRawIDImproperlyConfigured(ImproperlyConfigured):
-    pass
-
-
 class DynamicRawIDWidget(widgets.ForeignKeyRawIdWidget):
     template_name: str = "dynamic_raw_id/admin/widgets/dynamic_raw_id_field.html"
 
     def get_context(self, name: str, value: Any, attrs: dict[str, Any]) -> Context:
         context = super().get_context(name, value, attrs)
-        model = self.rel.model
-        app_label = model._meta.app_label  # noqa: SLF001 Private member accessed
-        model_name = model._meta.object_name.lower()  # noqa: SLF001 Private member accessed
-        related_url = reverse(
-            f"admin:{app_label}_{model_name}_changelist",
-            current_app=self.admin_site.name,
-        )
+        app_name = self.rel.model._meta.app_label  # noqa: SLF001 Private member accessed
+        model_name = self.rel.model._meta.object_name.lower()  # noqa: SLF001 Private member accessed
 
-        params = self.url_parameters()
-        url = "?" + "&".join([f"{k}={v}" for k, v in params.items()]) if params else ""
-        if "class" not in attrs:
-            attrs["class"] = (
-                "vForeignKeyRawIdAdminField"  # The JavaScript looks for this hook.
-            )
-        app_name = model._meta.app_label.strip()  # noqa: SLF001 Private member accessed
-        model_name = model._meta.object_name.lower().strip()  # noqa: SLF001 Private member accessed
+        attrs.setdefault("class", "vForeignKeyRawIdAdminField")
 
         context.update(
-            {
-                "name": name,
-                "app_name": app_name,
-                "model_name": model_name,
-                "related_url": related_url,
-                "url": url,
-            }
+            name=name,
+            app_name=app_name,
+            model_name=model_name,
+            related_url=reverse(
+                f"admin:{app_name}_{model_name}_changelist",
+                current_app=self.admin_site.name,
+            ),
+            url=f"?{urlencode(self.url_parameters())}",
         )
         return context
 
     @property
     def media(self) -> forms.Media:
-        extra = "" if settings.DEBUG else ".min"
         return forms.Media(
             js=[
-                f"admin/js/vendor/jquery/jquery{extra}.js",
+                "admin/js/vendor/jquery/jquery.min.js",
                 "admin/js/jquery.init.js",
                 "admin/js/core.js",
                 "dynamic_raw_id/js/dynamic_raw_id.js",
             ]
         )
 
 
 class DynamicRawIDMultiIdWidget(DynamicRawIDWidget):
-    def value_from_datadict(
-        self,
-        data: dict[str, Any],
-        files: Any | None,
-        name: str,
-    ) -> str | None:
-        value = data.get(name)
-        if value:
-            return value.split(",")
-        return None
-
     def render(
         self,
         name: str,
         value: Any,
         attrs: dict[str, Any] | None = None,
         renderer: BaseRenderer | None = None,
     ) -> str:
```

### Comparing `django_dynamic_raw_id-4.0/pyproject.toml` & `django_dynamic_raw_id-4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 # Poetry -------------------------------------------------------------------------------
 [tool.poetry]
 name = "django-dynamic-raw-id"
-version = "4.0"
+version = "4.1"
 packages = [{include = "dynamic_raw_id"}]
 description = "raw_id_fields widget replacement that handles display of an object's string value on change."
 keywords = ["django", "widget", "field", "admin", "raw-id", "foreignkey"]
 authors = ["Martin Mahner", "Seth Buntin", "Yann Malet"]
 homepage = "https://github.com/lincolnloop/django-dynamic-raw-id"
 license = "MIT"
 readme = ["README.md", "CHANGELOG.md"]
@@ -84,14 +84,14 @@
 """
 filterwarnings = [
   "ignore::RuntimeWarning"
 ]
 
 [tool.coverage]
 run.omit = [
-  "django_markup/tests/*",
+  "dynamic_raw_id/tests/*",
 ]
 report.exclude_lines = [
     "pragma: no cover",
     "if TYPE_CHECKING:",
     "def __repr__",
 ]
```

### Comparing `django_dynamic_raw_id-4.0/PKG-INFO` & `django_dynamic_raw_id-4.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dynamic-raw-id
-Version: 4.0
+Version: 4.1
 Summary: raw_id_fields widget replacement that handles display of an object's string value on change.
 Home-page: https://github.com/lincolnloop/django-dynamic-raw-id
 License: MIT
 Keywords: django,widget,field,admin,raw-id,foreignkey
 Author: Martin Mahner
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -31,15 +31,15 @@
 # django-dynamic-raw-id
 
 A Django admin raw_id_fields widget replacement that handles display of an object's
 string value on change and can be overridden via a template.
 
 See this example:
 
-<img src="https://d.pr/i/1kv7d.png" style="max-height: 500px;" alt="Screenshot of Django Admin"/>
+<img src="https://d.pr/i/1kv7d.png" style="max-height: 400px;" alt="Screenshot of Django Admin"/>
 
 ## Compatibility Matrix:
 
 | Py/Dj     | 3.8 | 3.9 | 3.10 | 3.11 | 3.12 |
 |-----------|-----|-----|------|------|------|
 | 3.2 (LTS) | ✓   | ✓   | ✓    | ✓    | ✓    |
 | 4.0       | ✓   | ✓   | ✓    | ✓    | ✓    |
@@ -50,15 +50,15 @@
 ## Rationale
 
 By default, Django’s admin loads all possible related instances into a select-box
 interface (`<select>`) for fields that are ForeignKey. This can result in long load
 times and unresponsive admin pages for models with thousands of instances, or with
 multiple ForeinKeys.
 
-The normal fix is to use Django's [ModelAdmin.raw_id_fields](https://docs.djangoproject.com/en/4.0/ref/contrib/admin/#django.contrib.admin.ModelAdmin.raw_id_fields),
+The normal fix is to use Django's [ModelAdmin.raw_id_fields][raw_id_docs],
 but by default it *only* shows the raw id of the related model instance, which is
 somewhat unhelpful.
 
 This package improves the user experience by providing the string representation or
 other customized text for the related instance, linked to that instance's admin
 change form, in addition to the raw id itself.
 
@@ -123,76 +123,61 @@
 
 The coolest feature of django-dynamic-raw-id is the ability to customize the output
 of the value displayed alongside the `DynamicRawIDWidget`. There is a basic
 implementation if all you want is your object's `__unicode__` value. To change
 the value displayed all you need to do is implement the correct template.
 
 django-dynamic-raw-id looks for this template
-structure `dynamic_raw_id/<app>/<model>.html``
+structure `dynamic_raw_id/<app>/<model>.html`
 and `dynamic_raw_id/<app>/multi_<model>.html` (for multi-value lookups).
 
 For instance, if I have a blog post with a `User` dynamic_raw_id field that I want
-display as `Firstname Lastname``, I would create the template
-``dynamic_raw_id/auth/user.html` with:
+display as `Firstname Lastname`, I would create the template
+`dynamic_raw_id/auth/user.html` with:
 
 ```html
 <span>{{ object.0.first_name }} {{ object.0.last_name }}</span>
 ```
 
-A custom admin URL prefix
-=========================
+### A custom admin URL prefix
 
 If you have your admin *and* the dynamic_raw_id scripts located on a different
-prefix than `/admin/dynamic_raw_id/` you need adjust the `DYNAMIC_RAW_ID_MOUNT_URL``
-JS variable.
+prefix than `/admin/dynamic_raw_id/` you need adjust the `DYNAMIC_RAW_ID_MOUNT_URL`
+Javascript variable.
 
 Example:
 
 ```python
-    # In case the app is setup at /foobar/dynamic_raw_id/
+# In case the app is setup at /foobar/dynamic_raw_id/
 path('foobar/dynamic_raw_id/', include('dynamic_raw_id.urls')),
 ```
 
 ```html
 
-<script>window.DYNAMIC_RAW_ID_MOUNT_URL = "{% url "
-admin:index
-" %}";</script>
+<script>window.DYNAMIC_RAW_ID_MOUNT_URL = "{% url 'admin:index' %}";</script>
 ```
 
-An ideal place is the admin `base_site.html` template. Full example:
+An ideal place is the admin `admin/base_site.html` template. Full example:
 
 ```html
-{% extends "admin/base.html" %}
-
-{% block title %}{{ title }} | {{ site_title|default:_('Django site admin') }}{% endblock %}
+{% extends "admin/base_site.html" %}
 
 {% block extrahead %}
-{{ block.super }}
-<script>
-  window.DYNAMIC_RAW_ID_MOUNT_URL = "{% url "
-  admin:index
-  " %}";
-</script>
-{% endblock %}
-
-{% block branding %}
-<h1 id="site-name"><a href="{% url 'admin:index' %}">{{ site_header|default:_('Django
-  administration') }}</a></h1>
+  {{ block.super }}
+  <script>
+    window.DYNAMIC_RAW_ID_MOUNT_URL = "{% url 'admin:index' %}";
+  </script>
 {% endblock %}
-
-{% block nav-global %}{% endblock %}
 ```
 
-Testing and Local Development
-=============================
+# Testing and Local Development
 
 The testsuite uses Selenium to do frontend tests, we require Firefox and
-[geckodriver](https://github.com/mozilla/geckodriver) to be installed. You can
-install geckodriver on OS X with Homebrew:
+[geckodriver][geckodriver] to be installed. You can install geckodriver on OS X with
+Homebrew:
 
 ```bash
 $ brew install geckodriver
 ```
 
 Run the testsuite in your local environment using:
 
@@ -225,29 +210,37 @@
 $ poetry shell
 
 $ django-admin migrate
 $ django-admin createsuperuser
 $ django-admin runserver
 ```
 
+[raw_id_docs]: https://docs.djangoproject.com/en/dev/ref/contrib/admin/#django.contrib.admin.ModelAdmin.raw_id_fields
+[geckodriver]: https://github.com/mozilla/geckodriver
+
 # Changelog
 
+## v4.1 (2024-05-20)
+
+- Overall code cleanup.
+- Refactored tests. Now full test coverage.
+
 ## v4.0 (2024-04-21)
 
 - Django 4.2 compatibility and tests.
 - Django 5.0 compatibility and tests.
 - Requires Python 3.8 or up.
 - Switch package management to Poetry.
 
 ## v3.0 (2022-03-20)
 
 - Django 4.0 compatibility and tests.
 - Requires Django 3.2 or up.
 - Requires Python 3.7 or up.
-- *Note:* You may now need to change the order and put the dynamic-raw-id
+- _Note:_ You may now need to change the order and put the dynamic-raw-id
   include before the generic admin include. See Readme for details.
 
 ## v2.8 (2020-12-02)
 
 - Django 3.1 compatibility and tests.
 
 ## v2.7 (2020-05-02)
@@ -271,15 +264,15 @@
 
 - Fixes missing icons in Admin views.
 - Fixes missing JS handling when using a custom /admin/ url.
 
 ## v2.3 (2018-01-18)
 
 - BACKWARDS INCOMPATIBLE: Renamed the project to `django-dynamic-raw-id`.
-  to reflect what it's  actually doing.
+  to reflect what it's actually doing.
 - Fixed glass lookup icon in Django 1.10 and below.
 - Specific ordering of media asset loading.
 
 ## v1.2 (2018-01-17)
 
 - Multiple fixes and enhancements.
 - Full Selenium based testsuite.
```

