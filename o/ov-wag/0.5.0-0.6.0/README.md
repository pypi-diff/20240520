# Comparing `tmp/ov_wag-0.5.0.tar.gz` & `tmp/ov_wag-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ov_wag-0.5.0.tar", last modified: Fri Feb  9 21:44:49 2024, max compression
+gzip compressed data, was "ov_wag-0.6.0.tar", last modified: Mon May 20 21:13:48 2024, max compression
```

## Comparing `ov_wag-0.5.0.tar` & `ov_wag-0.6.0.tar`

### file list

```diff
@@ -1,86 +1,89 @@
--rw-r--r--   0        0        0     1697 2024-02-09 21:44:16.488020 ov_wag-0.5.0/README.md
--rw-r--r--   0        0        0        0 2024-02-09 21:44:16.488020 ov_wag-0.5.0/authors/__init__.py
--rw-r--r--   0        0        0      146 2024-02-09 21:44:16.492020 ov_wag-0.5.0/authors/apps.py
--rw-r--r--   0        0        0     1319 2024-02-09 21:44:16.492020 ov_wag-0.5.0/authors/migrations/0001_initial.py
--rw-r--r--   0        0        0     1080 2024-02-09 21:44:16.492020 ov_wag-0.5.0/authors/migrations/0002_authorsorderable.py
--rw-r--r--   0        0        0        0 2024-02-09 21:44:16.492020 ov_wag-0.5.0/authors/migrations/__init__.py
--rw-r--r--   0        0        0     2311 2024-02-09 21:44:16.492020 ov_wag-0.5.0/authors/models.py
--rw-r--r--   0        0        0      503 2024-02-09 21:44:16.492020 ov_wag-0.5.0/authors/serializers.py
--rw-r--r--   0        0        0      294 2024-02-09 21:44:16.492020 ov_wag-0.5.0/authors/views.py
--rw-r--r--   0        0        0       40 2024-02-09 21:44:16.492020 ov_wag-0.5.0/cli/__init__.py
--rw-r--r--   0        0        0     2548 2024-02-09 21:44:16.492020 ov_wag-0.5.0/cli/cli.py
--rw-r--r--   0        0        0      964 2024-02-09 21:44:16.492020 ov_wag-0.5.0/cli/utils.py
--rw-r--r--   0        0        0        0 2024-02-09 21:44:16.492020 ov_wag-0.5.0/exhibits/__init__.py
--rw-r--r--   0        0        0      282 2024-02-09 21:44:16.492020 ov_wag-0.5.0/exhibits/api.py
--rw-r--r--   0        0        0      148 2024-02-09 21:44:16.492020 ov_wag-0.5.0/exhibits/apps.py
--rw-r--r--   0        0        0     1280 2024-02-09 21:44:16.492020 ov_wag-0.5.0/exhibits/management/commands/rename.py
--rw-r--r--   0        0        0     1036 2024-02-09 21:44:16.492020 ov_wag-0.5.0/exhibits/migrations/0001_initial.py
--rw-r--r--   0        0        0      574 2024-02-09 21:44:16.492020 ov_wag-0.5.0/exhibits/migrations/0002_exhibitpage_cover_image.py
--rw-r--r--   0        0        0      589 2024-02-09 21:44:16.492020 ov_wag-0.5.0/exhibits/migrations/0003_exhibitpage_hero_image.py
--rw-r--r--   0        0        0     1057 2024-02-09 21:44:16.492020 ov_wag-0.5.0/exhibits/migrations/0004_exhibitsorderable.py
--rw-r--r--   0        0        0      393 2024-02-09 21:44:16.492020 ov_wag-0.5.0/exhibits/migrations/0005_exhibitpage_featured.py
--rw-r--r--   0        0        0      820 2024-02-09 21:44:16.492020 ov_wag-0.5.0/exhibits/migrations/0006_alter_exhibitpage_body.py
--rw-r--r--   0        0        0     1072 2024-02-09 21:44:16.492020 ov_wag-0.5.0/exhibits/migrations/0007_alter_exhibitpage_body.py
--rw-r--r--   0        0        0        0 2024-02-09 21:44:16.492020 ov_wag-0.5.0/exhibits/migrations/__init__.py
--rw-r--r--   0        0        0     5073 2024-02-09 21:44:16.492020 ov_wag-0.5.0/exhibits/models.py
--rw-r--r--   0        0        0      367 2024-02-09 21:44:16.492020 ov_wag-0.5.0/exhibits/templates/exhibit/exhibit_page.html
--rw-r--r--   0        0        0        0 2024-02-09 21:44:16.492020 ov_wag-0.5.0/exhibits/tests/__init__.py
--rw-r--r--   0        0        0      357 2024-02-09 21:44:16.492020 ov_wag-0.5.0/exhibits/tests/factories.py
--rw-r--r--   0        0        0      370 2024-02-09 21:44:16.492020 ov_wag-0.5.0/exhibits/tests/test_exhibit_page.py
--rw-r--r--   0        0        0      411 2024-02-09 21:44:16.492020 ov_wag-0.5.0/exhibits/views.py
--rw-r--r--   0        0        0        0 2024-02-09 21:44:16.492020 ov_wag-0.5.0/home/__init__.py
--rw-r--r--   0        0        0      604 2024-02-09 21:44:16.492020 ov_wag-0.5.0/home/migrations/0001_initial.py
--rw-r--r--   0        0        0     1745 2024-02-09 21:44:16.492020 ov_wag-0.5.0/home/migrations/0002_create_homepage.py
--rw-r--r--   0        0        0      398 2024-02-09 21:44:16.492020 ov_wag-0.5.0/home/migrations/0003_homepage_body.py
--rw-r--r--   0        0        0        0 2024-02-09 21:44:16.492020 ov_wag-0.5.0/home/migrations/__init__.py
--rw-r--r--   0        0        0      510 2024-02-09 21:44:16.492020 ov_wag-0.5.0/home/models.py
--rw-r--r--   0        0        0     3003 2024-02-09 21:44:16.492020 ov_wag-0.5.0/home/static/css/welcome_page.css
--rw-r--r--   0        0        0      175 2024-02-09 21:44:16.492020 ov_wag-0.5.0/home/templates/home/home_page.html
--rw-r--r--   0        0        0     6254 2024-02-09 21:44:16.492020 ov_wag-0.5.0/home/templates/home/welcome_page.html
--rw-r--r--   0        0        0        0 2024-02-09 21:44:16.492020 ov_wag-0.5.0/ov_collections/__init__.py
--rw-r--r--   0        0        0      157 2024-02-09 21:44:16.492020 ov_wag-0.5.0/ov_collections/apps.py
--rw-r--r--   0        0        0     1923 2024-02-09 21:44:16.492020 ov_wag-0.5.0/ov_collections/blocks.py
--rw-r--r--   0        0        0     1305 2024-02-09 21:44:16.492020 ov_wag-0.5.0/ov_collections/migrations/0001_initial.py
--rw-r--r--   0        0        0     1013 2024-02-09 21:44:16.492020 ov_wag-0.5.0/ov_collections/migrations/0002_alter_collection_content.py
--rw-r--r--   0        0        0     1419 2024-02-09 21:44:16.492020 ov_wag-0.5.0/ov_collections/migrations/0003_alter_collection_content.py
--rw-r--r--   0        0        0     3349 2024-02-09 21:44:16.492020 ov_wag-0.5.0/ov_collections/migrations/0004_alter_collection_content.py
--rw-r--r--   0        0        0     2880 2024-02-09 21:44:16.492020 ov_wag-0.5.0/ov_collections/migrations/0005_alter_collection_content.py
--rw-r--r--   0        0        0     2460 2024-02-09 21:44:16.492020 ov_wag-0.5.0/ov_collections/migrations/0006_alter_collection_content.py
--rw-r--r--   0        0        0      385 2024-02-09 21:44:16.492020 ov_wag-0.5.0/ov_collections/migrations/0007_rename_about_collection_introduction.py
--rw-r--r--   0        0        0     2689 2024-02-09 21:44:16.492020 ov_wag-0.5.0/ov_collections/migrations/0008_alter_collection_content.py
--rw-r--r--   0        0        0      704 2024-02-09 21:44:16.492020 ov_wag-0.5.0/ov_collections/migrations/0009_collection_hero_image.py
--rw-r--r--   0        0        0     2942 2024-02-09 21:44:16.492020 ov_wag-0.5.0/ov_collections/migrations/0010_collection_aapb_records_alter_collection_content.py
--rw-r--r--   0        0        0    10573 2024-02-09 21:44:16.492020 ov_wag-0.5.0/ov_collections/migrations/0011_alter_collection_aapb_records_and_more.py
--rw-r--r--   0        0        0    13066 2024-02-09 21:44:16.492020 ov_wag-0.5.0/ov_collections/migrations/0012_remove_collection_aapb_records_and_more.py
--rw-r--r--   0        0        0        0 2024-02-09 21:44:16.492020 ov_wag-0.5.0/ov_collections/migrations/__init__.py
--rw-r--r--   0        0        0     3052 2024-02-09 21:44:16.492020 ov_wag-0.5.0/ov_collections/models.py
--rw-r--r--   0        0        0       26 2024-02-09 21:44:16.492020 ov_wag-0.5.0/ov_collections/tests.py
--rw-r--r--   0        0        0      349 2024-02-09 21:44:16.492020 ov_wag-0.5.0/ov_collections/views.py
--rw-r--r--   0        0        0       61 2024-02-09 21:44:16.492020 ov_wag-0.5.0/ov_wag/__init__.py
--rw-r--r--   0        0        0       22 2024-02-09 21:44:16.492020 ov_wag-0.5.0/ov_wag/_version.py
--rw-r--r--   0        0        0     2398 2024-02-09 21:44:16.492020 ov_wag-0.5.0/ov_wag/api.py
--rw-r--r--   0        0        0      213 2024-02-09 21:44:16.492020 ov_wag-0.5.0/ov_wag/serializers.py
--rw-r--r--   0        0        0        0 2024-02-09 21:44:16.492020 ov_wag-0.5.0/ov_wag/settings/__init__.py
--rw-r--r--   0        0        0     6892 2024-02-09 21:44:16.496020 ov_wag-0.5.0/ov_wag/settings/base.py
--rw-r--r--   0        0        0      528 2024-02-09 21:44:16.496020 ov_wag-0.5.0/ov_wag/settings/dev.py
--rw-r--r--   0        0        0     1004 2024-02-09 21:44:16.496020 ov_wag-0.5.0/ov_wag/settings/production.py
--rw-r--r--   0        0        0      614 2024-02-09 21:44:16.496020 ov_wag-0.5.0/ov_wag/settings/test.py
--rw-r--r--   0        0        0        0 2024-02-09 21:44:16.496020 ov_wag-0.5.0/ov_wag/static/css/ov-wag.css
--rw-r--r--   0        0        0        0 2024-02-09 21:44:16.496020 ov_wag-0.5.0/ov_wag/static/js/ov-wag.js
--rw-r--r--   0        0        0      238 2024-02-09 21:44:16.496020 ov_wag-0.5.0/ov_wag/templates/404.html
--rw-r--r--   0        0        0      363 2024-02-09 21:44:16.496020 ov_wag-0.5.0/ov_wag/templates/500.html
--rw-r--r--   0        0        0     1318 2024-02-09 21:44:16.496020 ov_wag-0.5.0/ov_wag/templates/base.html
--rw-r--r--   0        0        0       57 2024-02-09 21:44:16.496020 ov_wag-0.5.0/ov_wag/templates/socialaccount/authentication_error.html
--rw-r--r--   0        0        0      554 2024-02-09 21:44:16.496020 ov_wag-0.5.0/ov_wag/templates/wagtailadmin/login.html
--rw-r--r--   0        0        0        0 2024-02-09 21:44:16.496020 ov_wag-0.5.0/ov_wag/templatetags/__init__.py
--rw-r--r--   0        0        0      259 2024-02-09 21:44:16.496020 ov_wag-0.5.0/ov_wag/templatetags/custom_tags.py
--rw-r--r--   0        0        0        0 2024-02-09 21:44:16.496020 ov_wag-0.5.0/ov_wag/tests/__init__.py
--rw-r--r--   0        0        0     2201 2024-02-09 21:44:16.496020 ov_wag-0.5.0/ov_wag/tests/test_api.py
--rw-r--r--   0        0        0      569 2024-02-09 21:44:16.496020 ov_wag-0.5.0/ov_wag/tests/test_env.py
--rw-r--r--   0        0        0     1284 2024-02-09 21:44:16.496020 ov_wag-0.5.0/ov_wag/urls.py
--rw-r--r--   0        0        0      453 2024-02-09 21:44:16.496020 ov_wag-0.5.0/ov_wag/wsgi.py
--rw-r--r--   0        0        0     2105 2024-02-09 21:44:49.063813 ov_wag-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-09 21:44:16.496020 ov_wag-0.5.0/search/__init__.py
--rw-r--r--   0        0        0     1301 2024-02-09 21:44:16.496020 ov_wag-0.5.0/search/templates/search/search.html
--rw-r--r--   0        0        0     1037 2024-02-09 21:44:16.496020 ov_wag-0.5.0/search/views.py
--rw-r--r--   0        0        0     2880 1970-01-01 00:00:00.000000 ov_wag-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1697 2024-05-20 21:13:09.379516 ov_wag-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 21:13:09.379516 ov_wag-0.6.0/authors/__init__.py
+-rw-r--r--   0        0        0      146 2024-05-20 21:13:09.379516 ov_wag-0.6.0/authors/apps.py
+-rw-r--r--   0        0        0     1319 2024-05-20 21:13:09.379516 ov_wag-0.6.0/authors/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1080 2024-05-20 21:13:09.379516 ov_wag-0.6.0/authors/migrations/0002_authorsorderable.py
+-rw-r--r--   0        0        0        0 2024-05-20 21:13:09.379516 ov_wag-0.6.0/authors/migrations/__init__.py
+-rw-r--r--   0        0        0     2311 2024-05-20 21:13:09.379516 ov_wag-0.6.0/authors/models.py
+-rw-r--r--   0        0        0      503 2024-05-20 21:13:09.379516 ov_wag-0.6.0/authors/serializers.py
+-rw-r--r--   0        0        0      294 2024-05-20 21:13:09.379516 ov_wag-0.6.0/authors/views.py
+-rw-r--r--   0        0        0       40 2024-05-20 21:13:09.379516 ov_wag-0.6.0/cli/__init__.py
+-rw-r--r--   0        0        0     2514 2024-05-20 21:13:09.379516 ov_wag-0.6.0/cli/cli.py
+-rw-r--r--   0        0        0      964 2024-05-20 21:13:09.379516 ov_wag-0.6.0/cli/utils.py
+-rw-r--r--   0        0        0        0 2024-05-20 21:13:09.379516 ov_wag-0.6.0/exhibits/__init__.py
+-rw-r--r--   0        0        0      282 2024-05-20 21:13:09.379516 ov_wag-0.6.0/exhibits/api.py
+-rw-r--r--   0        0        0      148 2024-05-20 21:13:09.379516 ov_wag-0.6.0/exhibits/apps.py
+-rw-r--r--   0        0        0     1280 2024-05-20 21:13:09.379516 ov_wag-0.6.0/exhibits/management/commands/rename.py
+-rw-r--r--   0        0        0     1036 2024-05-20 21:13:09.379516 ov_wag-0.6.0/exhibits/migrations/0001_initial.py
+-rw-r--r--   0        0        0      574 2024-05-20 21:13:09.379516 ov_wag-0.6.0/exhibits/migrations/0002_exhibitpage_cover_image.py
+-rw-r--r--   0        0        0      589 2024-05-20 21:13:09.379516 ov_wag-0.6.0/exhibits/migrations/0003_exhibitpage_hero_image.py
+-rw-r--r--   0        0        0     1057 2024-05-20 21:13:09.379516 ov_wag-0.6.0/exhibits/migrations/0004_exhibitsorderable.py
+-rw-r--r--   0        0        0      393 2024-05-20 21:13:09.379516 ov_wag-0.6.0/exhibits/migrations/0005_exhibitpage_featured.py
+-rw-r--r--   0        0        0      820 2024-05-20 21:13:09.379516 ov_wag-0.6.0/exhibits/migrations/0006_alter_exhibitpage_body.py
+-rw-r--r--   0        0        0     1072 2024-05-20 21:13:09.379516 ov_wag-0.6.0/exhibits/migrations/0007_alter_exhibitpage_body.py
+-rw-r--r--   0        0        0     1129 2024-05-20 21:13:09.379516 ov_wag-0.6.0/exhibits/migrations/0008_alter_exhibitpage_body.py
+-rw-r--r--   0        0        0     1776 2024-05-20 21:13:09.379516 ov_wag-0.6.0/exhibits/migrations/0009_alter_exhibitpage_body.py
+-rw-r--r--   0        0        0     1107 2024-05-20 21:13:09.379516 ov_wag-0.6.0/exhibits/migrations/0010_alter_exhibitpage_body.py
+-rw-r--r--   0        0        0        0 2024-05-20 21:13:09.379516 ov_wag-0.6.0/exhibits/migrations/__init__.py
+-rw-r--r--   0        0        0     5729 2024-05-20 21:13:09.379516 ov_wag-0.6.0/exhibits/models.py
+-rw-r--r--   0        0        0      367 2024-05-20 21:13:09.379516 ov_wag-0.6.0/exhibits/templates/exhibit/exhibit_page.html
+-rw-r--r--   0        0        0        0 2024-05-20 21:13:09.379516 ov_wag-0.6.0/exhibits/tests/__init__.py
+-rw-r--r--   0        0        0      357 2024-05-20 21:13:09.379516 ov_wag-0.6.0/exhibits/tests/factories.py
+-rw-r--r--   0        0        0      370 2024-05-20 21:13:09.379516 ov_wag-0.6.0/exhibits/tests/test_exhibit_page.py
+-rw-r--r--   0        0        0      414 2024-05-20 21:13:09.379516 ov_wag-0.6.0/exhibits/views.py
+-rw-r--r--   0        0        0        0 2024-05-20 21:13:09.379516 ov_wag-0.6.0/home/__init__.py
+-rw-r--r--   0        0        0      604 2024-05-20 21:13:09.383516 ov_wag-0.6.0/home/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1745 2024-05-20 21:13:09.383516 ov_wag-0.6.0/home/migrations/0002_create_homepage.py
+-rw-r--r--   0        0        0      398 2024-05-20 21:13:09.383516 ov_wag-0.6.0/home/migrations/0003_homepage_body.py
+-rw-r--r--   0        0        0        0 2024-05-20 21:13:09.383516 ov_wag-0.6.0/home/migrations/__init__.py
+-rw-r--r--   0        0        0      510 2024-05-20 21:13:09.383516 ov_wag-0.6.0/home/models.py
+-rw-r--r--   0        0        0     3003 2024-05-20 21:13:09.383516 ov_wag-0.6.0/home/static/css/welcome_page.css
+-rw-r--r--   0        0        0      175 2024-05-20 21:13:09.383516 ov_wag-0.6.0/home/templates/home/home_page.html
+-rw-r--r--   0        0        0     6254 2024-05-20 21:13:09.383516 ov_wag-0.6.0/home/templates/home/welcome_page.html
+-rw-r--r--   0        0        0        0 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_collections/__init__.py
+-rw-r--r--   0        0        0      157 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_collections/apps.py
+-rw-r--r--   0        0        0     1923 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_collections/blocks.py
+-rw-r--r--   0        0        0     1305 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_collections/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1013 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_collections/migrations/0002_alter_collection_content.py
+-rw-r--r--   0        0        0     1419 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_collections/migrations/0003_alter_collection_content.py
+-rw-r--r--   0        0        0     3349 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_collections/migrations/0004_alter_collection_content.py
+-rw-r--r--   0        0        0     2880 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_collections/migrations/0005_alter_collection_content.py
+-rw-r--r--   0        0        0     2460 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_collections/migrations/0006_alter_collection_content.py
+-rw-r--r--   0        0        0      385 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_collections/migrations/0007_rename_about_collection_introduction.py
+-rw-r--r--   0        0        0     2689 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_collections/migrations/0008_alter_collection_content.py
+-rw-r--r--   0        0        0      704 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_collections/migrations/0009_collection_hero_image.py
+-rw-r--r--   0        0        0     2942 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_collections/migrations/0010_collection_aapb_records_alter_collection_content.py
+-rw-r--r--   0        0        0    10573 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_collections/migrations/0011_alter_collection_aapb_records_and_more.py
+-rw-r--r--   0        0        0    13066 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_collections/migrations/0012_remove_collection_aapb_records_and_more.py
+-rw-r--r--   0        0        0        0 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_collections/migrations/__init__.py
+-rw-r--r--   0        0        0     3023 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_collections/models.py
+-rw-r--r--   0        0        0       26 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_collections/tests.py
+-rw-r--r--   0        0        0      352 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_collections/views.py
+-rw-r--r--   0        0        0       61 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_wag/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_wag/_version.py
+-rw-r--r--   0        0        0     2398 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_wag/api.py
+-rw-r--r--   0        0        0      509 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_wag/serializers.py
+-rw-r--r--   0        0        0        0 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_wag/settings/__init__.py
+-rw-r--r--   0        0        0     6917 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_wag/settings/base.py
+-rw-r--r--   0        0        0      528 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_wag/settings/dev.py
+-rw-r--r--   0        0        0     1004 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_wag/settings/production.py
+-rw-r--r--   0        0        0      614 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_wag/settings/test.py
+-rw-r--r--   0        0        0        0 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_wag/static/css/ov-wag.css
+-rw-r--r--   0        0        0        0 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_wag/static/js/ov-wag.js
+-rw-r--r--   0        0        0      238 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_wag/templates/404.html
+-rw-r--r--   0        0        0      363 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_wag/templates/500.html
+-rw-r--r--   0        0        0     1318 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_wag/templates/base.html
+-rw-r--r--   0        0        0       57 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_wag/templates/socialaccount/authentication_error.html
+-rw-r--r--   0        0        0      554 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_wag/templates/wagtailadmin/login.html
+-rw-r--r--   0        0        0        0 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_wag/templatetags/__init__.py
+-rw-r--r--   0        0        0      259 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_wag/templatetags/custom_tags.py
+-rw-r--r--   0        0        0        0 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_wag/tests/__init__.py
+-rw-r--r--   0        0        0     2201 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_wag/tests/test_api.py
+-rw-r--r--   0        0        0      569 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_wag/tests/test_env.py
+-rw-r--r--   0        0        0     1386 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_wag/urls.py
+-rw-r--r--   0        0        0      453 2024-05-20 21:13:09.383516 ov_wag-0.6.0/ov_wag/wsgi.py
+-rw-r--r--   0        0        0     2111 2024-05-20 21:13:48.523600 ov_wag-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-20 21:13:09.387516 ov_wag-0.6.0/search/__init__.py
+-rw-r--r--   0        0        0     1301 2024-05-20 21:13:09.387516 ov_wag-0.6.0/search/templates/search/search.html
+-rw-r--r--   0        0        0     1037 2024-05-20 21:13:09.387516 ov_wag-0.6.0/search/views.py
+-rw-r--r--   0        0        0     2858 1970-01-01 00:00:00.000000 ov_wag-0.6.0/PKG-INFO
```

### Comparing `ov_wag-0.5.0/README.md` & `ov_wag-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/authors/migrations/0001_initial.py` & `ov_wag-0.6.0/authors/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/authors/migrations/0002_authorsorderable.py` & `ov_wag-0.6.0/authors/migrations/0002_authorsorderable.py`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/authors/models.py` & `ov_wag-0.6.0/authors/models.py`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/cli/cli.py` & `ov_wag-0.6.0/cli/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,41 @@
-from typing import Optional
+from typing import Annotated
 
 from loguru import logger as log
 from trogon import Trogon
 from typer import Argument, Context, Option, Typer
 from typer.main import get_group
