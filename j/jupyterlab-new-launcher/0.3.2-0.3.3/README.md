# Comparing `tmp/jupyterlab_new_launcher-0.3.2.tar.gz` & `tmp/jupyterlab_new_launcher-0.3.3.tar.gz`

## Comparing `jupyterlab_new_launcher-0.3.2.tar` & `jupyterlab_new_launcher-0.3.3.tar`

### file list

```diff
@@ -1,64 +1,66 @@
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/.copier-answers.yml
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/CHANGELOG.md
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/babel.config.js
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/jest.config.js
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/junit.xml
--rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/setup.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/tsconfig.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/tsconfig.test.json
--rw-r--r--   0        0        0   376569 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/yarn.lock
--rw-r--r--   0        0        0    54951 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/docs/images/dialog.png
--rw-r--r--   0        0        0    58321 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/docs/images/launcher.png
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/jupyterlab_new_launcher/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/jupyterlab_new_launcher/_version.py
--rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/jupyterlab_new_launcher/labextension/package.json
--rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/package.json.orig
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/plugin.json
--rw-r--r--   0        0        0    11071 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/jupyterlab_new_launcher/labextension/static/728.5be4ee0b94a07decd5f8.js
--rw-r--r--   0        0        0    28580 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/jupyterlab_new_launcher/labextension/static/787.35a3d65624680cd50b5a.js
--rw-r--r--   0        0        0     7174 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/jupyterlab_new_launcher/labextension/static/remoteEntry.655eac004954212534b3.js
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/jupyterlab_new_launcher/labextension/static/style.js
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/jupyterlab_new_launcher/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/schema/plugin.json
--rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/src/commands.ts
--rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/src/database.ts
--rw-r--r--   0        0        0     9601 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/src/dialogs.tsx
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/src/icons.ts
--rw-r--r--   0        0        0     6052 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/src/index.ts
--rw-r--r--   0        0        0     4729 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/src/item.ts
--rw-r--r--   0        0        0    10204 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/src/launcher.tsx
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/src/svg.d.ts
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/src/types.ts
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/src/typings.d.ts
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/src/__tests__/jupyterlab_new_launcher.spec.ts
--rw-r--r--   0        0        0     6346 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/src/components/base-table.tsx
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/src/components/card.tsx
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/src/components/section.tsx
--rw-r--r--   0        0        0    12213 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/src/components/table.tsx
--rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/style/index.js
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/style/webkit.raw.css
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/style/icons/code-server.svg
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/style/icons/md/LICENSE
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/style/icons/md/file.svg
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/style/icons/md/star.svg
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/ui-tests/playwright.config.js
--rw-r--r--   0        0        0   148126 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/ui-tests/yarn.lock
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/ui-tests/tests/jupyterlab_new_launcher.spec.ts
--rw-r--r--   0        0        0    27608 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-linux.png
--rw-r--r--   0        0        0    28063 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-search-in-individual-linux.png
--rw-r--r--   0        0        0    33928 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-with-starred-linux.png
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/.gitignore
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/LICENSE
--rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/README.md
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/.copier-answers.yml
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/CHANGELOG.md
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/babel.config.js
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/jest.config.js
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/junit.xml
+-rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/setup.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/tsconfig.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/tsconfig.test.json
+-rw-r--r--   0        0        0   376569 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/yarn.lock
+-rw-r--r--   0        0        0    54951 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/docs/images/dialog.png
+-rw-r--r--   0        0        0    58321 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/docs/images/launcher.png
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/jupyterlab_new_launcher/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/jupyterlab_new_launcher/_version.py
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/jupyterlab_new_launcher/labextension/package.json
+-rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/package.json.orig
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/plugin.json
+-rw-r--r--   0        0        0    11071 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/jupyterlab_new_launcher/labextension/static/728.5be4ee0b94a07decd5f8.js
+-rw-r--r--   0        0        0    30575 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/jupyterlab_new_launcher/labextension/static/787.27ef72da905b049778be.js
+-rw-r--r--   0        0        0     7174 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/jupyterlab_new_launcher/labextension/static/remoteEntry.a10a814d39706cd65aea.js
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/jupyterlab_new_launcher/labextension/static/style.js
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/jupyterlab_new_launcher/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/schema/plugin.json
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/src/commands.ts
+-rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/src/database.ts
+-rw-r--r--   0        0        0    10672 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/src/dialogs.tsx
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/src/icons.ts
+-rw-r--r--   0        0        0     7271 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/src/index.ts
+-rw-r--r--   0        0        0     4627 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/src/item.ts
+-rw-r--r--   0        0        0    10633 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/src/launcher.tsx
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/src/svg.d.ts
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/src/types.ts
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/src/typings.d.ts
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/src/__tests__/jupyterlab_new_launcher.spec.ts
+-rw-r--r--   0        0        0     6346 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/src/components/base-table.tsx
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/src/components/card.tsx
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/src/components/section.tsx
+-rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/src/components/table.tsx
+-rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/style/index.js
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/style/webkit.raw.css
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/style/icons/code-server.svg
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/style/icons/md/LICENSE
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/style/icons/md/file.svg
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/style/icons/md/star.svg
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0   148126 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/ui-tests/yarn.lock
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/ui-tests/tests/jupyterlab_new_launcher.spec.ts
+-rw-r--r--   0        0        0    27608 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-linux.png
+-rw-r--r--   0        0        0    28063 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-search-in-individual-linux.png
+-rw-r--r--   0        0        0    33928 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-with-starred-linux.png
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/table-context-menu-linux.png
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/table-context-menu-visible-columns-linux.png
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/.gitignore
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/LICENSE
+-rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/README.md
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.3.3/PKG-INFO
```

### Comparing `jupyterlab_new_launcher-0.3.2/.copier-answers.yml` & `jupyterlab_new_launcher-0.3.3/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.2/RELEASE.md` & `jupyterlab_new_launcher-0.3.3/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.2/jest.config.js` & `jupyterlab_new_launcher-0.3.3/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.2/package.json` & `jupyterlab_new_launcher-0.3.3/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.3.3'"}*

```diff
@@ -195,9 +195,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.3.2"
+    "version": "0.3.3"
 }
```

### Comparing `jupyterlab_new_launcher-0.3.2/tsconfig.json` & `jupyterlab_new_launcher-0.3.3/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.2/yarn.lock` & `jupyterlab_new_launcher-0.3.3/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.2/docs/images/dialog.png` & `jupyterlab_new_launcher-0.3.3/docs/images/dialog.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.2/docs/images/launcher.png` & `jupyterlab_new_launcher-0.3.3/docs/images/launcher.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.2/jupyterlab_new_launcher/__init__.py` & `jupyterlab_new_launcher-0.3.3/jupyterlab_new_launcher/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.2/jupyterlab_new_launcher/labextension/package.json` & `jupyterlab_new_launcher-0.3.3/jupyterlab_new_launcher/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9788194444444445%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.a10a814d39706cd65aea.js'}}",*

 * * "'version'": "'0.3.3'"}*

```diff
@@ -108,15 +108,15 @@
         "src/**/*.{ts,tsx}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/nebari-dev/jupyterlab-new-launcher",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.655eac004954212534b3.js",
+            "load": "static/remoteEntry.a10a814d39706cd65aea.js",
             "style": "./style"
         },
         "disabledExtensions": [
             "@jupyterlab/launcher-extension",
             "@jupyterlab/apputils-extension:sessionDialogs"
         ],
         "extension": true,
@@ -200,9 +200,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.3.2"
+    "version": "0.3.3"
 }
```

### Comparing `jupyterlab_new_launcher-0.3.2/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/package.json.orig` & `jupyterlab_new_launcher-0.3.3/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.3.3'"}*

```diff
@@ -195,9 +195,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.3.2"
+    "version": "0.3.3"
 }
```

