# Comparing `tmp/r3dir-0.1.1.tar.gz` & `tmp/r3dir-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r3dir-0.1.1.tar", last modified: Thu Dec 21 17:44:11 2023, max compression
+gzip compressed data, was "r3dir-0.2.1.tar", last modified: Mon May 20 15:43:32 2024, max compression
```

## Comparing `r3dir-0.1.1.tar` & `r3dir-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 vladyslav   (501) staff       (20)        0 2023-12-21 17:44:11.968290 r3dir-0.1.1/
--rw-r--r--   0 vladyslav   (501) staff       (20)    11357 2023-02-22 16:24:18.000000 r3dir-0.1.1/LICENSE
--rw-r--r--   0 vladyslav   (501) staff       (20)     4127 2023-12-21 17:44:11.968122 r3dir-0.1.1/PKG-INFO
--rw-r--r--   0 vladyslav   (501) staff       (20)     3617 2023-04-11 16:46:52.000000 r3dir-0.1.1/PYPIREADME.md
--rw-r--r--   0 vladyslav   (501) staff       (20)     8734 2023-12-21 17:31:38.000000 r3dir-0.1.1/README.md
--rw-r--r--   0 vladyslav   (501) staff       (20)      683 2023-12-21 17:43:53.000000 r3dir-0.1.1/pyproject.toml
-drwxr-xr-x   0 vladyslav   (501) staff       (20)        0 2023-12-21 17:44:11.966674 r3dir-0.1.1/r3dir/
--rw-r--r--   0 vladyslav   (501) staff       (20)        0 2023-02-22 16:24:18.000000 r3dir-0.1.1/r3dir/__init__.py
--rw-r--r--   0 vladyslav   (501) staff       (20)     7107 2023-04-10 15:55:28.000000 r3dir-0.1.1/r3dir/encoder.py
--rw-r--r--   0 vladyslav   (501) staff       (20)      484 2023-04-05 17:33:07.000000 r3dir-0.1.1/r3dir/exceptions.py
-drwxr-xr-x   0 vladyslav   (501) staff       (20)        0 2023-12-21 17:44:11.967938 r3dir-0.1.1/r3dir.egg-info/
--rw-r--r--   0 vladyslav   (501) staff       (20)     4127 2023-12-21 17:44:11.000000 r3dir-0.1.1/r3dir.egg-info/PKG-INFO
--rw-r--r--   0 vladyslav   (501) staff       (20)      299 2023-12-21 17:44:11.000000 r3dir-0.1.1/r3dir.egg-info/SOURCES.txt
--rw-r--r--   0 vladyslav   (501) staff       (20)        1 2023-12-21 17:44:11.000000 r3dir-0.1.1/r3dir.egg-info/dependency_links.txt
--rw-r--r--   0 vladyslav   (501) staff       (20)       45 2023-12-21 17:44:11.000000 r3dir-0.1.1/r3dir.egg-info/entry_points.txt
--rw-r--r--   0 vladyslav   (501) staff       (20)       13 2023-12-21 17:44:11.000000 r3dir-0.1.1/r3dir.egg-info/requires.txt
--rw-r--r--   0 vladyslav   (501) staff       (20)        6 2023-12-21 17:44:11.000000 r3dir-0.1.1/r3dir.egg-info/top_level.txt
--rw-r--r--   0 vladyslav   (501) staff       (20)       38 2023-12-21 17:44:11.968327 r3dir-0.1.1/setup.cfg
-drwxr-xr-x   0 vladyslav   (501) staff       (20)        0 2023-12-21 17:44:11.967610 r3dir-0.1.1/tests/
--rw-r--r--   0 vladyslav   (501) staff       (20)     9266 2023-04-05 16:32:59.000000 r3dir-0.1.1/tests/test_encoder.py
+drwxr-xr-x   0 vladyslav   (501) staff       (20)        0 2024-05-20 15:43:32.237931 r3dir-0.2.1/
+-rw-r--r--   0 vladyslav   (501) staff       (20)    11357 2023-02-22 16:24:18.000000 r3dir-0.2.1/LICENSE
+-rw-r--r--   0 vladyslav   (501) staff       (20)     4608 2024-05-20 15:43:32.237748 r3dir-0.2.1/PKG-INFO
+-rw-r--r--   0 vladyslav   (501) staff       (20)     4073 2024-05-20 15:31:46.000000 r3dir-0.2.1/PYPIREADME.md
+-rw-r--r--   0 vladyslav   (501) staff       (20)     8758 2024-05-20 15:23:08.000000 r3dir-0.2.1/README.md
+-rw-r--r--   0 vladyslav   (501) staff       (20)      763 2024-05-20 15:43:17.000000 r3dir-0.2.1/pyproject.toml
+drwxr-xr-x   0 vladyslav   (501) staff       (20)        0 2024-05-20 15:43:32.235190 r3dir-0.2.1/r3dir/
+-rw-r--r--   0 vladyslav   (501) staff       (20)        0 2023-02-22 16:24:18.000000 r3dir-0.2.1/r3dir/__init__.py
+-rw-r--r--   0 vladyslav   (501) staff       (20)     4840 2024-05-20 15:30:32.000000 r3dir-0.2.1/r3dir/_cli.py
+-rw-r--r--   0 vladyslav   (501) staff       (20)     5016 2024-05-14 16:39:37.000000 r3dir-0.2.1/r3dir/encoder.py
+-rw-r--r--   0 vladyslav   (501) staff       (20)      484 2023-04-05 17:33:07.000000 r3dir-0.2.1/r3dir/exceptions.py
+drwxr-xr-x   0 vladyslav   (501) staff       (20)        0 2024-05-20 15:43:32.236113 r3dir-0.2.1/r3dir/hackvertor/
+-rw-r--r--   0 vladyslav   (501) staff       (20)    57159 2024-05-20 12:52:49.000000 r3dir-0.2.1/r3dir/hackvertor/encoder.js
+drwxr-xr-x   0 vladyslav   (501) staff       (20)        0 2024-05-20 15:43:32.237530 r3dir-0.2.1/r3dir.egg-info/
+-rw-r--r--   0 vladyslav   (501) staff       (20)     4608 2024-05-20 15:43:32.000000 r3dir-0.2.1/r3dir.egg-info/PKG-INFO
+-rw-r--r--   0 vladyslav   (501) staff       (20)      341 2024-05-20 15:43:32.000000 r3dir-0.2.1/r3dir.egg-info/SOURCES.txt
+-rw-r--r--   0 vladyslav   (501) staff       (20)        1 2024-05-20 15:43:32.000000 r3dir-0.2.1/r3dir.egg-info/dependency_links.txt
+-rw-r--r--   0 vladyslav   (501) staff       (20)       42 2024-05-20 15:43:32.000000 r3dir-0.2.1/r3dir.egg-info/entry_points.txt
+-rw-r--r--   0 vladyslav   (501) staff       (20)       23 2024-05-20 15:43:32.000000 r3dir-0.2.1/r3dir.egg-info/requires.txt
+-rw-r--r--   0 vladyslav   (501) staff       (20)        6 2024-05-20 15:43:32.000000 r3dir-0.2.1/r3dir.egg-info/top_level.txt
+-rw-r--r--   0 vladyslav   (501) staff       (20)       38 2024-05-20 15:43:32.237973 r3dir-0.2.1/setup.cfg
+drwxr-xr-x   0 vladyslav   (501) staff       (20)        0 2024-05-20 15:43:32.236255 r3dir-0.2.1/tests/
+-rw-r--r--   0 vladyslav   (501) staff       (20)     9098 2024-05-14 09:22:39.000000 r3dir-0.2.1/tests/test_encoder.py
```

### Comparing `r3dir-0.1.1/LICENSE` & `r3dir-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `r3dir-0.1.1/PKG-INFO` & `r3dir-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,66 +1,89 @@
 Metadata-Version: 2.1
 Name: r3dir
-Version: 0.1.1
+Version: 0.2.1
 Summary: r3dir encoder/decoder package with CLI tool
 Author: Horlad
 Project-URL: Homepage, https://github.com/Horlad/r3dir
 Project-URL: Bug Tracker, https://github.com/Horlad/r3dir/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: unishox2-py3
+Requires-Dist: pyperclip
 
 # r3dir 
 CLI tool for `r3dir` target-dynamic redirection service which helps bypass weak SSRF filters without redirection location validation.
 
 Read details how `r3dir` works at [Github README page](https://github.com/Horlad/r3dir).
 
 ## CLI tool
 
 ### Installation
 ```bash
