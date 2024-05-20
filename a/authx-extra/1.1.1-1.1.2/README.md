# Comparing `tmp/authx_extra-1.1.1.tar.gz` & `tmp/authx_extra-1.1.2.tar.gz`

## Comparing `authx_extra-1.1.1.tar` & `authx_extra-1.1.2.tar`

### file list

```diff
@@ -1,44 +1,42 @@
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 authx_extra-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 authx_extra-1.1.1/.github/FUNDING.yml
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 authx_extra-1.1.1/.github/dependabot.yaml
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 authx_extra-1.1.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 authx_extra-1.1.1/.github/workflows/release.yml
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 authx_extra-1.1.1/authx_extra/__init__.py
--rw-r--r--   0        0        0     6189 2020-02-02 00:00:00.000000 authx_extra-1.1.1/authx_extra/cache.py
--rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 authx_extra-1.1.1/authx_extra/metrics.py
--rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 authx_extra-1.1.1/authx_extra/oauth2.py
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 authx_extra-1.1.1/authx_extra/profiler.py
--rw-r--r--   0        0        0     9282 2020-02-02 00:00:00.000000 authx_extra-1.1.1/authx_extra/session.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx_extra-1.1.1/authx_extra/addons/__init__.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 authx_extra-1.1.1/authx_extra/addons/expiry.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 authx_extra-1.1.1/authx_extra/addons/keys.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx_extra-1.1.1/authx_extra/extra/__init__.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 authx_extra-1.1.1/authx_extra/extra/_cache.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 authx_extra-1.1.1/requirements/all.txt
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 authx_extra-1.1.1/requirements/linting.in
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 authx_extra-1.1.1/requirements/linting.txt
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 authx_extra-1.1.1/requirements/optional.in
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 authx_extra-1.1.1/requirements/optional.txt
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 authx_extra-1.1.1/requirements/pyproject.txt
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 authx_extra-1.1.1/requirements/testing.in
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 authx_extra-1.1.1/requirements/testing.txt
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 authx_extra-1.1.1/scripts/clean.sh
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 authx_extra-1.1.1/scripts/docker.sh
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 authx_extra-1.1.1/scripts/format.sh
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 authx_extra-1.1.1/scripts/lint.sh
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 authx_extra-1.1.1/scripts/requirements.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx_extra-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0     6560 2020-02-02 00:00:00.000000 authx_extra-1.1.1/tests/test_cache.py
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 authx_extra-1.1.1/tests/test_keys.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 authx_extra-1.1.1/tests/test_method_cache.py
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 authx_extra-1.1.1/tests/test_metrics.py
--rw-r--r--   0        0        0    15238 2020-02-02 00:00:00.000000 authx_extra-1.1.1/tests/test_oauth2.py
--rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 authx_extra-1.1.1/tests/test_profiler.py
--rw-r--r--   0        0        0     7375 2020-02-02 00:00:00.000000 authx_extra-1.1.1/tests/test_session_middleware.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 authx_extra-1.1.1/tests/test_skip_session_header_check_dict.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 authx_extra-1.1.1/tests/test_skip_session_header_check_list.py
--rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 authx_extra-1.1.1/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 authx_extra-1.1.1/LICENSE
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 authx_extra-1.1.1/README.md
--rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 authx_extra-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 authx_extra-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 authx_extra-1.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 authx_extra-1.1.2/.github/FUNDING.yml
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 authx_extra-1.1.2/.github/dependabot.yaml
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 authx_extra-1.1.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 authx_extra-1.1.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 authx_extra-1.1.2/authx_extra/__init__.py
+-rw-r--r--   0        0        0     6189 2020-02-02 00:00:00.000000 authx_extra-1.1.2/authx_extra/cache.py
+-rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 authx_extra-1.1.2/authx_extra/metrics.py
+-rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 authx_extra-1.1.2/authx_extra/oauth2.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 authx_extra-1.1.2/authx_extra/profiler.py
+-rw-r--r--   0        0        0     9282 2020-02-02 00:00:00.000000 authx_extra-1.1.2/authx_extra/session.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx_extra-1.1.2/authx_extra/addons/__init__.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 authx_extra-1.1.2/authx_extra/addons/expiry.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 authx_extra-1.1.2/authx_extra/addons/keys.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx_extra-1.1.2/authx_extra/extra/__init__.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 authx_extra-1.1.2/authx_extra/extra/_cache.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 authx_extra-1.1.2/requirements/all.txt
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 authx_extra-1.1.2/requirements/linting.in
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 authx_extra-1.1.2/requirements/linting.txt
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 authx_extra-1.1.2/requirements/pyproject.txt
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 authx_extra-1.1.2/requirements/testing.in
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 authx_extra-1.1.2/requirements/testing.txt
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 authx_extra-1.1.2/scripts/clean.sh
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 authx_extra-1.1.2/scripts/docker.sh
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 authx_extra-1.1.2/scripts/format.sh
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 authx_extra-1.1.2/scripts/lint.sh
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 authx_extra-1.1.2/scripts/requirements.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx_extra-1.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     6560 2020-02-02 00:00:00.000000 authx_extra-1.1.2/tests/test_cache.py
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 authx_extra-1.1.2/tests/test_keys.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 authx_extra-1.1.2/tests/test_method_cache.py
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 authx_extra-1.1.2/tests/test_metrics.py
+-rw-r--r--   0        0        0    15238 2020-02-02 00:00:00.000000 authx_extra-1.1.2/tests/test_oauth2.py
+-rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 authx_extra-1.1.2/tests/test_profiler.py
+-rw-r--r--   0        0        0     7375 2020-02-02 00:00:00.000000 authx_extra-1.1.2/tests/test_session_middleware.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 authx_extra-1.1.2/tests/test_skip_session_header_check_dict.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 authx_extra-1.1.2/tests/test_skip_session_header_check_list.py
+-rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 authx_extra-1.1.2/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 authx_extra-1.1.2/LICENSE
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 authx_extra-1.1.2/README.md
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 authx_extra-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 authx_extra-1.1.2/PKG-INFO
```

