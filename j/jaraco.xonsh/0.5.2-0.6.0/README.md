# Comparing `tmp/jaraco_xonsh-0.5.2.tar.gz` & `tmp/jaraco_xonsh-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco_xonsh-0.5.2.tar", last modified: Tue Apr 30 13:42:46 2024, max compression
+gzip compressed data, was "jaraco_xonsh-0.6.0.tar", last modified: Mon May 20 01:51:05 2024, max compression
```

## Comparing `jaraco_xonsh-0.5.2.tar` & `jaraco_xonsh-0.6.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-04-30 13:42:46.778018 jaraco_xonsh-0.5.2/
--rw-r--r--   0 jaraco     (501) staff       (20)      200 2024-02-10 03:17:09.000000 jaraco_xonsh-0.5.2/.coveragerc
--rw-r--r--   0 jaraco     (501) staff       (20)      246 2024-02-02 02:03:10.000000 jaraco_xonsh-0.5.2/.editorconfig
-drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-04-30 13:42:46.774630 jaraco_xonsh-0.5.2/.github/
--rw-r--r--   0 jaraco     (501) staff       (20)      148 2024-02-02 02:03:10.000000 jaraco_xonsh-0.5.2/.github/dependabot.yml
-drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-04-30 13:42:46.774730 jaraco_xonsh-0.5.2/.github/workflows/
--rw-r--r--   0 jaraco     (501) staff       (20)     3051 2024-04-30 13:42:36.000000 jaraco_xonsh-0.5.2/.github/workflows/main.yml
--rw-r--r--   0 jaraco     (501) staff       (20)      116 2024-02-02 02:03:10.000000 jaraco_xonsh-0.5.2/.pre-commit-config.yaml
--rw-r--r--   0 jaraco     (501) staff       (20)      335 2024-03-24 16:04:55.000000 jaraco_xonsh-0.5.2/.readthedocs.yaml
--rw-r--r--   0 jaraco     (501) staff       (20)     1023 2024-02-02 02:03:10.000000 jaraco_xonsh-0.5.2/LICENSE
--rw-r--r--   0 jaraco     (501) staff       (20)      954 2024-04-28 19:37:03.000000 jaraco_xonsh-0.5.2/NEWS.rst
--rw-r--r--   0 jaraco     (501) staff       (20)     2041 2024-04-30 13:42:46.777767 jaraco_xonsh-0.5.2/PKG-INFO
--rw-r--r--   0 jaraco     (501) staff       (20)      826 2024-02-10 03:17:09.000000 jaraco_xonsh-0.5.2/README.rst
-drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-04-30 13:42:46.775029 jaraco_xonsh-0.5.2/docs/
--rw-r--r--   0 jaraco     (501) staff       (20)     1122 2024-02-02 02:03:10.000000 jaraco_xonsh-0.5.2/docs/conf.py
--rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-02-02 02:03:10.000000 jaraco_xonsh-0.5.2/docs/history.rst
--rw-r--r--   0 jaraco     (501) staff       (20)      248 2024-02-02 02:03:10.000000 jaraco_xonsh-0.5.2/docs/index.rst
-drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-04-30 13:42:46.775141 jaraco_xonsh-0.5.2/jaraco/
--rw-r--r--   0 jaraco     (501) staff       (20)    12620 2024-04-28 19:34:55.000000 jaraco_xonsh-0.5.2/jaraco/xonsh.xsh
-drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-04-30 13:42:46.776660 jaraco_xonsh-0.5.2/jaraco.xonsh.egg-info/
--rw-r--r--   0 jaraco     (501) staff       (20)     2041 2024-04-30 13:42:46.000000 jaraco_xonsh-0.5.2/jaraco.xonsh.egg-info/PKG-INFO
--rw-r--r--   0 jaraco     (501) staff       (20)      493 2024-04-30 13:42:46.000000 jaraco_xonsh-0.5.2/jaraco.xonsh.egg-info/SOURCES.txt
--rw-r--r--   0 jaraco     (501) staff       (20)        1 2024-04-30 13:42:46.000000 jaraco_xonsh-0.5.2/jaraco.xonsh.egg-info/dependency_links.txt
--rw-r--r--   0 jaraco     (501) staff       (20)       45 2024-04-30 13:42:46.000000 jaraco_xonsh-0.5.2/jaraco.xonsh.egg-info/entry_points.txt
--rw-r--r--   0 jaraco     (501) staff       (20)      225 2024-04-30 13:42:46.000000 jaraco_xonsh-0.5.2/jaraco.xonsh.egg-info/requires.txt
--rw-r--r--   0 jaraco     (501) staff       (20)        7 2024-04-30 13:42:46.000000 jaraco_xonsh-0.5.2/jaraco.xonsh.egg-info/top_level.txt
--rw-r--r--   0 jaraco     (501) staff       (20)      154 2024-02-02 02:03:10.000000 jaraco_xonsh-0.5.2/mypy.ini
--rw-r--r--   0 jaraco     (501) staff       (20)     1143 2024-04-30 07:01:07.000000 jaraco_xonsh-0.5.2/pyproject.toml
--rw-r--r--   0 jaraco     (501) staff       (20)      584 2024-04-02 14:34:12.000000 jaraco_xonsh-0.5.2/pytest.ini
--rw-r--r--   0 jaraco     (501) staff       (20)      419 2024-03-24 16:04:55.000000 jaraco_xonsh-0.5.2/ruff.toml
--rw-r--r--   0 jaraco     (501) staff       (20)       38 2024-04-30 13:42:46.778204 jaraco_xonsh-0.5.2/setup.cfg
--rw-r--r--   0 jaraco     (501) staff       (20)       44 2024-02-02 02:03:10.000000 jaraco_xonsh-0.5.2/towncrier.toml
--rw-r--r--   0 jaraco     (501) staff       (20)     1364 2024-02-19 08:35:02.000000 jaraco_xonsh-0.5.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:51:05.005307 jaraco_xonsh-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:51:04.997307 jaraco_xonsh-0.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:51:04.997307 jaraco_xonsh-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-20 01:51:05.005307 jaraco_xonsh-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:51:05.001307 jaraco_xonsh-0.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:51:05.001307 jaraco_xonsh-0.6.0/jaraco/
+-rw-r--r--   0 runner    (1001) docker     (127)    12990 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/jaraco/xonsh.xsh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:51:05.001307 jaraco_xonsh-0.6.0/jaraco.xonsh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-20 01:51:04.000000 jaraco_xonsh-0.6.0/jaraco.xonsh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-20 01:51:04.000000 jaraco_xonsh-0.6.0/jaraco.xonsh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 01:51:04.000000 jaraco_xonsh-0.6.0/jaraco.xonsh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-20 01:51:04.000000 jaraco_xonsh-0.6.0/jaraco.xonsh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-20 01:51:04.000000 jaraco_xonsh-0.6.0/jaraco.xonsh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 01:51:04.000000 jaraco_xonsh-0.6.0/jaraco.xonsh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 01:51:05.005307 jaraco_xonsh-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-20 01:50:43.000000 jaraco_xonsh-0.6.0/tox.ini
```

### Comparing `jaraco_xonsh-0.5.2/.github/workflows/main.yml` & `jaraco_xonsh-0.6.0/.github/workflows/main.yml`

 * *Files 7% similar despite different names*

```diff
@@ -43,30 +43,33 @@
         include:
         - python: "3.9"
           platform: ubuntu-latest
         - python: "3.10"
           platform: ubuntu-latest
         - python: "3.11"
           platform: ubuntu-latest