-pip3 install r3dir
+pipx install r3dir
 ```
 
 ### Encode mode 
 ```bash
 $ r3dir encode -h
-  usage: r3dir encode [-h] [-c STATUS_CODE] [-d MAIN_DOMAIN] [-i IGNORE_PART | -s] [--slient_mode] target_url
+  usage: r3dir encode [-h] [-c STATUS_CODE] [-i IGNORE_PART | -s] [--slient_mode] target_url
 
-positional arguments:
-  target_url            Target URL which r3dir tool should redirect to.
+  positional arguments:
+    target_url            Target URL which r3dir tool should redirect to
 
-options:
-  -h, --help            show this help message and exit
-  -c STATUS_CODE, --status_code STATUS_CODE
-                        HTTP status code of a redirect response.
-  -d MAIN_DOMAIN, --main_domain MAIN_DOMAIN
-                        Domain where r3dir tool is hosted on.
-  -i IGNORE_PART, --ignore_part IGNORE_PART
-                        String, which will be ignored during decoding. Used to bypass weak REGEXs.
-  -s, --https           HTTPS enforced encoding(TLS certificate length limitation)
-  --slient_mode         Slient mode for automations(e.g Hackvertor tags)
+  options:
+    -h, --help            show this help message and exit
+    -c STATUS_CODE, --status_code STATUS_CODE
+                          HTTP status code of a redirect response (default: 302)
+    -i IGNORE_PART, --ignore_part IGNORE_PART
+                          String, which will be ignored during decoding. Used to bypass weak REGEXs
+    -s, --https           HTTPS enforced encoding(TLS certificate length limitation)
+    --slient_mode         Slient mode for automations (e.g Hackvertor tags)
 ```
 
 ### Decode mode 
 ```bash
 $ r3dir decode -h