### Comparing `jupyterlab_new_launcher-0.3.2/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/plugin.json` & `jupyterlab_new_launcher-0.3.3/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.2/jupyterlab_new_launcher/labextension/static/728.5be4ee0b94a07decd5f8.js` & `jupyterlab_new_launcher-0.3.3/jupyterlab_new_launcher/labextension/static/728.5be4ee0b94a07decd5f8.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.2/jupyterlab_new_launcher/labextension/static/787.35a3d65624680cd50b5a.js` & `jupyterlab_new_launcher-0.3.3/jupyterlab_new_launcher/labextension/static/787.27ef72da905b049778be.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 "use strict";
 (self.webpackChunkjupyterlab_new_launcher = self.webpackChunkjupyterlab_new_launcher || []).push([
     [787], {
         787: (e, t, n) => {
             n.r(t), n.d(t, {
-                default: () => V
+                default: () => W
             });
             var a = n(626),
                 s = n(923),
                 o = n(670),
                 r = n(260),
                 l = n(825),
                 c = n(265),
@@ -23,85 +23,95 @@
                     name: "jupyterlab-new-launcher:file",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">\n  <path class="jp-icon3" fill="rgb(97,97,97)" d="M13.81 22H6C4.89 22 4 21.11 4 20V4C4 2.9 4.89 2 6 2H14L20 8V13.09C19.67 13.04 19.34 13 19 13S18.33 13.04 18 13.09V9H13V4H6V20H13.09C13.21 20.72 13.46 21.39 13.81 22M23 18H20V15H18V18H15V20H18V23H20V20H23V18Z" />\n</svg>'
                 }),
                 g = new i.LabIcon({
                     name: "jupyterlab-new-launcher:code-server",
                     svgstr: '<svg width="64" viewBox="0 0 2250 2250" version="1.1" xmlns="http://www.w3.org/2000/svg" style="fill-rule:evenodd;clip-rule:evenodd;stroke-linejoin:round;stroke-miterlimit:2;">\n<g class="jp-icon0" fill="#000" style="fill-rule:nonzero;">\n  <path d="M1991.66,1034.72c-38.493,0 -64.144,-22.57 -64.144,-68.897l-0,-266.084c-0,-169.867 -69.982,-263.709 -250.762,-263.709l-83.976,0l-0,179.368l25.661,0c71.144,0 104.967,39.201 104.967,109.285l0,235.201c0,102.156 30.324,143.733 96.806,165.114c-66.482,20.196 -96.806,62.958 -96.806,165.114l0,174.621c0,48.7 0,96.216 -12.829,144.917c-12.829,45.141 -33.823,87.903 -62.98,124.726c-16.329,21.386 -34.991,39.202 -55.981,55.835l-0,23.755l83.971,-0c180.781,-0 250.763,-93.843 250.763,-263.709l-0,-266.084c-0,-47.516 24.485,-68.897 64.144,-68.897l47.822,-0l-0,-179.37l-46.656,-0l0,-1.186Z"/>\n  <path d="M1420.16,706.904l-258.923,0c-5.833,0 -10.495,-4.752 -10.495,-10.691l-0,-20.192c-0,-5.941 4.662,-10.692 10.495,-10.692l260.089,0c5.83,0 10.495,4.751 10.495,10.692l0,20.192c0,5.939 -5.833,10.691 -11.661,10.691Z" />\n  <path d="M1464.48,963.474l-188.942,0c-5.833,0 -10.501,-4.754 -10.501,-10.693l0,-20.192c0,-5.938 4.668,-10.691 10.501,-10.691l188.942,-0c5.833,-0 10.495,4.753 10.495,10.691l-0,20.192c-0,4.754 -4.662,10.693 -10.495,10.693Z"/>\n  <path d="M1539.12,835.188l-377.885,0c-5.833,0 -10.495,-4.75 -10.495,-10.689l-0,-20.196c-0,-5.939 4.662,-10.69 10.495,-10.69l376.719,0c5.833,0 10.499,4.751 10.499,10.69l-0,20.196c-0,4.75 -3.5,10.689 -9.333,10.689Z"/>\n  <path d="M861.493,765.074c25.658,0 51.319,2.376 75.811,8.316l0,-48.705c0,-68.897 34.989,-109.285 104.971,-109.285l25.658,0l-0,-179.368l-83.977,0c-180.781,0 -250.758,93.842 -250.758,263.709l0,87.901c40.819,-14.252 83.977,-22.568 128.295,-22.568Z"/>\n  <path d="M1618.44,1411.25c-18.662,-150.861 -132.962,-276.776 -279.919,-305.285c-40.818,-8.314 -81.642,-9.504 -121.295,-2.376c-1.166,-0 -1.166,-1.189 -2.332,-1.189c-64.148,-136.605 -201.772,-226.884 -351.063,-226.884c-149.289,-0 -285.747,87.905 -351.062,224.51c-1.166,-0 -1.166,1.188 -2.332,1.188c-41.987,-4.753 -83.975,-2.379 -125.963,8.314c-144.623,35.634 -254.257,159.175 -274.085,308.847c-2.332,15.441 -3.499,30.883 -3.499,45.141c0,45.136 30.325,86.713 74.645,92.652c54.817,8.317 102.636,-34.448 101.469,-89.089c0,-8.317 0,-17.821 1.167,-26.134c9.331,-76.025 66.48,-140.168 141.123,-157.99c23.328,-5.939 46.654,-7.124 68.814,-3.559c71.146,9.502 141.124,-27.324 171.449,-91.467c22.162,-47.516 57.151,-89.094 103.804,-111.664c51.314,-24.946 109.633,-28.506 163.286,-9.499c55.979,20.192 97.966,62.954 123.627,116.409c26.824,52.27 39.653,89.093 96.805,96.221c23.325,3.559 88.639,2.374 113.132,1.185c47.82,0 95.64,16.631 129.463,51.079c22.156,23.757 38.485,53.455 45.486,86.715c10.495,53.455 -2.334,106.908 -33.825,147.296c-22.162,28.509 -52.485,49.89 -86.308,59.394c-16.329,4.754 -32.657,5.939 -48.986,5.939l-257.757,0c-51.314,0 -92.138,-41.573 -92.138,-93.842l0,-348.049c0,-14.251 -11.661,-26.13 -25.658,-26.13l-36.156,0c-71.148,1.185 -128.295,81.964 -128.295,167.488l-0,312.415c-0,92.652 73.476,167.488 164.451,167.488c0,0 404.714,-1.19 410.544,-1.19c93.304,-9.503 179.614,-58.204 237.927,-133.04c58.319,-72.46 85.142,-167.492 73.481,-264.894Z"/>\n</g></svg>'
                 });
-            var v = n(602);
-            class f {
+            var f = n(602);
+            class v {
                 constructor(e) {
-                    var t, n, a, s, o;
-                    this._options = e, this._refreshLastUsed = new v.Signal(this), this._refreshClock = null, this._lastUsed = null;
+                    var t, n, a, s;
+                    this._options = e, this._refreshLastUsed = new f.Signal(this), this._refreshClock = null;
                     const {
-                        item: r,
-                        commands: l,
-                        lastUsedDatabase: c,
-                        favoritesDatabase: i,
-                        cwd: d
-                    } = e, m = {
-                        ...r.args,
-                        cwd: d
+                        item: o,
+                        commands: r,
+                        cwd: l
+                    } = e, c = {
+                        ...o.args,
+                        cwd: l
                     };
-                    this.command = r.command, this.args = m, this.category = r.category, this.rank = r.rank, this.kernelIconUrl = r.kernelIconUrl, this.metadata = null !== (t = r.metadata) && void 0 !== t ? t : {}, this.iconClass = l.iconClass(r.command, m), this.icon = l.icon(r.command, m), this.caption = l.caption(r.command, m), this.label = l.label(r.command, m), this.lastUsed = c.get(r), this.starred = null !== (n = i.get(r)) && void 0 !== n && n;
-                    const u = this.metadata.kernel;
-                    if (u) {
-                        const e = (null !== (a = u.conda_env_name) && void 0 !== a ? a : "").match(/(?<namespace>.+)-(?<duplicate>\1)-(?<environment>.+)/);
+                    this.command = o.command, this.args = c, this.category = o.category, this.rank = o.rank, this.kernelIconUrl = o.kernelIconUrl, this.metadata = null !== (t = o.metadata) && void 0 !== t ? t : {}, this.iconClass = r.iconClass(o.command, c), this.icon = r.icon(o.command, c), this.caption = r.caption(o.command, c), this.label = r.label(o.command, c);
+                    const i = this.metadata.kernel;
+                    if (i) {
+                        const e = (null !== (n = i.conda_env_name) && void 0 !== n ? n : "").match(/(?<namespace>.+)-(?<duplicate>\1)-(?<environment>.+)/);
                         if (e && this.metadata) {
                             const t = e.groups;
-                            this.label = null !== (s = u.conda_language) && void 0 !== s ? s : t.environment, this.metadata = {
+                            this.label = null !== (a = i.conda_language) && void 0 !== a ? a : t.environment, this.metadata = {
                                 ...this.metadata,
                                 kernel: {
                                     Namespace: t.namespace,
                                     conda_env_name: t.environment,
-                                    ...u
+                                    ...i
                                 }
                             }
                         }
                     }
-                    "server-proxy:open" === this.command && (null === (o = this.kernelIconUrl) || void 0 === o ? void 0 : o.endsWith("/vscode")) && (this.icon = g)
+                    "server-proxy:open" === this.command && (null === (s = this.kernelIconUrl) || void 0 === s ? void 0 : s.endsWith("/vscode")) && (this.icon = g)
+                }
+                get starred() {
+                    var e;
+                    const {
+                        item: t,
+                        favoritesDatabase: n
+                    } = this._options;
+                    return null !== (e = n.get(t)) && void 0 !== e && e
                 }
                 get lastUsed() {
-                    return this._lastUsed
+                    const e = this._lastUsed;
+                    return this._setRefreshClock(e), e
                 }
-                set lastUsed(e) {
-                    this._lastUsed = e, this._setRefreshClock()
+                get _lastUsed() {
+                    const {
+                        item: e,
+                        lastUsedDatabase: t
+                    } = this._options;
+                    return t.get(e)
                 }
                 get refreshLastUsed() {
                     return this._refreshLastUsed
                 }
                 async execute() {
                     const {
                         item: e,
                         commands: t,
                         lastUsedDatabase: n
                     } = this._options;
-                    await t.execute(e.command, this.args), await n.recordAsUsedNow(e), this.lastUsed = n.get(e), this._refreshLastUsed.emit()
+                    await t.execute(e.command, this.args), await n.recordAsUsedNow(e), this._refreshLastUsed.emit()
                 }
-                async markAsUsed() {
+                async markAsUsedNow() {
                     const {
                         item: e,
                         lastUsedDatabase: t
                     } = this._options;
-                    await t.recordAsUsedNow(e), this.lastUsed = t.get(e), this._refreshLastUsed.emit()
+                    await t.recordAsUsedNow(e), this._refreshLastUsed.emit()
                 }
-                toggleStar() {
+                async toggleStar() {
                     const {
                         item: e,
                         favoritesDatabase: t
                     } = this._options, n = !t.get(e);
-                    return this.starred = n, t.set(e, n)
+                    return t.set(e, n)
                 }
-                _setRefreshClock() {
-                    const e = this._lastUsed;
+                _setRefreshClock(e) {
                     if (null !== this._refreshClock && (window.clearTimeout(this._refreshClock), this._refreshClock = null), !e) return;
                     const t = Date.now() - e.getTime(),
                         n = t < 6e4 ? 1e4 : t < 36e5 ? 6e4 : 36e5;
                     this._refreshClock = window.setTimeout((() => {
-                        this._refreshLastUsed.emit(), this._setRefreshClock()
+                        this._refreshLastUsed.emit(), this._setRefreshClock(this._lastUsed)
                     }), n)
                 }
             }
             var b = n(702);
             const _ = "jp-sortable-table";
 
             function w(e) {
@@ -185,35 +195,35 @@
                                     if (!r.current) throw Error("Cannot resize: no reference to the current table");
                                     console.warn("Resize cache for column was not available"), n = r.current.getBoundingClientRect().left
                                 } else n = d;
                                 o(t.clientX - n), e.onResize()
                             }
                         },
                         n = e => {
-                            l && (document.body.classList.remove(v), c(!1), e.stopImmediatePropagation())
+                            l && (document.body.classList.remove(f), c(!1), e.stopImmediatePropagation())
                         };
                     return document.body.addEventListener("pointermove", t), document.body.addEventListener("pointerup", n), () => {
                         document.body.removeEventListener("pointermove", t), document.body.removeEventListener("pointerup", n)
                     }
                 }));
                 const p = [];
                 n && p.push("jp-sorted-header"), l && p.push("jp-header-resizing");
                 const g = "jp-sortable-table-resize-handle",
-                    v = "jp-mod-resize-table";
+                    f = "jp-mod-resize-table";
                 return u().createElement("th", {
                     key: e.id,
                     ref: r,
                     onClick: () => e.onSort(),
                     className: p.join(" "),
                     "data-id": e.id,
                     style: {
                         width: null !== s ? `${Math.max(null!==(t=e.minWidth)&&void 0!==t?t:50,s)}px` : ""
                     },
                     onPointerDown: e => {
-                        e.target instanceof HTMLElement && e.target.className === g && (document.body.classList.add(v), c(!0))
+                        e.target instanceof HTMLElement && e.target.className === g && (document.body.classList.add(f), c(!0))
                     }
                 }, u().createElement("div", {
                     className: "jp-sortable-table-th-wrapper"
                 }, u().createElement("label", null, e.label), u().createElement(a.react, {
                     tag: "span",
                     className: "jp-sort-icon"
                 })), u().createElement("div", {
@@ -222,17 +232,17 @@
             }
             var C = n(262);
             const k = "jupyterlab-new-launcher:plugin";
             var E;
             ! function(e) {
                 e.create = "launcher:create", e.moveColumn = "new-launcher:table-move-column", e.toggleColumn = "new-launcher:table-toggle-column"
             }(E || (E = {}));
-            const j = new C.Token("jupyterlab-new-launcher:ILauncherDatabase", "Databases for new launcher."),
-                D = "jp-starIconButton",
-                L = "jp-TableKernelItem";
+            const D = new C.Token("jupyterlab-new-launcher:ILauncherDatabase", "Databases for new launcher."),
+                L = "jp-starIconButton",
+                j = "jp-TableKernelItem";
 
             function N(e) {
                 if (0 === e.length) return "(empty)";
                 switch (e) {
                     case "conda_env_name":
                         return "Environment";
                     case "conda_env_path":
@@ -246,31 +256,45 @@
                     case "conda_is_currently_running":
                         return "Running?"
                 }
                 return e[0].toUpperCase() + e.substring(1)
             }
 
             function S(e) {
+                const [t, n] = m.useState(void 0), a = m.useRef(null);
                 return m.createElement("div", {
                     className: "jp-ellipsis-wrapper",
                     title: e.title
                 }, m.createElement("div", {
-                    className: "jp-ellipsis"
+                    className: "jp-ellipsis",
+                    title: t,
+                    ref: a,
+                    onMouseEnter: () => {
+                        if (e.title) return;
+                        const t = a.current;
+                        t && t.scrollWidth > t.clientWidth ? n(t.innerText) : n(void 0)
+                    }
                 }, e.children))
             }
 
-            function I(e) {
+            function U(e) {
                 var t, n, a, s;
                 const {
                     trans: o
                 } = e;
                 let r, l;
                 const [c, d] = m.useState("");
                 e.showSearchBox ? (r = c, l = d) : r = e.query;
-                const [, u] = m.useReducer((e => e + 1), 0), p = new Set;
+                const [, u] = m.useReducer((e => e + 1), 0);
+                m.useEffect((() => (e.favouritesChanged.connect(u), () => {
+                    e.favouritesChanged.disconnect(u)
+                }))), m.useEffect((() => (e.lastUsedChanged.connect(u), () => {
+                    e.lastUsedChanged.disconnect(u)
+                })));
+                const p = new Set;
                 for (const n of e.items) {
                     const e = null === (t = n.metadata) || void 0 === t ? void 0 : t.kernel;
                     if (e)
                         for (const t of Object.keys(e)) p.add(t)
                 }
                 const g = [...p].map((e => ({
                     id: e,
@@ -295,19 +319,19 @@
                 })));
                 e.showWidgetType && g.push({
                     id: "widget-type",
                     label: o.__("Type"),
                     renderCell: e => e.command.split(":")[0],
                     sort: (e, t) => e.command.localeCompare(t.command)
                 });
-                const v = [{
+                const f = [{
                         id: "kernel",
                         label: o.__("Kernel"),
                         renderCell: t => m.createElement(S, null, m.createElement("span", {
-                            className: L,
+                            className: j,
                             onClick: n => {
                                 e.onClick(t), n.stopPropagation()
                             },
                             onKeyDown: e => {
                                 "Enter" === e.key && t.execute()
                             },
                             tabIndex: 0
@@ -336,37 +360,37 @@
                     }, {
                         id: "star",
                         label: "",
                         renderCell: e => {
                             const t = e.starred,
                                 n = t ? o.__("Click to remove the kernel from favourites") : o.__("Click to add this kernel to favourites");
                             return m.createElement("button", {
-                                className: t ? `${D} jp-mod-starred` : D,
+                                className: t ? `${L} jp-mod-starred` : L,
                                 title: n,
-                                onClick: t => {
-                                    e.toggleStar(), u(), t.stopPropagation()
+                                onClick: async t => {
+                                    t.stopPropagation(), await e.toggleStar()
                                 }
                             }, m.createElement(h.react, {
                                 className: "jp-starIcon"
                             }))
                         },
                         sort: (e, t) => Number(e.starred) - Number(t.starred)
                     }],
-                    f = null !== (n = e.hideColumns) && void 0 !== n ? n : [],
-                    _ = v.filter((e => !f.includes(e.id))),
+                    v = null !== (n = e.hideColumns) && void 0 !== n ? n : [],
+                    _ = f.filter((e => !v.includes(e.id))),
                     [y, C] = m.useState(null !== (a = e.settings.composite.hiddenColumns) && void 0 !== a ? a : {}),
                     k = _.map((e => e.id)),
-                    [j, I] = m.useState(null !== (s = e.settings.composite.columnOrder) && void 0 !== s ? s : k),
-                    U = w,
+                    [D, U] = m.useState(null !== (s = e.settings.composite.columnOrder) && void 0 !== s ? s : k),
+                    I = w,
                     x = () => {
                         var t, n;
                         const a = null !== (t = e.settings.composite.hiddenColumns) && void 0 !== t ? t : {};
                         y !== a && C(a);
                         const s = null !== (n = e.settings.composite.columnOrder) && void 0 !== n ? n : k;
-                        j !== s && I(s)
+                        D !== s && U(s)
                     };
                 return m.useEffect((() => (e.settings.changed.connect(x), () => {
                     e.settings.changed.disconnect(x)
                 }))), m.createElement("div", {
                     className: "jp-NewLauncher-table"
                 }, e.showSearchBox ? m.createElement("div", {
                     className: "jp-Launcher-searchBox"
@@ -379,19 +403,21 @@
                     useFuzzyFilter: !1
                 })) : null, m.createElement("div", {
                     className: "jp-NewLauncher-table-scroller",
                     onContextMenu: t => {
                         var n;
                         t.preventDefault();
                         const a = new i.MenuSvg({
-                                commands: e.commands
-                            }),
-                            s = new i.MenuSvg({
-                                commands: e.commands
-                            });
+                            commands: e.commands
+                        });
+                        a.addClass("jp-NewLauncher-contextMenu");
+                        const s = new i.MenuSvg({
+                            commands: e.commands
+                        });
+                        s.addClass("jp-NewLauncher-contextMenu-visibleColumns");
                         for (const e of _) s.addItem({
                             command: E.toggleColumn,
                             args: {
                                 id: e.id,
                                 label: e.label
                             }
                         });
@@ -400,53 +426,65 @@
                             submenu: s
                         });
                         const r = null === (n = t.target.closest("th[data-id]")) || void 0 === n ? void 0 : n.dataset.id;
                         r && (a.addItem({
                             command: E.moveColumn,
                             args: {
                                 direction: "left",
-                                order: j,
+                                order: D,
                                 id: r
                             }
                         }), a.addItem({
                             command: E.moveColumn,
                             args: {
                                 direction: "right",
-                                order: j,
+                                order: D,
                                 id: r
                             }
                         })), a.open(t.clientX, t.clientY)
                     }
-                }, m.createElement(U, {
-                    rows: e.items.filter((e => -1 !== e.label.toLowerCase().indexOf(r.toLowerCase()))).map((e => ({
+                }, m.createElement(I, {
+                    rows: e.items.filter((e => {
+                        var t;
+                        const n = r.toLowerCase();
+                        if (e.label.toLowerCase().includes(n)) return !0;
+                        const a = null === (t = e.metadata) || void 0 === t ? void 0 : t.kernel;
+                        if (a) {
+                            for (const e of p) {
+                                const t = a[e];
+                                if ("string" == typeof t && t.toLowerCase().includes(n)) return !0
+                            }
+                            return !1
+                        }
+                    })).map((e => ({
                         data: e,
                         key: e.command + JSON.stringify(e.args)
                     }))),
                     blankIndicator: () => m.createElement("div", null, o.__("No entries")),
                     sortKey: "kernel",
                     onRowClick: e => {
                         const t = e.target,
                             n = t.closest("tr");
                         if (!n) return;
                         const a = t.closest("td"),
-                            s = null == a ? void 0 : a.querySelector(`.${D}`);
+                            s = null == a ? void 0 : a.querySelector(`.${L}`);
                         if (s) return s.click();
-                        n.querySelector(`.${L}`).click()
+                        n.querySelector(`.${j}`).click()
                     },
                     columns: _.filter((e => "hidden" !== y[e.id])).map((e => {
                         var t;
                         return {
                             ...e,
-                            rank: null !== (t = j.indexOf(e.id)) && void 0 !== t ? t : 10
+                            rank: null !== (t = D.indexOf(e.id)) && void 0 !== t ? t : 10
                         }
                     })).sort(((e, t) => e.rank - t.rank))
                 })))
             }
 
-            function U(e) {
+            function I(e) {
                 const [t, n] = m.useState(e.open);
                 return m.createElement("details", {
                     onToggle: t => {
                         n(t.currentTarget.open), e.onToggled && e.onToggled(t.currentTarget.open)
                     },
                     className: (0, i.classes)(e.className, "jp-CollapsibleSection"),
                     open: t
@@ -488,19 +526,19 @@
                 var t;
                 const {
                     trans: n,
                     cwd: a,
                     typeItems: s,
                     otherItems: o,
                     favouritesChanged: r
-                } = e, [l, c] = m.useState(""), [, d] = m.useReducer((e => e + 1), 0), [u, g] = m.useState(e.settings.composite.starredSection), [v, f] = m.useState(e.settings.composite.searchAllSections), b = () => {
+                } = e, [l, c] = m.useState(""), [, d] = m.useReducer((e => e + 1), 0), [u, g] = m.useState(e.settings.composite.starredSection), [f, v] = m.useState(e.settings.composite.searchAllSections), b = () => {
                     const t = e.settings.composite.starredSection;
                     u !== t && g(t);
                     const n = e.settings.composite.searchAllSections;
-                    v !== n && f(n)
+                    f !== n && v(n)
                 };
                 if (m.useEffect((() => (e.settings.changed.connect(b), () => {
                         e.settings.changed.disconnect(b)
                     }))), r) {
                     const e = () => {
                         u && d()
                     };
@@ -523,77 +561,83 @@
                 }, m.createElement("div", {
                     className: "jp-Launcher-cwd"
                 }, m.createElement("h3", null, n.__("Current folder:"), " ", m.createElement("code", null, a || "/"))), m.createElement("div", {
                     className: "jp-NewLauncher-OtherItems"
                 }, o.map((e => m.createElement(x, {
                     item: e,
                     trans: n
-                }))))), v ? m.createElement("div", {
+                }))))), f ? m.createElement("div", {
                     className: "jp-Launcher-searchBox"
                 }, m.createElement(i.FilterBox, {
                     placeholder: n.__("Filter"),
                     updateFilter: (e, t) => {
                         c(null != t ? t : "")
                     },
                     initialQuery: "",
                     useFuzzyFilter: !1
-                })) : null, m.createElement(U, {
+                })) : null, m.createElement(I, {
                     className: "jp-Launcher-openByType",
                     title: n.__("Create Empty"),
                     icon: p,
                     open: "collapsed" !== y["create-empty"]
                 }, s.filter((e => !l || -1 !== e.label.toLowerCase().indexOf(l.toLowerCase()))).map((e => m.createElement(x, {
                     item: e,
                     trans: n
-                })))), u ? m.createElement(U, {
+                })))), u ? m.createElement(I, {
                     className: "jp-Launcher-openByKernel",
                     title: n.__("Starred"),
                     icon: h,
                     open: "collapsed" !== y.starred
-                }, w.length > 0 ? m.createElement(I, {
+                }, w.length > 0 ? m.createElement(U, {
                     items: w,
                     commands: e.commands,
-                    showSearchBox: !v,
+                    showSearchBox: !f,
                     showWidgetType: !0,
                     query: l,
                     settings: e.settings,
                     trans: n,
-                    onClick: e => e.execute()
-                }) : "No starred items") : null, m.createElement(U, {
+                    onClick: e => e.execute(),
+                    favouritesChanged: e.favouritesChanged,
+                    lastUsedChanged: e.lastUsedChanged
+                }) : "No starred items") : null, m.createElement(I, {
                     className: "jp-Launcher-openByKernel jp-Launcher-launchNotebook",
                     title: n.__("Launch New Notebook"),
                     icon: i.notebookIcon,
                     open: "collapsed" !== y["launch-notebook"]
-                }, m.createElement(I, {
+                }, m.createElement(U, {
                     items: e.notebookItems,
                     commands: e.commands,
-                    showSearchBox: !v,
+                    showSearchBox: !f,
                     query: l,
                     settings: e.settings,
                     trans: n,
-                    onClick: e => e.execute()
-                })), m.createElement(U, {
+                    onClick: e => e.execute(),
+                    favouritesChanged: e.favouritesChanged,
+                    lastUsedChanged: e.lastUsedChanged
+                })), m.createElement(I, {
                     className: "jp-Launcher-openByKernel jp-Launcher-launchConsole",
                     title: n.__("Launch New Console"),
                     icon: i.consoleIcon,
                     open: "collapsed" !== y["launch-console"]
-                }, m.createElement(I, {
+                }, m.createElement(U, {
                     items: e.consoleItems,
                     commands: e.commands,
-                    showSearchBox: !v,
+                    showSearchBox: !f,
                     query: l,
                     settings: e.settings,
                     trans: n,
-                    onClick: e => e.execute()
+                    onClick: e => e.execute(),
+                    favouritesChanged: e.favouritesChanged,
+                    lastUsedChanged: e.lastUsedChanged
                 })))
             }
             const K = "server-proxy:open";
-            class T extends r.Launcher {
+            class M extends r.Launcher {
                 constructor(e) {
-                    super(e), this.renderCommand = e => new f({
+                    super(e), this.renderCommand = e => new v({
                         item: e,
                         cwd: this.cwd,
                         commands: this.commands,
                         lastUsedDatabase: this._lastUsedDatabase,
                         favoritesDatabase: this._favoritesDatabase
                     }), this.renderKernelCommand = e => this.renderCommand(e), this.commands = e.commands, this.trans = this.translator.load("jupyterlab-new-launcher"), this._lastUsedDatabase = e.lastUsedDatabase, this._favoritesDatabase = e.favoritesDatabase, this._settings = e.settings
                 }
@@ -631,19 +675,20 @@
                         cwd: this.cwd,
                         commands: this.commands,
                         typeItems: h,
                         notebookItems: d,
                         consoleItems: u,
                         otherItems: r,
                         settings: this._settings,
-                        favouritesChanged: this._favoritesDatabase.changed
+                        favouritesChanged: this._favoritesDatabase.changed,
+                        lastUsedChanged: this._lastUsedDatabase.changed
                     })
                 }
             }
-            class A extends s.SessionContextDialogs {
+            class T extends s.SessionContextDialogs {
                 constructor(e) {
                     var t;
                     super(e), this.options = e;
                     const n = null !== (t = e.translator) && void 0 !== t ? t : c.nullTranslator;
                     this.trans = n.load("jupyterlab")
                 }
                 async selectKernel(e) {
@@ -673,15 +718,16 @@
                                 commands: this.options.commands,
                                 favoritesDatabase: this.options.database.favorites,
                                 lastUsedDatabase: this.options.database.lastUsed,
                                 settings: l,
                                 trans: t,
                                 acceptDialog: () => {
                                     c.resolve(1)
-                                }
+                                },
+                                type: e.type
                             }),
                             buttons: a,
                             checkbox: r ? {
                                 label: t.__("Always start the preferred kernel"),
                                 caption: t.__("Remember my choice and always start the preferred kernel"),
                                 checked: o
                             } : null
@@ -694,30 +740,30 @@
                         autoStartDefault: i.isChecked
                     });
                     const d = i.value;
                     if (null === d && !e.hasNoKernel) return e.shutdown();
                     d && await e.changeKernel(d)
                 }
             }
-            const M = {
+            const A = {
                 id: "jupyterlab-new-launcher:dialogs",
                 description: "Session dialogs for redesigned JupyterLab launcher",
                 provides: s.ISessionContextDialogs,
                 autoStart: !0,
-                requires: [c.ITranslator, j, l.ISettingRegistry],
-                activate: (e, t, n, a) => new A({
+                requires: [c.ITranslator, D, l.ISettingRegistry],
+                activate: (e, t, n, a) => new T({
                     translator: t,
                     database: n,
                     commands: e.commands,
                     settingRegistry: a
                 })
             };
             class R extends s.ReactWidget {
                 constructor(e) {
-                    super(), this.options = e, this.renderKernelCommand = e => new f({
+                    super(), this.options = e, this.renderKernelCommand = e => new v({
                         item: e,
                         cwd: "",
                         commands: this.commands,
                         lastUsedDatabase: this._lastUsedDatabase,
                         favoritesDatabase: this._favoritesDatabase
                     }), this._selection = null, this.commands = e.commands, this._lastUsedDatabase = e.lastUsedDatabase, this._favoritesDatabase = e.favoritesDatabase, this._settings = e.settings, this._name = e.name, this.trans = e.trans
                 }
@@ -729,91 +775,106 @@
                         const e = this.node.getBoundingClientRect();
                         this.node.style.minWidth = e.width + "px", this.node.style.minHeight = e.height + "px"
                     }))
                 }
                 render() {
                     var e;
                     const t = [],
-                        n = this.options.data.specs.kernelspecs;
+                        n = this.options.data.specs.kernelspecs,
+                        a = "console" === this.options.type ? "console:create" : "notebook:create-new";
                     for (const e of Object.values(n)) {
                         if (!e) continue;
                         const n = e.resources["logo-svg"] || e.resources["logo-64x64"];
                         t.push({
-                            command: "notebook:create-new",
-                            args: {
+                            command: a,
+                            args: "console" === this.options.type ? {
+                                isLauncher: !0,
+                                kernelPreference: {
+                                    name: e.name
+                                }
+                            } : {
                                 isLauncher: !0,
                                 kernelName: e.name
                             },
                             kernelIconUrl: n,
                             metadata: {
                                 kernel: C.JSONExt.deepCopy(e.metadata || {})
                             }
                         })
                     }
-                    const a = [];
+                    const s = [];
                     for (const t of this.options.data.sessions) {
-                        const s = t.kernel;
-                        if (!s) continue;
-                        const o = n[s.name],
-                            r = o.resources["logo-svg"] || o.resources["logo-64x64"];
-                        a.push({
-                            command: "notebook:create-new",
-                            args: {
+                        const o = t.kernel;
+                        if (!o) continue;
+                        const r = n[o.name],
+                            l = r.resources["logo-svg"] || r.resources["logo-64x64"];
+                        s.push({
+                            command: a,
+                            args: "console" === this.options.type ? {
                                 isLauncher: !0,
-                                kernelName: o.name
+                                kernelPreference: {
+                                    name: r.name
+                                }
+                            } : {
+                                isLauncher: !0,
+                                kernelName: r.name
                             },
-                            kernelIconUrl: r,
+                            kernelIconUrl: l,
                             metadata: {
                                 kernel: {
-                                    ...C.JSONExt.deepCopy(o.metadata || {}),
-                                    state: null !== (e = s.execution_state) && void 0 !== e ? e : "running",
+                                    ...C.JSONExt.deepCopy(r.metadata || {}),
+                                    state: null !== (e = o.execution_state) && void 0 !== e ? e : "running",
                                     "used by": t.name
                                 },
-                                model: s
+                                model: o
                             }
                         })
                     }
-                    const s = t.map(this.renderKernelCommand),
-                        o = a.map(this.renderKernelCommand);
+                    const o = t.map(this.renderKernelCommand),
+                        r = s.map(this.renderKernelCommand);
                     return m.createElement(m.Fragment, null, m.createElement("h3", {
                         className: "jp-KernelSelector-Section"
-                    }, this.trans.__('Start a new kernel for "%1"', this._name)), m.createElement(I, {
+                    }, this.trans.__('Start a new kernel for "%1"', this._name)), m.createElement(U, {
                         trans: this.trans,
                         commands: this.commands,
-                        items: s,
+                        items: o,
                         settings: this._settings,
                         query: "",
                         showSearchBox: !0,
                         onClick: e => {
                             this._selection = e, this.options.acceptDialog()
-                        }
-                    }), o.length > 0 ? m.createElement(m.Fragment, null, m.createElement("h3", {
+                        },
+                        favouritesChanged: this._favoritesDatabase.changed,
+                        lastUsedChanged: this._lastUsedDatabase.changed
+                    }), r.length > 0 ? m.createElement(m.Fragment, null, m.createElement("h3", {
                         className: "jp-KernelSelector-Section"
-                    }, this.trans.__("Connect to a running kernel")), m.createElement(I, {
+                    }, this.trans.__("Connect to a running kernel")), m.createElement(U, {
                         trans: this.trans,
                         commands: this.commands,
-                        items: o,
+                        items: r,
                         settings: this._settings,
                         query: "",
                         showSearchBox: !1,
                         onClick: e => {
                             this._selection = e, this.options.acceptDialog()
                         },
-                        hideColumns: ["last-used", "star"]
+                        hideColumns: ["last-used", "star"],
+                        favouritesChanged: this._favoritesDatabase.changed,
+                        lastUsedChanged: this._lastUsedDatabase.changed
                     })) : null)
                 }
                 getValue() {
                     var e;
-                    return this._selection ? (null === (e = this._selection.metadata) || void 0 === e ? void 0 : e.model) ? this._selection.metadata.model : {
+                    return this._selection ? (this._selection.markAsUsedNow().catch(console.warn), (null === (e = this._selection.metadata) || void 0 === e ? void 0 : e.model) ? this._selection.metadata.model : {
                         name: this._selection.args.kernelName
-                    } : null
+                    }) : null
                 }
             }
-            var O = n(101);
-            class z {
+            var z = n(101);
+            class O {
                 constructor(e) {
                     this._updateDB = async () => {
                         const e = await this._fetch();
                         this._db = e
                     }, this._db = null, this._stateDB = e.stateDB;
                     const t = new C.PromiseDelegate;
                     this.ready = t.promise, this._updateDB().then((() => t.resolve())), window.setInterval(this._updateDB, e.fetchInterval)
@@ -826,147 +887,176 @@
                     this._db = n, n[this._itemKey(e)] = t, await this._stateDB.save(this._stateDBKey, n)
                 }
                 async _fetch() {
                     let e = await this._stateDB.fetch(this._stateDBKey);
                     return void 0 === e && (e = await this._stateDB.fetch(this._stateDBKey)), void 0 === e ? {} : e
                 }
             }
-            class H extends z {
+            class H extends O {
                 _itemKey(e) {
                     return e.command + "_" + JSON.stringify(e.args)
                 }
             }
             class F extends H {
                 constructor() {
-                    super(...arguments), this._stateDBKey = "new-launcher:last-used"
+                    super(...arguments), this._stateDBKey = "new-launcher:last-used", this._changed = new f.Signal(this)
                 }
                 get(e) {
                     const t = super._get(e);
                     return t ? new Date(t) : null
                 }
                 async recordAsUsedNow(e) {
-                    this._set(e, (new Date).toUTCString())
+                    await this.recordAsUsed(e, new Date)
+                }
+                async recordAsUsed(e, t) {
+                    await this._set(e, t.toUTCString()), this._changed.emit()
+                }
+                get changed() {
+                    return this._changed
                 }
             }
-            class q extends H {
+            class P extends H {
                 constructor() {
-                    super(...arguments), this._stateDBKey = "new-launcher:favorites", this._changed = new v.Signal(this)
+                    super(...arguments), this._stateDBKey = "new-launcher:favorites", this._changed = new f.Signal(this)
                 }
                 get(e) {
                     var t;
                     return null !== (t = super._get(e)) && void 0 !== t ? t : null
                 }
                 async set(e, t) {
-                    this._set(e, t), this._changed.emit()
+                    await this._set(e, t), this._changed.emit()
                 }
                 get changed() {
                     return this._changed
                 }
             }
-            const P = {
+            const q = {
                     id: "jupyterlab-new-launcher:database",
                     description: "A redesigned JupyterLab launcher databases",
-                    provides: j,
+                    provides: D,
                     autoStart: !0,
-                    requires: [O.IStateDB],
+                    requires: [z.IStateDB],
                     activate: (e, t) => {
                         const n = {
                             stateDB: t,
                             fetchInterval: 1e4
                         };
                         return {
                             lastUsed: new F(n),
-                            favorites: new q(n)
+                            favorites: new P(n)
                         }
                     }
                 },
-                V = [{
+                W = [{
                     id: k,
                     description: "A redesigned JupyterLab launcher",
                     provides: r.ILauncher,
                     autoStart: !0,
-                    requires: [c.ITranslator, l.ISettingRegistry, j],
+                    requires: [c.ITranslator, l.ISettingRegistry, D],
                     optional: [a.ILabShell, s.ICommandPalette, o.IDefaultFileBrowser],
                     activate: function(e, t, n, a, o, l, c) {
                         const {
                             commands: m,
                             shell: u
                         } = e, h = t.load("jupyterlab-new-launcher"), p = new r.LauncherModel;
                         if (-1 !== navigator.userAgent.indexOf("AppleWebKit") && -1 === navigator.userAgent.indexOf("Chrome")) {
                             const e = function(e) {
                                 const t = document.createElement("style");
                                 return t.setAttribute("type", "text/css"), t.appendChild(document.createTextNode(".jp-starIconButton {\n  /* do not rotate on webkit as the result is off when zoomed in see https://bugs.webkit.org/show_bug.cgi?id=194903 */\n  --jp-transition-transform: rotate(0deg);\n}\n\n.jp-starIcon .jp-star-filled,\n.jp-starIcon .jp-star-border {\n  /* disable animation on webkit */\n  transition-property: none;\n}\n")), t
                             }();
                             document.body.appendChild(e)
                         }
-                        return n.load(k).then((t => {
+                        n.load(k).then((t => {
                             ! function(e, t, n) {
                                 e.commands.addCommand(E.toggleColumn, {
                                     label: e => {
                                         if (e.label) return e.label;
                                         if (e.id) {
                                             const t = e.id;
                                             return t[0].toLocaleUpperCase() + t.substring(1)
                                         }
                                         return t.__("Toggle given column")
                                     },
                                     execute: async e => {
                                         var t;
                                         const a = e.id;
                                         if (!a) return console.error("Column ID missing");
-                                        const s = null !== (t = n.user.hiddenColumns) && void 0 !== t ? t : {};
+                                        const s = null !== (t = n.composite.hiddenColumns) && void 0 !== t ? t : {};
                                         "visible" !== s[a] && s[a] ? s[a] = "visible" : s[a] = "hidden", await n.set("hiddenColumns", s)
                                     },
                                     isToggleable: !0,
                                     isToggled: e => {
                                         var t;
                                         const a = e.id;
-                                        return a ? "hidden" !== (null !== (t = n.user.hiddenColumns) && void 0 !== t ? t : {})[a] : (console.error("Column ID missing for checking if toggled"), !1)
+                                        return a ? "hidden" !== (null !== (t = n.composite.hiddenColumns) && void 0 !== t ? t : {})[a] : (console.error("Column ID missing for checking if toggled"), !1)
                                     }
                                 }), e.commands.addCommand(E.moveColumn, {
                                     label: e => "left" === e.direction ? t.__("Move Column Left") : "right" === e.direction ? t.__("Move Column Right") : t.__("Move column left or right"),
                                     execute: async e => {
                                         const t = e.order,
                                             a = e.id,
                                             s = t.indexOf(a),
                                             o = s + ("left" === e.direction ? -1 : 1);
                                         if (o < 0 || o >= t.length) return void console.log("Cannot move the column any further");
                                         const r = t[o];
                                         t[o] = a, t[s] = r, await n.set("columnOrder", t)
                                     }
                                 })
                             }(e, h, t)
-                        })), m.addCommand(E.create, {
+                        }));
+                        const g = {},
+                            f = async () => {
+                                const t = [...e.serviceManager.sessions.running()];
+                                for (const e of t) {
+                                    if (!e.kernel) continue;
+                                    let t;
+                                    t = "notebook" === e.type ? "notebook:create-new" : "console" === e.type ? "console:create" : "unknown";
+                                    const n = t + "-" + e.kernel.name,
+                                        s = e.kernel.last_activity;
+                                    if (s && g[n] !== s) {
+                                        g[n] = s;
+                                        const o = {
+                                            command: t,
+                                            args: {
+                                                isLauncher: !0,
+                                                kernelName: e.kernel.name
+                                            }
+                                        };
+                                        await a.lastUsed.recordAsUsed(o, new Date(s))
+                                    }
+                                }
+                            };
+                        return e.serviceManager.sessions.ready.then(f), e.serviceManager.sessions.runningChanged.connect(f), m.addCommand(E.create, {
                             label: h.__("New Launcher"),
                             icon: e => e.toolbar ? i.addIcon : void 0,
                             execute: async e => {
                                 var r, l;
                                 const g = null !== (l = null !== (r = e.cwd) && void 0 !== r ? r : null == c ? void 0 : c.model.path) && void 0 !== l ? l : "",
-                                    v = "launcher-" + W.id++,
-                                    f = await n.load(k);
+                                    f = "launcher-" + V.id++,
+                                    v = await n.load(k);
                                 await Promise.all([a.lastUsed.ready, a.favorites.ready]);
-                                const b = new T({
+                                const b = new M({
                                     model: p,
                                     cwd: g,
                                     callback: e => {
                                         (0, d.find)(u.widgets("main"), (t => t === e)) && (u.add(e, "main", {
-                                            ref: v
+                                            ref: f
                                         }), b.dispose())
                                     },
                                     commands: m,
                                     translator: t,
                                     lastUsedDatabase: a.lastUsed,
                                     favoritesDatabase: a.favorites,
-                                    settings: f
+                                    settings: v
                                 });
                                 b.model = p, b.title.icon = i.launcherIcon, b.title.label = h.__("Launcher");
                                 const _ = new s.MainAreaWidget({
                                     content: b
                                 });
-                                if (_.title.closable = !!Array.from(u.widgets("main")).length, _.id = v, u.add(_, "main", {
+                                if (_.title.closable = !!Array.from(u.widgets("main")).length, _.id = f, u.add(_, "main", {
                                         activate: e.activate,
                                         ref: e.ref
                                     }), o && o.layoutModified.connect((() => {
                                         _.title.closable = Array.from(o.widgets("main")).length > 1
                                     }), _), c) {
                                     const e = e => {
                                         b.cwd = e.path
@@ -988,15 +1078,15 @@
                             var n;
                             const a = (null === (n = t.currentTitle) || void 0 === n ? void 0 : n.owner.id) || t.titles[t.titles.length - 1].owner.id;
                             return m.execute(E.create, {
                                 ref: a
                             })
                         }))), p
                     }
-                }, M, P];
-            var W;
+                }, A, q];
+            var V;
             ! function(e) {
                 e.id = 0
-            }(W || (W = {}))
+            }(V || (V = {}))
         }
     }
 ]);
```

### Comparing `jupyterlab_new_launcher-0.3.2/jupyterlab_new_launcher/labextension/static/remoteEntry.655eac004954212534b3.js` & `jupyterlab_new_launcher-0.3.3/jupyterlab_new_launcher/labextension/static/remoteEntry.a10a814d39706cd65aea.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -44,18 +44,18 @@
     }, m.d = (e, r) => {
         for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
         728: "5be4ee0b94a07decd5f8",
-        787: "35a3d65624680cd50b5a"
+        787: "27ef72da905b049778be"
     } [e] + ".js?v=" + {
         728: "5be4ee0b94a07decd5f8",
-        787: "35a3d65624680cd50b5a"
+        787: "27ef72da905b049778be"
     } [e], m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -106,15 +106,15 @@
                     var a = o[e] = o[e] || {},
                         u = a[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (a[r] = {
                         get: () => m.e(787).then((() => () => m(787))),
                         from: i,
                         eager: !1
                     })
-                })("jupyterlab-new-launcher", "0.3.2"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("jupyterlab-new-launcher", "0.3.3"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         m.g.importScripts && (e = m.g.location + "");
         var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupyterlab_new_launcher-0.3.2/jupyterlab_new_launcher/labextension/static/third-party-licenses.json` & `jupyterlab_new_launcher-0.3.3/jupyterlab_new_launcher/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.2/schema/plugin.json` & `jupyterlab_new_launcher-0.3.3/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.2/src/commands.ts` & `jupyterlab_new_launcher-0.3.3/src/commands.ts`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     },
     execute: async args => {
       const id = args.id as string | undefined;
       if (!id) {
         return console.error('Column ID missing');
       }
       const columns =
-        (settings.user.hiddenColumns as
+        (settings.composite.hiddenColumns as
           | ISettingsLayout['hiddenColumns']
           | undefined) ?? {};
       if (columns[id] === 'visible' || !columns[id]) {
         columns[id] = 'hidden';
       } else {
         columns[id] = 'visible';
       }
@@ -40,15 +40,15 @@
     isToggled: args => {
       const id = args.id as string | undefined;
       if (!id) {
         console.error('Column ID missing for checking if toggled');
         return false;
       }
       const columns =
-        (settings.user.hiddenColumns as
+        (settings.composite.hiddenColumns as
           | ISettingsLayout['hiddenColumns']
           | undefined) ?? {};
       return columns[id] !== 'hidden';
     }
   });
   app.commands.addCommand(CommandIDs.moveColumn, {
     label: args => {
```

### Comparing `jupyterlab_new_launcher-0.3.2/src/database.ts` & `jupyterlab_new_launcher-0.3.3/src/database.ts`

 * *Files 5% similar despite different names*

```diff
@@ -75,30 +75,41 @@
 
   get(item: ILauncher.IItemOptions) {
     const date = super._get(item);
     return date ? new Date(date) : null;
   }
 
   async recordAsUsedNow(item: ILauncher.IItemOptions) {
-    this._set(item, new Date().toUTCString());
+    await this.recordAsUsed(item, new Date());
   }
+
+  async recordAsUsed(item: ILauncher.IItemOptions, date: Date) {
+    await this._set(item, date.toUTCString());
+    this._changed.emit();
+  }
+
+  get changed() {
+    return this._changed;
+  }
+
+  private _changed = new Signal<LastUsedDatabase, void>(this);
 }
 
 export class FavoritesDatabase
   extends ItemDatabase<boolean>
   implements IFavoritesDatabase
 {
   protected _stateDBKey = 'new-launcher:favorites';
 
   get(item: ILauncher.IItemOptions) {
     return super._get(item) ?? null;
   }
 
   async set(item: ILauncher.IItemOptions, isFavourite: boolean) {
-    this._set(item, isFavourite);
+    await this._set(item, isFavourite);
     this._changed.emit();
   }
 
   get changed() {
     return this._changed;
   }
```

### Comparing `jupyterlab_new_launcher-0.3.2/src/dialogs.tsx` & `jupyterlab_new_launcher-0.3.3/src/dialogs.tsx`

 * *Files 11% similar despite different names*

```diff
@@ -82,15 +82,16 @@
         commands: this.options.commands,
         favoritesDatabase: this.options.database.favorites,
         lastUsedDatabase: this.options.database.lastUsed,
         settings,
         trans,
         acceptDialog: () => {
           dialog.resolve(1);
-        }
+        },
+        type: sessionContext.type
       }),
       buttons,
       checkbox: hasCheckbox
         ? {
             label: trans.__('Always start the preferred kernel'),
             caption: trans.__(
               'Remember my choice and always start the preferred kernel'
@@ -200,27 +201,38 @@
 
   /**
    * Render the launcher to virtual DOM nodes.
    */
   protected render(): React.ReactElement<any> | null {
     const items: ILauncher.IItemOptions[] = [];
     const specs = this.options.data.specs!.kernelspecs!;
+    // Note: this command is not executed, but it is only used to match favourite/last used metadata
+    const command =
+      this.options.type === 'console'
+        ? 'console:create'
+        : 'notebook:create-new';
 
     for (const spec of Object.values(specs)) {
       if (!spec) {
         continue;
       }
       const kernelIconUrl =
         spec.resources['logo-svg'] || spec.resources['logo-64x64'];
       items.push({
-        command: 'notebook:create-new',
-        args: {
-          isLauncher: true,
-          kernelName: spec.name
-        },
+        command,
+        args:
+          this.options.type === 'console'
+            ? {
+                isLauncher: true,
+                kernelPreference: { name: spec.name }
+              }
+            : {
+                isLauncher: true,
+                kernelName: spec.name
+              },
         kernelIconUrl,
         metadata: {
           kernel: JSONExt.deepCopy(spec.metadata || {}) as ReadonlyJSONValue
         }
       });
     }
     const runningItems: ILauncher.IItemOptions[] = [];
@@ -229,19 +241,25 @@
       if (!kernel) {
         continue;
       }
       const spec = specs[kernel.name]!;
       const kernelIconUrl =
         spec.resources['logo-svg'] || spec.resources['logo-64x64'];
       runningItems.push({
-        command: 'notebook:create-new',
-        args: {
-          isLauncher: true,
-          kernelName: spec.name
-        },
+        command,
+        args:
+          this.options.type === 'console'
+            ? {
+                isLauncher: true,
+                kernelPreference: { name: spec.name }
+              }
+            : {
+                isLauncher: true,
+                kernelName: spec.name
+              },
         kernelIconUrl,
         metadata: {
           kernel: {
             ...JSONExt.deepCopy(spec.metadata || {}),
             state: kernel.execution_state ?? 'running',
             'used by': model.name
           } as ReadonlyJSONValue,
@@ -264,14 +282,16 @@
           settings={this._settings}
           query=""
           showSearchBox={true}
           onClick={item => {
             this._selection = item;
             this.options.acceptDialog();
           }}
+          favouritesChanged={this._favoritesDatabase.changed}
+          lastUsedChanged={this._lastUsedDatabase.changed}
         />
         {runningKernelsItems.length > 0 ? (
           <>
             <h3 className="jp-KernelSelector-Section">
               {this.trans.__('Connect to a running kernel')}
             </h3>
             <KernelTable
@@ -282,28 +302,34 @@
               query=""
               showSearchBox={false}
               onClick={item => {
                 this._selection = item;
                 this.options.acceptDialog();
               }}
               hideColumns={['last-used', 'star']}
+              favouritesChanged={this._favoritesDatabase.changed}
+              lastUsedChanged={this._lastUsedDatabase.changed}
             />
           </>
         ) : null}
       </>
     );
   }
 
   getValue(): Partial<Kernel.IModel> | null {
     if (!this._selection) {
       return null;
     }
+    // Update last used date
+    this._selection.markAsUsedNow().catch(console.warn);
+    // User selected an existing kernel
     if (this._selection.metadata?.model) {
       return this._selection.metadata.model as unknown as Kernel.IModel;
     }
+    // User starts a new kernel
     return { name: this._selection.args!.kernelName as string };
   }
 
   protected commands: CommandRegistry;
   private _settings: ISettingRegistry.ISettings;
   private _selection: IKernelItem | null = null;
   private _lastUsedDatabase: ILastUsedDatabase;
@@ -317,9 +343,11 @@
     favoritesDatabase: IFavoritesDatabase;
     settings: ISettingRegistry.ISettings;
     commands: CommandRegistry;
     trans: TranslationBundle;
     data: SessionContext.IKernelSearch;
     acceptDialog: () => void;
     name: string;
+    // known values are "notebook" and "console"
+    type: string;
   }
 }
```

### Comparing `jupyterlab_new_launcher-0.3.2/src/icons.ts` & `jupyterlab_new_launcher-0.3.3/src/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.2/src/index.ts` & `jupyterlab_new_launcher-0.3.3/src/index.ts`

 * *Files 13% similar despite different names*

```diff
@@ -67,14 +67,48 @@
     document.body.appendChild(style);
   }
 
   settingRegistry.load(MAIN_PLUGIN_ID).then(settings => {
     addCommands(app, trans, settings);
   });
 
+  // Detect kernels started outside of the launcher, e.g. automatically due to having notebooks open from previous session
+  const lastSessionActivity: Record<string, string> = {};
+  const recordSessionActivity = async () => {
+    const models = [...app.serviceManager.sessions.running()];
+    for (const model of models) {
+      if (!model.kernel) {
+        continue;
+      }
+      let command: string;
+      if (model.type === 'notebook') {
+        command = 'notebook:create-new';
+      } else if (model.type === 'console') {
+        command = 'console:create';
+      } else {
+        command = 'unknown';
+      }
+      const key = command + '-' + model.kernel.name;
+      const activity = model.kernel.last_activity;
+      if (activity && lastSessionActivity[key] !== activity) {
+        lastSessionActivity[key] = activity;
+        const item = {
+          command,
+          args: {
+            isLauncher: true,
+            kernelName: model.kernel.name
+          }
+        };
+        await database.lastUsed.recordAsUsed(item, new Date(activity));
+      }
+    }
+  };
+  app.serviceManager.sessions.ready.then(recordSessionActivity);
+  app.serviceManager.sessions.runningChanged.connect(recordSessionActivity);
+
   commands.addCommand(CommandIDs.create, {
     label: trans.__('New Launcher'),
     icon: args => (args.toolbar ? addIcon : undefined),
     execute: async (args: ReadonlyPartialJSONObject) => {
       const cwd = (args['cwd'] as string) ?? defaultBrowser?.model.path ?? '';
       const id = `launcher-${Private.id++}`;
       const callback = (item: Widget) => {
@@ -83,14 +117,15 @@
           shell.add(item, 'main', { ref: id });
           launcher.dispose();
         }
       };
 
       const settings = await settingRegistry.load(MAIN_PLUGIN_ID);
       await Promise.all([database.lastUsed.ready, database.favorites.ready]);
+
       const launcher = new Launcher({
         model,
         cwd,
         callback,
         commands,
         translator,
         lastUsedDatabase: database.lastUsed,
```

### Comparing `jupyterlab_new_launcher-0.3.2/src/item.ts` & `jupyterlab_new_launcher-0.3.3/src/item.ts`

 * *Files 16% similar despite different names*

```diff
@@ -17,42 +17,38 @@
   kernelIconUrl?: string;
   metadata?: ReadonlyJSONObject;
   // custom additions
   label: string;
   caption: string;
   icon: VirtualElement.IRenderer | undefined;
   iconClass: string;
-  starred: boolean;
 
   constructor(
     private _options: {
       commands: CommandRegistry;
       item: ILauncher.IItemOptions;
       cwd: string;
       lastUsedDatabase: ILastUsedDatabase;
       favoritesDatabase: IFavoritesDatabase;
     }
   ) {
-    const { item, commands, lastUsedDatabase, favoritesDatabase, cwd } =
-      _options;
+    const { item, commands, cwd } = _options;
     const args = { ...item.args, cwd };
     // base
     this.command = item.command;
     this.args = args;
     this.category = item.category;
     this.rank = item.rank;
     this.kernelIconUrl = item.kernelIconUrl;
     this.metadata = item.metadata ?? {};
     // custom
     this.iconClass = commands.iconClass(item.command, args);
     this.icon = commands.icon(item.command, args);
     this.caption = commands.caption(item.command, args);
     this.label = commands.label(item.command, args);
-    this.lastUsed = lastUsedDatabase.get(item);
-    this.starred = favoritesDatabase.get(item) ?? false;
     // special handling for conda-store
     // https://www.nebari.dev/docs/faq/#why-is-there-duplication-in-names-of-environments
     const kernel = this.metadata['kernel'] as JSONObject | undefined;
     if (kernel) {
       const condaStoreMatch = (
         (kernel['conda_env_name'] as string | undefined) ?? ''
       ).match(/(?<namespace>.+)-(?<duplicate>\1)-(?<environment>.+)/);
@@ -75,46 +71,48 @@
     if (
       this.command === 'server-proxy:open' &&
       this.kernelIconUrl?.endsWith('/vscode')
     ) {
       this.icon = codeServerIcon;
     }
   }
+  get starred() {
+    const { item, favoritesDatabase } = this._options;
+    return favoritesDatabase.get(item) ?? false;
+  }
   get lastUsed(): Date | null {
-    return this._lastUsed;
+    const value = this._lastUsed;
+    this._setRefreshClock(value);
+    return value;
   }
-  set lastUsed(value: Date | null) {
-    this._lastUsed = value;
-    this._setRefreshClock();
+  private get _lastUsed(): Date | null {
+    const { item, lastUsedDatabase } = this._options;
+    return lastUsedDatabase.get(item);
   }
   get refreshLastUsed(): ISignal<IItem, void> {
     return this._refreshLastUsed;
   }
   async execute() {
     const { item, commands, lastUsedDatabase } = this._options;
     await commands.execute(item.command, this.args);
     await lastUsedDatabase.recordAsUsedNow(item);
-    this.lastUsed = lastUsedDatabase.get(item);
     this._refreshLastUsed.emit();
   }
-  async markAsUsed() {
+  async markAsUsedNow() {
     const { item, lastUsedDatabase } = this._options;
     await lastUsedDatabase.recordAsUsedNow(item);
-    this.lastUsed = lastUsedDatabase.get(item);
     this._refreshLastUsed.emit();
   }
-  toggleStar() {
+  async toggleStar() {
     const { item, favoritesDatabase } = this._options;
     const wasStarred = favoritesDatabase.get(item);
     const newState = !wasStarred;
-    this.starred = newState;
     return favoritesDatabase.set(item, newState);
   }
-  private _setRefreshClock() {
-    const value = this._lastUsed;
+  private _setRefreshClock(value: Date | null) {
     if (this._refreshClock !== null) {
       window.clearTimeout(this._refreshClock);
       this._refreshClock = null;
     }
     if (!value) {
       return;
     }
@@ -128,14 +126,13 @@
       delta < 1 * minute
         ? 10 * second
         : delta < 60 * minute
           ? 1 * minute
           : 60 * minute;
     this._refreshClock = window.setTimeout(() => {
       this._refreshLastUsed.emit();
-      this._setRefreshClock();
+      this._setRefreshClock(this._lastUsed);
     }, interval);
   }
   private _refreshLastUsed = new Signal<Item, void>(this);
   private _refreshClock: number | null = null;
-  private _lastUsed: Date | null = null;
 }
```

### Comparing `jupyterlab_new_launcher-0.3.2/src/launcher.tsx` & `jupyterlab_new_launcher-0.3.3/src/launcher.tsx`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,16 @@
   cwd: string;
   typeItems: IItem[];
   notebookItems: IKernelItem[];
   consoleItems: IKernelItem[];
   otherItems: IItem[];
   commands: CommandRegistry;
   settings: ISettingRegistry.ISettings;
-  favouritesChanged?: ISignal<IFavoritesDatabase, void>;
+  favouritesChanged: ISignal<IFavoritesDatabase, void>;
+  lastUsedChanged: ISignal<ILastUsedDatabase, void>;
 }): React.ReactElement {
   const { trans, cwd, typeItems, otherItems, favouritesChanged } = props;
   const [query, updateQuery] = React.useState<string>('');
   const [, forceUpdate] = React.useReducer(x => x + 1, 0);
   const [showStarred, updateShowStarred] = React.useState<
     ISettingsLayout['starredSection']
   >(
@@ -158,14 +159,16 @@
               commands={props.commands}
               showSearchBox={!searchAll}
               showWidgetType={true}
               query={query}
               settings={props.settings}
               trans={trans}
               onClick={item => item.execute()}
+              favouritesChanged={props.favouritesChanged}
+              lastUsedChanged={props.lastUsedChanged}
             />
           ) : (
             'No starred items'
           )}
         </CollapsibleSection>
       ) : null}
       <CollapsibleSection
@@ -178,14 +181,16 @@
           items={props.notebookItems}
           commands={props.commands}
           showSearchBox={!searchAll}
           query={query}
           settings={props.settings}
           trans={trans}
           onClick={item => item.execute()}
+          favouritesChanged={props.favouritesChanged}
+          lastUsedChanged={props.lastUsedChanged}
         />
       </CollapsibleSection>
       <CollapsibleSection
         className="jp-Launcher-openByKernel jp-Launcher-launchConsole"
         title={trans.__('Launch New Console')}
         icon={consoleIcon}
         open={startCollapsed['launch-console'] !== 'collapsed'}
@@ -194,14 +199,16 @@
           items={props.consoleItems}
           commands={props.commands}
           showSearchBox={!searchAll}
           query={query}
           settings={props.settings}
           trans={trans}
           onClick={item => item.execute()}
+          favouritesChanged={props.favouritesChanged}
+          lastUsedChanged={props.lastUsedChanged}
         />
       </CollapsibleSection>
     </div>
   );
 }
 
 export namespace NewLauncher {
@@ -322,13 +329,14 @@
         commands={this.commands}
         typeItems={typeItems}
         notebookItems={notebookItems}
         consoleItems={consoleItems}
         otherItems={otherItems}
         settings={this._settings}
         favouritesChanged={this._favoritesDatabase.changed}
+        lastUsedChanged={this._lastUsedDatabase.changed}
       />
     );
   }
   protected commands: CommandRegistry;
   private _settings: ISettingRegistry.ISettings;
 }
```

### Comparing `jupyterlab_new_launcher-0.3.2/src/types.ts` & `jupyterlab_new_launcher-0.3.3/src/types.ts`

 * *Files 6% similar despite different names*

```diff
@@ -29,26 +29,29 @@
   label: string;
   caption: string;
   icon: VirtualElement.IRenderer | undefined;
   iconClass: string;
   execute: () => Promise<void>;
   lastUsed: Date | null;
   starred: boolean;
-  toggleStar: () => void;
+  toggleStar: () => Promise<void>;
   refreshLastUsed: ISignal<IItem, void>;
+  markAsUsedNow: () => Promise<void>;
 }
 
 export interface IKernelItem extends IItem {
   //kernel: string;
 }
 
 export interface ILastUsedDatabase {
   ready: Promise<void>;
   get(item: ILauncher.IItemOptions): Date | null;
+  recordAsUsed(item: ILauncher.IItemOptions, date: Date): Promise<void>;
   recordAsUsedNow(item: ILauncher.IItemOptions): Promise<void>;
+  changed: ISignal<ILastUsedDatabase, void>;
 }
 
 export interface IFavoritesDatabase {
   ready: Promise<void>;
   get(item: ILauncher.IItemOptions): boolean | null;
   set(item: ILauncher.IItemOptions, isFavourite: boolean): Promise<void>;
   changed: ISignal<IFavoritesDatabase, void>;
```

### Comparing `jupyterlab_new_launcher-0.3.2/src/components/base-table.tsx` & `jupyterlab_new_launcher-0.3.3/src/components/base-table.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.2/src/components/card.tsx` & `jupyterlab_new_launcher-0.3.3/src/components/card.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.2/src/components/section.tsx` & `jupyterlab_new_launcher-0.3.3/src/components/section.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.2/src/components/table.tsx` & `jupyterlab_new_launcher-0.3.3/src/components/table.tsx`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 // Copyright (c) Nebari Development Team.
 // Distributed under the terms of the Modified BSD License.
 import type { CommandRegistry } from '@lumino/commands';
 import { ReadonlyJSONObject } from '@lumino/coreutils';
+import type { ISignal } from '@lumino/signaling';
 import { Time } from '@jupyterlab/coreutils';
 import { ISettingRegistry } from '@jupyterlab/settingregistry';
 import { TranslationBundle } from '@jupyterlab/translation';
 import { FilterBox, UseSignal, MenuSvg } from '@jupyterlab/ui-components';
 import { Table } from './base-table';
 import * as React from 'react';
-import { ISettingsLayout, CommandIDs, IKernelItem } from '../types';
+import {
+  ISettingsLayout,
+  IFavoritesDatabase,
+  ILastUsedDatabase,
+  CommandIDs,
+  IKernelItem
+} from '../types';
 import { starIcon } from '../icons';
 
 const STAR_BUTTON_CLASS = 'jp-starIconButton';
 const KERNEL_ITEM_CLASS = 'jp-TableKernelItem';
 
 function columnLabelFromKey(key: string): string {
   if (key.length === 0) {
@@ -34,31 +41,56 @@
     case 'conda_is_currently_running':
       return 'Running?';
   }
   return key[0].toUpperCase() + key.substring(1);
 }
 
 function EllipsedCell(props: React.PropsWithChildren<{ title?: string }>) {
+  const [innerTitle, setInnerTitle] = React.useState<string | undefined>(
+    undefined
+  );
+  const elementRef = React.useRef<HTMLDivElement>(null);
   return (
     <div className="jp-ellipsis-wrapper" title={props.title}>
-      <div className="jp-ellipsis">{props.children}</div>
+      <div
+        className="jp-ellipsis"
+        title={innerTitle}
+        ref={elementRef}
+        onMouseEnter={() => {
+          if (props.title) {
+            // do nothing if there is a parent title
+            return;
+          }
+          const el = elementRef.current;
+          // if the ellipsis is active, add a title so that user can see the full text on hover
+          if (el && el.scrollWidth > el.clientWidth) {
+            setInnerTitle(el.innerText);
+          } else {
+            setInnerTitle(undefined);
+          }
+        }}
+      >
+        {props.children}
+      </div>
     </div>
   );
 }
 
 export function KernelTable(props: {
   trans: TranslationBundle;
   items: IKernelItem[];
   commands: CommandRegistry;
   settings: ISettingRegistry.ISettings;
   showSearchBox: boolean;
   query: string;
   onClick: (item: IKernelItem) => void;
   hideColumns?: string[];
   showWidgetType?: boolean;
+  favouritesChanged: ISignal<IFavoritesDatabase, void>;
+  lastUsedChanged: ISignal<ILastUsedDatabase, void>;
 }) {
   const { trans } = props;
   let query: string;
   let updateQuery: (value: string) => void;
   // Note: state cannot be defined in conditionals, or React will error out when toggling it.
   const [_query, _updateQuery] = React.useState<string>('');
   if (props.showSearchBox) {
@@ -67,14 +99,27 @@
   } else {
     query = props.query;
   }
 
   // Hoisted to avoid "Rendered fewer hooks than expected" error on toggling the Star column
   const [, forceUpdate] = React.useReducer(x => x + 1, 0);
 
+  React.useEffect(() => {
+    props.favouritesChanged.connect(forceUpdate);
+    return () => {
+      props.favouritesChanged.disconnect(forceUpdate);
+    };
+  });
+  React.useEffect(() => {
+    props.lastUsedChanged.connect(forceUpdate);
+    return () => {
+      props.lastUsedChanged.disconnect(forceUpdate);
+    };
+  });
+
   const metadataAvailable = new Set<string>();
   for (const item of props.items) {
     const kernelMetadata = item.metadata?.kernel;
     if (!kernelMetadata) {
       continue;
     }
     for (const key of Object.keys(kernelMetadata)) {
@@ -236,18 +281,17 @@
           <button
             className={
               starred
                 ? `${STAR_BUTTON_CLASS} jp-mod-starred`
                 : STAR_BUTTON_CLASS
             }
             title={title}
-            onClick={event => {
-              row.toggleStar();
-              forceUpdate();
+            onClick={async event => {
               event.stopPropagation();
+              await row.toggleStar();
             }}
           >
             <starIcon.react className="jp-starIcon" />
           </button>
         );
       },
       sort: (a: IKernelItem, b: IKernelItem) =>
@@ -311,15 +355,17 @@
         </div>
       ) : null}
       <div
         className="jp-NewLauncher-table-scroller"
         onContextMenu={(event: React.MouseEvent) => {
           event.preventDefault();
           const contextMenu = new MenuSvg({ commands: props.commands });
+          contextMenu.addClass('jp-NewLauncher-contextMenu');
           const columnsSubMenu = new MenuSvg({ commands: props.commands });
+          columnsSubMenu.addClass('jp-NewLauncher-contextMenu-visibleColumns');
           for (const column of columns) {
             columnsSubMenu.addItem({
               command: CommandIDs.toggleColumn,
               args: { id: column.id, label: column.label }
             });
           }
           columnsSubMenu.title.label = trans.__('Visible Columns');
@@ -341,18 +387,37 @@
             });
           }
           contextMenu.open(event.clientX, event.clientY);
         }}
       >
         <KernelItemTable
           rows={props.items
-            .filter(
-              kernel =>
-                kernel.label.toLowerCase().indexOf(query.toLowerCase()) !== -1
-            )
+            .filter(kernel => {
+              const lowerCaseQuery = query.toLowerCase();
+              // search in label
+              if (kernel.label.toLowerCase().includes(lowerCaseQuery)) {
+                return true;
+              }
+              // search in columns generated out of metadata
+              const kernelMeta = kernel.metadata?.kernel as
+                | ReadonlyJSONObject
+                | undefined;
+              if (!kernelMeta) {
+                return;
+              }
+              for (const metadataKey of metadataAvailable) {
+                const value = kernelMeta[metadataKey];
+                if (typeof value === 'string') {
+                  if (value.toLowerCase().includes(lowerCaseQuery)) {
+                    return true;
+                  }
+                }
+              }
+              return false;
+            })
             .map(data => {
               return {
                 data: data,
                 key: data.command + JSON.stringify(data.args)
               };
             })}
           blankIndicator={() => {
```

### Comparing `jupyterlab_new_launcher-0.3.2/style/base.css` & `jupyterlab_new_launcher-0.3.3/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.2/style/icons/code-server.svg` & `jupyterlab_new_launcher-0.3.3/style/icons/code-server.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.2/style/icons/md/LICENSE` & `jupyterlab_new_launcher-0.3.3/style/icons/md/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.2/ui-tests/README.md` & `jupyterlab_new_launcher-0.3.3/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.2/ui-tests/yarn.lock` & `jupyterlab_new_launcher-0.3.3/ui-tests/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.2/ui-tests/tests/jupyterlab_new_launcher.spec.ts` & `jupyterlab_new_launcher-0.3.3/ui-tests/tests/jupyterlab_new_launcher.spec.ts`

 * *Files 25% similar despite different names*

```diff
@@ -3,14 +3,37 @@
 const SETTINGS_ID = 'jupyterlab-new-launcher:plugin';
 
 test.describe('Default settings', () => {
   test('should render new launcher', async ({ page }) => {
     const launcher = page.locator('.jp-LauncherBody');
     expect(await launcher.screenshot()).toMatchSnapshot('launcher.png');
   });
+
+  test('should open table context menu', async ({ page }) => {
+    const tableHead = page.locator(
+      '.jp-Launcher-launchNotebook thead > tr > th[data-id="star"]'
+    );
+    await tableHead.click({ button: 'right' });
+    const contextMenu = page.locator('.jp-NewLauncher-contextMenu');
+    await expect(contextMenu).toBeVisible();
+    expect
+      .soft(await contextMenu.screenshot())
+      .toMatchSnapshot('table-context-menu.png');
+    const visibleColumnsEntry = page.locator(
+      '.jp-NewLauncher-contextMenu li >> text="Visible Columns"'
+    );
+    await visibleColumnsEntry.hover();
+    const columnsContextMenu = page.locator(
+      '.jp-NewLauncher-contextMenu-visibleColumns'
+    );
+    await expect(columnsContextMenu).toBeVisible();
+    expect
+      .soft(await columnsContextMenu.screenshot())
+      .toMatchSnapshot('table-context-menu-visible-columns.png');
+  });
 });
 
 test.describe('With starred section', () => {
   test.use({
     mockSettings: {
       ...galata.DEFAULT_SETTINGS,
       [SETTINGS_ID]: {
```

### Comparing `jupyterlab_new_launcher-0.3.2/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-linux.png` & `jupyterlab_new_launcher-0.3.3/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.2/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-search-in-individual-linux.png` & `jupyterlab_new_launcher-0.3.3/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-search-in-individual-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.2/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-with-starred-linux.png` & `jupyterlab_new_launcher-0.3.3/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-with-starred-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.2/.gitignore` & `jupyterlab_new_launcher-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.2/LICENSE` & `jupyterlab_new_launcher-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.2/README.md` & `jupyterlab_new_launcher-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.2/pyproject.toml` & `jupyterlab_new_launcher-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.3.2/PKG-INFO` & `jupyterlab_new_launcher-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlab-new-launcher
-Version: 0.3.2
+Version: 0.3.3
 Dynamic: Keywords
 Summary: A redesigned JupyterLab launcher
 Project-URL: Homepage, https://github.com/nebari-dev/jupyterlab-new-launcher
 Project-URL: Bug Tracker, https://github.com/nebari-dev/jupyterlab-new-launcher/issues
 Project-URL: Repository, https://github.com/nebari-dev/jupyterlab-new-launcher.git
 Author-email: Nebari development team <internal-it@quansight.com>
 License: BSD 3-Clause License
```