### Comparing `authx_extra-1.1.1/.github/workflows/ci.yml` & `authx_extra-1.1.2/.github/workflows/ci.yml`

 * *Files 8% similar despite different names*

```diff
@@ -59,15 +59,15 @@
           python-version: ${{ matrix.python-version }}
       - name: setup uv
         uses: yezz123/setup-uv@v4
         with:
           uv-version: "0.1.27"
           uv-venv: ".venv"
       - name: Install Dependencies
-        run: uv pip install -r requirements/pyproject.txt && uv pip install -r requirements/optional.txt && uv pip install -r requirements/testing.txt
+        run: uv pip install -r requirements/pyproject.txt && uv pip install -r requirements/testing.txt
       - name: Test Suite
         run: pytest --cov=authx_extra --cov-report=xml
         env:
           ENV: test
           REDIS_URL: "redis://0.0.0.0:6379"
       - name: Upload coverage
         uses: codecov/codecov-action@v4
```

### Comparing `authx_extra-1.1.1/.github/workflows/release.yml` & `authx_extra-1.1.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.1/authx_extra/cache.py` & `authx_extra-1.1.2/authx_extra/cache.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.1/authx_extra/metrics.py` & `authx_extra-1.1.2/authx_extra/metrics.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.1/authx_extra/oauth2.py` & `authx_extra-1.1.2/authx_extra/oauth2.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.1/authx_extra/profiler.py` & `authx_extra-1.1.2/authx_extra/profiler.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.1/authx_extra/session.py` & `authx_extra-1.1.2/authx_extra/session.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.1/authx_extra/addons/expiry.py` & `authx_extra-1.1.2/authx_extra/addons/expiry.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.1/authx_extra/addons/keys.py` & `authx_extra-1.1.2/authx_extra/addons/keys.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.1/authx_extra/extra/_cache.py` & `authx_extra-1.1.2/authx_extra/extra/_cache.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.1/requirements/testing.txt` & `authx_extra-1.1.2/requirements/testing.txt`

 * *Files 13% similar despite different names*