-        # disable PyPy as it breaks CI
-        # - python: pypy3.10
-        #  platform: ubuntu-latest
+        - python: pypy3.10
+          platform: ubuntu-latest
     runs-on: ${{ matrix.platform }}
     continue-on-error: ${{ matrix.python == '3.13' || (matrix.python == '3.8' || matrix.python == '3.9') && matrix.platform == 'macos-latest' }}
     steps:
       - uses: actions/checkout@v4
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
           allow-prereleases: true
       - name: Install tox
         run: python -m pip install tox
       - name: Run
         run: tox
+        env:
+          # workaround for jaraco/jaraco.xonsh#1
+          TOX_OVERRIDE: testenv.pass_env+=PYTEST_ADDOPTS
+          PYTEST_ADDOPTS: -p no:xonsh
 
   collateral:
     strategy:
       fail-fast: false
       matrix:
         job:
         - diffcov
@@ -80,14 +83,18 @@
         uses: actions/setup-python@v4
         with:
           python-version: 3.x
       - name: Install tox
         run: python -m pip install tox
       - name: Eval ${{ matrix.job }}
         run: tox -e ${{ matrix.job }}
+        env:
+          # workaround for jaraco/jaraco.xonsh#1
+          TOX_OVERRIDE: testenv.pass_env+=PYTEST_ADDOPTS
+          PYTEST_ADDOPTS: -p no:xonsh
 
   check:  # This job does nothing and is only used for the branch protection
     if: always()
 
     needs:
     - test
     - collateral
