# Comparing `tmp/identity-0.7.0.tar.gz` & `tmp/identity-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "identity-0.7.0.tar", last modified: Sat Mar 30 01:38:46 2024, max compression
+gzip compressed data, was "identity-0.8.0.tar", last modified: Mon May 20 06:00:10 2024, max compression
```

## Comparing `identity-0.7.0.tar` & `identity-0.8.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 01:38:46.959323 identity-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-30 01:38:43.000000 identity-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-03-30 01:38:46.959323 identity-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-03-30 01:38:43.000000 identity-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 01:38:46.955323 identity-0.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-03-30 01:38:43.000000 identity-0.7.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 01:38:46.955323 identity-0.7.0/identity/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-30 01:38:43.000000 identity-0.7.0/identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8013 2024-03-30 01:38:43.000000 identity-0.7.0/identity/django.py
--rw-r--r--   0 runner    (1001) docker     (127)     6487 2024-03-30 01:38:43.000000 identity-0.7.0/identity/flask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 01:38:46.955323 identity-0.7.0/identity/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 01:38:46.959323 identity-0.7.0/identity/templates/identity/
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-30 01:38:43.000000 identity-0.7.0/identity/templates/identity/auth_error.html
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-03-30 01:38:43.000000 identity-0.7.0/identity/templates/identity/login.html
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-30 01:38:43.000000 identity-0.7.0/identity/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    23033 2024-03-30 01:38:43.000000 identity-0.7.0/identity/web.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 01:38:46.959323 identity-0.7.0/identity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-03-30 01:38:46.000000 identity-0.7.0/identity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-30 01:38:46.000000 identity-0.7.0/identity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 01:38:46.000000 identity-0.7.0/identity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-30 01:38:46.000000 identity-0.7.0/identity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-30 01:38:46.000000 identity-0.7.0/identity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-30 01:38:43.000000 identity-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-03-30 01:38:46.959323 identity-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-30 01:38:43.000000 identity-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 01:38:46.959323 identity-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-03-30 01:38:43.000000 identity-0.7.0/tests/test_django.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-30 01:38:43.000000 identity-0.7.0/tests/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:00:10.009603 identity-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-20 06:00:05.000000 identity-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-05-20 06:00:10.009603 identity-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-20 06:00:05.000000 identity-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:00:10.005603 identity-0.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-05-20 06:00:05.000000 identity-0.8.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:00:10.005603 identity-0.8.0/identity/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-20 06:00:05.000000 identity-0.8.0/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7960 2024-05-20 06:00:05.000000 identity-0.8.0/identity/django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-20 06:00:05.000000 identity-0.8.0/identity/flask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-20 06:00:05.000000 identity-0.8.0/identity/quart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:00:10.001603 identity-0.8.0/identity/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:00:10.005603 identity-0.8.0/identity/templates/identity/
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-20 06:00:05.000000 identity-0.8.0/identity/templates/identity/auth_error.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-20 06:00:05.000000 identity-0.8.0/identity/templates/identity/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-20 06:00:05.000000 identity-0.8.0/identity/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23033 2024-05-20 06:00:05.000000 identity-0.8.0/identity/web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:00:10.005603 identity-0.8.0/identity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-05-20 06:00:09.000000 identity-0.8.0/identity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-20 06:00:10.000000 identity-0.8.0/identity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 06:00:09.000000 identity-0.8.0/identity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-20 06:00:09.000000 identity-0.8.0/identity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-20 06:00:09.000000 identity-0.8.0/identity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-20 06:00:05.000000 identity-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-20 06:00:10.009603 identity-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-20 06:00:05.000000 identity-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:00:10.005603 identity-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-20 06:00:05.000000 identity-0.8.0/tests/test_django.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-20 06:00:05.000000 identity-0.8.0/tests/test_quart.py
```

### Comparing `identity-0.7.0/LICENSE` & `identity-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `identity-0.7.0/PKG-INFO` & `identity-0.8.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: identity
-Version: 0.7.0
+Version: 0.8.0
 Summary: This is an authentication/authorization library, currently optimized for web apps. It provides some higher level APIs built on top of Microsoft's MSAL Python.
 Home-page: https://github.com/rayluo/identity
 Author: Ray Luo
 Author-email: rayluo.mba@gmail.com
 License: MIT
 Project-URL: Changelog, https://github.com/rayluo/identity/releases
 Project-URL: Documentation, https://identity-library.readthedocs.io/
@@ -21,16 +21,28 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: msal<2,>=1.28
 Requires-Dist: requests<3,>=2.0.0
+Provides-Extra: all-for-docs
+Requires-Dist: django<6,>=3.2; extra == "all-for-docs"
+Requires-Dist: flask; extra == "all-for-docs"
+Requires-Dist: Flask-Session<0.6,>=0.3.2; extra == "all-for-docs"
+Requires-Dist: quart; extra == "all-for-docs"
+Requires-Dist: Quart-Session; extra == "all-for-docs"
+Provides-Extra: django
+Requires-Dist: django<6,>=3.2; extra == "django"
 Provides-Extra: flask
+Requires-Dist: flask; extra == "flask"
 Requires-Dist: Flask-Session<0.6,>=0.3.2; extra == "flask"
+Provides-Extra: quart
+Requires-Dist: quart; extra == "quart"
+Requires-Dist: Quart-Session; extra == "quart"
 
 # Identity library
 
 <!-- The following summary is reused in, and needs to be in-sync with, the docs/index.rst -->
 This Identity library is an authentication/authorization library that:
 
 * Suitable for apps that are targeting end users on
@@ -89,21 +101,34 @@
     <th>Web App Sign In & Sign Out</th>
     <td colspan=4>
 
 By using this library, it will automatically renew signed-in session when the ID token expires.
 
 * [Sample written in ![Django](https://raw.githubusercontent.com/rayluo/identity/dev/docs/django.webp)](https://github.com/Azure-Samples/ms-identity-python-webapp-django)
 * [Sample written in ![Flask](https://raw.githubusercontent.com/rayluo/identity/dev/docs/flask.webp)](https://github.com/Azure-Samples/ms-identity-python-webapp)
+* [Sample written in ![Quart](https://raw.githubusercontent.com/rayluo/identity/dev/docs/quart.webp)](https://github.com/rayluo/python-webapp-quart)
 * Need support for more web frameworks?
   [Upvote existing feature request or create a new one](https://github.com/rayluo/identity/issues)
 
 </td>
   </tr>
 
   <tr>
+    <th>How to customize the login page</th>
+    <td colspan=4>
+
+The default login page will typically redirect users to your Identity Provider,
+so you don't have to customize it.
+But if the default login page is shown in your browser,
+you can read its HTML source code, and find the how-to instructions there.
+
+</td>
+  </tr>
+
+  <tr>
     <th>Web App Calls a web API</th>
     <td colspan=4>
 
 This library supports:
 
 + Incremental consent. If the user needs to consent to more permissions,
   the library will automatically redirect the user to the consent page.
@@ -144,15 +169,19 @@
 
 </table>
 
 
 ## Installation
 
 This package is [available on PyPI](https://pypi.org/project/identity/).
-You can install it by `pip install identity`.
+Choose the package declaration that matches your web framework:
+
+* Django: `pip install identity[django]`
+* Flask: `pip install identity[flask]`
+* Quart: `pip install identity[quart]`
 
 ## Versions
 
 This library follows [Semantic Versioning](http://semver.org/).
 Your project should declare `identity` dependency with proper lower and upper bound.
 
 You can find the changes for each version under
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: identity Version: 0.7.0 Summary: This is an
+Metadata-Version: 2.1 Name: identity Version: 0.8.0 Summary: This is an
 authentication/authorization library, currently optimized for web apps. It
 provides some higher level APIs built on top of Microsoft's MSAL Python. Home-
 page: https://github.com/rayluo/identity Author: Ray Luo Author-email:
 rayluo.mba@gmail.com License: MIT Project-URL: Changelog, https://github.com/
 rayluo/identity/releases Project-URL: Documentation, https://identity-
 library.readthedocs.io/ Keywords: identity,auth,authentication,authorization
 Classifier: Development Status :: 4 - Beta Classifier: License :: OSI Approved
@@ -10,32 +10,39 @@
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: msal<2,>=1.28 Requires-Dist: requests<3,>=2.0.0
-Provides-Extra: flask Requires-Dist: Flask-Session<0.6,>=0.3.2; extra ==
-"flask" # Identity library This Identity library is an authentication/
-authorization library that: * Suitable for apps that are targeting end users on
-[Microsoft identity platform, a.k.a. Microsoft Entra ID](https://
-learn.microsoft.com/en-us/azure/active-directory/develop/v2-overview) (which
-includes Work or school accounts provisioned through Azure AD, and Personal
-Microsoft accounts such as Skype, Xbox, Outlook.com). * Currently designed for
-web apps, regardless of which Python web framework you are using. * Provides a
-set of high level API that is built on top of, and easier to be used than
-[Microsoft's MSAL Python library](https://github.com/AzureAD/microsoft-
-authentication-library-for-python). * Written in Python, for Python apps. >
-DISCLAIMER: The code in this repo is not officially supported by Microsoft and
-is not intended for production use. > The intention of this repo is to unblock
-customers who would like to use a higher level API, > before such an API has
-been migrated to an Microsoft library with official support. Migration of this
-API to official support is not guaranteed and is not currently on the MSAL
-roadmap. > Please ensure to fully test any code used from this repository to
-ensure it works in your environment. ## Scenarios supported
+Provides-Extra: all-for-docs Requires-Dist: django<6,>=3.2; extra == "all-for-
+docs" Requires-Dist: flask; extra == "all-for-docs" Requires-Dist: Flask-
+Session<0.6,>=0.3.2; extra == "all-for-docs" Requires-Dist: quart; extra ==
+"all-for-docs" Requires-Dist: Quart-Session; extra == "all-for-docs" Provides-
+Extra: django Requires-Dist: django<6,>=3.2; extra == "django" Provides-Extra:
+flask Requires-Dist: flask; extra == "flask" Requires-Dist: Flask-
+Session<0.6,>=0.3.2; extra == "flask" Provides-Extra: quart Requires-Dist:
+quart; extra == "quart" Requires-Dist: Quart-Session; extra == "quart" #
+Identity library This Identity library is an authentication/authorization
+library that: * Suitable for apps that are targeting end users on [Microsoft
+identity platform, a.k.a. Microsoft Entra ID](https://learn.microsoft.com/en-
+us/azure/active-directory/develop/v2-overview) (which includes Work or school
+accounts provisioned through Azure AD, and Personal Microsoft accounts such as
+Skype, Xbox, Outlook.com). * Currently designed for web apps, regardless of
+which Python web framework you are using. * Provides a set of high level API
+that is built on top of, and easier to be used than [Microsoft's MSAL Python
+library](https://github.com/AzureAD/microsoft-authentication-library-for-
+python). * Written in Python, for Python apps. > DISCLAIMER: The code in this
+repo is not officially supported by Microsoft and is not intended for
+production use. > The intention of this repo is to unblock customers who would
+like to use a higher level API, > before such an API has been migrated to an
+Microsoft library with official support. Migration of this API to official
+support is not guaranteed and is not currently on the MSAL roadmap. > Please
+ensure to fully test any code used from this repository to ensure it works in
+your environment. ## Scenarios supported
  _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
 |            |                    |                    |MMiiccrroossoofftt|                    |
 |            |                    |                    |EEnnttrraa    |                    |
 |            |MMiiccrroossoofftt EEnnttrraa IIDD  |MMiiccrroossoofftt EEnnttrraa     |EExxtteerrnnaall |AAzzuurree AADD BB22CC        |
 |            |                    |EExxtteerrnnaall IIDD         |IIDD wwiitthh  |                    |
 |            |                    |                    |CCuussttoomm   |                    |
 |_ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_DD_oo_mm_aa_ii_nn_ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
@@ -54,20 +61,26 @@
 |            |web-app-python-sign-|tenant)             |         |configure-          |
 |            |in?tabs=windows)    |                    |         |authentication-     |
 |            |                    |                    |         |sample-python-web-  |
 |_ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_a_p_p_?_t_a_b_s_=_l_i_n_u_x_)_ _ _ _ _ |
 |            |By using this library, it will automatically renew signed-in session    |
 |            |when the ID token expires. * [Sample written in ![Django](https://      |
 |            |raw.githubusercontent.com/rayluo/identity/dev/docs/django.webp)](https:/|
-|WWeebb AApppp SSiiggnn|/github.com/Azure-Samples/ms-identity-python-webapp-django) * [Sample   |
-|IInn && SSiiggnn   |written in ![Flask](https://raw.githubusercontent.com/rayluo/identity/  |
-|OOuutt         |dev/docs/flask.webp)](https://github.com/Azure-Samples/ms-identity-     |
-|            |python-webapp) * Need support for more web frameworks? [Upvote existing |
-|            |feature request or create a new one](https://github.com/rayluo/identity/|
-|_ _ _ _ _ _ _ _ _ _ _ _ _|_i_s_s_u_e_s_)_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
+|            |/github.com/Azure-Samples/ms-identity-python-webapp-django) * [Sample   |
+|WWeebb AApppp SSiiggnn|written in ![Flask](https://raw.githubusercontent.com/rayluo/identity/  |
+|IInn && SSiiggnn   |dev/docs/flask.webp)](https://github.com/Azure-Samples/ms-identity-     |
+|OOuutt         |python-webapp) * [Sample written in ![Quart](https://                   |
+|            |raw.githubusercontent.com/rayluo/identity/dev/docs/quart.webp)](https://|
+|            |github.com/rayluo/python-webapp-quart) * Need support for more web      |
+|            |frameworks? [Upvote existing feature request or create a new one](https:|
+|_ _ _ _ _ _ _ _ _ _ _ _ _|_/_/_g_i_t_h_u_b_._c_o_m_/_r_a_y_l_u_o_/_i_d_e_n_t_i_t_y_/_i_s_s_u_e_s_)_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
+|HHooww ttoo      |The default login page will typically redirect users to your Identity   |
+|ccuussttoommiizzee   |Provider, so you don't have to customize it. But if the default login   |
+|tthhee llooggiinn   |page is shown in your browser, you can read its HTML source code, and   |
+|_pp_aa_gg_ee_ _ _ _ _ _ _ _ _|_f_i_n_d_ _t_h_e_ _h_o_w_-_t_o_ _i_n_s_t_r_u_c_t_i_o_n_s_ _t_h_e_r_e_._ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 |WWeebb AApppp     |This library supports: + Incremental consent. If the user needs to      |
 |CCaallllss aa wweebb |consent to more permissions, the library will automatically redirect the|
 |AAPPII         |user to the consent page. + Automatically cache the access token and    |
 |_ _ _ _ _ _ _ _ _ _ _ _ _|_r_e_n_e_w_ _i_t_ _w_h_e_n_ _n_e_e_d_e_d_ _T_h_e_y_ _a_r_e_ _d_e_m_o_n_s_t_r_a_t_e_d_ _b_y_ _t_h_e_ _s_a_m_e_ _s_a_m_p_l_e_s_ _a_b_o_v_e_._ _ _ |
 |WWeebb AAPPII     |                                                                        |
 |CCaallllss       |                                                                        |
 |aannootthheerr wweebb |In roadmap.                                                             |
@@ -76,12 +89,13 @@
 |HHooww ttoo bbuuiilldd|                                                                        |
 |tthhee ssaammpplleess |Read our [docs here](https://identity-library.readthedocs.io/en/latest/)|
 |aabboovvee ffrroomm  |                                                                        |
 |_ss_cc_rr_aa_tt_cc_hh_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 |OOtthheerr       |[Upvote existing feature request or create a new one](https://          |
 |_ss_cc_ee_nn_aa_rr_ii_oo_ss_ _ _ _|_g_i_t_h_u_b_._c_o_m_/_r_a_y_l_u_o_/_i_d_e_n_t_i_t_y_/_i_s_s_u_e_s_)_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 ## Installation This package is [available on PyPI](https://pypi.org/project/
-identity/). You can install it by `pip install identity`. ## Versions This
-library follows [Semantic Versioning](http://semver.org/). Your project should
-declare `identity` dependency with proper lower and upper bound. You can find
-the changes for each version under [Releases](https://github.com/rayluo/
-identity/releases).
+identity/). Choose the package declaration that matches your web framework: *
+Django: `pip install identity[django]` * Flask: `pip install identity[flask]` *
+Quart: `pip install identity[quart]` ## Versions This library follows [Semantic
+Versioning](http://semver.org/). Your project should declare `identity`
+dependency with proper lower and upper bound. You can find the changes for each
+version under [Releases](https://github.com/rayluo/identity/releases).
```

