# Comparing `tmp/eea.volto.policy-3.5.zip` & `tmp/eea.volto.policy-4.0.zip`

## zipinfo {}

```diff
@@ -1,273 +1,277 @@
-Zip file size: 84255 bytes, number of entries: 271
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/docs/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea.volto.policy.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/
--rw-r--r--  2.0 unx       38 b- defN 24-May-16 09:49 eea.volto.policy-3.5/setup.cfg
--rw-r--r--  2.0 unx     2286 b- defN 24-May-16 09:49 eea.volto.policy-3.5/CONTRIBUTING.md
--rw-r--r--  2.0 unx     6223 b- defN 24-May-16 09:49 eea.volto.policy-3.5/PKG-INFO
--rw-r--r--  2.0 unx     2989 b- defN 24-May-16 09:49 eea.volto.policy-3.5/README.rst
--rw-r--r--  2.0 unx     1672 b- defN 24-May-16 09:49 eea.volto.policy-3.5/setup.py
--rw-r--r--  2.0 unx      126 b- defN 24-May-16 09:49 eea.volto.policy-3.5/MANIFEST.in
--rw-r--r--  2.0 unx     2371 b- defN 24-May-16 09:49 eea.volto.policy-3.5/docs/HISTORY.txt
--rw-r--r--  2.0 unx      915 b- defN 24-May-16 09:49 eea.volto.policy-3.5/docs/LICENSE.txt
--rw-r--r--  2.0 unx    18092 b- defN 24-May-16 09:49 eea.volto.policy-3.5/docs/LICENSE.GPL
--rw-r--r--  2.0 unx       40 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea.volto.policy.egg-info/entry_points.txt
--rw-r--r--  2.0 unx        1 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea.volto.policy.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx     6223 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea.volto.policy.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       14 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea.volto.policy.egg-info/namespace_packages.txt
--rw-r--r--  2.0 unx        1 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea.volto.policy.egg-info/not-zip-safe
--rw-r--r--  2.0 unx       49 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea.volto.policy.egg-info/requires.txt
--rw-r--r--  2.0 unx        4 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea.volto.policy.egg-info/top_level.txt
--rw-r--r--  2.0 unx     8350 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea.volto.policy.egg-info/SOURCES.txt
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/
--rw-r--r--  2.0 unx       93 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/
--rw-r--r--  2.0 unx       93 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/contentrules/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/restapi/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/upgrades/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/tests/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/behaviors/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/profiles/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/vocabularies/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/image_scales/
--rw-r--r--  2.0 unx        4 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/version.txt
--rw-r--r--  2.0 unx      671 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/configure.zcml
--rw-r--r--  2.0 unx      759 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/setuphandlers.py
--rw-r--r--  2.0 unx      357 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/interfaces.py
--rw-r--r--  2.0 unx      346 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/README.txt
--rw-r--r--  2.0 unx      355 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/overrides.zcml
--rw-r--r--  2.0 unx     1039 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/profiles.zcml
--rw-r--r--  2.0 unx      221 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/__init__.py
--rw-r--r--  2.0 unx     1092 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/contentrules/configure.zcml
--rw-r--r--  2.0 unx       22 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/contentrules/__init__.py
--rw-r--r--  2.0 unx     1964 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/contentrules/actions.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/zh_TW/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/en/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/hr/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/es/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/pt_BR/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/ro/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/eu/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/el/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/it/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/ru/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/is/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/lt/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/hu/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/nl/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/pt/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/fi/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/lv/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/sl/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/mt/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/tr/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/no/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/sv/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/bg/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/kl/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/et/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/sk/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/pl/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/cs/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/da/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/fr/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/de/
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/eea.pot
--rwxr-xr-x  2.0 unx      218 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/update.sh
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/plone-manual.pot
--rw-r--r--  2.0 unx       13 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/zh_TW/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/zh_TW/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/zh_TW/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/zh_TW/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/zh_TW/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/en/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/en/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/en/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/en/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/en/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/hr/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/hr/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/hr/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/hr/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/hr/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/es/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/es/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/es/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/es/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/es/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/pt_BR/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/pt_BR/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/pt_BR/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/pt_BR/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/pt_BR/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/ro/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/ro/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/ro/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/ro/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/ro/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/eu/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/eu/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/eu/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/eu/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/eu/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/el/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/el/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/el/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/el/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/el/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/it/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/it/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/it/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/it/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/it/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/ru/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/ru/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/ru/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/ru/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/ru/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/is/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/is/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/is/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/is/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/is/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/lt/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/lt/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/lt/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/lt/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/lt/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/hu/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/hu/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/hu/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/hu/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/hu/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/nl/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/nl/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/nl/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/nl/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/nl/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/pt/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/pt/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/pt/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/pt/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/pt/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/fi/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/fi/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/fi/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/fi/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/fi/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/lv/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/lv/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/lv/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/lv/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/lv/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/sl/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/sl/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/sl/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/sl/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/sl/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/mt/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/mt/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/mt/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/mt/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/mt/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/tr/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/tr/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/tr/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/tr/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/tr/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/no/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/no/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/no/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/no/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/no/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/sv/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/sv/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/sv/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/sv/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/sv/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/bg/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/bg/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/bg/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/bg/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/bg/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/kl/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/kl/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/kl/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/kl/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/kl/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/et/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/et/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/et/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/et/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/et/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/sk/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/sk/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/sk/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/sk/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/sk/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/pl/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/pl/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/pl/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/pl/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/pl/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/cs/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/cs/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/cs/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/cs/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/cs/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/da/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/da/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/da/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/da/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/da/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/fr/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/fr/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/fr/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/fr/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/fr/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/de/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/de/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/de/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/de/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/locales/de/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/restapi/deserializer/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/restapi/serializer/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/restapi/navigation/
--rw-r--r--  2.0 unx      213 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/restapi/configure.zcml
--rw-r--r--  2.0 unx       16 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/restapi/__init__.py
--rw-r--r--  2.0 unx      168 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/restapi/deserializer/configure.zcml
--rw-r--r--  2.0 unx     2497 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/restapi/deserializer/dxfields.py
--rw-r--r--  2.0 unx       29 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/restapi/deserializer/__init__.py
--rw-r--r--  2.0 unx      305 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/restapi/serializer/configure.zcml
--rw-r--r--  2.0 unx      961 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/restapi/serializer/summary.py
--rw-r--r--  2.0 unx     1311 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/restapi/serializer/dxfields.py
--rw-r--r--  2.0 unx       27 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/restapi/serializer/__init__.py
--rw-r--r--  2.0 unx     1547 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/restapi/navigation/navigation.py
--rw-r--r--  2.0 unx      416 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/restapi/navigation/configure.zcml
--rw-r--r--  2.0 unx     1361 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/upgrades/configure.zcml
--rw-r--r--  2.0 unx       17 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/upgrades/__init__.py
--rw-r--r--  2.0 unx     1428 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/tests/base.py
--rw-r--r--  2.0 unx      672 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/tests/test_doctests.py
--rw-r--r--  2.0 unx       14 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/tests/__init__.py
--rw-r--r--  2.0 unx      139 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/behaviors/configure.zcml
--rw-r--r--  2.0 unx       18 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/behaviors/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/profiles/uninstall/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/profiles/default/
--rw-r--r--  2.0 unx      126 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/profiles/uninstall/browserlayer.xml
--rw-r--r--  2.0 unx      179 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/profiles/default/metadata.xml
--rw-r--r--  2.0 unx      145 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/profiles/default/catalog.xml
--rw-r--r--  2.0 unx      620 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/profiles/default/contentrules.xml
--rw-r--r--  2.0 unx      780 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/profiles/default/registry.xml
--rw-r--r--  2.0 unx      173 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/profiles/default/browserlayer.xml
--rw-r--r--  2.0 unx       88 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/vocabularies/configure.zcml
--rw-r--r--  2.0 unx       21 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/vocabularies/__init__.py
--rw-r--r--  2.0 unx      346 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/image_scales/configure.zcml
--rw-r--r--  2.0 unx     5804 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/image_scales/adapters.py
--rw-r--r--  2.0 unx     7107 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/image_scales/interfaces.py
--rw-r--r--  2.0 unx      893 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/image_scales/indexer.py
--rw-r--r--  2.0 unx       42 b- defN 24-May-16 09:49 eea.volto.policy-3.5/eea/volto/policy/image_scales/__init__.py
-271 files, 85840 bytes uncompressed, 30685 bytes compressed:  64.3%
+Zip file size: 87114 bytes, number of entries: 275
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/docs/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea.volto.policy.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/
+-rw-r--r--  2.0 unx       38 b- defN 24-May-20 16:40 eea.volto.policy-4.0/setup.cfg
+-rw-r--r--  2.0 unx     2286 b- defN 24-May-20 16:40 eea.volto.policy-4.0/CONTRIBUTING.md
+-rw-r--r--  2.0 unx     6370 b- defN 24-May-20 16:40 eea.volto.policy-4.0/PKG-INFO
+-rw-r--r--  2.0 unx     2989 b- defN 24-May-20 16:40 eea.volto.policy-4.0/README.rst
+-rw-r--r--  2.0 unx     1920 b- defN 24-May-20 16:40 eea.volto.policy-4.0/setup.py
+-rw-r--r--  2.0 unx      126 b- defN 24-May-20 16:40 eea.volto.policy-4.0/MANIFEST.in
+-rw-r--r--  2.0 unx     2518 b- defN 24-May-20 16:40 eea.volto.policy-4.0/docs/HISTORY.txt
+-rw-r--r--  2.0 unx      915 b- defN 24-May-20 16:40 eea.volto.policy-4.0/docs/LICENSE.txt
+-rw-r--r--  2.0 unx    18092 b- defN 24-May-20 16:40 eea.volto.policy-4.0/docs/LICENSE.GPL
+-rw-r--r--  2.0 unx       40 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea.volto.policy.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea.volto.policy.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx     6370 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea.volto.policy.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       14 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea.volto.policy.egg-info/namespace_packages.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea.volto.policy.egg-info/not-zip-safe
+-rw-r--r--  2.0 unx       49 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea.volto.policy.egg-info/requires.txt
+-rw-r--r--  2.0 unx        4 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea.volto.policy.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     8462 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea.volto.policy.egg-info/SOURCES.txt
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/
+-rw-r--r--  2.0 unx       93 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/
+-rw-r--r--  2.0 unx       93 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/contentrules/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/restapi/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/upgrades/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/tests/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/behaviors/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/browser/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/profiles/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/vocabularies/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/image_scales/
+-rw-r--r--  2.0 unx        3 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/version.txt
+-rw-r--r--  2.0 unx      704 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/configure.zcml
+-rw-r--r--  2.0 unx      751 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/setuphandlers.py
+-rw-r--r--  2.0 unx      357 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/interfaces.py
+-rw-r--r--  2.0 unx      346 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/README.txt
+-rw-r--r--  2.0 unx      355 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/overrides.zcml
+-rw-r--r--  2.0 unx     1039 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/profiles.zcml
+-rw-r--r--  2.0 unx      221 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/__init__.py
+-rw-r--r--  2.0 unx     1092 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/contentrules/configure.zcml
+-rw-r--r--  2.0 unx       22 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/contentrules/__init__.py
+-rw-r--r--  2.0 unx     1956 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/contentrules/actions.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/zh_TW/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/en/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/hr/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/es/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/pt_BR/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/ro/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/eu/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/el/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/it/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/ru/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/is/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/lt/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/hu/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/nl/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/pt/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/fi/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/lv/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/sl/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/mt/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/tr/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/no/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/sv/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/bg/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/kl/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/et/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/sk/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/pl/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/cs/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/da/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/fr/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/de/
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/eea.pot
+-rwxr-xr-x  2.0 unx      218 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/update.sh
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/plone-manual.pot
+-rw-r--r--  2.0 unx       13 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/zh_TW/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/zh_TW/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/zh_TW/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/zh_TW/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/zh_TW/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/en/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/en/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/en/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/en/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/en/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/hr/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/hr/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/hr/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/hr/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/hr/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/es/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/es/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/es/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/es/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/es/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/pt_BR/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/pt_BR/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/pt_BR/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/pt_BR/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/pt_BR/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/ro/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/ro/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/ro/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/ro/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/ro/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/eu/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/eu/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/eu/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/eu/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/eu/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/el/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/el/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/el/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/el/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/el/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/it/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/it/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/it/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/it/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/it/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/ru/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/ru/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/ru/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/ru/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/ru/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/is/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/is/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/is/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/is/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/is/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/lt/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/lt/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/lt/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/lt/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/lt/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/hu/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/hu/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/hu/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/hu/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/hu/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/nl/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/nl/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/nl/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/nl/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/nl/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/pt/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/pt/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/pt/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/pt/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/pt/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/fi/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/fi/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/fi/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/fi/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/fi/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/lv/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/lv/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/lv/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/lv/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/lv/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/sl/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/sl/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/sl/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/sl/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/sl/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/mt/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/mt/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/mt/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/mt/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/mt/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/tr/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/tr/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/tr/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/tr/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/tr/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/no/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/no/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/no/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/no/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/no/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/sv/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/sv/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/sv/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/sv/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/sv/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/bg/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/bg/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/bg/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/bg/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/bg/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/kl/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/kl/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/kl/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/kl/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/kl/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/et/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/et/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/et/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/et/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/et/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/sk/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/sk/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/sk/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/sk/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/sk/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/pl/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/pl/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/pl/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/pl/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/pl/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/cs/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/cs/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/cs/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/cs/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/cs/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/da/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/da/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/da/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/da/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/da/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/fr/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/fr/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/fr/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/fr/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/fr/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/de/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/de/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/de/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/de/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/locales/de/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/restapi/deserializer/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/restapi/serializer/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/restapi/navigation/
+-rw-r--r--  2.0 unx      213 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/restapi/configure.zcml
+-rw-r--r--  2.0 unx       16 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/restapi/__init__.py
+-rw-r--r--  2.0 unx      168 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/restapi/deserializer/configure.zcml
+-rw-r--r--  2.0 unx     2497 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/restapi/deserializer/dxfields.py
+-rw-r--r--  2.0 unx       29 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/restapi/deserializer/__init__.py
+-rw-r--r--  2.0 unx      305 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/restapi/serializer/configure.zcml
+-rw-r--r--  2.0 unx      961 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/restapi/serializer/summary.py
+-rw-r--r--  2.0 unx     1311 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/restapi/serializer/dxfields.py
+-rw-r--r--  2.0 unx       27 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/restapi/serializer/__init__.py
+-rw-r--r--  2.0 unx     1547 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/restapi/navigation/navigation.py
+-rw-r--r--  2.0 unx      416 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/restapi/navigation/configure.zcml
+-rw-r--r--  2.0 unx     1361 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/upgrades/configure.zcml
+-rw-r--r--  2.0 unx       17 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/upgrades/__init__.py
+-rw-r--r--  2.0 unx     1420 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/tests/base.py
+-rw-r--r--  2.0 unx      672 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/tests/test_doctests.py
+-rw-r--r--  2.0 unx       14 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/tests/__init__.py
+-rw-r--r--  2.0 unx      139 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/behaviors/configure.zcml
+-rw-r--r--  2.0 unx       18 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/behaviors/__init__.py
+-rw-r--r--  2.0 unx      860 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/browser/configure.zcml
+-rw-r--r--  2.0 unx     6147 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/browser/teaser.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/browser/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/profiles/uninstall/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/profiles/default/
+-rw-r--r--  2.0 unx      126 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/profiles/uninstall/browserlayer.xml
+-rw-r--r--  2.0 unx      179 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/profiles/default/metadata.xml
+-rw-r--r--  2.0 unx      145 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/profiles/default/catalog.xml
+-rw-r--r--  2.0 unx      620 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/profiles/default/contentrules.xml
+-rw-r--r--  2.0 unx      780 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/profiles/default/registry.xml
+-rw-r--r--  2.0 unx      173 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/profiles/default/browserlayer.xml
+-rw-r--r--  2.0 unx       88 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/vocabularies/configure.zcml
+-rw-r--r--  2.0 unx       21 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/vocabularies/__init__.py
+-rw-r--r--  2.0 unx      346 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/image_scales/configure.zcml
+-rw-r--r--  2.0 unx     5788 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/image_scales/adapters.py
+-rw-r--r--  2.0 unx     7107 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/image_scales/interfaces.py
+-rw-r--r--  2.0 unx      893 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/image_scales/indexer.py
+-rw-r--r--  2.0 unx       42 b- defN 24-May-20 16:40 eea.volto.policy-4.0/eea/volto/policy/image_scales/__init__.py
+275 files, 93640 bytes uncompressed, 32804 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -1,814 +1,826 @@
-Filename: eea.volto.policy-3.5/
+Filename: eea.volto.policy-4.0/
 Comment: 
 
-Filename: eea.volto.policy-3.5/docs/
+Filename: eea.volto.policy-4.0/docs/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea.volto.policy.egg-info/
+Filename: eea.volto.policy-4.0/eea.volto.policy.egg-info/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/
+Filename: eea.volto.policy-4.0/eea/
 Comment: 
 
-Filename: eea.volto.policy-3.5/setup.cfg
+Filename: eea.volto.policy-4.0/setup.cfg
 Comment: 
 
-Filename: eea.volto.policy-3.5/CONTRIBUTING.md
+Filename: eea.volto.policy-4.0/CONTRIBUTING.md
 Comment: 
 
-Filename: eea.volto.policy-3.5/PKG-INFO
+Filename: eea.volto.policy-4.0/PKG-INFO
 Comment: 
 
-Filename: eea.volto.policy-3.5/README.rst
+Filename: eea.volto.policy-4.0/README.rst
 Comment: 
 
-Filename: eea.volto.policy-3.5/setup.py
+Filename: eea.volto.policy-4.0/setup.py
 Comment: 
 
-Filename: eea.volto.policy-3.5/MANIFEST.in
+Filename: eea.volto.policy-4.0/MANIFEST.in
 Comment: 
 
-Filename: eea.volto.policy-3.5/docs/HISTORY.txt
+Filename: eea.volto.policy-4.0/docs/HISTORY.txt
 Comment: 
 
-Filename: eea.volto.policy-3.5/docs/LICENSE.txt
+Filename: eea.volto.policy-4.0/docs/LICENSE.txt
 Comment: 
 
-Filename: eea.volto.policy-3.5/docs/LICENSE.GPL
+Filename: eea.volto.policy-4.0/docs/LICENSE.GPL
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea.volto.policy.egg-info/entry_points.txt
+Filename: eea.volto.policy-4.0/eea.volto.policy.egg-info/entry_points.txt
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea.volto.policy.egg-info/dependency_links.txt
+Filename: eea.volto.policy-4.0/eea.volto.policy.egg-info/dependency_links.txt
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea.volto.policy.egg-info/PKG-INFO
+Filename: eea.volto.policy-4.0/eea.volto.policy.egg-info/PKG-INFO
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea.volto.policy.egg-info/namespace_packages.txt
+Filename: eea.volto.policy-4.0/eea.volto.policy.egg-info/namespace_packages.txt
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea.volto.policy.egg-info/not-zip-safe
+Filename: eea.volto.policy-4.0/eea.volto.policy.egg-info/not-zip-safe
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea.volto.policy.egg-info/requires.txt
+Filename: eea.volto.policy-4.0/eea.volto.policy.egg-info/requires.txt
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea.volto.policy.egg-info/top_level.txt
+Filename: eea.volto.policy-4.0/eea.volto.policy.egg-info/top_level.txt
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea.volto.policy.egg-info/SOURCES.txt
+Filename: eea.volto.policy-4.0/eea.volto.policy.egg-info/SOURCES.txt
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/
+Filename: eea.volto.policy-4.0/eea/volto/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/__init__.py
+Filename: eea.volto.policy-4.0/eea/__init__.py
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/
+Filename: eea.volto.policy-4.0/eea/volto/policy/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/__init__.py
+Filename: eea.volto.policy-4.0/eea/volto/__init__.py
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/contentrules/
+Filename: eea.volto.policy-4.0/eea/volto/policy/contentrules/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/restapi/
+Filename: eea.volto.policy-4.0/eea/volto/policy/restapi/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/upgrades/
+Filename: eea.volto.policy-4.0/eea/volto/policy/upgrades/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/tests/
+Filename: eea.volto.policy-4.0/eea/volto/policy/tests/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/behaviors/
+Filename: eea.volto.policy-4.0/eea/volto/policy/behaviors/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/profiles/
+Filename: eea.volto.policy-4.0/eea/volto/policy/browser/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/vocabularies/
+Filename: eea.volto.policy-4.0/eea/volto/policy/profiles/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/image_scales/
+Filename: eea.volto.policy-4.0/eea/volto/policy/vocabularies/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/version.txt
+Filename: eea.volto.policy-4.0/eea/volto/policy/image_scales/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/configure.zcml
+Filename: eea.volto.policy-4.0/eea/volto/policy/version.txt
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/setuphandlers.py
+Filename: eea.volto.policy-4.0/eea/volto/policy/configure.zcml
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/interfaces.py
+Filename: eea.volto.policy-4.0/eea/volto/policy/setuphandlers.py
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/README.txt
+Filename: eea.volto.policy-4.0/eea/volto/policy/interfaces.py
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/overrides.zcml
+Filename: eea.volto.policy-4.0/eea/volto/policy/README.txt
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/profiles.zcml
+Filename: eea.volto.policy-4.0/eea/volto/policy/overrides.zcml
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/__init__.py
+Filename: eea.volto.policy-4.0/eea/volto/policy/profiles.zcml
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/contentrules/configure.zcml
+Filename: eea.volto.policy-4.0/eea/volto/policy/__init__.py
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/contentrules/__init__.py
+Filename: eea.volto.policy-4.0/eea/volto/policy/contentrules/configure.zcml
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/contentrules/actions.py
+Filename: eea.volto.policy-4.0/eea/volto/policy/contentrules/__init__.py
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/zh_TW/
+Filename: eea.volto.policy-4.0/eea/volto/policy/contentrules/actions.py
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/en/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/zh_TW/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/hr/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/en/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/es/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/hr/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/pt_BR/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/es/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/ro/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/pt_BR/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/eu/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/ro/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/el/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/eu/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/it/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/el/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/ru/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/it/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/is/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/ru/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/lt/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/is/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/hu/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/lt/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/nl/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/hu/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/pt/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/nl/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/fi/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/pt/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/lv/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/fi/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/sl/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/lv/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/mt/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/sl/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/tr/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/mt/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/no/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/tr/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/sv/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/no/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/bg/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/sv/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/kl/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/bg/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/et/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/kl/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/sk/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/et/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/pl/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/sk/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/cs/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/pl/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/da/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/cs/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/fr/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/da/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/de/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/fr/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/eea.pot
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/de/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/update.sh
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/eea.pot
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/plone-manual.pot
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/update.sh
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/__init__.py
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/plone-manual.pot
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/zh_TW/LC_MESSAGES/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/__init__.py
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/zh_TW/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/zh_TW/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/zh_TW/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/zh_TW/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/zh_TW/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/zh_TW/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/zh_TW/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/zh_TW/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/en/LC_MESSAGES/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/zh_TW/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/en/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/en/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/en/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/en/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/en/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/en/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/en/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/en/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/hr/LC_MESSAGES/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/en/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/hr/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/hr/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/hr/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/hr/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/hr/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/hr/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/hr/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/hr/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/es/LC_MESSAGES/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/hr/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/es/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/es/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/es/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/es/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/es/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/es/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/es/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/es/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/pt_BR/LC_MESSAGES/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/es/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/pt_BR/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/pt_BR/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/pt_BR/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/pt_BR/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/pt_BR/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/pt_BR/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/pt_BR/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/pt_BR/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/ro/LC_MESSAGES/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/pt_BR/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/ro/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/ro/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/ro/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/ro/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/ro/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/ro/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/ro/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/ro/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/eu/LC_MESSAGES/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/ro/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/eu/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/eu/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/eu/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/eu/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/eu/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/eu/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/eu/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/eu/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/el/LC_MESSAGES/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/eu/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/el/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/el/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/el/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/el/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/el/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/el/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/el/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/el/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/it/LC_MESSAGES/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/el/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/it/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/it/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/it/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/it/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/it/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/it/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/it/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/it/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/ru/LC_MESSAGES/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/it/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/ru/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/ru/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/ru/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/ru/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/ru/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/ru/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/ru/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/ru/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/is/LC_MESSAGES/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/ru/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/is/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/is/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/is/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/is/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/is/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/is/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/is/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/is/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/lt/LC_MESSAGES/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/is/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/lt/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/lt/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/lt/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/lt/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/lt/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/lt/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/lt/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/lt/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/hu/LC_MESSAGES/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/lt/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/hu/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/hu/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/hu/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/hu/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/hu/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/hu/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/hu/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/hu/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/nl/LC_MESSAGES/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/hu/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/nl/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/nl/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/nl/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/nl/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/nl/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/nl/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/nl/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/nl/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/pt/LC_MESSAGES/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/nl/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/pt/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/pt/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/pt/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/pt/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/pt/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/pt/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/pt/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/pt/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/fi/LC_MESSAGES/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/pt/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/fi/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/fi/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/fi/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/fi/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/fi/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/fi/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/fi/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/fi/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/lv/LC_MESSAGES/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/fi/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/lv/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/lv/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/lv/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/lv/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/lv/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/lv/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/lv/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/lv/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/sl/LC_MESSAGES/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/lv/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/sl/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/sl/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/sl/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/sl/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/sl/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/sl/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/sl/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/sl/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/mt/LC_MESSAGES/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/sl/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/mt/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/mt/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/mt/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/mt/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/mt/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/mt/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/mt/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/mt/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/tr/LC_MESSAGES/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/mt/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/tr/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/tr/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/tr/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/tr/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/tr/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/tr/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/tr/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/tr/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/no/LC_MESSAGES/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/tr/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/no/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/no/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/no/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/no/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/no/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/no/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/no/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/no/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/sv/LC_MESSAGES/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/no/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/sv/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/sv/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/sv/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/sv/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/sv/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/sv/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/sv/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/sv/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/bg/LC_MESSAGES/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/sv/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/bg/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/bg/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/bg/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/bg/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/bg/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/bg/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/bg/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/bg/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/kl/LC_MESSAGES/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/bg/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/kl/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/kl/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/kl/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/kl/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/kl/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/kl/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/kl/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/kl/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/et/LC_MESSAGES/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/kl/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/et/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/et/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/et/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/et/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/et/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/et/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/et/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/et/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/sk/LC_MESSAGES/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/et/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/sk/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/sk/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/sk/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/sk/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/sk/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/sk/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/sk/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/sk/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/pl/LC_MESSAGES/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/sk/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/pl/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/pl/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/pl/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/pl/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/pl/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/pl/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/pl/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/pl/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/cs/LC_MESSAGES/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/pl/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/cs/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/cs/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/cs/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/cs/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/cs/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/cs/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/cs/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/cs/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/da/LC_MESSAGES/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/cs/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/da/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/da/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/da/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/da/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/da/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/da/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/da/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/da/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/fr/LC_MESSAGES/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/da/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/fr/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/fr/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/fr/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/fr/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/fr/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/fr/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/fr/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/fr/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/de/LC_MESSAGES/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/fr/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/de/LC_MESSAGES/plone.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/de/LC_MESSAGES/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/de/LC_MESSAGES/eea.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/de/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/de/LC_MESSAGES/eea.mo
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/de/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/locales/de/LC_MESSAGES/plone.po
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/de/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/restapi/deserializer/
+Filename: eea.volto.policy-4.0/eea/volto/policy/locales/de/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/restapi/serializer/
+Filename: eea.volto.policy-4.0/eea/volto/policy/restapi/deserializer/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/restapi/navigation/
+Filename: eea.volto.policy-4.0/eea/volto/policy/restapi/serializer/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/restapi/configure.zcml
+Filename: eea.volto.policy-4.0/eea/volto/policy/restapi/navigation/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/restapi/__init__.py
+Filename: eea.volto.policy-4.0/eea/volto/policy/restapi/configure.zcml
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/restapi/deserializer/configure.zcml
+Filename: eea.volto.policy-4.0/eea/volto/policy/restapi/__init__.py
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/restapi/deserializer/dxfields.py
+Filename: eea.volto.policy-4.0/eea/volto/policy/restapi/deserializer/configure.zcml
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/restapi/deserializer/__init__.py
+Filename: eea.volto.policy-4.0/eea/volto/policy/restapi/deserializer/dxfields.py
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/restapi/serializer/configure.zcml
+Filename: eea.volto.policy-4.0/eea/volto/policy/restapi/deserializer/__init__.py
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/restapi/serializer/summary.py
+Filename: eea.volto.policy-4.0/eea/volto/policy/restapi/serializer/configure.zcml
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/restapi/serializer/dxfields.py
+Filename: eea.volto.policy-4.0/eea/volto/policy/restapi/serializer/summary.py
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/restapi/serializer/__init__.py
+Filename: eea.volto.policy-4.0/eea/volto/policy/restapi/serializer/dxfields.py
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/restapi/navigation/navigation.py
+Filename: eea.volto.policy-4.0/eea/volto/policy/restapi/serializer/__init__.py
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/restapi/navigation/configure.zcml
+Filename: eea.volto.policy-4.0/eea/volto/policy/restapi/navigation/navigation.py
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/upgrades/configure.zcml
+Filename: eea.volto.policy-4.0/eea/volto/policy/restapi/navigation/configure.zcml
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/upgrades/__init__.py
+Filename: eea.volto.policy-4.0/eea/volto/policy/upgrades/configure.zcml
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/tests/base.py
+Filename: eea.volto.policy-4.0/eea/volto/policy/upgrades/__init__.py
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/tests/test_doctests.py
+Filename: eea.volto.policy-4.0/eea/volto/policy/tests/base.py
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/tests/__init__.py
+Filename: eea.volto.policy-4.0/eea/volto/policy/tests/test_doctests.py
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/behaviors/configure.zcml
+Filename: eea.volto.policy-4.0/eea/volto/policy/tests/__init__.py
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/behaviors/__init__.py
+Filename: eea.volto.policy-4.0/eea/volto/policy/behaviors/configure.zcml
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/profiles/uninstall/
+Filename: eea.volto.policy-4.0/eea/volto/policy/behaviors/__init__.py
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/profiles/default/
+Filename: eea.volto.policy-4.0/eea/volto/policy/browser/configure.zcml
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/profiles/uninstall/browserlayer.xml
+Filename: eea.volto.policy-4.0/eea/volto/policy/browser/teaser.py
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/profiles/default/metadata.xml
+Filename: eea.volto.policy-4.0/eea/volto/policy/browser/__init__.py
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/profiles/default/catalog.xml
+Filename: eea.volto.policy-4.0/eea/volto/policy/profiles/uninstall/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/profiles/default/contentrules.xml
+Filename: eea.volto.policy-4.0/eea/volto/policy/profiles/default/
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/profiles/default/registry.xml
+Filename: eea.volto.policy-4.0/eea/volto/policy/profiles/uninstall/browserlayer.xml
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/profiles/default/browserlayer.xml
+Filename: eea.volto.policy-4.0/eea/volto/policy/profiles/default/metadata.xml
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/vocabularies/configure.zcml
+Filename: eea.volto.policy-4.0/eea/volto/policy/profiles/default/catalog.xml
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/vocabularies/__init__.py
+Filename: eea.volto.policy-4.0/eea/volto/policy/profiles/default/contentrules.xml
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/image_scales/configure.zcml
+Filename: eea.volto.policy-4.0/eea/volto/policy/profiles/default/registry.xml
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/image_scales/adapters.py
+Filename: eea.volto.policy-4.0/eea/volto/policy/profiles/default/browserlayer.xml
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/image_scales/interfaces.py
+Filename: eea.volto.policy-4.0/eea/volto/policy/vocabularies/configure.zcml
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/image_scales/indexer.py
+Filename: eea.volto.policy-4.0/eea/volto/policy/vocabularies/__init__.py
 Comment: 
 
-Filename: eea.volto.policy-3.5/eea/volto/policy/image_scales/__init__.py
+Filename: eea.volto.policy-4.0/eea/volto/policy/image_scales/configure.zcml
+Comment: 
+
+Filename: eea.volto.policy-4.0/eea/volto/policy/image_scales/adapters.py
+Comment: 
+
+Filename: eea.volto.policy-4.0/eea/volto/policy/image_scales/interfaces.py
+Comment: 
+
+Filename: eea.volto.policy-4.0/eea/volto/policy/image_scales/indexer.py
+Comment: 
+
+Filename: eea.volto.policy-4.0/eea/volto/policy/image_scales/__init__.py
 Comment: 
 
 Zip file comment:
```

