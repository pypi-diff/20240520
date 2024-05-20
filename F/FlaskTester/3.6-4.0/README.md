# Comparing `tmp/FlaskTester-3.6.tar.gz` & `tmp/flasktester-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlaskTester-3.6.tar", last modified: Sat Mar 30 15:25:39 2024, max compression
+gzip compressed data, was "flasktester-4.0.tar", last modified: Mon May 20 09:42:17 2024, max compression
```

## Comparing `FlaskTester-3.6.tar` & `flasktester-4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwx------   0 fabien    (1001) fabien    (1001)        0 2024-03-30 15:25:39.531699 FlaskTester-3.6/
-drwx------   0 fabien    (1001) fabien    (1001)        0 2024-03-30 15:25:39.531699 FlaskTester-3.6/FlaskTester.egg-info/
--rw-r--r--   0 fabien    (1001) fabien    (1001)     6040 2024-03-30 15:25:39.000000 FlaskTester-3.6/FlaskTester.egg-info/PKG-INFO
--rw-------   0 fabien    (1001) fabien    (1001)      270 2024-03-30 15:25:39.000000 FlaskTester-3.6/FlaskTester.egg-info/SOURCES.txt
--rw-------   0 fabien    (1001) fabien    (1001)        1 2024-03-30 15:25:39.000000 FlaskTester-3.6/FlaskTester.egg-info/dependency_links.txt
--rw-------   0 fabien    (1001) fabien    (1001)      222 2024-03-30 15:25:39.000000 FlaskTester-3.6/FlaskTester.egg-info/requires.txt
--rw-------   0 fabien    (1001) fabien    (1001)       12 2024-03-30 15:25:39.000000 FlaskTester-3.6/FlaskTester.egg-info/top_level.txt
--rwx------   0 fabien    (1001) fabien    (1001)    20854 2024-03-30 15:13:17.000000 FlaskTester-3.6/FlaskTester.py
--rw-------   0 fabien    (1001) fabien    (1001)       33 2024-03-12 08:26:22.000000 FlaskTester-3.6/LICENSE
--rw-------   0 fabien    (1001) fabien    (1001)       26 2024-03-16 17:14:38.000000 FlaskTester-3.6/MANIFEST.in
--rw-r--r--   0 fabien    (1001) fabien    (1001)     6040 2024-03-30 15:25:39.531699 FlaskTester-3.6/PKG-INFO
--rw-------   0 fabien    (1001) fabien    (1001)     4318 2024-03-30 15:08:23.000000 FlaskTester-3.6/README.md
--rw-------   0 fabien    (1001) fabien    (1001)     1427 2024-03-30 15:12:14.000000 FlaskTester-3.6/pyproject.toml
--rw-------   0 fabien    (1001) fabien    (1001)       38 2024-03-30 15:25:39.531699 FlaskTester-3.6/setup.cfg
-drwx------   0 fabien    (1001) fabien    (1001)        0 2024-03-30 15:25:39.531699 FlaskTester-3.6/tests/
--rw-------   0 fabien    (1001) fabien    (1001)    14021 2024-03-30 15:20:14.000000 FlaskTester-3.6/tests/test_app.py
--rw-------   0 fabien    (1001) fabien    (1001)     1017 2024-03-30 13:28:13.000000 FlaskTester-3.6/tests/test_app2.py
+drwx------   0 fabien    (1001) fabien    (1001)        0 2024-05-20 09:42:17.858802 flasktester-4.0/
+drwx------   0 fabien    (1001) fabien    (1001)        0 2024-05-20 09:42:17.858802 flasktester-4.0/FlaskTester.egg-info/
+-rw-r--r--   0 fabien    (1001) fabien    (1001)     6045 2024-05-20 09:42:17.000000 flasktester-4.0/FlaskTester.egg-info/PKG-INFO
+-rw-------   0 fabien    (1001) fabien    (1001)      270 2024-05-20 09:42:17.000000 flasktester-4.0/FlaskTester.egg-info/SOURCES.txt
+-rw-------   0 fabien    (1001) fabien    (1001)        1 2024-05-20 09:42:17.000000 flasktester-4.0/FlaskTester.egg-info/dependency_links.txt
+-rw-------   0 fabien    (1001) fabien    (1001)      222 2024-05-20 09:42:17.000000 flasktester-4.0/FlaskTester.egg-info/requires.txt
+-rw-------   0 fabien    (1001) fabien    (1001)       12 2024-05-20 09:42:17.000000 flasktester-4.0/FlaskTester.egg-info/top_level.txt
+-rwx------   0 fabien    (1001) fabien    (1001)    20761 2024-05-20 08:50:26.000000 flasktester-4.0/FlaskTester.py
+-rw-------   0 fabien    (1001) fabien    (1001)       33 2024-03-12 08:26:22.000000 flasktester-4.0/LICENSE
+-rw-------   0 fabien    (1001) fabien    (1001)       26 2024-03-16 17:14:38.000000 flasktester-4.0/MANIFEST.in
+-rw-r--r--   0 fabien    (1001) fabien    (1001)     6045 2024-05-20 09:42:17.858802 flasktester-4.0/PKG-INFO
+-rw-------   0 fabien    (1001) fabien    (1001)     4323 2024-03-30 15:48:31.000000 flasktester-4.0/README.md
+-rw-------   0 fabien    (1001) fabien    (1001)     1427 2024-05-20 09:40:44.000000 flasktester-4.0/pyproject.toml
+-rw-------   0 fabien    (1001) fabien    (1001)       38 2024-05-20 09:42:17.858802 flasktester-4.0/setup.cfg
+drwx------   0 fabien    (1001) fabien    (1001)        0 2024-05-20 09:42:17.858802 flasktester-4.0/tests/
+-rw-------   0 fabien    (1001) fabien    (1001)    13746 2024-05-20 08:51:20.000000 flasktester-4.0/tests/test_app.py
+-rw-------   0 fabien    (1001) fabien    (1001)     1081 2024-03-31 07:28:43.000000 flasktester-4.0/tests/test_app2.py
```

### Comparing `FlaskTester-3.6/FlaskTester.egg-info/PKG-INFO` & `flasktester-4.0/FlaskTester.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlaskTester
-Version: 3.6
+Version: 4.0
 Summary: Pytest fixtures for Flask internal and external authenticated tests
 Author-email: Fabien Coelho <flask.tester@coelho.net>
 License: CC0
 Project-URL: repository, https://github.com/zx80/flask-tester
 Project-URL: documentation, https://zx80.github.io/flask-tester/
 Project-URL: issues, https://github.com/zx80/flask-tester/issues
 Project-URL: package, https://pypi.org/project/FlaskTester/