-  usage: r3dir decode [-h] [-d MAIN_DOMAIN] encoded_url
-  
+  usage: r3dir decode [-h] encoded_domain
+
   positional arguments:
-    encoded_url           r3dir encoded URL to decode
+    encoded_domain  r3dir encoded domain to decode
 
   options:
-    -h, --help            show this help message and exit
-    -d MAIN_DOMAIN, --main_domain MAIN_DOMAIN
-                          Domain where r3dir tool is hosted on.
+    -h, --help      show this help message and exit
+```
+
+### Hackvertor mode
+```bash
+$ r3dir hackvertor -h
+  usage: r3dir hackvertor [-h] [--print]
+
+  options:
+    -h, --help  show this help message and exit
+    --print     Output Hackvertor tags into terminal
+```
+
+To use CLI tool with own server, set your domain with `-d` option:
+```bash
+$ r3dir -h
+usage: r3dir [-h] [-d MAIN_DOMAIN] {encode,decode,hackvertor} ...
+
+Encoded/decoder CLI tool for r3dir service
+
+options:
+  -h, --help            show this help message and exit
+  -d MAIN_DOMAIN, --main_domain MAIN_DOMAIN
+                        Domain where r3dir tool is hosted on (default: r3dir.me)
+
+# Example of --main_domain option
+$ r3dir -d your.host encode http://localhost
 ```
 
 ## Python package 
 
 You also can use `r3dir.encoder` module to build your own scripts or tools. It contains `encode()` and `decode()` functions which parameters corresponds to CLI options.
 
 Custom errors which encoder or decoder may raise, you can find in `r3dir.exceptions`.
```