```

### Comparing `jaraco_xonsh-0.5.2/LICENSE` & `jaraco_xonsh-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco_xonsh-0.5.2/NEWS.rst` & `jaraco_xonsh-0.6.0/NEWS.rst`

 * *Files identical despite different names*

### Comparing `jaraco_xonsh-0.5.2/PKG-INFO` & `jaraco_xonsh-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.xonsh
-Version: 0.5.2
+Version: 0.6.0
 Summary: Xonsh facilities used by jaraco
 Author-email: "Jason R. Coombs" <jaraco@jaraco.com>
 Project-URL: Homepage, https://github.com/jaraco/jaraco.xonsh
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jaraco_xonsh-0.5.2/README.rst` & `jaraco_xonsh-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `jaraco_xonsh-0.5.2/docs/conf.py` & `jaraco_xonsh-0.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco_xonsh-0.5.2/jaraco/xonsh.xsh` & `jaraco_xonsh-0.6.0/jaraco/xonsh.xsh`

 * *Files 2% similar despite different names*

```diff
@@ -436,7 +436,13 @@
 
 aliases['re-log'] = re_log
 
 
 # workaround for https://github.com/xonsh/xonsh/issues/3207
 if '/.local/bin' not in os.environ['PATH']:
 	os.environ['PATH'] = os.pathsep.join($PATH)
+
+
+def gemini(args):
+	prompt = ' '.join(args)
+	http https://generativelanguage.googleapis.com/v1/models/gemini-pro:generateContent x-goog-api-key:@(keyring.get_password('https://generativelanguage.googleapis.com/', 'jaraco@jaraco.com')) contents[0][role]=user f'contents[0][parts][][text]={prompt}' | jq -r .candidates[0].content.parts[0].text
+aliases['gemini'] = gemini
```

### Comparing `jaraco_xonsh-0.5.2/jaraco.xonsh.egg-info/PKG-INFO` & `jaraco_xonsh-0.6.0/jaraco.xonsh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.xonsh
-Version: 0.5.2
+Version: 0.6.0
 Summary: Xonsh facilities used by jaraco
 Author-email: "Jason R. Coombs" <jaraco@jaraco.com>
 Project-URL: Homepage, https://github.com/jaraco/jaraco.xonsh
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jaraco_xonsh-0.5.2/pyproject.toml` & `jaraco_xonsh-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jaraco_xonsh-0.5.2/pytest.ini` & `jaraco_xonsh-0.6.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `jaraco_xonsh-0.5.2/tox.ini` & `jaraco_xonsh-0.6.0/tox.ini`

 * *Files identical despite different names*