-from typing import Annotated
 
 from .utils import AliasGroup, run, version_callback
 
 COMPOSE = "docker compose -f docker-compose.yml"
 DEV = "-f dev.yml"
 MANAGE = "run --entrypoint python wagtail manage.py"
 TESTS = '-f test.yml'
 
 app = Typer(cls=AliasGroup, context_settings={'help_option_names': ['-h', '--help']})
 
 
 @app.command('d | dev')
 def dev(
     args: Annotated[
-        Optional[list[str]],
+        list[str] | None,
         Option(help='Additional arguments to pass to the build step'),
     ] = None
 ):
     """Run the dev environment"""
     if args is None:
         args = []
     run(f'{COMPOSE} {DEV} up {" ".join(args)}')
 
 
 @app.command('b | build')
 def build(
     args: Annotated[
-        Optional[list[str]],
+        list[str] | None,
         Option(help='Additional arguments to pass to the build step'),
     ] = None,
 ):
     """Build the dev environment"""
     run(f'{COMPOSE} build {" ".join(args)}')
```

### Comparing `ov_wag-0.5.0/cli/utils.py` & `ov_wag-0.6.0/cli/utils.py`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/exhibits/management/commands/rename.py` & `ov_wag-0.6.0/exhibits/management/commands/rename.py`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/exhibits/migrations/0001_initial.py` & `ov_wag-0.6.0/exhibits/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/exhibits/migrations/0002_exhibitpage_cover_image.py` & `ov_wag-0.6.0/exhibits/migrations/0002_exhibitpage_cover_image.py`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/exhibits/migrations/0003_exhibitpage_hero_image.py` & `ov_wag-0.6.0/exhibits/migrations/0003_exhibitpage_hero_image.py`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/exhibits/migrations/0004_exhibitsorderable.py` & `ov_wag-0.6.0/exhibits/migrations/0004_exhibitsorderable.py`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/exhibits/migrations/0006_alter_exhibitpage_body.py` & `ov_wag-0.6.0/exhibits/migrations/0006_alter_exhibitpage_body.py`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/exhibits/migrations/0007_alter_exhibitpage_body.py` & `ov_wag-0.6.0/exhibits/migrations/0007_alter_exhibitpage_body.py`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/exhibits/models.py` & `ov_wag-0.6.0/exhibits/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,17 +7,41 @@
 from wagtail.admin.panels import FieldPanel, InlinePanel, MultiFieldPanel
 from wagtail.api import APIField
 from wagtail.blocks import RichTextBlock
 from wagtail.fields import StreamField
 from wagtail.images.api.fields import ImageRenditionField
 from wagtail.models import Orderable, Page
 from wagtail.search import index
+from wagtail_footnotes.blocks import RichTextBlockWithFootnotes
 from wagtail_headless_preview.models import HeadlessMixin
 
 from authors.serializers import AuthorSerializer
+from ov_wag.serializers import FootnotesSerializer
+
+
+class RichTextFootnotesBlock(RichTextBlockWithFootnotes):
+    def __init__(
+        self,
+        features=(
+            'bold',
+            'italic',
+            'h2',
+            'h3',
+            'h4',
+            'ol',
+            'ul',
+            'hr',
+            'link',
+            'image',
+            'blockquote',
+            'footnotes',
+        ),
+        **kwargs,
+    ):
+        super().__init__(features=features, **kwargs)
 
 
 class ExhibitsOrderable(Orderable):
     """Ordered list of other exhibits related to this exhibit"""
 
     page = ParentalKey('exhibits.ExhibitPage', related_name='other_exhibits', null=True)
     exhibit = models.ForeignKey(
@@ -101,29 +125,28 @@
 class ExhibitPageApiSchema(ExhibitsApiSchema):
     body: list[str]
 
 
 class ExhibitPage(HeadlessMixin, Page):
     body = StreamField(
         [
-            ('text', RichTextBlock()),
+            ('text', RichTextFootnotesBlock()),
             (
                 'heading',
                 RichTextBlock(
                     form_classname='title', features=['italic'], icon='title'
                 ),
             ),
             (
                 'subheading',
                 RichTextBlock(
                     form_classname='title', features=['italic'], icon='title'
                 ),
             ),
         ],
-        use_json_field=True,
     )
 
     cover_image = models.ForeignKey(
         'wagtailimages.Image',
         null=True,
         blank=True,
         on_delete=models.SET_NULL,
@@ -149,14 +172,15 @@
         *Page.content_panels,
         MultiFieldPanel(
             [FieldPanel('cover_image'), FieldPanel('hero_image')], heading='Images'
         ),
         FieldPanel('body', classname='collapsed'),
         InlinePanel('authors', heading='Author(s)'),
         InlinePanel('other_exhibits', heading='Other Exhibits', max_num=3),
+        InlinePanel('footnotes', label='Footnotes'),
     ]
 
     promote_panels: ClassVar[list[FieldPanel]] = [
         FieldPanel(
             'featured',
             heading='Featured Exhibit',
             help_text='Featured exhibits will be displayed on the home page, and as "other exhibits" on other exhibit pages.',  # noqa: E501
@@ -180,11 +204,12 @@
             serializer=ImageRenditionField('fill-1600x500'),
         ),
         APIField(
             'hero_thumb',
             serializer=ImageRenditionField('fill-480x270', source='hero_image'),
         ),
         APIField('authors'),
+        APIField('footnotes', serializer=FootnotesSerializer()),
         OtherExhibitsField(
             'other_exhibits', serializer=OtherExhibitsSerializer(many=True)
         ),
     ]
```