### Comparing `identity-0.7.0/README.md` & `identity-0.8.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -59,21 +59,34 @@
     <th>Web App Sign In & Sign Out</th>
     <td colspan=4>
 
 By using this library, it will automatically renew signed-in session when the ID token expires.
 
 * [Sample written in ![Django](https://raw.githubusercontent.com/rayluo/identity/dev/docs/django.webp)](https://github.com/Azure-Samples/ms-identity-python-webapp-django)
 * [Sample written in ![Flask](https://raw.githubusercontent.com/rayluo/identity/dev/docs/flask.webp)](https://github.com/Azure-Samples/ms-identity-python-webapp)
+* [Sample written in ![Quart](https://raw.githubusercontent.com/rayluo/identity/dev/docs/quart.webp)](https://github.com/rayluo/python-webapp-quart)
 * Need support for more web frameworks?
   [Upvote existing feature request or create a new one](https://github.com/rayluo/identity/issues)
 
 </td>
   </tr>
 
   <tr>
+    <th>How to customize the login page</th>
+    <td colspan=4>
+
+The default login page will typically redirect users to your Identity Provider,
+so you don't have to customize it.
+But if the default login page is shown in your browser,
+you can read its HTML source code, and find the how-to instructions there.
+
+</td>
+  </tr>
+
+  <tr>
     <th>Web App Calls a web API</th>
     <td colspan=4>
 
 This library supports:
 
 + Incremental consent. If the user needs to consent to more permissions,
   the library will automatically redirect the user to the consent page.
@@ -114,15 +127,19 @@
 
 </table>
 
 
 ## Installation
 
 This package is [available on PyPI](https://pypi.org/project/identity/).
-You can install it by `pip install identity`.
+Choose the package declaration that matches your web framework:
+
+* Django: `pip install identity[django]`
+* Flask: `pip install identity[flask]`
+* Quart: `pip install identity[quart]`
 
 ## Versions
 
 This library follows [Semantic Versioning](http://semver.org/).
 Your project should declare `identity` dependency with proper lower and upper bound.
 
 You can find the changes for each version under
```

#### html2text {}

```diff
@@ -37,20 +37,26 @@
 |            |web-app-python-sign-|tenant)             |         |configure-          |
 |            |in?tabs=windows)    |                    |         |authentication-     |
 |            |                    |                    |         |sample-python-web-  |
 |_ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_a_p_p_?_t_a_b_s_=_l_i_n_u_x_)_ _ _ _ _ |
 |            |By using this library, it will automatically renew signed-in session    |
 |            |when the ID token expires. * [Sample written in ![Django](https://      |
 |            |raw.githubusercontent.com/rayluo/identity/dev/docs/django.webp)](https:/|
-|WWeebb AApppp SSiiggnn|/github.com/Azure-Samples/ms-identity-python-webapp-django) * [Sample   |
-|IInn && SSiiggnn   |written in ![Flask](https://raw.githubusercontent.com/rayluo/identity/  |
-|OOuutt         |dev/docs/flask.webp)](https://github.com/Azure-Samples/ms-identity-     |
-|            |python-webapp) * Need support for more web frameworks? [Upvote existing |
-|            |feature request or create a new one](https://github.com/rayluo/identity/|
-|_ _ _ _ _ _ _ _ _ _ _ _ _|_i_s_s_u_e_s_)_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
+|            |/github.com/Azure-Samples/ms-identity-python-webapp-django) * [Sample   |
+|WWeebb AApppp SSiiggnn|written in ![Flask](https://raw.githubusercontent.com/rayluo/identity/  |
+|IInn && SSiiggnn   |dev/docs/flask.webp)](https://github.com/Azure-Samples/ms-identity-     |
+|OOuutt         |python-webapp) * [Sample written in ![Quart](https://                   |
+|            |raw.githubusercontent.com/rayluo/identity/dev/docs/quart.webp)](https://|
+|            |github.com/rayluo/python-webapp-quart) * Need support for more web      |
+|            |frameworks? [Upvote existing feature request or create a new one](https:|
+|_ _ _ _ _ _ _ _ _ _ _ _ _|_/_/_g_i_t_h_u_b_._c_o_m_/_r_a_y_l_u_o_/_i_d_e_n_t_i_t_y_/_i_s_s_u_e_s_)_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
+|HHooww ttoo      |The default login page will typically redirect users to your Identity   |
+|ccuussttoommiizzee   |Provider, so you don't have to customize it. But if the default login   |
+|tthhee llooggiinn   |page is shown in your browser, you can read its HTML source code, and   |
+|_pp_aa_gg_ee_ _ _ _ _ _ _ _ _|_f_i_n_d_ _t_h_e_ _h_o_w_-_t_o_ _i_n_s_t_r_u_c_t_i_o_n_s_ _t_h_e_r_e_._ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 |WWeebb AApppp     |This library supports: + Incremental consent. If the user needs to      |
 |CCaallllss aa wweebb |consent to more permissions, the library will automatically redirect the|
 |AAPPII         |user to the consent page. + Automatically cache the access token and    |
 |_ _ _ _ _ _ _ _ _ _ _ _ _|_r_e_n_e_w_ _i_t_ _w_h_e_n_ _n_e_e_d_e_d_ _T_h_e_y_ _a_r_e_ _d_e_m_o_n_s_t_r_a_t_e_d_ _b_y_ _t_h_e_ _s_a_m_e_ _s_a_m_p_l_e_s_ _a_b_o_v_e_._ _ _ |
 |WWeebb AAPPII     |                                                                        |
 |CCaallllss       |                                                                        |
 |aannootthheerr wweebb |In roadmap.                                                             |
@@ -59,12 +65,13 @@
 |HHooww ttoo bbuuiilldd|                                                                        |
 |tthhee ssaammpplleess |Read our [docs here](https://identity-library.readthedocs.io/en/latest/)|
 |aabboovvee ffrroomm  |                                                                        |
 |_ss_cc_rr_aa_tt_cc_hh_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 |OOtthheerr       |[Upvote existing feature request or create a new one](https://          |
 |_ss_cc_ee_nn_aa_rr_ii_oo_ss_ _ _ _|_g_i_t_h_u_b_._c_o_m_/_r_a_y_l_u_o_/_i_d_e_n_t_i_t_y_/_i_s_s_u_e_s_)_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 ## Installation This package is [available on PyPI](https://pypi.org/project/
-identity/). You can install it by `pip install identity`. ## Versions This
-library follows [Semantic Versioning](http://semver.org/). Your project should
-declare `identity` dependency with proper lower and upper bound. You can find
-the changes for each version under [Releases](https://github.com/rayluo/
-identity/releases).
+identity/). Choose the package declaration that matches your web framework: *
+Django: `pip install identity[django]` * Flask: `pip install identity[flask]` *
+Quart: `pip install identity[quart]` ## Versions This library follows [Semantic
+Versioning](http://semver.org/). Your project should declare `identity`
+dependency with proper lower and upper bound. You can find the changes for each
+version under [Releases](https://github.com/rayluo/identity/releases).
```

### Comparing `identity-0.7.0/docs/conf.py` & `identity-0.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `identity-0.7.0/identity/django.py` & `identity-0.8.0/identity/django.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 
                 @settings.AUTH.login_required(scopes=["scope1", "scope2"])
                 def my_view2(request, *, context):
                     api_result = requests.get(  # Use access token to call an api
                         "https://example.com/endpoint",
                         headers={'Authorization': 'Bearer ' + context['access_token']},
                         timeout=30,
-                    ).json()  # Here we assume the response format is json
+                    )
                     ...
         """
         # With or without brackets. Inspired by https://stackoverflow.com/a/39335652/728675
 
         # Called with brackets, i.e. @login_required()
         if function is None:
             logger.debug(f"Called as @login_required(..., scopes={scopes})")
```

### Comparing `identity-0.7.0/identity/flask.py` & `identity-0.8.0/identity/flask.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,14 @@
             self._endpoint_prefix,
             __name__,  # It decides blueprint resource folder
             template_folder='templates',
         )
         # Manually register the routes, since we cannot use @app or @bp on methods
         if self._redirect_uri:
             redirect_path = urlparse(self._redirect_uri).path
-            #bp.route(redirect_path or "/auth_response")(self.auth_response)
             bp.route(redirect_path)(self.auth_response)
             bp.route(
                 f"{os.path.dirname(redirect_path)}/logout"  # Use it in template by url_for("identity.logout")
                 )(self.logout)
         else:  # For Device Code Flow, we don't have a redirect_uri
             bp.route("/auth_response")(self.auth_response)
             bp.route("/logout")(self.logout)
@@ -103,35 +102,38 @@
 
         A user not meeting the requirement(s) will be brought to the login page.
         For already logged-in user, the view will be called with a keyword argument
         named "context" which is a dict containing the user object.
 
         Usage::
 
-            @settings.AUTH.login_required
-            def my_view(request, *, context):
-                return render(request, 'index.html', dict(
+            @app.route("/")
+            @auth.login_required
+            def index(*, context):
+                return render_template(
+                    'index.html',
                     user=context["user"],  # User is guaranteed to be present
                         # because we decorated this view with @login_required
-                    ))
+                )
 
         :param list[str] scopes:
             A list of scopes that your app will need to use.
             When present, the context will also contain an "access_token",
             "token_type", and likely "expires_in" and "refresh_token".
 
             Usage::
 
-                @settings.AUTH.login_required(scopes=["scope1", "scope2"])
-                def my_view2(request, *, context):
+                @app.route("/call_api")
+                @auth.login_required(scopes=["scope1", "scope2"])
+                def call_an_api(*, context):
                     api_result = requests.get(  # Use access token to call an api
                         "https://example.com/endpoint",
                         headers={'Authorization': 'Bearer ' + context['access_token']},
                         timeout=30,
-                    ).json()  # Here we assume the response format is json
+                    )
                     ...
         """
         # With or without brackets. Inspired by https://stackoverflow.com/a/39335652/728675
 
         # Called with brackets, i.e. @login_required()
         if function is None:
             logger.debug(f"Called as @login_required(..., scopes={scopes})")
```

### Comparing `identity-0.7.0/identity/templates/identity/auth_error.html` & `identity-0.8.0/identity/templates/identity/auth_error.html`

 * *Files identical despite different names*

### Comparing `identity-0.7.0/identity/web.py` & `identity-0.8.0/identity/web.py`

 * *Files identical despite different names*

### Comparing `identity-0.7.0/identity.egg-info/PKG-INFO` & `identity-0.8.0/identity.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: identity
-Version: 0.7.0
+Version: 0.8.0
 Summary: This is an authentication/authorization library, currently optimized for web apps. It provides some higher level APIs built on top of Microsoft's MSAL Python.
 Home-page: https://github.com/rayluo/identity
 Author: Ray Luo
 Author-email: rayluo.mba@gmail.com
 License: MIT
 Project-URL: Changelog, https://github.com/rayluo/identity/releases
 Project-URL: Documentation, https://identity-library.readthedocs.io/
@@ -21,16 +21,28 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: msal<2,>=1.28
 Requires-Dist: requests<3,>=2.0.0
+Provides-Extra: all-for-docs
+Requires-Dist: django<6,>=3.2; extra == "all-for-docs"
+Requires-Dist: flask; extra == "all-for-docs"
+Requires-Dist: Flask-Session<0.6,>=0.3.2; extra == "all-for-docs"
+Requires-Dist: quart; extra == "all-for-docs"
+Requires-Dist: Quart-Session; extra == "all-for-docs"
+Provides-Extra: django
+Requires-Dist: django<6,>=3.2; extra == "django"
 Provides-Extra: flask
+Requires-Dist: flask; extra == "flask"
 Requires-Dist: Flask-Session<0.6,>=0.3.2; extra == "flask"
+Provides-Extra: quart
+Requires-Dist: quart; extra == "quart"
+Requires-Dist: Quart-Session; extra == "quart"
 
 # Identity library
 
 <!-- The following summary is reused in, and needs to be in-sync with, the docs/index.rst -->
 This Identity library is an authentication/authorization library that:
 
 * Suitable for apps that are targeting end users on
@@ -89,21 +101,34 @@
     <th>Web App Sign In & Sign Out</th>
     <td colspan=4>
 
 By using this library, it will automatically renew signed-in session when the ID token expires.
 
 * [Sample written in ![Django](https://raw.githubusercontent.com/rayluo/identity/dev/docs/django.webp)](https://github.com/Azure-Samples/ms-identity-python-webapp-django)
 * [Sample written in ![Flask](https://raw.githubusercontent.com/rayluo/identity/dev/docs/flask.webp)](https://github.com/Azure-Samples/ms-identity-python-webapp)
+* [Sample written in ![Quart](https://raw.githubusercontent.com/rayluo/identity/dev/docs/quart.webp)](https://github.com/rayluo/python-webapp-quart)
 * Need support for more web frameworks?
   [Upvote existing feature request or create a new one](https://github.com/rayluo/identity/issues)
 
 </td>
   </tr>
 
   <tr>
+    <th>How to customize the login page</th>
+    <td colspan=4>
+
+The default login page will typically redirect users to your Identity Provider,
+so you don't have to customize it.
+But if the default login page is shown in your browser,
+you can read its HTML source code, and find the how-to instructions there.
+
+</td>
+  </tr>
+
+  <tr>
     <th>Web App Calls a web API</th>
     <td colspan=4>
 
 This library supports:
 
 + Incremental consent. If the user needs to consent to more permissions,
   the library will automatically redirect the user to the consent page.
@@ -144,15 +169,19 @@
 
 </table>
 
 
 ## Installation
 
 This package is [available on PyPI](https://pypi.org/project/identity/).
-You can install it by `pip install identity`.
+Choose the package declaration that matches your web framework:
+
+* Django: `pip install identity[django]`
+* Flask: `pip install identity[flask]`
+* Quart: `pip install identity[quart]`
 
 ## Versions
 
 This library follows [Semantic Versioning](http://semver.org/).
 Your project should declare `identity` dependency with proper lower and upper bound.
 
 You can find the changes for each version under
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: identity Version: 0.7.0 Summary: This is an
+Metadata-Version: 2.1 Name: identity Version: 0.8.0 Summary: This is an
 authentication/authorization library, currently optimized for web apps. It
 provides some higher level APIs built on top of Microsoft's MSAL Python. Home-
 page: https://github.com/rayluo/identity Author: Ray Luo Author-email:
 rayluo.mba@gmail.com License: MIT Project-URL: Changelog, https://github.com/
 rayluo/identity/releases Project-URL: Documentation, https://identity-
 library.readthedocs.io/ Keywords: identity,auth,authentication,authorization
 Classifier: Development Status :: 4 - Beta Classifier: License :: OSI Approved
@@ -10,32 +10,39 @@
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: msal<2,>=1.28 Requires-Dist: requests<3,>=2.0.0
-Provides-Extra: flask Requires-Dist: Flask-Session<0.6,>=0.3.2; extra ==
-"flask" # Identity library This Identity library is an authentication/
-authorization library that: * Suitable for apps that are targeting end users on
-[Microsoft identity platform, a.k.a. Microsoft Entra ID](https://
-learn.microsoft.com/en-us/azure/active-directory/develop/v2-overview) (which
-includes Work or school accounts provisioned through Azure AD, and Personal
-Microsoft accounts such as Skype, Xbox, Outlook.com). * Currently designed for
-web apps, regardless of which Python web framework you are using. * Provides a
-set of high level API that is built on top of, and easier to be used than
-[Microsoft's MSAL Python library](https://github.com/AzureAD/microsoft-
-authentication-library-for-python). * Written in Python, for Python apps. >
-DISCLAIMER: The code in this repo is not officially supported by Microsoft and
-is not intended for production use. > The intention of this repo is to unblock
-customers who would like to use a higher level API, > before such an API has
-been migrated to an Microsoft library with official support. Migration of this
-API to official support is not guaranteed and is not currently on the MSAL
-roadmap. > Please ensure to fully test any code used from this repository to
-ensure it works in your environment. ## Scenarios supported
+Provides-Extra: all-for-docs Requires-Dist: django<6,>=3.2; extra == "all-for-
+docs" Requires-Dist: flask; extra == "all-for-docs" Requires-Dist: Flask-
+Session<0.6,>=0.3.2; extra == "all-for-docs" Requires-Dist: quart; extra ==
+"all-for-docs" Requires-Dist: Quart-Session; extra == "all-for-docs" Provides-
+Extra: django Requires-Dist: django<6,>=3.2; extra == "django" Provides-Extra:
+flask Requires-Dist: flask; extra == "flask" Requires-Dist: Flask-
+Session<0.6,>=0.3.2; extra == "flask" Provides-Extra: quart Requires-Dist:
+quart; extra == "quart" Requires-Dist: Quart-Session; extra == "quart" #
+Identity library This Identity library is an authentication/authorization
+library that: * Suitable for apps that are targeting end users on [Microsoft
+identity platform, a.k.a. Microsoft Entra ID](https://learn.microsoft.com/en-
+us/azure/active-directory/develop/v2-overview) (which includes Work or school
+accounts provisioned through Azure AD, and Personal Microsoft accounts such as
+Skype, Xbox, Outlook.com). * Currently designed for web apps, regardless of
+which Python web framework you are using. * Provides a set of high level API
+that is built on top of, and easier to be used than [Microsoft's MSAL Python
+library](https://github.com/AzureAD/microsoft-authentication-library-for-
+python). * Written in Python, for Python apps. > DISCLAIMER: The code in this
+repo is not officially supported by Microsoft and is not intended for
+production use. > The intention of this repo is to unblock customers who would
+like to use a higher level API, > before such an API has been migrated to an
+Microsoft library with official support. Migration of this API to official
+support is not guaranteed and is not currently on the MSAL roadmap. > Please
+ensure to fully test any code used from this repository to ensure it works in
+your environment. ## Scenarios supported
  _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
 |            |                    |                    |MMiiccrroossoofftt|                    |
 |            |                    |                    |EEnnttrraa    |                    |
 |            |MMiiccrroossoofftt EEnnttrraa IIDD  |MMiiccrroossoofftt EEnnttrraa     |EExxtteerrnnaall |AAzzuurree AADD BB22CC        |
 |            |                    |EExxtteerrnnaall IIDD         |IIDD wwiitthh  |                    |
 |            |                    |                    |CCuussttoomm   |                    |
 |_ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_DD_oo_mm_aa_ii_nn_ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
@@ -54,20 +61,26 @@
 |            |web-app-python-sign-|tenant)             |         |configure-          |
 |            |in?tabs=windows)    |                    |         |authentication-     |
 |            |                    |                    |         |sample-python-web-  |
 |_ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _|_a_p_p_?_t_a_b_s_=_l_i_n_u_x_)_ _ _ _ _ |
 |            |By using this library, it will automatically renew signed-in session    |
 |            |when the ID token expires. * [Sample written in ![Django](https://      |
 |            |raw.githubusercontent.com/rayluo/identity/dev/docs/django.webp)](https:/|
-|WWeebb AApppp SSiiggnn|/github.com/Azure-Samples/ms-identity-python-webapp-django) * [Sample   |
-|IInn && SSiiggnn   |written in ![Flask](https://raw.githubusercontent.com/rayluo/identity/  |
-|OOuutt         |dev/docs/flask.webp)](https://github.com/Azure-Samples/ms-identity-     |
-|            |python-webapp) * Need support for more web frameworks? [Upvote existing |
-|            |feature request or create a new one](https://github.com/rayluo/identity/|
-|_ _ _ _ _ _ _ _ _ _ _ _ _|_i_s_s_u_e_s_)_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
+|            |/github.com/Azure-Samples/ms-identity-python-webapp-django) * [Sample   |
+|WWeebb AApppp SSiiggnn|written in ![Flask](https://raw.githubusercontent.com/rayluo/identity/  |
+|IInn && SSiiggnn   |dev/docs/flask.webp)](https://github.com/Azure-Samples/ms-identity-     |
+|OOuutt         |python-webapp) * [Sample written in ![Quart](https://                   |
+|            |raw.githubusercontent.com/rayluo/identity/dev/docs/quart.webp)](https://|
+|            |github.com/rayluo/python-webapp-quart) * Need support for more web      |
+|            |frameworks? [Upvote existing feature request or create a new one](https:|
+|_ _ _ _ _ _ _ _ _ _ _ _ _|_/_/_g_i_t_h_u_b_._c_o_m_/_r_a_y_l_u_o_/_i_d_e_n_t_i_t_y_/_i_s_s_u_e_s_)_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
+|HHooww ttoo      |The default login page will typically redirect users to your Identity   |
+|ccuussttoommiizzee   |Provider, so you don't have to customize it. But if the default login   |
+|tthhee llooggiinn   |page is shown in your browser, you can read its HTML source code, and   |
+|_pp_aa_gg_ee_ _ _ _ _ _ _ _ _|_f_i_n_d_ _t_h_e_ _h_o_w_-_t_o_ _i_n_s_t_r_u_c_t_i_o_n_s_ _t_h_e_r_e_._ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 |WWeebb AApppp     |This library supports: + Incremental consent. If the user needs to      |
 |CCaallllss aa wweebb |consent to more permissions, the library will automatically redirect the|
 |AAPPII         |user to the consent page. + Automatically cache the access token and    |
 |_ _ _ _ _ _ _ _ _ _ _ _ _|_r_e_n_e_w_ _i_t_ _w_h_e_n_ _n_e_e_d_e_d_ _T_h_e_y_ _a_r_e_ _d_e_m_o_n_s_t_r_a_t_e_d_ _b_y_ _t_h_e_ _s_a_m_e_ _s_a_m_p_l_e_s_ _a_b_o_v_e_._ _ _ |
 |WWeebb AAPPII     |                                                                        |
 |CCaallllss       |                                                                        |
 |aannootthheerr wweebb |In roadmap.                                                             |
@@ -76,12 +89,13 @@
 |HHooww ttoo bbuuiilldd|                                                                        |
 |tthhee ssaammpplleess |Read our [docs here](https://identity-library.readthedocs.io/en/latest/)|
 |aabboovvee ffrroomm  |                                                                        |
 |_ss_cc_rr_aa_tt_cc_hh_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 |OOtthheerr       |[Upvote existing feature request or create a new one](https://          |
 |_ss_cc_ee_nn_aa_rr_ii_oo_ss_ _ _ _|_g_i_t_h_u_b_._c_o_m_/_r_a_y_l_u_o_/_i_d_e_n_t_i_t_y_/_i_s_s_u_e_s_)_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 ## Installation This package is [available on PyPI](https://pypi.org/project/
-identity/). You can install it by `pip install identity`. ## Versions This
-library follows [Semantic Versioning](http://semver.org/). Your project should
-declare `identity` dependency with proper lower and upper bound. You can find
-the changes for each version under [Releases](https://github.com/rayluo/
-identity/releases).
+identity/). Choose the package declaration that matches your web framework: *
+Django: `pip install identity[django]` * Flask: `pip install identity[flask]` *
+Quart: `pip install identity[quart]` ## Versions This library follows [Semantic
+Versioning](http://semver.org/). Your project should declare `identity`
+dependency with proper lower and upper bound. You can find the changes for each
+version under [Releases](https://github.com/rayluo/identity/releases).
```

### Comparing `identity-0.7.0/setup.cfg` & `identity-0.8.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -30,16 +30,26 @@
 install_requires = 
 	msal>=1.28,<2
 	requests>=2.0.0,<3
 packages = find_namespace:
 include_package_data = True
 
 [options.extras_require]
+all_for_docs = 
+	%(django)s
+	%(flask)s
+	%(quart)s
+django = 
+	django>=3.2,<6
 flask = 
+	flask
 	Flask-Session>=0.3.2,<0.6
+quart = 
+	quart
+	Quart-Session
 
 [options.entry_points]
 console_scripts = 
 gui_scripts = 
 
 [options.packages.find]
 exclude = tests
```

### Comparing `identity-0.7.0/tests/test_django.py` & `identity-0.8.0/tests/test_django.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from unittest import mock
-import pytest  # pytest requires at least one test case to run
+
+import pytest
 from identity.django import _parse_redirect_uri, Auth
 
 def test_parse_redirect_uri():
     with pytest.raises(ValueError):
         _parse_redirect_uri("https://example.com")
     with pytest.raises(ValueError):
         _parse_redirect_uri("https://example.com/")
```

