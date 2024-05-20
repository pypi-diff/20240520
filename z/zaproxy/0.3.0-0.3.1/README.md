# Comparing `tmp/zaproxy-0.3.0.tar.gz` & `tmp/zaproxy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zaproxy-0.3.0.tar", max compression
+gzip compressed data, was "zaproxy-0.3.1.tar", max compression
```

## Comparing `zaproxy-0.3.0.tar` & `zaproxy-0.3.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    11357 2024-05-10 07:42:35.993695 zaproxy-0.3.0/LICENSE
--rw-r--r--   0        0        0     1114 2024-05-10 07:42:35.993695 zaproxy-0.3.0/README.md
--rw-r--r--   0        0        0     1467 2024-05-10 07:42:35.993695 zaproxy-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     7894 2024-05-10 07:42:35.993695 zaproxy-0.3.0/src/zapv2/__init__.py
--rw-r--r--   0        0        0     3123 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/accessControl.py
--rw-r--r--   0        0        0     2610 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/acsrf.py
--rw-r--r--   0        0        0    16351 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/ajaxSpider.py
--rw-r--r--   0        0        0     7597 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/alert.py
--rw-r--r--   0        0        0     9098 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/alertFilter.py
--rw-r--r--   0        0        0    28082 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/ascan.py
--rw-r--r--   0        0        0     3694 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/authentication.py
--rw-r--r--   0        0        0     2266 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/authorization.py
--rw-r--r--   0        0        0     1693 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/automation.py
--rw-r--r--   0        0        0     8349 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/autoupdate.py
--rw-r--r--   0        0        0     4479 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/brk.py
--rw-r--r--   0        0        0     7885 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/context.py
--rw-r--r--   0        0        0    30289 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/core.py
--rw-r--r--   0        0        0     4430 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/custompayloads.py
--rw-r--r--   0        0        0     4089 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/exim.py
--rw-r--r--   0        0        0     2036 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/forcedUser.py
--rw-r--r--   0        0        0     8201 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/graphql.py
--rw-r--r--   0        0        0     5977 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/httpSessions.py
--rw-r--r--   0        0        0     2127 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/localProxies.py
--rw-r--r--   0        0        0    19754 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/network.py
--rw-r--r--   0        0        0     1938 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/openapi.py
--rw-r--r--   0        0        0     1195 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/params.py
--rw-r--r--   0        0        0     2921 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/pnh.py
--rw-r--r--   0        0        0     5392 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/pscan.py
--rw-r--r--   0        0        0     3296 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/replacer.py
--rw-r--r--   0        0        0     2988 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/reports.py
--rw-r--r--   0        0        0     1132 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/retest.py
--rw-r--r--   0        0        0     1512 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/reveal.py
--rw-r--r--   0        0        0     1754 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/revisit.py
--rw-r--r--   0        0        0     2229 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/ruleConfig.py
--rw-r--r--   0        0        0     8741 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/script.py
--rw-r--r--   0        0        0    10589 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/search.py
--rw-r--r--   0        0        0     8074 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/selenium.py
--rw-r--r--   0        0        0     2358 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/sessionManagement.py
--rw-r--r--   0        0        0     1493 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/soap.py
--rw-r--r--   0        0        0    26424 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/spider.py
--rw-r--r--   0        0        0     4617 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/stats.py
--rw-r--r--   0        0        0     7030 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/users.py
--rw-r--r--   0        0        0     1870 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/wappalyzer.py
--rw-r--r--   0        0        0     3906 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/websocket.py
--rw-r--r--   0        0        0     2226 1970-01-01 00:00:00.000000 zaproxy-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-20 14:20:20.751332 zaproxy-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1114 2024-05-20 14:20:20.751332 zaproxy-0.3.1/README.md
+-rw-r--r--   0        0        0     1467 2024-05-20 14:20:20.751332 zaproxy-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     7894 2024-05-20 14:20:20.751332 zaproxy-0.3.1/src/zapv2/__init__.py
+-rw-r--r--   0        0        0     3123 2024-05-20 14:20:20.751332 zaproxy-0.3.1/src/zapv2/accessControl.py
+-rw-r--r--   0        0        0     2610 2024-05-20 14:20:20.751332 zaproxy-0.3.1/src/zapv2/acsrf.py
+-rw-r--r--   0        0        0    16351 2024-05-20 14:20:20.751332 zaproxy-0.3.1/src/zapv2/ajaxSpider.py
+-rw-r--r--   0        0        0     7597 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/alert.py
+-rw-r--r--   0        0        0     9098 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/alertFilter.py
+-rw-r--r--   0        0        0    28082 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/ascan.py
+-rw-r--r--   0        0        0     3694 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/authentication.py
+-rw-r--r--   0        0        0     2266 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/authorization.py
+-rw-r--r--   0        0        0     1669 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/automation.py
+-rw-r--r--   0        0        0     8349 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/autoupdate.py
+-rw-r--r--   0        0        0     4479 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/brk.py
+-rw-r--r--   0        0        0     7885 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/context.py
+-rw-r--r--   0        0        0    30289 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/core.py
+-rw-r--r--   0        0        0     4430 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/custompayloads.py
+-rw-r--r--   0        0        0     4089 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/exim.py
+-rw-r--r--   0        0        0     2036 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/forcedUser.py
+-rw-r--r--   0        0        0     8201 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/graphql.py
+-rw-r--r--   0        0        0     5977 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/httpSessions.py
+-rw-r--r--   0        0        0     2127 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/localProxies.py
+-rw-r--r--   0        0        0    19754 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/network.py
+-rw-r--r--   0        0        0     1938 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/openapi.py
+-rw-r--r--   0        0        0     1195 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/params.py
+-rw-r--r--   0        0        0     2921 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/pnh.py
+-rw-r--r--   0        0        0     5392 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/pscan.py
+-rw-r--r--   0        0        0     3296 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/replacer.py
+-rw-r--r--   0        0        0     2988 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/reports.py
+-rw-r--r--   0        0        0     1132 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/retest.py
+-rw-r--r--   0        0        0     1512 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/reveal.py
+-rw-r--r--   0        0        0     1754 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/revisit.py
+-rw-r--r--   0        0        0     2229 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/ruleConfig.py
+-rw-r--r--   0        0        0     8741 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/script.py
+-rw-r--r--   0        0        0    10589 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/search.py
+-rw-r--r--   0        0        0     8074 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/selenium.py
+-rw-r--r--   0        0        0     2358 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/sessionManagement.py
+-rw-r--r--   0        0        0     1493 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/soap.py
+-rw-r--r--   0        0        0    26424 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/spider.py
+-rw-r--r--   0        0        0     4617 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/stats.py
+-rw-r--r--   0        0        0     7030 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/users.py
+-rw-r--r--   0        0        0     1870 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/wappalyzer.py
+-rw-r--r--   0        0        0     3906 2024-05-20 14:20:20.755332 zaproxy-0.3.1/src/zapv2/websocket.py
+-rw-r--r--   0        0        0     2226 1970-01-01 00:00:00.000000 zaproxy-0.3.1/PKG-INFO
```

### Comparing `zaproxy-0.3.0/LICENSE` & `zaproxy-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/README.md` & `zaproxy-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/pyproject.toml` & `zaproxy-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "zaproxy"
 # Ensure __version__ in src/zapv2/__init__.py matches.