### Comparing `ov_wag-0.5.0/home/migrations/0001_initial.py` & `ov_wag-0.6.0/home/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/home/migrations/0002_create_homepage.py` & `ov_wag-0.6.0/home/migrations/0002_create_homepage.py`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/home/static/css/welcome_page.css` & `ov_wag-0.6.0/home/static/css/welcome_page.css`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/home/templates/home/welcome_page.html` & `ov_wag-0.6.0/home/templates/home/welcome_page.html`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/ov_collections/blocks.py` & `ov_wag-0.6.0/ov_collections/blocks.py`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/ov_collections/migrations/0001_initial.py` & `ov_wag-0.6.0/ov_collections/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/ov_collections/migrations/0002_alter_collection_content.py` & `ov_wag-0.6.0/ov_collections/migrations/0002_alter_collection_content.py`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/ov_collections/migrations/0003_alter_collection_content.py` & `ov_wag-0.6.0/ov_collections/migrations/0003_alter_collection_content.py`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/ov_collections/migrations/0004_alter_collection_content.py` & `ov_wag-0.6.0/ov_collections/migrations/0004_alter_collection_content.py`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/ov_collections/migrations/0005_alter_collection_content.py` & `ov_wag-0.6.0/ov_collections/migrations/0005_alter_collection_content.py`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/ov_collections/migrations/0006_alter_collection_content.py` & `ov_wag-0.6.0/ov_collections/migrations/0006_alter_collection_content.py`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/ov_collections/migrations/0008_alter_collection_content.py` & `ov_wag-0.6.0/ov_collections/migrations/0008_alter_collection_content.py`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/ov_collections/migrations/0009_collection_hero_image.py` & `ov_wag-0.6.0/ov_collections/migrations/0009_collection_hero_image.py`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/ov_collections/migrations/0010_collection_aapb_records_alter_collection_content.py` & `ov_wag-0.6.0/ov_collections/migrations/0010_collection_aapb_records_alter_collection_content.py`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/ov_collections/migrations/0011_alter_collection_aapb_records_and_more.py` & `ov_wag-0.6.0/ov_collections/migrations/0011_alter_collection_aapb_records_and_more.py`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/ov_collections/migrations/0012_remove_collection_aapb_records_and_more.py` & `ov_wag-0.6.0/ov_collections/migrations/0012_remove_collection_aapb_records_and_more.py`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/ov_collections/models.py` & `ov_wag-0.6.0/ov_collections/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,14 @@
                     form_classname='title', features=['italic'], icon='title'
                 ),
             ),
             ('text', TextBlock()),
             ('image', ImageChooserBlock()),
             ('html', RawHTMLBlock(label='HTML')),
         ],