### Comparing `r3dir-0.1.1/PYPIREADME.md` & `r3dir-0.2.1/PYPIREADME.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,49 +3,71 @@
 
 Read details how `r3dir` works at [Github README page](https://github.com/Horlad/r3dir).
 
 ## CLI tool
 
 ### Installation
 ```bash
-pip3 install r3dir
+pipx install r3dir
 ```
 
 ### Encode mode 
 ```bash
 $ r3dir encode -h
-  usage: r3dir encode [-h] [-c STATUS_CODE] [-d MAIN_DOMAIN] [-i IGNORE_PART | -s] [--slient_mode] target_url
+  usage: r3dir encode [-h] [-c STATUS_CODE] [-i IGNORE_PART | -s] [--slient_mode] target_url
 
-positional arguments:
-  target_url            Target URL which r3dir tool should redirect to.
+  positional arguments:
+    target_url            Target URL which r3dir tool should redirect to
 
-options:
-  -h, --help            show this help message and exit
-  -c STATUS_CODE, --status_code STATUS_CODE
-                        HTTP status code of a redirect response.
-  -d MAIN_DOMAIN, --main_domain MAIN_DOMAIN
-                        Domain where r3dir tool is hosted on.
-  -i IGNORE_PART, --ignore_part IGNORE_PART
-                        String, which will be ignored during decoding. Used to bypass weak REGEXs.
-  -s, --https           HTTPS enforced encoding(TLS certificate length limitation)
-  --slient_mode         Slient mode for automations(e.g Hackvertor tags)
+  options:
+    -h, --help            show this help message and exit
+    -c STATUS_CODE, --status_code STATUS_CODE
+                          HTTP status code of a redirect response (default: 302)
+    -i IGNORE_PART, --ignore_part IGNORE_PART
+                          String, which will be ignored during decoding. Used to bypass weak REGEXs
+    -s, --https           HTTPS enforced encoding(TLS certificate length limitation)
+    --slient_mode         Slient mode for automations (e.g Hackvertor tags)
 ```
 
 ### Decode mode 
 ```bash
 $ r3dir decode -h
-  usage: r3dir decode [-h] [-d MAIN_DOMAIN] encoded_url
-  
+  usage: r3dir decode [-h] encoded_domain
+
   positional arguments:
-    encoded_url           r3dir encoded URL to decode
+    encoded_domain  r3dir encoded domain to decode
 
   options:
-    -h, --help            show this help message and exit
-    -d MAIN_DOMAIN, --main_domain MAIN_DOMAIN
-                          Domain where r3dir tool is hosted on.
+    -h, --help      show this help message and exit
+```
+
+### Hackvertor mode
+```bash
+$ r3dir hackvertor -h
+  usage: r3dir hackvertor [-h] [--print]
+
+  options:
+    -h, --help  show this help message and exit
+    --print     Output Hackvertor tags into terminal
+```
+
+To use CLI tool with own server, set your domain with `-d` option:
+```bash
+$ r3dir -h
+usage: r3dir [-h] [-d MAIN_DOMAIN] {encode,decode,hackvertor} ...
+
+Encoded/decoder CLI tool for r3dir service
+
+options:
+  -h, --help            show this help message and exit
+  -d MAIN_DOMAIN, --main_domain MAIN_DOMAIN
+                        Domain where r3dir tool is hosted on (default: r3dir.me)
+
+# Example of --main_domain option
+$ r3dir -d your.host encode http://localhost
 ```
 
 ## Python package 
 
 You also can use `r3dir.encoder` module to build your own scripts or tools. It contains `encode()` and `decode()` functions which parameters corresponds to CLI options.
 
 Custom errors which encoder or decoder may raise, you can find in `r3dir.exceptions`.
```

### Comparing `r3dir-0.1.1/README.md` & `r3dir-0.2.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # r3dir 
 ![Version](https://img.shields.io/pypi/v/r3dir) ![PyPI pyversions](https://img.shields.io/pypi/pyversions/r3dir)  ![LICENSE](https://img.shields.io/pypi/l/r3dir)
 
 Redirection service designed to help bypass SSRF filters that do not validate the redirect location. It allows you to:
 
-- Define the redirection target via URL parameters or subdomains;
+- Set the redirection target via URL parameters or subdomains;
 - Control HTTP response codes;
 - Obfuscate the target URL with Base32 encoding;
-- Bypass certain allowlist filters.
+- Bypass some allowlist filters.
 
 Details about features of HTTP redirects in SSRF cases and how to utilize them via `r3dir` tool you can find in my article.
 
-The service is currently run at the `r3dir.me` and supports both HTTP and HTTPS.
+The service is currently run at the `r3dir.me` domain and supports both HTTP and HTTPS.
 
 ## Usage
-r3dir provides two approaches to set redirection targets: parameter-based and domain-based.
+`r3dir` provides two approaches to set redirection targets: parameter-based and domain-based.
 
 ### Setting HTTP status code
 Both approaches let you control HTTP status code of a response via first subdomain of `r3dir.me` URL.
 
 ```bash
 302.r3dir.me -> 302 Found
 307.r3dir.me -> 307 Temporary Redirect
@@ -32,24 +32,24 @@
 ```bash
 #Redirects to http://localhost with `307 Temporary Redirect` status code
 https://307.r3dir.me/--to/?url=http://localhost 
 ```
 
 ### Domain-based redirection
 
-Basically, you can control only host part of URL to successfully perform SSRF via HTTP redirection. While existing tools require manual configuration of redirection targets in such case, `r3dir` provides an ability to dynamically define a target via subdomains. 
+Basically, you can control only host part of URL to successfully perform SSRF via HTTP redirection. While existing tools require manual configuration of redirection targets in such case, `r3dir` provides an ability to dynamically set a target via subdomains. 
 
 ![r3dir_decoding_flow_upd](https://user-images.githubusercontent.com/62111809/231235695-54ad0d45-ed57-42a3-a3cd-a38538ca8215.png)
 
 As you can see, subdomains contain splited Base32-encoded compressed target which r3dir use to create redirect. 
 
 To create encoded domain, use CLI tool or embed it in BurpSuite as Hackvertor tag(see details below).
 
 ### Length limit
-Maximum domain length is 253 characters. Unishox2 compression (around 30-40% for common SSRF payloads) compensates Base32 encoding. Thus r3dir provides 1-to-1 ratio for encoded targets in average and you can use r3dir with targets up to 230 characters (considering length of other parts of domain).
+Maximum domain length is 253 characters. Unishox2 compression (around 30-40% for common SSRF payloads) compensates Base32 encoding. Thus r3dir provides 1-to-1 ratio for encoded targets on average and you can use r3dir with targets up to 230 characters (considering length of other parts of domain).
 
 ### HTTPS limitations
 
 Due to [limitations of wildcard TLS cerficates](https://en.wikipedia.org/wiki/Wildcard_certificate#Limitations) which do not work with multipule wildcard domains(like `*.*.301.r3dir.me`) HTTPS domain-based redirection works with targets that are not longer that 63 symbols(maximum length of one subdomain) in encoded form. In addition, `--ignore_part` feature also is not available due to the limit. 
 
 ```bash
 #Redirects to http://169.254.169.254/latest/meta-data with `302 Found` status code
@@ -82,88 +82,90 @@
 
 Also, there is [PyPi package](https://pypi.org/project/r3dir) which can be used as library for your own Python scripts and tools. Details and examples how to use you can find on PyPi page.
 
 ## CLI tool
 
 ### Installation
 ```bash
-pip3 install r3dir
+pipx install r3dir
 ```
 
 ### Encode mode 
 ```bash
 $ r3dir encode -h
-  usage: r3dir encode [-h] [-c STATUS_CODE] [-d MAIN_DOMAIN] [-a] [-i IGNORE_PART | -s] target_url
-  
+  usage: r3dir encode [-h] [-c STATUS_CODE] [-i IGNORE_PART | -s] [--slient_mode] target_url
+
   positional arguments:
-    target_url            Target URL which r3dir tool should redirect to.
-  
+    target_url            Target URL which r3dir tool should redirect to
+
   options:
     -h, --help            show this help message and exit
     -c STATUS_CODE, --status_code STATUS_CODE
-                          HTTP status code of a redirect response.
-    -d MAIN_DOMAIN, --main_domain MAIN_DOMAIN
-                          Domain where r3dir tool is hosted on.
+                          HTTP status code of a redirect response (default: 302)
     -i IGNORE_PART, --ignore_part IGNORE_PART
-                          String, which will be ignored during decoding. Used to bypass weak REGEXs.
+                          String, which will be ignored during decoding. Used to bypass weak REGEXs
     -s, --https           HTTPS enforced encoding(TLS certificate length limitation)
-    --slient_mode         Slient mode for automations(e.g Hackvertor tags)
+    --slient_mode         Slient mode for automations (e.g Hackvertor tags)
 ```
 
 ### Decode mode 
 ```bash
 $ r3dir decode -h
-  usage: r3dir decode [-h] [-d MAIN_DOMAIN] encoded_url
-  
+  usage: r3dir decode [-h] encoded_domain
+
   positional arguments:
-    encoded_url           r3dir encoded URL to decode
+    encoded_domain  r3dir encoded domain to decode
 
   options:
-    -h, --help            show this help message and exit
-    -d MAIN_DOMAIN, --main_domain MAIN_DOMAIN
-                          Domain where r3dir tool is hosted on.
+    -h, --help      show this help message and exit
+```
+
+To use CLI tool with own server, set your domain with `-d` option:
+```bash
+$ r3dir -h
+usage: r3dir [-h] [-d MAIN_DOMAIN] {encode,decode,hackvertor} ...
+
+Encoded/decoder CLI tool for r3dir service
+
+options:
+  -h, --help            show this help message and exit
+  -d MAIN_DOMAIN, --main_domain MAIN_DOMAIN
+                        Domain where r3dir tool is hosted on (default: r3dir.me)
+
+# Example of --main_domain option
+$ r3dir -d your.host encode http://localhost
 ```
 
 ## Hackvertor tag
 
 For seamless web application fuzzing, r3dir has a custom Hackvertor tag for BurpSuite. If you haven't seen Hackvertor extension in BurpSuite before, [check it](https://portswigger.net/bappstore/65033cbd2c344fbabe57ac060b5dd100).
 
 To install r3dir Hackvertor tag in BurpSuite, follow next steps:
 
 1. Install CLI tool
 ```bash
 pip3 install r3dir
 ```
 
-2. Run `type r3dir` to get command path (or `where r3dir` for Windows)
-- Unix:
+2. Run `r3dir hackvertor` to copy Hackvertor tags into clipboard:
+- If you have set up own server, use `-d` option to set a custom `main_domain` for Hackvertor tags.
 ```bash
-# Example output: r3dir is /opt/homebrew/bin/r3dir
-type r3dir
+r3dir -d your.host hackvertor
 ```
-- Windows:
-```powershell
-where r3dir
-```
-3. Replace `/PATH/TO/R3DIR` placeholder in `hackvertor_tag.json` with obtained path.
-- Unix:
+- If CLI tool does not copy tags in your clipboard, you can use `--print` opiton to output into terminal and copy it manually
 ```bash
-sed -i 's|/PATH/TO/R3DIR|/YOUR/PATH/TO/R3DIR|g' hackvertor_tag.json
-```
-- Windows:
-```powershell
-(Get-Content hackvertor_tag.json) | ForEach-Object { $_ -replace "/PATH/TO/R3DIR", "/YOUR/PATH/TO/R3DIR" } | Set-Content hackvertor_tag.json
+r3dir hackvertor --print
 ```
-4. Add the tag to Hackvertor extension:
-- Copy content of `hackvertor_tag.json`. 
+
+3. Add the tag to Hackvertor extension:
 - Open Hackvertor menu in BurpSuite sidebar and ensure that ***Allow code execution tags*** is enabled. Go to ***List custom tags***.
 ![Screenshot 2023-04-10 at 17 35 51](https://user-images.githubusercontent.com/62111809/231236253-012f7357-08ae-4336-959e-6616694184ac.png)
 - Then press ***Load tags from clipboard***. 
 
-If you have your own custom tags, export them via ***Export all my tags to clipboard***, add r3dir tag to the exported JSON document and then reimport them.
+If you have your own custom tags, export them via ***Export all my tags to clipboard***, add r3dir tags to the exported JSON document and then reimport them.
 
 ## HTTP server self-hosting
 
 To spin up own instance, follow next steps:
 
 1. Download the repository
 ```bash
```

### Comparing `r3dir-0.1.1/r3dir/encoder.py` & `r3dir-0.2.1/r3dir/encoder.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import math, base64, binascii, argparse
+import math, base64, binascii
 import unishox2
 import hashlib
+
 from .exceptions import Base32DecodingError, StatusCodeNotInRangeError, WrongEncodedURLFormat, TooLongTarget
 
 MAX_DOMAIN_LENGTH = 253
 MAX_SUBDOMAIN_LENGTH = 63
 IGNORE_PART_SEP = "--"
 MAX_COMPRESSION_TARGET_SIZE = 1024 # we assume that compression rate can't go futher than 85% on usefull links(1024*0.15*8/5=245,76)
 
@@ -57,20 +58,20 @@
     subdomains = ".".join(_b32encode_dns(target))
     
     encoded_domain = f"{subdomains}.{status_code}.{main_domain}"
 
     #check whether encoded domain length corresponds to limitations of DNS and TLS certificates
     try:
         if https_enforced:
-            if len(subdomains) > MAX_SUBDOMAIN_LENGTH:
+            if ignore_part or len(subdomains) > MAX_SUBDOMAIN_LENGTH:
                 raise TooLongTarget(f"The target length is longer than maximum allowed for HTTPS mode. Remove ignoring part, or short the target.")
         elif ignore_part:
             encoded_domain = f"{ignore_part}.{IGNORE_PART_SEP}.{encoded_domain}"
 
-        if len(encoded_domain) > 253:
+        if len(encoded_domain) > MAX_DOMAIN_LENGTH:
             raise TooLongTarget(f"The target length is longer than maximum allowed. Remove ignoring part or short the target.")
     except TooLongTarget:
         if not slient_mode:
             raise
         target_hash = hashlib.sha1(target.encode("UTF-8")).hexdigest()
         error_domain = f"too-long-target-{target_hash}.{status_code}.{main_domain}"
         return error_domain
@@ -106,46 +107,7 @@
     try:
         target = _b32decode_dns(encoded_subdomains[:-1])
     except (UnicodeDecodeError, binascii.Error) as e:
         raise Base32DecodingError("Base32-encoded target decoding error")
     
     return target, status_code
 
-
-def _cli():
-    argParser = argparse.ArgumentParser(description='Encoded/decoder CLI tool for r3dir service')
-    subparsers = argParser.add_subparsers(dest='mode', required=True, description="Encoding/decoding mode")
-
-    encoder = subparsers.add_parser('encode', help="r3dir CLI encoder")
-
-    https_opts = encoder.add_mutually_exclusive_group()
-
-    encoder.add_argument('target_url', type = str,
-                            help = "Target URL which r3dir tool should redirect to.")
-    encoder.add_argument('-c', '--status_code', type = int,
-                            default = 302,
-                            help = f"HTTP status code of a redirect response.")
-    encoder.add_argument('-d', '--main_domain', type = str,
-                            default = "r3dir.me",
-                            help = f"Domain where r3dir tool is hosted on.")                    
-    https_opts.add_argument('-i', '--ignore_part', type = str,
-                            default = None,
-                            help = f"String, which will be ignored during decoding. Used to bypass weak REGEXs.")
-    https_opts.add_argument("-s", "--https", help="HTTPS enforced encoding(TLS certificate length limitation)",
-                            action="store_true")
-    encoder.add_argument("--slient_mode", help="Slient mode for automations(e.g Hackvertor tags)",
-                            action="store_true")
-
-    decoder = subparsers.add_parser('decode', help="r3dir CLI decoder")        
-
-    decoder.add_argument('encoded_domain', type = str,
-                            help = "r3dir encoded domain to decode")
-    decoder.add_argument('-d', '--main_domain', type = str,
-                            default = "r3dir.me",
-                            help = f"Domain where r3dir tool is hosted on.")
-
-    args = argParser.parse_args()
-
-    if args.mode == 'encode':
-        print(encode(args.target_url, args.status_code, args.main_domain, args.ignore_part, https_enforced = args.https, slient_mode=args.slient_mode))
-    elif args.mode == 'decode':
-        print(decode(args.encoded_domain, args.main_domain))
```

### Comparing `r3dir-0.1.1/r3dir.egg-info/PKG-INFO` & `r3dir-0.2.1/r3dir.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,66 +1,89 @@
 Metadata-Version: 2.1
 Name: r3dir
-Version: 0.1.1
+Version: 0.2.1
 Summary: r3dir encoder/decoder package with CLI tool
 Author: Horlad
 Project-URL: Homepage, https://github.com/Horlad/r3dir
 Project-URL: Bug Tracker, https://github.com/Horlad/r3dir/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: unishox2-py3
+Requires-Dist: pyperclip
 
 # r3dir 
 CLI tool for `r3dir` target-dynamic redirection service which helps bypass weak SSRF filters without redirection location validation.
 
 Read details how `r3dir` works at [Github README page](https://github.com/Horlad/r3dir).
 
 ## CLI tool
 
 ### Installation
 ```bash
-pip3 install r3dir
+pipx install r3dir
 ```
 
 ### Encode mode 
 ```bash
 $ r3dir encode -h
-  usage: r3dir encode [-h] [-c STATUS_CODE] [-d MAIN_DOMAIN] [-i IGNORE_PART | -s] [--slient_mode] target_url
+  usage: r3dir encode [-h] [-c STATUS_CODE] [-i IGNORE_PART | -s] [--slient_mode] target_url
 
-positional arguments:
-  target_url            Target URL which r3dir tool should redirect to.
+  positional arguments:
+    target_url            Target URL which r3dir tool should redirect to
 
-options:
-  -h, --help            show this help message and exit
-  -c STATUS_CODE, --status_code STATUS_CODE
-                        HTTP status code of a redirect response.
-  -d MAIN_DOMAIN, --main_domain MAIN_DOMAIN
-                        Domain where r3dir tool is hosted on.
-  -i IGNORE_PART, --ignore_part IGNORE_PART
-                        String, which will be ignored during decoding. Used to bypass weak REGEXs.
-  -s, --https           HTTPS enforced encoding(TLS certificate length limitation)
-  --slient_mode         Slient mode for automations(e.g Hackvertor tags)
+  options:
+    -h, --help            show this help message and exit
+    -c STATUS_CODE, --status_code STATUS_CODE
+                          HTTP status code of a redirect response (default: 302)
+    -i IGNORE_PART, --ignore_part IGNORE_PART
+                          String, which will be ignored during decoding. Used to bypass weak REGEXs
+    -s, --https           HTTPS enforced encoding(TLS certificate length limitation)
+    --slient_mode         Slient mode for automations (e.g Hackvertor tags)
 ```
 
 ### Decode mode 
 ```bash
 $ r3dir decode -h
-  usage: r3dir decode [-h] [-d MAIN_DOMAIN] encoded_url
-  
+  usage: r3dir decode [-h] encoded_domain
+
   positional arguments:
-    encoded_url           r3dir encoded URL to decode
+    encoded_domain  r3dir encoded domain to decode
 
   options:
-    -h, --help            show this help message and exit
-    -d MAIN_DOMAIN, --main_domain MAIN_DOMAIN
-                          Domain where r3dir tool is hosted on.
+    -h, --help      show this help message and exit
+```
+
+### Hackvertor mode
+```bash
+$ r3dir hackvertor -h
+  usage: r3dir hackvertor [-h] [--print]
+
+  options:
+    -h, --help  show this help message and exit
+    --print     Output Hackvertor tags into terminal
+```
+
+To use CLI tool with own server, set your domain with `-d` option:
+```bash
+$ r3dir -h
+usage: r3dir [-h] [-d MAIN_DOMAIN] {encode,decode,hackvertor} ...
+
+Encoded/decoder CLI tool for r3dir service
+
+options:
+  -h, --help            show this help message and exit
+  -d MAIN_DOMAIN, --main_domain MAIN_DOMAIN
+                        Domain where r3dir tool is hosted on (default: r3dir.me)
+
+# Example of --main_domain option
+$ r3dir -d your.host encode http://localhost
 ```
 
 ## Python package 
 
 You also can use `r3dir.encoder` module to build your own scripts or tools. It contains `encode()` and `decode()` functions which parameters corresponds to CLI options.
 
 Custom errors which encoder or decoder may raise, you can find in `r3dir.exceptions`.
```

### Comparing `r3dir-0.1.1/tests/test_encoder.py` & `r3dir-0.2.1/tests/test_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,16 @@
     assert target == decoded_target
     assert status_code == decoded_code
 
 def test_normal_target_with_ignore_part_and_https():
     main_domain = "r3dir.me"
     ignore_part = "testingtest"
     target, status_code = "http://169.254.169.254", 301
-    encoded_domain = encoder.encode(target, status_code=status_code, main_domain=main_domain, ignore_part=ignore_part, https_enforced=True)
-    decoded_target, decoded_code = encoder.decode(encoded_domain, main_domain=main_domain)
-    assert ignore_part not in encoded_domain
-    assert target == decoded_target
-    assert status_code == decoded_code
+    with pytest.raises(TooLongTarget):
+        encoded_domain = encoder.encode(target, status_code=status_code, main_domain=main_domain, ignore_part=ignore_part, https_enforced=True)
 
 def test_normal_empty_encoded_target():
     main_domain = "r3dir.me"
     encoded_domain = "302.r3dir.me"
     decoded_target, decoded_code = encoder.decode(encoded_domain, main_domain=main_domain)
     assert decoded_code == 302
     assert decoded_target == ""
```