```diff
@@ -7,52 +7,52 @@
     #   httpcore
     #   httpx
     #   requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via uvicorn
-coverage==7.4.4
+coverage==7.5.1
     # via pytest-cov
-freezegun==1.4.0
+freezegun==1.5.1
 h11==0.14.0
     # via
     #   httpcore
     #   uvicorn
 httpcore==1.0.5
     # via httpx
 httpx==0.27.0
-idna==3.6
+idna==3.7
     # via
     #   anyio
     #   httpx
     #   requests
 iniconfig==2.0.0
     # via pytest
-itsdangerous==2.1.2
+itsdangerous==2.2.0
 packaging==24.0
     # via pytest
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-pytest==8.1.1
+pytest==8.2.1
     # via
     #   pytest-asyncio
     #   pytest-cov
-pytest-asyncio==0.23.6
+pytest-asyncio==0.23.7
 pytest-cov==5.0.0
 python-dateutil==2.9.0.post0
     # via freezegun
-requests==2.31.0
+requests==2.32.0
 six==1.16.0
     # via python-dateutil
 sniffio==1.3.1
     # via
     #   anyio
     #   httpx
-sqlalchemy==2.0.29
-typing-extensions==4.10.0
+sqlalchemy==2.0.30
+typing-extensions==4.11.0
     # via sqlalchemy
 urllib3==2.2.1
     # via requests
 uvicorn==0.29.0
 uvloop==0.19.0
 websockets==12.0
```

### Comparing `authx_extra-1.1.1/scripts/clean.sh` & `authx_extra-1.1.2/scripts/clean.sh`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.1/scripts/docker.sh` & `authx_extra-1.1.2/scripts/docker.sh`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.1/tests/test_cache.py` & `authx_extra-1.1.2/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.1/tests/test_keys.py` & `authx_extra-1.1.2/tests/test_keys.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.1/tests/test_method_cache.py` & `authx_extra-1.1.2/tests/test_method_cache.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.1/tests/test_metrics.py` & `authx_extra-1.1.2/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.1/tests/test_oauth2.py` & `authx_extra-1.1.2/tests/test_oauth2.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.1/tests/test_profiler.py` & `authx_extra-1.1.2/tests/test_profiler.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.1/tests/test_session_middleware.py` & `authx_extra-1.1.2/tests/test_session_middleware.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.1/tests/test_skip_session_header_check_dict.py` & `authx_extra-1.1.2/tests/test_skip_session_header_check_dict.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.1/tests/test_skip_session_header_check_list.py` & `authx_extra-1.1.2/tests/test_skip_session_header_check_list.py`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.1/.gitignore` & `authx_extra-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.1/LICENSE` & `authx_extra-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.1/README.md` & `authx_extra-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `authx_extra-1.1.1/pyproject.toml` & `authx_extra-1.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "Development Status :: 5 - Production/Stable",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
     "Framework :: FastAPI",
     "Framework :: AsyncIO",
     "Framework :: Pydantic",
-    "Framework :: Pydantic :: 1",
+    "Framework :: Pydantic :: 2",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
@@ -41,38 +41,30 @@
     "Topic :: Internet :: WWW/HTTP :: Session",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Internet",
     "Typing :: Typed",
 ]
 
 dependencies = [
-    "authx >=1.0.0",
+    "authx>=1.1.0,<2.0.0",
+    "redis>=4.3.3,<5.0.5",
+    "prometheus-client>=0.16.0,<1.0.0",
+    "pyinstrument>=4.1.1,<4.7.0",
 ]
 
 dynamic = ["version"]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [project.urls]
 Homepage = "https://github.com/yezz123/authx_extra"
 Documentation = "https://authx.yezz.me/installation/#extra-dependencies"
 Funding = 'https://github.com/sponsors/yezz123'
 