-        use_json_field=True,
     )
 
     cover_image = models.ForeignKey(
         'wagtailimages.Image',
         null=True,
         blank=True,
         on_delete=models.SET_NULL,
```

### Comparing `ov_wag-0.5.0/ov_wag/api.py` & `ov_wag-0.6.0/ov_wag/api.py`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/ov_wag/settings/base.py` & `ov_wag-0.6.0/ov_wag/settings/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     'django.contrib.auth',
     'django.contrib.contenttypes',
     'django.contrib.sessions',
     'django.contrib.messages',
     'django.contrib.staticfiles',
     'wagtail_headless_preview',
     'wagtail.contrib.search_promotions',
+    "wagtail_footnotes",
     'django.contrib.sites',
     'allauth',
     'allauth.account',
     'allauth.socialaccount',
     'allauth.socialaccount.providers.auth0',
 ]
```

### Comparing `ov_wag-0.5.0/ov_wag/settings/dev.py` & `ov_wag-0.6.0/ov_wag/settings/dev.py`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/ov_wag/settings/production.py` & `ov_wag-0.6.0/ov_wag/settings/production.py`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/ov_wag/settings/test.py` & `ov_wag-0.6.0/ov_wag/settings/test.py`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/ov_wag/templates/base.html` & `ov_wag-0.6.0/ov_wag/templates/base.html`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/ov_wag/templates/wagtailadmin/login.html` & `ov_wag-0.6.0/ov_wag/templates/wagtailadmin/login.html`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/ov_wag/tests/test_api.py` & `ov_wag-0.6.0/ov_wag/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/ov_wag/tests/test_env.py` & `ov_wag-0.6.0/ov_wag/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/ov_wag/urls.py` & `ov_wag-0.6.0/ov_wag/urls.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from django.conf import settings
 from django.contrib import admin
 from django.urls import include, path
 from wagtail import urls as wagtail_urls
 from wagtail.admin import urls as wagtailadmin_urls
 from wagtail.documents import urls as wagtaildocs_urls
+from wagtail_footnotes import urls as footnotes_urls
 
 from search import views as search_views
 
 from .api import api_router
 
 urlpatterns = [
     path('django-admin/', admin.site.urls),
     path('admin/', include(wagtailadmin_urls)),
     path('documents/', include(wagtaildocs_urls)),
     path('search/', search_views.search, name='search'),
     path('api/v2/', api_router.urls),
     path('accounts/', include('allauth.urls')),
+    path("footnotes/", include(footnotes_urls)),
 ]
 
 
 if settings.DEBUG:
     from django.conf.urls.static import static
     from django.contrib.staticfiles.urls import staticfiles_urlpatterns
```

### Comparing `ov_wag-0.5.0/pyproject.toml` & `ov_wag-0.6.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,97 +3,109 @@
 dynamic = []
 description = "WGBH Open Vault Wagtail backend"
 authors = [
     { name = "WGBH-MLA", email = "ryan_harbert@wgbh.org" },
 ]
 readme = "README.md"
 dependencies = [
-    "Django~=4.2",
-    "wagtail~=5.2",
+    "Django~=5.0",
+    "wagtail~=6.1",
     "wagtail-factories~=4.1",
-    "pydantic~=2.6",
+    "pydantic~=2.7",
     "psycopg2~=2.9",
     "python-dotenv~=1.0",
-    "gunicorn~=21.2",
-    "wagtail-headless-preview~=0.7",
+    "gunicorn~=22.0",
+    "wagtail-headless-preview~=0.8",
     "django-cors-headers~=4.3",
-    "django-allauth~=0.60",
-    "elasticsearch~=8.12",
+    "django-allauth~=0.63",
+    "elasticsearch~=8.13",
+    "wagtail-footnotes~=0.10",
 ]
-requires-python = ">=3.9,<4.0"
-version = "0.5.0"
+requires-python = ">=3.10,<4.0"
+version = "0.6.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 documentation = "https://wgbh-mla.github.io/ov-wag/"
 homepage = "https://github.com/WGBH-MLA/ov-wag"
 repository = "https://github.com/WGBH-MLA/ov-wag"
 
 [project.scripts]
 ov = "cli:app"
 
 [project.optional-dependencies]
 cli = [
-    "typer~=0.9",
+    "typer~=0.12",
     "loguru~=0.7",
     "trogon~=0.5",
 ]
 production = [
-    "gunicorn[standard]~=21.2",
+    "gunicorn[standard]~=22.0",
     "django-storages[s3]~=1.14",
 ]
-dev = [
-    "black~=24.1",
-]
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
+[tool.black]
+extend-exclude = "migrations"
+
+[tool.ruff]
+extend-exclude = [
+    "migrations",
+]
+
 [tool.pdm.version]
 source = "file"
 path = "ov_wag/_version.py"
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "ruff~=0.2",
-    "pre-commit~=3.6",
+    "black~=24.4",
+    "ruff~=0.4",
+    "pre-commit~=3.7",
 ]
 docs = [
-    "mkdocs~=1.5",
-    "mkdocs-material~=9.4",
-    "mike~=2.0",
-    "mkdocstrings[python]~=0.23",
+    "mkdocs~=1.6",
+    "mkdocs-material~=9.5",
+    "mike~=2.1",
+    "mkdocstrings[python]~=0.25",
     "mkdocs-git-revision-date-localized-plugin~=1.2",
     "mkdocs-jupyter~=0.24",
 ]
 test = [
-    "pytest~=8.0",
+    "pytest~=8.2",
     "pytest-django~=4.8",
-    "pytest-cov~=4.1",
+    "pytest-cov~=5.0",
     "pytest-sugar~=1.0",
-    "pytest-xdist~=3.5",
+    "pytest-xdist~=3.6",
     "nbmake~=1.5",
-    "coverage~=7.4",
+    "coverage~=7.5",
 ]
 