-version = "0.3.0"
+version = "0.3.1"
 description = "ZAP API Client"
 readme = "README.md"
 authors = ["ZAP Development Team <zaproxy-develop@googlegroups.com>"]
 license = "Apache-2.0"
 
 homepage = "https://www.zaproxy.org/"
 repository = "https://github.com/zaproxy/zap-api-python.git"
```

### Comparing `zaproxy-0.3.0/src/zapv2/__init__.py` & `zaproxy-0.3.1/src/zapv2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 Client implementation for using the ZAP pentesting proxy remotely.
 """
 
 __docformat__ = 'restructuredtext'
-__version__ = '0.3.0'
+__version__ = '0.3.1'
 
 import requests
 from requests.packages.urllib3.exceptions import InsecureRequestWarning
 
 from .accessControl import accessControl
 from .acsrf import acsrf
 from .alert import alert
```

### Comparing `zaproxy-0.3.0/src/zapv2/accessControl.py` & `zaproxy-0.3.1/src/zapv2/accessControl.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/acsrf.py` & `zaproxy-0.3.1/src/zapv2/acsrf.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/ajaxSpider.py` & `zaproxy-0.3.1/src/zapv2/ajaxSpider.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/alert.py` & `zaproxy-0.3.1/src/zapv2/alert.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/alertFilter.py` & `zaproxy-0.3.1/src/zapv2/alertFilter.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/ascan.py` & `zaproxy-0.3.1/src/zapv2/ascan.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/authentication.py` & `zaproxy-0.3.1/src/zapv2/authentication.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/authorization.py` & `zaproxy-0.3.1/src/zapv2/authorization.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/automation.py` & `zaproxy-0.3.1/src/zapv2/automation.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     def __init__(self, zap):
         self.zap = zap
 
     def plan_progress(self, planid):
         """
         This component is optional and therefore the API will only work if it is installed
         """
-        return six.next(six.itervalues(self.zap._request(self.zap.base + 'automation/view/planProgress/', {'planId': planid})))
+        return (self.zap._request(self.zap.base + 'automation/view/planProgress/', {'planId': planid}))
 
     def run_plan(self, filepath, apikey=''):
         """
         This component is optional and therefore the API will only work if it is installed
         """
         return six.next(six.itervalues(self.zap._request(self.zap.base + 'automation/action/runPlan/', {'filePath': filepath})))
```

### Comparing `zaproxy-0.3.0/src/zapv2/autoupdate.py` & `zaproxy-0.3.1/src/zapv2/autoupdate.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/brk.py` & `zaproxy-0.3.1/src/zapv2/brk.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/context.py` & `zaproxy-0.3.1/src/zapv2/context.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/core.py` & `zaproxy-0.3.1/src/zapv2/core.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/custompayloads.py` & `zaproxy-0.3.1/src/zapv2/custompayloads.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/exim.py` & `zaproxy-0.3.1/src/zapv2/exim.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/forcedUser.py` & `zaproxy-0.3.1/src/zapv2/forcedUser.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/graphql.py` & `zaproxy-0.3.1/src/zapv2/graphql.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/httpSessions.py` & `zaproxy-0.3.1/src/zapv2/httpSessions.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/localProxies.py` & `zaproxy-0.3.1/src/zapv2/localProxies.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/network.py` & `zaproxy-0.3.1/src/zapv2/network.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/openapi.py` & `zaproxy-0.3.1/src/zapv2/openapi.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/params.py` & `zaproxy-0.3.1/src/zapv2/params.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/pnh.py` & `zaproxy-0.3.1/src/zapv2/pnh.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/pscan.py` & `zaproxy-0.3.1/src/zapv2/pscan.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/replacer.py` & `zaproxy-0.3.1/src/zapv2/replacer.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/reports.py` & `zaproxy-0.3.1/src/zapv2/reports.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/retest.py` & `zaproxy-0.3.1/src/zapv2/retest.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/reveal.py` & `zaproxy-0.3.1/src/zapv2/reveal.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/revisit.py` & `zaproxy-0.3.1/src/zapv2/revisit.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/ruleConfig.py` & `zaproxy-0.3.1/src/zapv2/ruleConfig.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/script.py` & `zaproxy-0.3.1/src/zapv2/script.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/search.py` & `zaproxy-0.3.1/src/zapv2/search.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/selenium.py` & `zaproxy-0.3.1/src/zapv2/selenium.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/sessionManagement.py` & `zaproxy-0.3.1/src/zapv2/sessionManagement.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/soap.py` & `zaproxy-0.3.1/src/zapv2/soap.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/spider.py` & `zaproxy-0.3.1/src/zapv2/spider.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/stats.py` & `zaproxy-0.3.1/src/zapv2/stats.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/users.py` & `zaproxy-0.3.1/src/zapv2/users.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/wappalyzer.py` & `zaproxy-0.3.1/src/zapv2/wappalyzer.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/src/zapv2/websocket.py` & `zaproxy-0.3.1/src/zapv2/websocket.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.3.0/PKG-INFO` & `zaproxy-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zaproxy
-Version: 0.3.0
+Version: 0.3.1
 Summary: ZAP API Client
 Home-page: https://www.zaproxy.org/
 License: Apache-2.0
 Author: ZAP Development Team
 Author-email: zaproxy-develop@googlegroups.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

