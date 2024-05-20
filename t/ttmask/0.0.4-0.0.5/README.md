# Comparing `tmp/ttmask-0.0.4.tar.gz` & `tmp/ttmask-0.0.5.tar.gz`

## Comparing `ttmask-0.0.4.tar` & `ttmask-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 ttmask-0.0.4/.copier-answers.yml
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 ttmask-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 ttmask-0.0.4/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 ttmask-0.0.4/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 ttmask-0.0.4/.github/dependabot.yml
--rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 ttmask-0.0.4/.github/workflows/ci.yml
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 ttmask-0.0.4/src/ttmask/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 ttmask-0.0.4/src/ttmask/_cli.py
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 ttmask-0.0.4/src/ttmask/cylinder.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 ttmask-0.0.4/src/ttmask/py.typed
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 ttmask-0.0.4/src/ttmask/sphere.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ttmask-0.0.4/tests/test_ttmask.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 ttmask-0.0.4/.gitignore
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 ttmask-0.0.4/LICENSE
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 ttmask-0.0.4/README.md
--rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 ttmask-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 ttmask-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 ttmask-0.0.5/.copier-answers.yml
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 ttmask-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 ttmask-0.0.5/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 ttmask-0.0.5/.github/TEST_FAIL_TEMPLATE.md
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 ttmask-0.0.5/.github/dependabot.yml
+-rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 ttmask-0.0.5/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 ttmask-0.0.5/src/ttmask/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 ttmask-0.0.5/src/ttmask/_cli.py
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ttmask-0.0.5/src/ttmask/cuboid.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 ttmask-0.0.5/src/ttmask/cylinder.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 ttmask-0.0.5/src/ttmask/py.typed
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 ttmask-0.0.5/src/ttmask/sphere.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ttmask-0.0.5/tests/test_ttmask.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 ttmask-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 ttmask-0.0.5/LICENSE
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 ttmask-0.0.5/README.md
+-rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 ttmask-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 ttmask-0.0.5/PKG-INFO
```

### Comparing `ttmask-0.0.4/.pre-commit-config.yaml` & `ttmask-0.0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ttmask-0.0.4/.github/workflows/ci.yml` & `ttmask-0.0.5/.github/workflows/ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
         platform: [ubuntu-latest, ] # macos-latest, windows-latest]
 
     steps:
       - uses: actions/checkout@v4
 
       - name: 🐍 Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
           cache-dependency-path: "pyproject.toml"
           cache: "pip"
 
       - name: Install Dependencies
         run: |
@@ -65,15 +65,15 @@
           RUN_ID: ${{ github.run_id }}
           TITLE: "[test-bot] pip install --pre is failing"
         with:
           filename: .github/TEST_FAIL_TEMPLATE.md
           update_existing: true
 
       - name: Coverage
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
 
   deploy:
     name: Deploy
     needs: test
     if: success() && startsWith(github.ref, 'refs/tags/') && github.event_name != 'schedule'
     runs-on: ubuntu-latest
 
@@ -86,23 +86,23 @@
 
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - name: 🐍 Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.x"
 
       - name: 👷 Build
         run: |
           python -m pip install build
           python -m build
 
       - name: 🚢 Publish to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
 
-      - uses: softprops/action-gh-release@v1
+      - uses: softprops/action-gh-release@v2
         with:
           generate_release_notes: true
           files: './dist/*'
```

### Comparing `ttmask-0.0.4/src/ttmask/cylinder.py` & `ttmask-0.0.5/src/ttmask/cylinder.py`

 * *Files identical despite different names*

### Comparing `ttmask-0.0.4/src/ttmask/sphere.py` & `ttmask-0.0.5/src/ttmask/sphere.py`

 * *Files identical despite different names*

### Comparing `ttmask-0.0.4/.gitignore` & `ttmask-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `ttmask-0.0.4/LICENSE` & `ttmask-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ttmask-0.0.4/README.md` & `ttmask-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ttmask-0.0.4/pyproject.toml` & `ttmask-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ttmask-0.0.4/PKG-INFO` & `ttmask-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ttmask
-Version: 0.0.4
+Version: 0.0.5
 Summary: CLI tool for mask creation in cryo-EM/ET
 Project-URL: homepage, https://github.com/teamtomo/ttmask
 Project-URL: repository, https://github.com/teamtomo/ttmask
 Author-email: Miles Graham <miles.graham@balliol.ox.ac.uk>
 License: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
```