-[tool.black]
-extend-exclude = "migrations"
-
-[tool.ruff]
-extend-exclude = [
-    "migrations",
+[tool.pytest.ini_options]
+DJANGO_SETTINGS_MODULE = "ov_wag.settings.test"
+python_files = [
+    "tests.py",
+    "test_*.py",
+    "*_tests.py",
 ]
-ignore = [
-    "Q000",
+testpaths = [
+    "authors",
+    "exhibits",
+    "ov_collections",
+    "ov_wag",
 ]
+
+[lint]
 select = [
     "B",
     "C4",
     "C90",
     "E",
     "ERA",
     "F",
@@ -106,21 +118,7 @@
     "Q",
     "RET",
     "RUF",
     "SIM",
     "UP",
     "W",
 ]
-
-[tool.pytest.ini_options]
-DJANGO_SETTINGS_MODULE = "ov_wag.settings.test"
-python_files = [
-    "tests.py",
-    "test_*.py",
-    "*_tests.py",
-]
-testpaths = [
-    "authors",
-    "exhibits",
-    "ov_collections",
-    "ov_wag",
-]
```

### Comparing `ov_wag-0.5.0/search/templates/search/search.html` & `ov_wag-0.6.0/search/templates/search/search.html`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/search/views.py` & `ov_wag-0.6.0/search/views.py`

 * *Files identical despite different names*

### Comparing `ov_wag-0.5.0/PKG-INFO` & `ov_wag-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: ov-wag
-Version: 0.5.0
+Version: 0.6.0
 Summary: WGBH Open Vault Wagtail backend
 Home-page: https://github.com/WGBH-MLA/ov-wag
 Author-Email: WGBH-MLA <ryan_harbert@wgbh.org>
 License: MIT
 Project-URL: Documentation, https://wgbh-mla.github.io/ov-wag/
 Project-URL: Homepage, https://github.com/WGBH-MLA/ov-wag
 Project-URL: Repository, https://github.com/WGBH-MLA/ov-wag
-Requires-Python: <4.0,>=3.9
-Requires-Dist: Django~=4.2
-Requires-Dist: wagtail~=5.2
+Requires-Python: <4.0,>=3.10
+Requires-Dist: Django~=5.0
+Requires-Dist: wagtail~=6.1
 Requires-Dist: wagtail-factories~=4.1
-Requires-Dist: pydantic~=2.6
+Requires-Dist: pydantic~=2.7
 Requires-Dist: psycopg2~=2.9
 Requires-Dist: python-dotenv~=1.0
-Requires-Dist: gunicorn~=21.2
-Requires-Dist: wagtail-headless-preview~=0.7
+Requires-Dist: gunicorn~=22.0
+Requires-Dist: wagtail-headless-preview~=0.8
 Requires-Dist: django-cors-headers~=4.3
-Requires-Dist: django-allauth~=0.60
-Requires-Dist: elasticsearch~=8.12
-Requires-Dist: typer~=0.9; extra == "cli"
+Requires-Dist: django-allauth~=0.63
+Requires-Dist: elasticsearch~=8.13
+Requires-Dist: wagtail-footnotes~=0.10
+Requires-Dist: typer~=0.12; extra == "cli"
 Requires-Dist: loguru~=0.7; extra == "cli"
 Requires-Dist: trogon~=0.5; extra == "cli"
-Requires-Dist: gunicorn[standard]~=21.2; extra == "production"
+Requires-Dist: gunicorn[standard]~=22.0; extra == "production"
 Requires-Dist: django-storages[s3]~=1.14; extra == "production"
-Requires-Dist: black~=24.1; extra == "dev"
 Provides-Extra: cli
 Provides-Extra: production
-Provides-Extra: dev
 Description-Content-Type: text/markdown
 
 ![CI](https://github.com/WGBH-MLA/ov-wag/actions/workflows/CI.yml/badge.svg) [![Coverage Status](https://coveralls.io/repos/github/WGBH-MLA/ov-wag/badge.svg)](https://coveralls.io/github/WGBH-MLA/ov-wag)
 
 # Open Vault: Wagtail
 #### From GBH
 Wagtail CMS for [Open Vault](https://openvault.wgbh.org/)
```