## Comparing `eea.volto.policy-3.5/CONTRIBUTING.md` & `eea.volto.policy-4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

## Comparing `eea.volto.policy-3.5/PKG-INFO` & `eea.volto.policy-4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eea.volto.policy
-Version: 3.5
+Version: 4.0
 Summary: An add-on for Plone
 Home-page: https://github.com/eea/eea.volto.policy
 Author: European Environment Agency: IDM2 A-Team
 Author-email: eea-edw-a-team-alerts@googlegroups.com
 License: GPL version 2
 Keywords: EEA Add-ons Plone Zope
 Classifier: Environment :: Web Environment
@@ -124,14 +124,19 @@
 
 .. _EEA: https://www.eea.europa.eu/
 .. _`EEA Web Systems Training`: http://www.youtube.com/user/eeacms/videos?view=1
 
 Changelog
 =========
 
+4.0 - (2024-05-20)
+---------------------------
+* Feature: Migrate teaserGrid to gridBlock structure from Volto 17 core
+  [avoinea - refs #265726]
+
 3.5 - (2024-05-14)
 ---------------------------
 * Change: feat(serializer): added effective to the default_metadata_fields
   [ichim-david]
 
 3.4 - (2024-03-28)
 ---------------------------
```

## Comparing `eea.volto.policy-3.5/README.rst` & `eea.volto.policy-4.0/README.rst`

 * *Files identical despite different names*

## Comparing `eea.volto.policy-3.5/setup.py` & `eea.volto.policy-4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,25 +2,33 @@
 """
 import os
 from os.path import join
 from setuptools import setup, find_packages
 
 NAME = 'eea.volto.policy'
 PATH = NAME.split('.') + ['version.txt']
-VERSION = open(join(*PATH)).read().strip()
+VERSION = ""
+with open(join(*PATH), "r", encoding="utf-8") as version_file:
+    VERSION = version_file.read().strip()
+
+LONG_DESCRIPTION = ""
+with open("README.rst", "r", encoding="utf-8") as readme_file:
+    LONG_DESCRIPTION = readme_file.read()
+
+with open(os.path.join("docs", "HISTORY.txt"),
+          "r", encoding="utf-8") as hfile:
+    LONG_DESCRIPTION += "\n" + hfile.read()
+
 
 setup(
     name=NAME,
     version=VERSION,
     description="An add-on for Plone",
     long_description_content_type="text/x-rst",
-    long_description=(
-        open("README.rst").read() + "\n" +
-        open(os.path.join("docs", "HISTORY.txt")).read()
-    ),
+    long_description=LONG_DESCRIPTION,
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
         "Framework :: Plone :: 5.2",
         "Framework :: Plone :: 6.0",
         "Programming Language :: Python",
```

## Comparing `eea.volto.policy-3.5/docs/HISTORY.txt` & `eea.volto.policy-4.0/docs/HISTORY.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+4.0 - (2024-05-20)
+---------------------------
+* Feature: Migrate teaserGrid to gridBlock structure from Volto 17 core
+  [avoinea - refs #265726]
+
 3.5 - (2024-05-14)
 ---------------------------
 * Change: feat(serializer): added effective to the default_metadata_fields
   [ichim-david]
 
 3.4 - (2024-03-28)
 ---------------------------
```

## Comparing `eea.volto.policy-3.5/docs/LICENSE.txt` & `eea.volto.policy-4.0/docs/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `eea.volto.policy-3.5/docs/LICENSE.GPL` & `eea.volto.policy-4.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

## Comparing `eea.volto.policy-3.5/eea.volto.policy.egg-info/PKG-INFO` & `eea.volto.policy-4.0/eea.volto.policy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eea.volto.policy
-Version: 3.5
+Version: 4.0
 Summary: An add-on for Plone
 Home-page: https://github.com/eea/eea.volto.policy
 Author: European Environment Agency: IDM2 A-Team
 Author-email: eea-edw-a-team-alerts@googlegroups.com
 License: GPL version 2
 Keywords: EEA Add-ons Plone Zope
 Classifier: Environment :: Web Environment
@@ -124,14 +124,19 @@
 
 .. _EEA: https://www.eea.europa.eu/
 .. _`EEA Web Systems Training`: http://www.youtube.com/user/eeacms/videos?view=1
 
 Changelog
 =========
 
+4.0 - (2024-05-20)
+---------------------------
+* Feature: Migrate teaserGrid to gridBlock structure from Volto 17 core
+  [avoinea - refs #265726]
+
 3.5 - (2024-05-14)
 ---------------------------
 * Change: feat(serializer): added effective to the default_metadata_fields
   [ichim-david]
 
 3.4 - (2024-03-28)
 ---------------------------
```

## Comparing `eea.volto.policy-3.5/eea.volto.policy.egg-info/SOURCES.txt` & `eea.volto.policy-4.0/eea.volto.policy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 eea/volto/policy/interfaces.py
 eea/volto/policy/overrides.zcml
 eea/volto/policy/profiles.zcml
 eea/volto/policy/setuphandlers.py
 eea/volto/policy/version.txt
 eea/volto/policy/behaviors/__init__.py
 eea/volto/policy/behaviors/configure.zcml
+eea/volto/policy/browser/__init__.py
+eea/volto/policy/browser/configure.zcml
+eea/volto/policy/browser/teaser.py
 eea/volto/policy/contentrules/__init__.py
 eea/volto/policy/contentrules/actions.py
 eea/volto/policy/contentrules/configure.zcml
 eea/volto/policy/image_scales/__init__.py
 eea/volto/policy/image_scales/adapters.py
 eea/volto/policy/image_scales/configure.zcml
 eea/volto/policy/image_scales/indexer.py
```

## Comparing `eea.volto.policy-3.5/eea/volto/policy/configure.zcml` & `eea.volto.policy-4.0/eea/volto/policy/configure.zcml`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,15 @@
   i18n_domain="eea">
 
   <i18n:registerTranslations directory="locales" />
 
   <include package="plone.volto" />
   <include file="profiles.zcml" />
 
+  <include package=".browser" />
   <include package=".behaviors" />
   <include package=".contentrules" />
   <include package=".restapi" />
   <include package=".vocabularies" />
   <include package=".upgrades" />
 
   <configure zcml:condition="not-installed Products.CMFPlone.image_scales">
```

## Comparing `eea.volto.policy-3.5/eea/volto/policy/setuphandlers.py` & `eea.volto.policy-4.0/eea/volto/policy/setuphandlers.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from zope.interface import implementer
 
 
 logger = logging.getLogger("eea.volto.policy")
 
 
 @implementer(INonInstallable)
-class HiddenProfiles(object):
+class HiddenProfiles:
     """ Hidden profiles
     """
 
     def getNonInstallableProfiles(self):
         """ Hide uninstall profile from site-creation and quickinstaller.
         """
         return [
```

## Comparing `eea.volto.policy-3.5/eea/volto/policy/profiles.zcml` & `eea.volto.policy-4.0/eea/volto/policy/profiles.zcml`

 * *Files identical despite different names*

## Comparing `eea.volto.policy-3.5/eea/volto/policy/contentrules/configure.zcml` & `eea.volto.policy-4.0/eea/volto/policy/contentrules/configure.zcml`

 * *Files identical despite different names*

## Comparing `eea.volto.policy-3.5/eea/volto/policy/contentrules/actions.py` & `eea.volto.policy-4.0/eea/volto/policy/contentrules/actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     summary = (
         "I will set publication date to null"
     )
 
 
 @implementer(IExecutable)
 @adapter(Interface, ISetPublicationDateToNullAction, Interface)
-class SetPublicationDateToNullExecutor(object):
+class SetPublicationDateToNullExecutor:
     """Set Publication Date to null executor"""
 
     def __init__(self, context, element, event):
         self.context = context
         self.element = element
         self.event = event
```

## Comparing `eea.volto.policy-3.5/eea/volto/policy/restapi/deserializer/dxfields.py` & `eea.volto.policy-4.0/eea/volto/policy/restapi/deserializer/dxfields.py`

 * *Files identical despite different names*

## Comparing `eea.volto.policy-3.5/eea/volto/policy/restapi/serializer/summary.py` & `eea.volto.policy-4.0/eea/volto/policy/restapi/serializer/summary.py`

 * *Files identical despite different names*

## Comparing `eea.volto.policy-3.5/eea/volto/policy/restapi/serializer/dxfields.py` & `eea.volto.policy-4.0/eea/volto/policy/restapi/serializer/dxfields.py`

 * *Files identical despite different names*

## Comparing `eea.volto.policy-3.5/eea/volto/policy/restapi/navigation/navigation.py` & `eea.volto.policy-4.0/eea/volto/policy/restapi/navigation/navigation.py`

 * *Files identical despite different names*

## Comparing `eea.volto.policy-3.5/eea/volto/policy/upgrades/configure.zcml` & `eea.volto.policy-4.0/eea/volto/policy/upgrades/configure.zcml`

 * *Files identical despite different names*

## Comparing `eea.volto.policy-3.5/eea/volto/policy/tests/base.py` & `eea.volto.policy-4.0/eea/volto/policy/tests/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 """
 from plone.testing import z2
 from plone.app.testing import TEST_USER_ID
 from plone.app.testing import PloneSandboxLayer
 from plone.app.testing import applyProfile
 from plone.app.testing import FunctionalTesting
 from plone.app.testing import setRoles
+import eea.volto.policy
 
 
 class EEAFixture(PloneSandboxLayer):
     """ EEA Testing Policy
     """
     def setUpZope(self, app, configurationContext):
         """ Setup Zope
         """
-        import eea.volto.policy
         self.loadZCML(package=eea.volto.policy)
         z2.installProduct(app, 'eea.volto.policy')
 
 
     def setUpPloneSite(self, portal):
         """ Setup Plone
         """
```

## Comparing `eea.volto.policy-3.5/eea/volto/policy/tests/test_doctests.py` & `eea.volto.policy-4.0/eea/volto/policy/tests/test_doctests.py`

 * *Files identical despite different names*

## Comparing `eea.volto.policy-3.5/eea/volto/policy/profiles/default/contentrules.xml` & `eea.volto.policy-4.0/eea/volto/policy/profiles/default/contentrules.xml`

 * *Files identical despite different names*

## Comparing `eea.volto.policy-3.5/eea/volto/policy/profiles/default/registry.xml` & `eea.volto.policy-4.0/eea/volto/policy/profiles/default/registry.xml`

 * *Files identical despite different names*

## Comparing `eea.volto.policy-3.5/eea/volto/policy/image_scales/adapters.py` & `eea.volto.policy-4.0/eea/volto/policy/image_scales/adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     IImageScalesFieldAdapter,
     IImagingSchema,
 )
 
 
 @implementer(IImageScalesAdapter)
 @adapter(IDexterityContent, Interface)
-class ImageScales(object):
+class ImageScales:
     """
     Adapter for getting image scales
     """
 
     def __init__(self, context, request):
         self.context = context
         self.request = request
@@ -70,15 +70,15 @@
     )
     allowed_sizes = imaging_settings.allowed_sizes
     return [_split_scale_info(size) for size in allowed_sizes]
 
 
 @implementer(IImageScalesFieldAdapter)
 @adapter(INamedImageField, IDexterityContent, Interface)
-class ImageFieldScales(object):
+class ImageFieldScales:
     """
     Image scale serializer
     """
 
     def __init__(self, field, context, request):
         self.context = context
         self.request = request
```

## Comparing `eea.volto.policy-3.5/eea/volto/policy/image_scales/interfaces.py` & `eea.volto.policy-4.0/eea/volto/policy/image_scales/interfaces.py`

 * *Files identical despite different names*

## Comparing `eea.volto.policy-3.5/eea/volto/policy/image_scales/indexer.py` & `eea.volto.policy-4.0/eea/volto/policy/image_scales/indexer.py`

 * *Files identical despite different names*