@@ -45,15 +45,15 @@
 
 This package allows to run authenticated tests against a Flask application,
 either with internal Flask tests (aka `test_client`) or external tests (with
 `requests` which performs actual HTTP requests), including password and token
 authentication and per-user cookies.
 
 Only one set of tests is needed, switching from internal to external is
-achieved through environment variables.
+achieved by setting an environment variable.
 
 ![Status](https://github.com/zx80/flask-tester/actions/workflows/package.yml/badge.svg?branch=main&style=flat)
 ![Tests](https://img.shields.io/badge/tests-14%20✓-success)
 ![Coverage](https://img.shields.io/badge/coverage-100%25-success)
 ![Issues](https://img.shields.io/github/issues/zx80/flask-tester?style=flat)
 ![Python](https://img.shields.io/badge/python-3-informational)
 ![Version](https://img.shields.io/pypi/v/FlaskTester)
```

### Comparing `FlaskTester-3.6/FlaskTester.py` & `flasktester-4.0/FlaskTester.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,20 +25,23 @@
 
 
 class _AssertError(FlaskTesterError):
     """User assertion Exception, only for internal testing."""
     pass
 
 
-def _raiseError(msg: str):
-    """Undocumented switch for FlaskTester own tests."""
+def _pytestFail(msg: str):
+    """Undocumented switch for FlaskTester own tests.
+
+    A pytest test cannot check an expected pytest failure without failing.
+    """
     log.error(msg)
     if "FLASK_TESTER_TESTING" in os.environ:
         raise _AssertError(msg)
-    else:  # pragma: no cover  # cannot cover an expected pytest failure!
+    else:  # pragma: no cover
         pytest.fail(msg)
 
 
 class Authenticator:
     """Manage HTTP request authentication.
 
     Supported schemes:
@@ -50,32 +53,32 @@
     - ``cookie``: token in a cookie.
     - ``tparam``: token in a parameter.
     - ``fake``: fake scheme, login directly passed as a parameter.
     - ``none``: no authentication, only cookies.
 
     Constructor parameters:
 
-    - ``allow``: list of allowed schemes.
-      default is ``["bearer", "basic", "param", "none"]``.
-    - ``user``: parameter for user on ``param`` password authentication,
-      default is ``USER``.
-    - ``pwd``: parameter for password on ``param`` password authentication,
-      default is ``PASS``.
-    - ``login``: parameter for user on ``fake`` authentication,
-      default is ``LOGIN``.
-    - ``bearer``: name of bearer scheme for token,
-      default is ``Bearer``.
-    - ``header``: name of header for token,
-      default is ``Auth``.
-    - ``cookie``: name of cookie for token,
-      default is ``auth``.
-    - ``tparam``: name of parameter for token,
-      default is ``AUTH``.
-    - ``ptype``: default parameter type, either ``data`` or ``json``,
-      default is ``data``.
+    :param allow: List of allowed schemes.
+        defaults to ``["bearer", "basic", "param", "none"]``.
+    :param user: Parameter for user on ``param`` password authentication,
+        defaults to ``"USER"``.
+    :param pwd: Parameter for password on ``param`` password authentication,
+        defaults to ``"PASS"``.
+    :param login: Parameter for user on ``fake`` authentication,
+        defaults to ``"LOGIN"``.
+    :param bearer: Name of bearer scheme for token,
+        defaults to ``"Bearer"``.
+    :param header: Name of header for token,
+        defaults to ``"Auth"``.
+    :param cookie: Name of cookie for token,
+        defaults to ``"auth"``.
+    :param tparam: Name of parameter for token,
+        defaults to ``"AUTH"``.
+    :param ptype: Default parameter type, either *data* or *json*,
+        defaults to ``"data"``.
 
     Note: default values are consistent with `FlaskSimpleAuth <https://pypi.org/project/FlaskSimpleAuth/>`_.
     """
 
     _TOKEN_SCHEMES = {"bearer", "header", "cookie", "tparam"}
     _PASS_SCHEMES = {"basic", "param"}
 
@@ -178,20 +181,20 @@
     def _try_auth(self, auth: str|None, scheme: str) -> bool:
         """Whether to try this authentication scheme."""
         return auth in (None, scheme) and scheme in self._allow
 
     def setAuth(self, login: str|None, kwargs: dict[str, Any], cookies: dict[str, str], auth: str|None = None):
         """Set request authentication.
 
-        - ``login``: login target, None means no authentication.
-        - ``kwargs``: request parameters.
-        - ``cookies``: request cookies.
-        - ``auth``: authentication method, default is None.
+        :param login: Login target, *None* means no authentication.
+        :param kwargs: Request parameters to modify.
+        :param cookies: Request cookies to modify.
+        :param auth: Authentication method, default is *None*.
 
-        The default behavior is to try allowed schemes: tokens first,
+        The default behavior is to try allowed schemes: token first,
         then password, then fake.
         """
 
         log.debug(f"setAuth: login={login} auth={auth} allow={self._allow}")
 
         if login is None:  # not needed
             return
@@ -247,29 +250,29 @@
         if headers:  # put headers back if needed
             kwargs["headers"] = headers
 
 
 class RequestFlaskResponse:
     """Wrapper to return a Flask-looking response from a request response.
 
-    This only work for simple responses.
+    This only works for simple responses.
 
-    Available attributes:
+    Available public attributes:
 
     - ``status_code``: integer status code.
     - ``data``: body as bytes.
     - ``text``: body as a string.
     - ``headers``: dict of headers and their values.
     - ``cookies``: dict of cookies.
     - ``json``: JSON-converted body, or *None*.
     - ``is_json``: whether body was in JSON.
 
     Constructor parameter:
 
-    - ``response``: from request.
+    :param response: Response from request.
     """
 
     def __init__(self, response):
 
         self._response = response
         self.status_code = response.status_code
         self.data = response.content
@@ -285,16 +288,16 @@
 
 
 class Client:
     """Common (partial) class for flask authenticated testing.
 
     Constructor parameters:
 
-    - ``auth``: authenticator.
-    - ``default_login``: if ``login`` is not set.
+    :param auth: Authenticator.
+    :param default_login: When ``login`` is not set.
     """
 
     def __init__(self, auth: Authenticator, default_login: str|None = None):
         self._auth = auth
         self._cookies: dict[str, dict[str, str]] = {}  # login -> name -> value
         self._default_login = default_login
 
@@ -316,24 +319,24 @@
 
     def request(self, method: str, path: str, status: int|None = None, content: str|None = None,
                 auth: str|None = None, **kwargs):
         """Run a possibly authenticated HTTP request.
 
         Mandatory parameters:
 
-        - ``method``: HTTP method ("GET", "POST", "PATCH", "DELETE"…).
-        - ``path``: local path under the base URL.
+        :param method: HTTP method ("GET", "POST", "PATCH", "DELETE"…).
+        :param path: Local path under the base URL.
 
         Optional parameters:
 
-        - ``status``: expected HTTP status, *None* to skip status check.
-        - ``content``: regular expression for response body, *None* to skip content check.
-        - ``login``: authenticated user, use **explicit** *None* to skip.
-        - ``auth``: authentication scheme to use instead of default behavior.
-        - ``**kwargs``: more request parameters (headers, data, json…).
+        :param status: Expected HTTP status, *None* to skip status check.
+        :param content: Regular expression for response body, *None* to skip content check.
+        :param login: Authenticated user, use **explicit** *None* to skip default.
+        :param auth: Authentication scheme to use instead of default behavior.
+        :param **kwargs: More request parameters (headers, data, json…).
         """
 
         if "login" in kwargs:
             login = kwargs["login"]
             del kwargs["login"]
         else:  # if unset, use default
             login = self._default_login
@@ -345,56 +348,52 @@
 
         self._auth.setAuth(login, kwargs, cookies, auth=auth)
         res = self._request(method, path, cookies, **kwargs)  # type: ignore
 
         # check status
         if status is not None:
             if res.status_code != status:  # show error before aborting
-                _raiseError(f"bad {status} result: {res.status_code} {res.text[:512]}...")
+                _pytestFail(f"bad {status} result: {res.status_code} {res.text[:512]}...")
 
         # check content
         if content is not None:
             if not re.search(content, res.text, re.DOTALL):
-                _raiseError(f"cannot find {content} in {res.text[:512]}...")
+                _pytestFail(f"cannot find {content} in {res.text[:512]}...")
 
         return res
 
     def get(self, path: str, status: int|None = None, content: str|None = None, **kwargs):
-        """HTTP GET request, see ``request`` parameters."""
+        """HTTP GET request, see `Client.request`."""
         return self.request("GET", path, status=status, content=content, **kwargs)
 
     def post(self, path: str, status: int|None = None, content: str|None = None, **kwargs):
-        """HTTP POST request, see ``request`` parameters."""
+        """HTTP POST request, see `Client.request`."""
         return self.request("POST", path, status=status, content=content, **kwargs)
 
     def put(self, path: str, status: int|None = None, content: str|None = None, **kwargs):
-        """HTTP PUT request, see ``request`` parameters."""
+        """HTTP PUT request, see `Client.request`."""
         return self.request("PUT", path, status=status, content=content, **kwargs)
 
     def patch(self, path: str, status: int|None = None, content: str|None = None, **kwargs):
-        """HTTP PATCH request, see ``request`` parameters."""
+        """HTTP PATCH request, see `Client.request`."""
         return self.request("PATCH", path, status=status, content=content, **kwargs)
 
     def delete(self, path: str, status: int|None = None, content: str|None = None, **kwargs):
-        """HTTP DELETE request, see ``request`` parameters."""
+        """HTTP DELETE request, see `Client.request`."""
         return self.request("DELETE", path, status=status, content=content, **kwargs)
 
-    def check(self, method: str, path: str, status: int, content: str|None = None, **kwargs):
-        """Deprecated, use ``request`` or HTTP-method-specific methods."""
-        return self.request(method, path, status=status, content=content, **kwargs)
-
 
 class RequestClient(Client):
     """Request-based test provider.
 
     Constructor parameters:
 
-    - ``auth``: authenticator.
-    - ``base_url``: target server.
-    - ``default_login``: if ``login`` is not set.
+    :param auth: Authenticator.
+    :param base_url: Target server.
+    :param default_login: When ``login`` is not set.
     """
 
     def __init__(self, auth: Authenticator, base_url: str, default_login=None):
         super().__init__(auth, default_login)
         self._base_url = base_url
         # reuse connections, otherwise it is too slow…
         from requests import Session
@@ -430,17 +429,17 @@
 
 
 class FlaskClient(Client):
     """Flask-based test provider.
 
     Constructor parameters:
 
-    - ``auth``: authenticator.
-    - ``client``: Flask actual ``test_client``.
-    - ``default_login``: if ``login`` is not set.
+    :param auth: Authenticator.
+    :param client: Flask actual ``test_client``.
+    :param default_login: When ``login`` is not set.
 
     Note: this client handles `cookies`.
     """
 
     def __init__(self, auth: Authenticator, client, default_login=None):
         super().__init__(auth, default_login)
         self._client = client
@@ -495,78 +494,80 @@
 @pytest.fixture
 def ft_authenticator():
     """Pytest Fixture: ft_authenticator.
 
     Environment variables:
 
     - ``FLASK_TESTER_LOG_LEVEL``: package log level in
-      ``DEBUG INFO WARNING ERROR CRITICAL NOSET``.
-      Default is ``NOTSET``.
+      ``DEBUG INFO WARNING ERROR CRITICAL NOSET``,
+      defaults to ``NOTSET``.
     - ``FLASK_TESTER_ALLOW``: allowed space-separated authentication schemes, in
-      ``basic param bearer header cookie tparam fake none``.
-      Default is ``bearer basic param none``.
-    - ``FLASK_TESTER_USER``: user login parameter for ``param`` authentication.
-      Default is ``USER``.
-    - ``FLASK_TESTER_PASS``: user password parameter for ``param`` authentication.
-      Default is ``PASS``.
-    - ``FLASK_TESTER_LOGIN``: user login parameter for ``fake`` authentication.
-      Default is ``LOGIN``.
-    - ``FLASK_TESTER_BEARER``: bearer name for *token* authentication.
-      Default is ``Bearer``.
-    - ``FLASK_TESTER_HEADER``: header name for *token* authentication.
-      Default is ``Auth``.
-    - ``FLASK_TESTER_COOKIE``: cookie name for *token* authentication.
-      Default is ``auth``.
-    - ``FLASK_TESTER_TPARAM``: parameter for *token* authentication.
-      Default is ``AUTH``.
-    - ``FLASK_TESTER_PTYPE``: default parameter type, ``data`` or ``json``.
-      Default is ``data``.
-    - ``FLASK_TESTER_AUTH``: initial comma-separated list of *login:password*.
-      Default is not set.
+      ``basic param bearer header cookie tparam fake none``,
+      defaults to ``bearer basic param none``.
+    - ``FLASK_TESTER_USER``: user login parameter for ``param`` authentication,
+      defaults to ``USER``.
+    - ``FLASK_TESTER_PASS``: user password parameter for ``param`` authentication,
+      defaults to ``PASS``.
+    - ``FLASK_TESTER_LOGIN``: user login parameter for ``fake`` authentication,
+      defaults to ``LOGIN``.
+    - ``FLASK_TESTER_BEARER``: bearer name for *token* authentication,
+      defaults to ``Bearer``.
+    - ``FLASK_TESTER_HEADER``: header name for *token* authentication,
+      defaults to ``Auth``.
+    - ``FLASK_TESTER_COOKIE``: cookie name for *token* authentication,
+      defaults to ``auth``.
+    - ``FLASK_TESTER_TPARAM``: parameter for *token* authentication,
+      defaults to ``AUTH``.
+    - ``FLASK_TESTER_PTYPE``: default parameter type, ``data`` or ``json``,
+      defaults to ``data``.
+    - ``FLASK_TESTER_AUTH``: initial comma-separated list of *login:password*,
+      defaults to not set.
     """
 
     yield _ft_authenticator()
 
 def _ft_client(authenticator):
     """Fixture implementation separated for testing."""
 
     default_login = os.environ.get("FLASK_TESTER_DEFAULT", None)
     client: Client
 
-    app_def = os.environ.get("FLASK_TESTER_URL", "app")
-    app_def = os.environ.get("FLASK_TESTER_APP", app_def)
+    test_app = os.environ.get("FLASK_TESTER_APP", "app")
 
-    if app_def.startswith("http://") or app_def.startswith("https://"):
-        client = RequestClient(authenticator, app_def, default_login)
+    if test_app.startswith("http://") or test_app.startswith("https://"):
+        client = RequestClient(authenticator, test_app, default_login)
     else:
         # load app package
-        pkg_name, app = app_def, None
-        app_names = ["app", "application", "create_app", "make_app"]
-        if ":" in pkg_name:  # override defaults
-            pkg_name, app_name = pkg_name.split(":", 1)
+        if ":" in test_app:  # override defaults
+            pkg_name, app_name = test_app.split(":", 1)
             app_names = [app_name]
+        else:
+            pkg_name = test_app
+            app_names = ["app", "application", "create_app", "make_app"]
         pkg = importlib.import_module(pkg_name)
         # find app in package
+        app = None
         for name in app_names:
             if hasattr(pkg, name):
                 app = getattr(pkg, name)
                 if callable(app) and not hasattr(app, "test_client"):
                     app = app()
                 break
+        # none found
         if not app:
-            raise FlaskTesterError(f"cannot find Flask app in {pkg_name}")
+            raise FlaskTesterError(f"cannot find Flask app in {pkg_name} ({test_app})")
         client = FlaskClient(authenticator, app.test_client(), default_login)
 
     return client
 
 @pytest.fixture
 def ft_client(ft_authenticator):
     """Pytest Fixture: ft_client.
 
-    Target environment variable:
+    Mandatory target environment variable:
 
     - ``FLASK_TESTER_APP``: find the Flask application, eg
       ``app:create_app`` for an internal test, or
       ``http://localhost:5000`` for an external test.
 
     Other environment variable:
```

### Comparing `FlaskTester-3.6/PKG-INFO` & `flasktester-4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlaskTester
-Version: 3.6
+Version: 4.0
 Summary: Pytest fixtures for Flask internal and external authenticated tests
 Author-email: Fabien Coelho <flask.tester@coelho.net>
 License: CC0
 Project-URL: repository, https://github.com/zx80/flask-tester
 Project-URL: documentation, https://zx80.github.io/flask-tester/
 Project-URL: issues, https://github.com/zx80/flask-tester/issues
 Project-URL: package, https://pypi.org/project/FlaskTester/
@@ -45,15 +45,15 @@
 
 This package allows to run authenticated tests against a Flask application,
 either with internal Flask tests (aka `test_client`) or external tests (with
 `requests` which performs actual HTTP requests), including password and token
 authentication and per-user cookies.
 
 Only one set of tests is needed, switching from internal to external is
-achieved through environment variables.
+achieved by setting an environment variable.
 
 ![Status](https://github.com/zx80/flask-tester/actions/workflows/package.yml/badge.svg?branch=main&style=flat)
 ![Tests](https://img.shields.io/badge/tests-14%20✓-success)
 ![Coverage](https://img.shields.io/badge/coverage-100%25-success)
 ![Issues](https://img.shields.io/github/issues/zx80/flask-tester?style=flat)
 ![Python](https://img.shields.io/badge/python-3-informational)
 ![Version](https://img.shields.io/pypi/v/FlaskTester)
```

### Comparing `FlaskTester-3.6/README.md` & `flasktester-4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 This package allows to run authenticated tests against a Flask application,
 either with internal Flask tests (aka `test_client`) or external tests (with
 `requests` which performs actual HTTP requests), including password and token
 authentication and per-user cookies.
 
 Only one set of tests is needed, switching from internal to external is
-achieved through environment variables.
+achieved by setting an environment variable.
 
 ![Status](https://github.com/zx80/flask-tester/actions/workflows/package.yml/badge.svg?branch=main&style=flat)
 ![Tests](https://img.shields.io/badge/tests-14%20✓-success)
 ![Coverage](https://img.shields.io/badge/coverage-100%25-success)
 ![Issues](https://img.shields.io/github/issues/zx80/flask-tester?style=flat)
 ![Python](https://img.shields.io/badge/python-3-informational)
 ![Version](https://img.shields.io/pypi/v/FlaskTester)
```

### Comparing `FlaskTester-3.6/pyproject.toml` & `flasktester-4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "FlaskTester"
-version = "3.6"
+version = "4.0"
 authors = [ { name = "Fabien Coelho", email = "flask.tester@coelho.net" } ]
 description = "Pytest fixtures for Flask internal and external authenticated tests"
 readme = "README.md"
 license = { text = "CC0" }
 requires-python = ">=3.10"
 dependencies = [
   "requests",
```

### Comparing `FlaskTester-3.6/tests/test_app.py` & `flasktester-4.0/tests/test_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     FLASK_TESTER_TESTING="*",
     FLASK_TESTER_ALLOW="bearer basic param none",
     FLASK_TESTER_AUTH=",".join(f"{l}:{p}" for l, p in secret.PASSES.items()),
 )
 
 def test_sanity():
     # must provide url or package of Flask application to test
-    assert "FLASK_TESTER_URL" in os.environ or "FLASK_TESTER_APP" in os.environ
+    assert "FLASK_TESTER_APP" in os.environ
     # log.debug(f"TEST_SEED={os.environ.get('TEST_SEED')}")
 
 # example from README.md
 @pytest.fixture
 def app(ft_client):
     # add test passwords for Calvin and Hobbes (must be consistent with app!)
     ft_client.setPass("calvin", secret.PASSES["calvin"])
@@ -292,42 +292,38 @@
     # start a tmp server on port 8888 for URL client coverage
     httpd = htsv.HTTPServer(("", 8888), htsv.SimpleHTTPRequestHandler)
     thread = threading.Thread(target = lambda: httpd.serve_forever())
     thread.start()
     try:
         client = ft.RequestClient(ft.Authenticator(), "http://localhost:8888")
         client.get("/", 200)
-        client.check("GET", "/", 200)
+        client.request("GET", "/", 200)
         hello = io.BytesIO(b"hello world")
         client.post("/", 501, data={"hello": hello})
         hello = io.BytesIO(b"hello world")
         client.post("/", 501, data={"hello": (hello, "hello.txt", "text/plain")})
         client.post("/", 501, data={"hello": "world!"})
     finally:
         httpd.shutdown()
 
 def test_client_fixture():
     # ft_client coverage
     auth = ft._ft_authenticator()
     # check and save env
-    url = None
-    if "FLASK_TESTER_URL" in os.environ:  # pragma: no cover
-        url = os.environ["FLASK_TESTER_URL"]
-        del os.environ["FLASK_TESTER_URL"]
     app = None
     if "FLASK_TESTER_APP" in os.environ:
         app = os.environ["FLASK_TESTER_APP"]
         del os.environ["FLASK_TESTER_APP"]
     # no url nor app, defaults to "app"
     init = ft._ft_client(auth)
     # url
-    os.environ["FLASK_TESTER_URL"] = "http://localhost:5000"
+    os.environ["FLASK_TESTER_APP"] = "http://localhost:5000"
     init = ft._ft_client(auth)
     assert isinstance(init, ft.RequestClient)
-    del os.environ["FLASK_TESTER_URL"]
+    del os.environ["FLASK_TESTER_APP"]
     # bad package
     os.environ["FLASK_TESTER_APP"] = "no_such_package"
     try:
         init = ft._ft_client(auth)
         pytest.fail("must fail on missing package")  # pragma: no cover
     except ModuleNotFoundError:
         assert True, "expected error raised"
@@ -336,11 +332,9 @@
     try:
         init = ft._ft_client(auth)
         pytest.fail("must fail on missing package")  # pragma: no cover
     except ft.FlaskTesterError:
         assert True, "expected error raised"
     del os.environ["FLASK_TESTER_APP"]
     # reset env
-    if url:  # pragma: no cover
-        os.environ["FLASK_TESTER_URL"] = url
     if app:
         os.environ["FLASK_TESTER_APP"] = app
```

### Comparing `FlaskTester-3.6/tests/test_app2.py` & `flasktester-4.0/tests/test_app2.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import os
 import pytest
 from FlaskTester import ft_client, ft_authenticator
+import secret
 
 os.environ.update(FLASK_TESTER_ALLOW="basic param none")
 
 @pytest.fixture
 def app(ft_client):
-    ft_client.setPass("calvin", "clv-pw")
+    ft_client.setPass("calvin", secret.PASSES["calvin"])
     ft_client.setCookie("calvin", "lang", "en")
-    ft_client.setPass("hobbes", "hbs-pw")
+    ft_client.setPass("hobbes", secret.PASSES["hobbes"])
     ft_client.setCookie("hobbes", "lang", "fr")
     yield ft_client
 
 def test_something(app):
     # requires an authentication
     app.get("/authenticated", 401, login=None)
-    res = app.get("/authenticated", 200, login="calvin")
-    assert "Hello" in res.text
+    app.get("/authenticated", 200, "Hello", login="calvin")
     app.get("/authenticated", 200, "Bonjour", login="hobbes")
     # only allowed to calvin
-    app.get("/only-calvin", 401, login=None)
-    app.get("/only-calvin", 200, login="calvin")
-    app.get("/only-calvin", 403, login="hobbes")
+    app.get("/only-admin", 401, login=None)
+    app.get("/only-admin", 200, "administrateur", login="calvin")
+    app.get("/only-admin", 403, "not in group", login="hobbes")
     # no authentication required, but depends on lang
-    res = app.get("/no-auth", 200, login="calvin", auth="none")
-    assert "Hello" in res.text
-    app.get("/no-auth", 200, "Bonjour", login="hobbes", auth="none")
+    app.get("/open", 200, "Hello", login="calvin", auth="none")
+    app.get("/open", 200, "Bonjour", login="hobbes", auth="none")
+    app.get("/open", 200, "Guten Tag", login=None)
```