-[project.optional-dependencies]
-profiler = [
-    "pyinstrument>=4.1.1,<4.7.0",
-]
-metrics = [
-    "prometheus-client>=0.16.0,<1.0.0",
-]
-cache = [
-    "redis>=4.3.3,<5.0.4",
-]
-
 [tool.hatch.version]
 path = "authx_extra/__init__.py"
 
 
 [tool.ruff.lint]
 mccabe = { max-complexity = 14 }
 select = [
```

### Comparing `authx_extra-1.1.1/PKG-INFO` & `authx_extra-1.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.3
 Name: authx_extra
-Version: 1.1.1
+Version: 1.1.2
 Summary: Extra utilities for authx, including session, profiler & caching ✨
 Project-URL: Homepage, https://github.com/yezz123/authx_extra
 Project-URL: Documentation, https://authx.yezz.me/installation/#extra-dependencies
 Project-URL: Funding, https://github.com/sponsors/yezz123
 Author-email: Yasser Tahiri <hello@yezz.me>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: Authentication,Cookie,FastAPI,JWT,Oauth2,Pydantic
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: Framework :: FastAPI
 Classifier: Framework :: Pydantic
-Classifier: Framework :: Pydantic :: 1
+Classifier: Framework :: Pydantic :: 2
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -27,21 +27,18 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: authx>=1.0.0
-Provides-Extra: cache
-Requires-Dist: redis<5.0.4,>=4.3.3; extra == 'cache'
-Provides-Extra: metrics
-Requires-Dist: prometheus-client<1.0.0,>=0.16.0; extra == 'metrics'
-Provides-Extra: profiler
-Requires-Dist: pyinstrument<4.7.0,>=4.1.1; extra == 'profiler'
+Requires-Dist: authx<2.0.0,>=1.1.0
+Requires-Dist: prometheus-client<1.0.0,>=0.16.0
+Requires-Dist: pyinstrument<4.7.0,>=4.1.1
+Requires-Dist: redis<5.0.5,>=4.3.3
 Description-Content-Type: text/markdown
 
 # authx-extra 💫
 
 <p align="center">
 <a href="https://authx.yezz.me" target="_blank">
     <img src="https://user-images.githubusercontent.com/52716203/136962014-280d82b0-0640-4ee5-9a11-b451b338f6d8.png" alt="AuthX">
```

#### html2text {}

```diff
@@ -1,32 +1,30 @@
-Metadata-Version: 2.3 Name: authx_extra Version: 1.1.1 Summary: Extra utilities
+Metadata-Version: 2.3 Name: authx_extra Version: 1.1.2 Summary: Extra utilities
 for authx, including session, profiler & caching â¨ Project-URL: Homepage,
 https://github.com/yezz123/authx_extra Project-URL: Documentation, https://
 authx.yezz.me/installation/#extra-dependencies Project-URL: Funding, https://
 github.com/sponsors/yezz123 Author-email: Yasser Tahiri
 yezz.me> License-Expression: MIT License-File: LICENSE Keywords:
 Authentication,Cookie,FastAPI,JWT,Oauth2,Pydantic Classifier: Development
 Status :: 5 - Production/Stable Classifier: Framework :: AsyncIO Classifier:
 Framework :: FastAPI Classifier: Framework :: Pydantic Classifier: Framework ::
-Pydantic :: 1 Classifier: Intended Audience :: Developers Classifier: Intended
+Pydantic :: 2 Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Information Technology Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Internet Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Typing :: Typed Requires-Python: >=3.8 Requires-Dist: authx>=1.0.0
-Provides-Extra: cache Requires-Dist: redis<5.0.4,>=4.3.3; extra == 'cache'
-Provides-Extra: metrics Requires-Dist: prometheus-client<1.0.0,>=0.16.0; extra
-== 'metrics' Provides-Extra: profiler Requires-Dist:
-pyinstrument<4.7.0,>=4.1.1; extra == 'profiler' Description-Content-Type: text/
-markdown # authx-extra ð«
+Classifier: Typing :: Typed Requires-Python: >=3.8 Requires-Dist:
+authx<2.0.0,>=1.1.0 Requires-Dist: prometheus-client<1.0.0,>=0.16.0 Requires-
+Dist: pyinstrument<4.7.0,>=4.1.1 Requires-Dist: redis<5.0.5,>=4.3.3
+Description-Content-Type: text/markdown # authx-extra ð«
                                     _[_A_u_t_h_X_]
      EExxttrraa uuttiilliittiieess ffoorr aauutthhxx,, iinncclluuddiinngg sseessssiioonn,, pprrooffiilleerr && ccaacchhiinngg ?â??¨
  _[_c_i_]_[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_y_e_z_z_1_2_3_/_a_u_t_h_x_-_e_x_t_r_a_/_b_r_a_n_c_h_/_m_a_i_n_/
                                _g_r_a_p_h_/_b_a_d_g_e_._s_v_g_]
 --- **Source Code**:
 github.com/yezz123/authx-extra> **Documentation**:
 authx.yezz.me/> --- ## Features ð§ - [x] Using Redis as a session store &
```

