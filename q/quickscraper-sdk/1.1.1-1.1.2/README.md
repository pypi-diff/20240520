# Comparing `tmp/quickscraper_sdk-1.1.1-py3-none-any.whl.zip` & `tmp/quickscraper_sdk-1.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 7063 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat    11777 b- defN 24-Jan-02 04:21 quickscraper_sdk/__init__.py
--rw-rw-rw-  2.0 fat      272 b- defN 24-Jan-02 04:26 quickscraper_sdk/constant.py
--rw-rw-rw-  2.0 fat       70 b- defN 23-Mar-31 09:41 tests/__init__.py
--rw-rw-rw-  2.0 fat      192 b- defN 23-Mar-31 09:41 tests/constant.py
--rw-rw-rw-  2.0 fat     5250 b- defN 23-Mar-31 09:41 tests/test_cases.py
--rw-rw-rw-  2.0 fat     1092 b- defN 24-Jan-02 05:03 quickscraper_sdk-1.1.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4851 b- defN 24-Jan-02 05:03 quickscraper_sdk-1.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Jan-02 05:03 quickscraper_sdk-1.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       23 b- defN 24-Jan-02 05:03 quickscraper_sdk-1.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      822 b- defN 24-Jan-02 05:03 quickscraper_sdk-1.1.1.dist-info/RECORD
-10 files, 24441 bytes uncompressed, 5655 bytes compressed:  76.9%
+Zip file size: 7017 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx    11519 b- defN 24-May-20 06:48 quickscraper_sdk/__init__.py
+-rw-rw-r--  2.0 unx      262 b- defN 24-May-20 06:48 quickscraper_sdk/constant.py
+-rw-rw-r--  2.0 unx       65 b- defN 24-May-20 06:20 tests/__init__.py
+-rw-rw-r--  2.0 unx      185 b- defN 24-May-20 06:20 tests/constant.py
+-rw-rw-r--  2.0 unx     5138 b- defN 24-May-20 06:20 tests/test_cases.py
+-rw-rw-r--  2.0 unx     1071 b- defN 24-May-20 06:50 quickscraper_sdk-1.1.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     4709 b- defN 24-May-20 06:50 quickscraper_sdk-1.1.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-20 06:50 quickscraper_sdk-1.1.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       23 b- defN 24-May-20 06:50 quickscraper_sdk-1.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      822 b- defN 24-May-20 06:50 quickscraper_sdk-1.1.2.dist-info/RECORD
+10 files, 23886 bytes uncompressed, 5609 bytes compressed:  76.5%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: tests/constant.py
 Comment: 
 
 Filename: tests/test_cases.py
 Comment: 
 
-Filename: quickscraper_sdk-1.1.1.dist-info/LICENSE
+Filename: quickscraper_sdk-1.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: quickscraper_sdk-1.1.1.dist-info/METADATA
+Filename: quickscraper_sdk-1.1.2.dist-info/METADATA
 Comment: 
 
-Filename: quickscraper_sdk-1.1.1.dist-info/WHEEL
+Filename: quickscraper_sdk-1.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: quickscraper_sdk-1.1.1.dist-info/top_level.txt
+Filename: quickscraper_sdk-1.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: quickscraper_sdk-1.1.1.dist-info/RECORD
+Filename: quickscraper_sdk-1.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## quickscraper_sdk/__init__.py

```diff
@@ -1,240 +1,240 @@
-"""
-quickscraper-sdk
-~~~~~~
-The quickscraper-sdk package - handles proxy servers, browsers, and
-CAPTCHA so that you can get the HTML from any website with an easy API call!
-"""
-
-from .constant import BASE_URL, VERSION
-from urllib.parse import urlencode
-from base64 import b64decode
-import requests
-
-
-class QuickScraper:
-    def __init__(self, access_token: str):
-        self.access_token = access_token
-        self.parse_url = BASE_URL + 'parse'
-        self.account_url = BASE_URL + 'account'
-
-    def getHtml(self, url: str,
-                render: bool = None,
-                session_number: str = None,
-                country_code: str = None,
-                premium: bool = None,
-                keep_headers: bool = None,
-                headers: dict = {},
-                format: str = 'html',
-                device_type: str = None,
-                parserSubscriptionId: str = None,
-                webhookRequestId: str = None,
-                customSelectors:list = [],
-                keepSelection: bool = None,
-                formData: dict = {},
-                isKeepFormDataSelection: bool  = None,
-                isScroll: bool = None,
-                scrollTimeout : int = None,
-                isPabbly : bool = None,
-                isZapier : bool = None,
-                dynamicInputs :list = []
-                ):
-        
-        if(customSelectors!=[] or formData != {} or (dynamicInputs !=[] and parserSubscriptionId)):
-                request_data = self.__prepareRequestBodyOrUrl(
-                url= url, render = render, session_number=session_number,country_code = country_code,
-                premium = premium, keep_headers = keep_headers, format=format, device_type = device_type,
-                parserSubscriptionId = parserSubscriptionId, webhookRequestId = webhookRequestId, 
-                isScroll = isScroll, scrollTimeout = scrollTimeout, isPabbly = isPabbly, isZapier = isZapier, 
-                customSelectors = customSelectors, keepSelection = keepSelection, formData = formData,
-                isKeepFormDataSelection = isKeepFormDataSelection, dynamicInputs=dynamicInputs, requestType= 'POST')
-        
-        else:
-            request_url = self.__prepareRequestBodyOrUrl(
-            url=url, render=render, session_number=session_number,
-            country_code=country_code,
-            premium=premium, keep_headers=keep_headers, format=format,
-            device_type=device_type, parserSubscriptionId=parserSubscriptionId,
-            webhookRequestId=webhookRequestId, isScroll = isScroll, scrollTimeout = scrollTimeout, 
-            isPabbly = isPabbly, isZapier = isZapier, keepSelection = None, isKeepFormDataSelection= None, requestType= 'GET')
-        
-        custom_headers = headers
-        request_options = self.__prepareHeaders(custom_headers, keep_headers)
-                
-        try:
-            if(customSelectors != [] or formData !={} or (dynamicInputs != [] and parserSubscriptionId)):
-                response = requests.post(url= request_data["request_url"], json = request_data["request_body"], headers=request_options)
-            else:
-                response = requests.get(request_url, headers=request_options)
-            
-            if parserSubscriptionId is not None:
-                response._content = response.json()
-            else:
-                response._content = response.text
-
-        except ValueError:
-            pass
-        return response
-
-    def writeHtmlToFile(self, url: str, file_path: str, render: bool = None,
-                        session_number: str = None, country_code: str = None,
-                        premium: bool = None, keep_headers: bool = None,
-                        headers: dict = {}, format: str = None,
-                        device_type: str = None,
-                        parserSubscriptionId: str = None,
-                        webhookRequestId: str = None, dynamicInputs :list = []):
-        with open(file_path, 'w+') as file:
-            response = self.getHtml(
-                url, render, session_number, country_code, premium,
-                keep_headers, headers, format, device_type, parserSubscriptionId,
-                webhookRequestId, dynamicInputs=dynamicInputs)
-            if format == 'images' or format == 'docx':
-                try:
-                    response._content = b64decode(response.text)
-                except ValueError:
-                    pass
-            file.write(str(response._content))
-        return response
-
-    # def writeCSVFile(self, url: str, file_path: str, render: bool = None,
-    #                  session_number: str = None, country_code: str = None,
-    #                  premium: bool = None, keep_headers: bool = None,
-    #                  headers: dict = {}):
-    #     response = self.writeHtmlToFile(url, file_path, render,
-    #                                     session_number,
-    #                                     country_code, premium,
-    #                                     keep_headers, headers,
-    #                                     format='tables')
-    #     return response
-
-    # def getAllImagesInZip(self, url: str, file_path: str,
-    #                       render: bool = None,
-    #                       session_number: str = None,
-    #                       country_code: str = None,
-    #                       premium: bool = None, keep_headers: bool = None,
-    #                       headers: dict = {}):
-    #     response = self.writeHtmlToFile(url, file_path, render,
-    #                                     session_number, country_code,
-    #                                     premium, keep_headers,
-    #                                     headers, format='images')
-    #     return response
-
-    # def writeDOCXFile(self, url: str, file_path: str, render: bool = None,
-    #                   session_number: str = None, country_code: str = None,
-    #                   premium: bool = None, keep_headers: bool = None,
-    #                   headers: dict = {}):
-    #     response = self.writeHtmlToFile(url, file_path, render,
-    #                                     session_number, country_code,
-    #                                     premium, keep_headers, headers,
-    #                                     format='docx')
-    #     return response
-
-    # def post(self, url: str, render: bool = None,
-    #          session_number: str = None, country_code: str = None,
-    #          premium: bool = None, keep_headers: bool = None,
-    #          headers: dict = {}):
-    #     response = self.getHtml(
-    #         url, render, session_number, country_code,
-    #         premium, keep_headers, headers)
-    #     return response
-
-    # def put(self, url: str, render: bool = None,
-    #         session_number: str = None, country_code: str = None,
-    #         premium: bool = None, keep_headers: bool = None,
-    #         headers: dict = {}):
-    #     response = self.getHtml(
-    #         url, render, session_number, country_code,
-    #         premium, keep_headers, headers)
-    #     return response
-
-    def scrapyGet(self, url: str,
-                  render: bool = None,
-                  session_number: str = None,
-                  country_code: str = None,
-                  premium: bool = None,
-                  keep_headers: bool = None,
-                  format: str = 'html',
-                  device_type: str = None,
-                  parserSubscriptionId: str = None,
-                  webhookRequestId: str = None):
-        request_url = self.__prepareRequestBodyOrUrl(
-            url=url, render=render, session_number=session_number,
-            country_code=country_code,
-            premium=premium, keep_headers=keep_headers, format=format,
-            device_type=device_type, parserSubscriptionId=parserSubscriptionId,
-            webhookRequestId=webhookRequestId, requestType = 'GET')
-        return request_url
-
-    def account(self):
-        response = requests.get(self.account_url,
-                                params={'access_token':
-                                        self.access_token}).json()
-        if response.get('message'):
-            response = response.get('message')
-        return response
-
-
-    def __prepareHeaders(self, custom_headers={}, keep_headers=None):
-        headers = {
-            'Client': 'PYTHON_CLIENT_LIB',
-            'Client-Version': VERSION
-        }
-        merged_headers = headers.copy()
-        merged_headers.update(custom_headers)
-        if keep_headers is True:
-            return merged_headers
-        return headers
-
-    # This function is used for csv, json, excel
-    def getData(self, url: str, render: bool = None, session_number: str = None,
-                country_code: str = None,
-                premium: bool = None, keep_headers: bool = None,
-                headers: dict = {}, format: str = None,
-                device_type: str = None,
-                parserSubscriptionId: str = None, webhookRequestId: str = None, dynamicInputs :list = []):
-        try:
-            response = self.getHtml(url, render, session_number, country_code, premium,
-                                    keep_headers, headers, format, device_type,
-                                    parserSubscriptionId, webhookRequestId, dynamicInputs = dynamicInputs)
-        except ValueError:
-            pass
-        return response
-
-    def __prepareRequestBodyOrUrl(self, **kwargs):
-         url_options = {
-            'access_token': self.access_token,
-            'URL': kwargs['url'],
-            'render': 'true' if kwargs['render'] is True else None,
-            'session_number': kwargs['session_number'],
-            'country_code': kwargs['country_code'],
-            'premium': 'true' if kwargs['premium'] is True else None,
-            'keep_headers': 'true' if kwargs['keep_headers'] is True else None,
-            'format': kwargs['format'],
-            'device_type': kwargs['device_type'],
-            'isScroll' : 'true' if kwargs['isScroll'] is True else None,
-            'scrollTimeout' : kwargs['scrollTimeout'],
-            'isPabbly' : 'true' if kwargs['isPabbly'] is True else None,
-            'isZapier' : 'true' if kwargs['isZapier'] is True else None,
-            'keepSelection' : 'true' if kwargs['keepSelection'] is True else None,
-            'isKeepFormDataSelection' : 'true' if kwargs['isKeepFormDataSelection'] is True else None,
-        }
-         if kwargs.get('parserSubscriptionId') is not None:
-            url_options['parserSubscriptionRequestId'] = kwargs['parserSubscriptionId']  
-         if kwargs.get('webhookRequestId') is not None:
-            url_options['webhookRequestId'] = kwargs['webhookRequestId']
-         if kwargs.get('customSelectors') is not None:
-            url_options['customSelectors'] = kwargs['customSelectors']
-         if kwargs.get('formData') is not None:
-            url_options['formData'] = kwargs['formData']
-         if kwargs.get('dynamicInputs') is not None:
-            url_options['dynamicInputs'] = kwargs['dynamicInputs']
-
-         if(kwargs['requestType'] == 'GET'):
-            url_options_filtered = {
-                key: value for key, value in 
-                url_options.items() if value is not None
-            }
-            option_string = urlencode(url_options_filtered)
-            request_url = self.parse_url + '?' + option_string
-            return request_url
-         requestData = { 'request_body':url_options, 'request_url': self.parse_url}
-         return requestData
+"""
+quickscraper-sdk
+~~~~~~
+The quickscraper-sdk package - handles proxy servers, browsers, and
+CAPTCHA so that you can get the HTML from any website with an easy API call!
+"""
+
+from .constant import BASE_URL, VERSION
+from urllib.parse import urlencode
+from base64 import b64decode
+import requests
+
+
+class QuickScraper:
+    def __init__(self, access_token: str):
+        self.access_token = access_token
+        self.parse_url = BASE_URL + 'parse'
+        self.account_url = BASE_URL + 'account'
+
+    def getHtml(self, url: str,
+                render: bool = None,
+                session_number: str = None,
+                country_code: str = None,
+                premium: bool = None,
+                keep_headers: bool = None,
+                headers: dict = {},
+                format: str = 'html',
+                device_type: str = None,
+                parserSubscriptionId: str = None,
+                webhookRequestId: str = None,
+                customSelectors:list = [],
+                keepSelection: bool = None,
+                formData: dict = {},
+                isKeepFormDataSelection: bool  = None,
+                isScroll: bool = None,
+                scrollTimeout : int = None,
+                isPabbly : bool = None,
+                isZapier : bool = None,
+                dynamicInputs :list = []
+                ):
+        
+        if(customSelectors!=[] or formData != {} or (dynamicInputs !=[] and parserSubscriptionId)):
+                request_data = self.__prepareRequestBodyOrUrl(
+                url= url, render = render, session_number=session_number,country_code = country_code,
+                premium = premium, keep_headers = keep_headers, format=format, device_type = device_type,
+                parserSubscriptionId = parserSubscriptionId, webhookRequestId = webhookRequestId, 
+                isScroll = isScroll, scrollTimeout = scrollTimeout, isPabbly = isPabbly, isZapier = isZapier, 
+                customSelectors = customSelectors, keepSelection = keepSelection, formData = formData,
+                isKeepFormDataSelection = isKeepFormDataSelection, dynamicInputs=dynamicInputs, requestType= 'POST')
+        
+        else:
+            request_url = self.__prepareRequestBodyOrUrl(
+            url=url, render=render, session_number=session_number,
+            country_code=country_code,
+            premium=premium, keep_headers=keep_headers, format=format,
+            device_type=device_type, parserSubscriptionId=parserSubscriptionId,
+            webhookRequestId=webhookRequestId, isScroll = isScroll, scrollTimeout = scrollTimeout, 
+            isPabbly = isPabbly, isZapier = isZapier, keepSelection = None, isKeepFormDataSelection= None, requestType= 'GET')
+        
+        custom_headers = headers
+        request_options = self.__prepareHeaders(custom_headers, keep_headers)
+                
+        try:
+            if(customSelectors != [] or formData !={} or (dynamicInputs != [] and parserSubscriptionId)):
+                response = requests.post(url= request_data["request_url"], json = request_data["request_body"], headers=request_options)
+            else:
+                response = requests.get(request_url, headers=request_options)
+            
+            if parserSubscriptionId is not None:
+                response._content = response.json()
+            else:
+                response._content = response.text
+
+        except ValueError:
+            pass
+        return response
+
+    def writeHtmlToFile(self, url: str, file_path: str, render: bool = None,
+                        session_number: str = None, country_code: str = None,
+                        premium: bool = None, keep_headers: bool = None,
+                        headers: dict = {}, format: str = None,
+                        device_type: str = None,
+                        parserSubscriptionId: str = None,
+                        webhookRequestId: str = None, dynamicInputs :list = []):
+        with open(file_path, 'w+') as file:
+            response = self.getHtml(
+                url, render, session_number, country_code, premium,
+                keep_headers, headers, format, device_type, parserSubscriptionId,
+                webhookRequestId, dynamicInputs=dynamicInputs)
+            if format == 'images' or format == 'docx':
+                try:
+                    response._content = b64decode(response.text)
+                except ValueError:
+                    pass
+            file.write(str(response._content))
+        return response
+
+    # def writeCSVFile(self, url: str, file_path: str, render: bool = None,
+    #                  session_number: str = None, country_code: str = None,
+    #                  premium: bool = None, keep_headers: bool = None,
+    #                  headers: dict = {}):
+    #     response = self.writeHtmlToFile(url, file_path, render,
+    #                                     session_number,
+    #                                     country_code, premium,
+    #                                     keep_headers, headers,
+    #                                     format='tables')
+    #     return response
+
+    # def getAllImagesInZip(self, url: str, file_path: str,
+    #                       render: bool = None,
+    #                       session_number: str = None,
+    #                       country_code: str = None,
+    #                       premium: bool = None, keep_headers: bool = None,
+    #                       headers: dict = {}):
+    #     response = self.writeHtmlToFile(url, file_path, render,
+    #                                     session_number, country_code,
+    #                                     premium, keep_headers,
+    #                                     headers, format='images')
+    #     return response
+
+    # def writeDOCXFile(self, url: str, file_path: str, render: bool = None,
+    #                   session_number: str = None, country_code: str = None,
+    #                   premium: bool = None, keep_headers: bool = None,
+    #                   headers: dict = {}):
+    #     response = self.writeHtmlToFile(url, file_path, render,
+    #                                     session_number, country_code,
+    #                                     premium, keep_headers, headers,
+    #                                     format='docx')
+    #     return response
+
+    # def post(self, url: str, render: bool = None,
+    #          session_number: str = None, country_code: str = None,
+    #          premium: bool = None, keep_headers: bool = None,
+    #          headers: dict = {}):
+    #     response = self.getHtml(
+    #         url, render, session_number, country_code,
+    #         premium, keep_headers, headers)
+    #     return response
+
+    # def put(self, url: str, render: bool = None,
+    #         session_number: str = None, country_code: str = None,
+    #         premium: bool = None, keep_headers: bool = None,
+    #         headers: dict = {}):
+    #     response = self.getHtml(
+    #         url, render, session_number, country_code,
+    #         premium, keep_headers, headers)
+    #     return response
+
+    def scrapyGet(self, url: str,
+                  render: bool = None,
+                  session_number: str = None,
+                  country_code: str = None,
+                  premium: bool = None,
+                  keep_headers: bool = None,
+                  format: str = 'html',
+                  device_type: str = None,
+                  parserSubscriptionId: str = None,
+                  webhookRequestId: str = None):
+        request_url = self.__prepareRequestBodyOrUrl(
+            url=url, render=render, session_number=session_number,
+            country_code=country_code,
+            premium=premium, keep_headers=keep_headers, format=format,
+            device_type=device_type, parserSubscriptionId=parserSubscriptionId,
+            webhookRequestId=webhookRequestId, requestType = 'GET')
+        return request_url
+
+    def account(self):
+        response = requests.get(self.account_url,
+                                params={'access_token':
+                                        self.access_token}).json()
+        if response.get('message'):
+            response = response.get('message')
+        return response
+
+
+    def __prepareHeaders(self, custom_headers={}, keep_headers=None):
+        headers = {
+            'Client': 'PYTHON_CLIENT_LIB',
+            'Client-Version': VERSION
+        }
+        merged_headers = headers.copy()
+        merged_headers.update(custom_headers)
+        if keep_headers is True:
+            return merged_headers
+        return headers
+
+    # This function is used for csv, json, excel
+    def getData(self, url: str, render: bool = None, session_number: str = None,
+                country_code: str = None,
+                premium: bool = None, keep_headers: bool = None,
+                headers: dict = {}, format: str = None,
+                device_type: str = None,
+                parserSubscriptionId: str = None, webhookRequestId: str = None, dynamicInputs :list = []):
+        try:
+            response = self.getHtml(url, render, session_number, country_code, premium,
+                                    keep_headers, headers, format, device_type,
+                                    parserSubscriptionId, webhookRequestId, dynamicInputs = dynamicInputs)
+        except ValueError:
+            pass
+        return response
+
+    def __prepareRequestBodyOrUrl(self, **kwargs):
+         url_options = {
+            'access_token': self.access_token,
+            'URL': kwargs['url'],
+            'render': kwargs.get('render', True),
+            'session_number': kwargs['session_number'],
+            'country_code': kwargs['country_code'],
+            'premium': 'true' if kwargs['premium'] is True else None,
+            'keep_headers': 'true' if kwargs['keep_headers'] is True else None,
+            'format': kwargs['format'],
+            'device_type': kwargs['device_type'],
+            'isScroll' : 'true' if kwargs['isScroll'] is True else None,
+            'scrollTimeout' : kwargs['scrollTimeout'],
+            'isPabbly' : 'true' if kwargs['isPabbly'] is True else None,
+            'isZapier' : 'true' if kwargs['isZapier'] is True else None,
+            'keepSelection' : 'true' if kwargs['keepSelection'] is True else None,
+            'isKeepFormDataSelection' : 'true' if kwargs['isKeepFormDataSelection'] is True else None,
+        }
+         if kwargs.get('parserSubscriptionId') is not None:
+            url_options['parserSubscriptionRequestId'] = kwargs['parserSubscriptionId']  
+         if kwargs.get('webhookRequestId') is not None:
+            url_options['webhookRequestId'] = kwargs['webhookRequestId']
+         if kwargs.get('customSelectors') is not None:
+            url_options['customSelectors'] = kwargs['customSelectors']
+         if kwargs.get('formData') is not None:
+            url_options['formData'] = kwargs['formData']
+         if kwargs.get('dynamicInputs') is not None:
+            url_options['dynamicInputs'] = kwargs['dynamicInputs']
+
+         if(kwargs['requestType'] == 'GET'):
+            url_options_filtered = {
+                key: value for key, value in 
+                url_options.items() if value is not None
+            }
+            option_string = urlencode(url_options_filtered)
+            request_url = self.parse_url + '?' + option_string
+            return request_url
+         requestData = { 'request_body':url_options, 'request_url': self.parse_url}
+         return requestData
```

## quickscraper_sdk/constant.py

```diff
@@ -1,10 +1,10 @@
-import os
-
-
-BASE_URL = os.environ.get('QS_BASE_URL') or 'https://api.quickscraper.co/'
-VERSION = '1.1.1'
-
-
-# from importlib.metadata import version
-# VERSION = version('quickscraper-sdk')
-# Not working this approach with pytest, so version is defined statically
+import os
+
+
+BASE_URL = os.environ.get('QS_BASE_URL') or 'https://api.quickscraper.co/'
+VERSION = '1.1.2'
+
+
+# from importlib.metadata import version
+# VERSION = version('quickscraper-sdk')
+# Not working this approach with pytest, so version is defined statically
```

## tests/__init__.py

 * *Ordering differences only*

```diff
@@ -1,5 +1,5 @@
-"""
-tests
-~~~~~
-Test suite for the quickscraper-sdk package.
-"""
+"""
+tests
+~~~~~
+Test suite for the quickscraper-sdk package.
+"""
```

## tests/constant.py

 * *Ordering differences only*

```diff
@@ -1,7 +1,7 @@
-
-import os
-
-
-ACCESS_TOKEN = os.environ.get('QS_ACCESS_TOKEN') or 'DUMMY'
-SAMPLE_REQUEST_URL_FOR_HTML = 'http://httpbin.org/ip'
-SAMPLE_REQUEST_URL_HEADER = 'https://httpbin.org/headers'
+
+import os
+
+
+ACCESS_TOKEN = os.environ.get('QS_ACCESS_TOKEN') or 'DUMMY'
+SAMPLE_REQUEST_URL_FOR_HTML = 'http://httpbin.org/ip'
+SAMPLE_REQUEST_URL_HEADER = 'https://httpbin.org/headers'
```

## tests/test_cases.py

 * *Ordering differences only*

```diff
@@ -1,112 +1,112 @@
-from unittest import TestCase
-from quickscraper_sdk import QuickScraper
-# from time import time
-import tests.constant as constant
-
-
-class Testing(TestCase):
-
-    def test_parse_url(self):
-        quickscraper_client = QuickScraper(constant.ACCESS_TOKEN)
-        request_url = constant.SAMPLE_REQUEST_URL_FOR_HTML
-        response = quickscraper_client.getHtml(request_url)
-        self.assertEqual(response.status_code, 200)
-        self.assertIsNotNone(response.text)
-
-    def test_dummy_token(self):
-        quickscraper_client = QuickScraper('DUMMY')
-        request_url = constant.SAMPLE_REQUEST_URL_FOR_HTML
-        response = quickscraper_client.getHtml(request_url)
-        self.assertEqual(response.status_code, 400)
-        self.assertEqual(response.text, 'Please enter valid access token')
-
-    def test_render_true(self):
-        quickscraper_client = QuickScraper(constant.ACCESS_TOKEN)
-        request_url = constant.SAMPLE_REQUEST_URL_FOR_HTML
-        response = quickscraper_client.getHtml(request_url, render=True)
-        self.assertEqual(response.status_code, 200)
-        self.assertIsNotNone(response.text)
-
-    def test_custom_headers(self):
-        quickscraper_client = QuickScraper(constant.ACCESS_TOKEN)
-        request_url = constant.SAMPLE_REQUEST_URL_HEADER
-        options = {
-            'X-Custom-Header-Key-1': 'THIS_IS_CUSTOM_HEADER_1',
-            'Qs-Custom-Header-Key': 'THIS_IS_QS_CUSTOM_HEADER'
-        }
-        response = quickscraper_client.getHtml(
-            request_url, keep_headers=True, headers=options)
-        self.assertEqual(response.status_code, 200)
-        self.assertIsNotNone(response.text)
-        self.assertIn('headers', response.text)
-        self.assertIn('X-Custom-Header-Key-1', response.text)
-        self.assertIn('THIS_IS_CUSTOM_HEADER_1', response.text)
-        self.assertIn('Qs-Custom-Header-Key', response.text)
-        self.assertIn('THIS_IS_QS_CUSTOM_HEADER', response.text)
-
-    # def test_session_number(self):
-    #     quickscraper_client = QuickScraper(constant.ACCESS_TOKEN)
-    #     request_url = constant.SAMPLE_REQUEST_URL_FOR_HTML
-    #     session_number = 'QS-' + str(int(time()))
-    #     response = quickscraper_client.getHtml(
-    #         request_url, session_number=session_number)
-    #     self.assertEqual(response.status_code, 200)
-    #     self.assertIsNotNone(response.text)
-
-    def test_country_code(self):
-        quickscraper_client = QuickScraper(constant.ACCESS_TOKEN)
-        request_url = constant.SAMPLE_REQUEST_URL_FOR_HTML
-        response = quickscraper_client.getHtml(request_url, country_code='US')
-        self.assertEqual(response.status_code, 200)
-        self.assertIsNotNone(response.text)
-
-    def test_premium_proxy(self):
-        quickscraper_client = QuickScraper(constant.ACCESS_TOKEN)
-        request_url = constant.SAMPLE_REQUEST_URL_FOR_HTML
-        response = quickscraper_client.getHtml(request_url, premium=True)
-        self.assertEqual(response.status_code, 200)
-        self.assertIsNotNone(response.text)
-
-    def test_write_html_to_file(self):
-        quickscraper_client = QuickScraper(constant.ACCESS_TOKEN)
-        request_url = constant.SAMPLE_REQUEST_URL_FOR_HTML
-        response = quickscraper_client.writeHtmlToFile(request_url, 'test.log')
-        self.assertEqual(response.status_code, 200)
-        self.assertIsNotNone(response.text)
-
-    # def test_write_csv_file(self):
-    #     quickscraper_client = QuickScraper(constant.ACCESS_TOKEN)
-    #     request_url = constant.SAMPLE_REQUEST_URL_FOR_CSV
-    #     response = quickscraper_client.writeCSVFile(request_url, 'test.csv')
-    #     self.assertEqual(response.status_code, 200)
-    #     self.assertIsNotNone(response.text)
-
-    # def test_get_all_images_in_zip(self):
-    #     quickscraper_client = QuickScraper(constant.ACCESS_TOKEN)
-    #     request_url = constant.SAMPLE_REQUEST_URL_FOR_ZIP
-    #     response = quickscraper_client.getAllImagesInZip(
-    #         request_url, 'test.zip')
-    #     self.assertEqual(response.status_code, 200)
-    #     self.assertIsNotNone(response.text)
-
-    # def test_write_docx_file(self):
-    #     quickscraper_client = QuickScraper(constant.ACCESS_TOKEN)
-    #     request_url = constant.SAMPLE_REQUEST_URL_FOR_DOCX
-    #     response = quickscraper_client.writeDOCXFile(request_url,
-    #                                                  'test.docx')
-    #     self.assertEqual(response.status_code, 200)
-    #     self.assertIsNotNone(response.text)
-
-    # def test_post(self):
-    #     quickscraper_client = QuickScraper(constant.ACCESS_TOKEN)
-    #     request_url = constant.SAMPLE_REQUEST_URL_FOR_HTML
-    #     response = quickscraper_client.getHtml(request_url)
-    #     self.assertEqual(response.status_code, 200)
-    #     self.assertIsNotNone(response.text)
-
-    # def test_put(self):
-    #     quickscraper_client = QuickScraper(constant.ACCESS_TOKEN)
-    #     request_url = constant.SAMPLE_REQUEST_URL_FOR_HTML
-    #     response = quickscraper_client.getHtml(request_url)
-    #     self.assertEqual(response.status_code, 200)
-    #     self.assertIsNotNone(response.text)
+from unittest import TestCase
+from quickscraper_sdk import QuickScraper
+# from time import time
+import tests.constant as constant
+
+
+class Testing(TestCase):
+
+    def test_parse_url(self):
+        quickscraper_client = QuickScraper(constant.ACCESS_TOKEN)
+        request_url = constant.SAMPLE_REQUEST_URL_FOR_HTML
+        response = quickscraper_client.getHtml(request_url)
+        self.assertEqual(response.status_code, 200)
+        self.assertIsNotNone(response.text)
+
+    def test_dummy_token(self):
+        quickscraper_client = QuickScraper('DUMMY')
+        request_url = constant.SAMPLE_REQUEST_URL_FOR_HTML
+        response = quickscraper_client.getHtml(request_url)
+        self.assertEqual(response.status_code, 400)
+        self.assertEqual(response.text, 'Please enter valid access token')
+
+    def test_render_true(self):
+        quickscraper_client = QuickScraper(constant.ACCESS_TOKEN)
+        request_url = constant.SAMPLE_REQUEST_URL_FOR_HTML
+        response = quickscraper_client.getHtml(request_url, render=True)
+        self.assertEqual(response.status_code, 200)
+        self.assertIsNotNone(response.text)
+
+    def test_custom_headers(self):
+        quickscraper_client = QuickScraper(constant.ACCESS_TOKEN)
+        request_url = constant.SAMPLE_REQUEST_URL_HEADER
+        options = {
+            'X-Custom-Header-Key-1': 'THIS_IS_CUSTOM_HEADER_1',
+            'Qs-Custom-Header-Key': 'THIS_IS_QS_CUSTOM_HEADER'
+        }
+        response = quickscraper_client.getHtml(
+            request_url, keep_headers=True, headers=options)
+        self.assertEqual(response.status_code, 200)
+        self.assertIsNotNone(response.text)
+        self.assertIn('headers', response.text)
+        self.assertIn('X-Custom-Header-Key-1', response.text)
+        self.assertIn('THIS_IS_CUSTOM_HEADER_1', response.text)
+        self.assertIn('Qs-Custom-Header-Key', response.text)
+        self.assertIn('THIS_IS_QS_CUSTOM_HEADER', response.text)
+
+    # def test_session_number(self):
+    #     quickscraper_client = QuickScraper(constant.ACCESS_TOKEN)
+    #     request_url = constant.SAMPLE_REQUEST_URL_FOR_HTML
+    #     session_number = 'QS-' + str(int(time()))
+    #     response = quickscraper_client.getHtml(
+    #         request_url, session_number=session_number)
+    #     self.assertEqual(response.status_code, 200)
+    #     self.assertIsNotNone(response.text)
+
+    def test_country_code(self):
+        quickscraper_client = QuickScraper(constant.ACCESS_TOKEN)
+        request_url = constant.SAMPLE_REQUEST_URL_FOR_HTML
+        response = quickscraper_client.getHtml(request_url, country_code='US')
+        self.assertEqual(response.status_code, 200)
+        self.assertIsNotNone(response.text)
+
+    def test_premium_proxy(self):
+        quickscraper_client = QuickScraper(constant.ACCESS_TOKEN)
+        request_url = constant.SAMPLE_REQUEST_URL_FOR_HTML
+        response = quickscraper_client.getHtml(request_url, premium=True)
+        self.assertEqual(response.status_code, 200)
+        self.assertIsNotNone(response.text)
+
+    def test_write_html_to_file(self):
+        quickscraper_client = QuickScraper(constant.ACCESS_TOKEN)
+        request_url = constant.SAMPLE_REQUEST_URL_FOR_HTML
+        response = quickscraper_client.writeHtmlToFile(request_url, 'test.log')
+        self.assertEqual(response.status_code, 200)
+        self.assertIsNotNone(response.text)
+
+    # def test_write_csv_file(self):
+    #     quickscraper_client = QuickScraper(constant.ACCESS_TOKEN)
+    #     request_url = constant.SAMPLE_REQUEST_URL_FOR_CSV
+    #     response = quickscraper_client.writeCSVFile(request_url, 'test.csv')
+    #     self.assertEqual(response.status_code, 200)
+    #     self.assertIsNotNone(response.text)
+
+    # def test_get_all_images_in_zip(self):
+    #     quickscraper_client = QuickScraper(constant.ACCESS_TOKEN)
+    #     request_url = constant.SAMPLE_REQUEST_URL_FOR_ZIP
+    #     response = quickscraper_client.getAllImagesInZip(
+    #         request_url, 'test.zip')
+    #     self.assertEqual(response.status_code, 200)
+    #     self.assertIsNotNone(response.text)
+
+    # def test_write_docx_file(self):
+    #     quickscraper_client = QuickScraper(constant.ACCESS_TOKEN)
+    #     request_url = constant.SAMPLE_REQUEST_URL_FOR_DOCX
+    #     response = quickscraper_client.writeDOCXFile(request_url,
+    #                                                  'test.docx')
+    #     self.assertEqual(response.status_code, 200)
+    #     self.assertIsNotNone(response.text)
+
+    # def test_post(self):
+    #     quickscraper_client = QuickScraper(constant.ACCESS_TOKEN)
+    #     request_url = constant.SAMPLE_REQUEST_URL_FOR_HTML
+    #     response = quickscraper_client.getHtml(request_url)
+    #     self.assertEqual(response.status_code, 200)
+    #     self.assertIsNotNone(response.text)
+
+    # def test_put(self):
+    #     quickscraper_client = QuickScraper(constant.ACCESS_TOKEN)
+    #     request_url = constant.SAMPLE_REQUEST_URL_FOR_HTML
+    #     response = quickscraper_client.getHtml(request_url)
+    #     self.assertEqual(response.status_code, 200)
+    #     self.assertIsNotNone(response.text)
```

## Comparing `quickscraper_sdk-1.1.1.dist-info/LICENSE` & `quickscraper_sdk-1.1.2.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 Bhushankumar L
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2021 Bhushankumar L
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

## Comparing `quickscraper_sdk-1.1.1.dist-info/METADATA` & `quickscraper_sdk-1.1.2.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,161 +1,163 @@
-Metadata-Version: 2.1
-Name: quickscraper-sdk
-Version: 1.1.1
-Summary: https://quickscraper.co
-Home-page: https://quickscraper.co/
-Author: QuickScraper
-Author-email: app@quickscraper.co
-License: BSD
-Keywords: quickscraper
-Classifier: Development Status :: 3 - Alpha
-Classifier: Topic :: Utilities
-Classifier: License :: OSI Approved :: BSD License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# quickscraper-sdk-python
-
-[Register For Free https://www.quickscraper.co](https://www.quickscraper.co)
-
-## Installation
-
-```bash
-pip install quickscraper-sdk
-```
-
-## Get Free Access (Free Forever)
-
-- Register yourself here [https://app.quickscraper.co/auth/register](https://app.quickscraper.co/auth/register)
-
-## Examples
-
-### Basic Usage
-
-```python
-from quickscraper_sdk import QuickScraper
-quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
-response = quickscraper_client.getHtml('http://httpbin.org/ip')
-print(response._content)
-```
-
-### Write a HTML to File
-
-```python
-from quickscraper_sdk import QuickScraper
-quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
-quickscraper_client.writeHtmlToFile(
-    'http://httpbin.org/ip', file_path='filename.html')
-```
-
-### Rendering Javascript
-
-```python
-from quickscraper_sdk import QuickScraper
-quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
-response = quickscraper_client.getHtml('http://httpbin.org/ip', render=True)
-print(response._content)
-```
-
-### Custom Headers
-
-```python
-from quickscraper_sdk import QuickScraper
-quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
-response = quickscraper_client.getHtml(
-    'https://httpbin.org/headers', keep_headers=True, headers={'X-My-Custom-Header': 'QS-APP'})
-print(response._content)
-```
-
-### Geographic Location
-
-```python
-from quickscraper_sdk import QuickScraper
-quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
-response = quickscraper_client.getHtml(
-    'http://httpbin.org/ip', country_code='US')
-print(response._content)
-```
-
-### Premium Residential/Mobile Proxy Pools
-
-```python
-from quickscraper_sdk import QuickScraper
-quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
-response = quickscraper_client.getHtml('http://httpbin.org/ip', premium=True)
-print(response._content)
-```
-
-### Device Type
-
-```python
-from quickscraper_sdk import QuickScraper
-quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
-response = quickscraper_client.getHtml('http://httpbin.org/ip', device_type='mobile')
-print(response._content)
-```
-
-### Account Information
-
-```python
-from quickscraper_sdk import QuickScraper
-quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
-usage = quickscraper_client.account()
-print(usage)
-```
-
-### Parser Addon
-
-```python
-from quickscraper_sdk import QuickScraper
-quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
-response = quickscraper_client.getHtml('http://httpbin.org/ip', parserSubscriptionId='PARSER_SUBSCRIPTION_ID')
-print(response._content)
-```
-
-### Webhook Addon
-
-```python
-from quickscraper_sdk import QuickScraper
-quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
-response = quickscraper_client.getHtml('http://httpbin.org/ip', webhookRequestId='WEBHOOK_ID')
-print(response._content)
-```
-### Get JSON from data
-
-```python
-from quickscraper_sdk import QuickScraper
-quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
-response = quickscraper_client.getData('http://httpbin.org/ip', parserSubscriptionId='PARSER_SUBSCRIPTION_ID')
-print(response._content)
-```
-### Write CSV, EXCEL to file from data
-
-```python
-from quickscraper_sdk import QuickScraper
-quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
-response = quickscraper_client.writeHtmlToFile('http://httpbin.org/ip', file_path='YOUR_FILE_PATH', parserSubscriptionId='PARSER_SUBSCRIPTION_ID')
-print(response._content)
-```
-
-### Add Dynamic Inputs With Parser
-
-```python
-from quickscraper_sdk import QuickScraper
-quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
-response = quickscraper_client.getData('http://httpbin.org/ip', parserSubscriptionId='PARSER_SUBSCRIPTION_ID', dynamicInputs= [ {'name': 'YOUR_INPUT_NAME', 'value': 'YOUR_INPUT_VALUE' } ])
-print(response._content)
-```
-
-### Scroll To Bottom Of the Page Feature
-
-```python
-from quickscraper_sdk import QuickScraper
-quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
-response = quickscraper_client.getHtml('http://httpbin.org/ip', isScroll=True, scrollTimeout=1000) # 1000 Consider as milliseconds for scroll after 1000 milliseconds
-print(response._content)
-```
-
-## Do you need an expert?
-
-Are you finding a developer for your world-class product? If yes, please contact here.
-Originally by [QuickScraper Developers - app@quickscraper.co](mailto:app@quickscraper.co).
+Metadata-Version: 2.1
+Name: quickscraper-sdk
+Version: 1.1.2
+Summary: https://quickscraper.co
+Home-page: https://quickscraper.co/
+Author: QuickScraper
+Author-email: app@quickscraper.co
+License: BSD
+Keywords: quickscraper
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Topic :: Utilities
+Classifier: License :: OSI Approved :: BSD License
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# quickscraper-sdk-python
+
+[Register For Free https://www.quickscraper.co](https://www.quickscraper.co)
+
+## Installation
+
+```bash
+pip install quickscraper-sdk
+```
+
+## Get Free Access (Free Forever)
+
+- Register yourself here [https://app.quickscraper.co/auth/register](https://app.quickscraper.co/auth/register)
+
+## Examples
+
+### Basic Usage
+
+```python
+from quickscraper_sdk import QuickScraper
+quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
+response = quickscraper_client.getHtml('http://httpbin.org/ip')
+print(response._content)
+```
+
+### Write a HTML to File
+
+```python
+from quickscraper_sdk import QuickScraper
+quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
+quickscraper_client.writeHtmlToFile(
+    'http://httpbin.org/ip', file_path='filename.html')
+```
+
+### Rendering Javascript
+
+```python
+from quickscraper_sdk import QuickScraper
+quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
+response = quickscraper_client.getHtml('http://httpbin.org/ip', render=True)
+print(response._content)
+```
+
+### Custom Headers
+
+```python
+from quickscraper_sdk import QuickScraper
+quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
+response = quickscraper_client.getHtml(
+    'https://httpbin.org/headers', keep_headers=True, headers={'X-My-Custom-Header': 'QS-APP'})
+print(response._content)
+```
+
+### Geographic Location
+
+```python
+from quickscraper_sdk import QuickScraper
+quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
+response = quickscraper_client.getHtml(
+    'http://httpbin.org/ip', country_code='US')
+print(response._content)
+```
+
+### Premium Residential/Mobile Proxy Pools
+
+```python
+from quickscraper_sdk import QuickScraper
+quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
+response = quickscraper_client.getHtml('http://httpbin.org/ip', premium=True)
+print(response._content)
+```
+
+### Device Type
+
+```python
+from quickscraper_sdk import QuickScraper
+quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
+response = quickscraper_client.getHtml('http://httpbin.org/ip', device_type='mobile')
+print(response._content)
+```
+
+### Account Information
+
+```python
+from quickscraper_sdk import QuickScraper
+quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
+usage = quickscraper_client.account()
+print(usage)
+```
+
+### Parser Addon
+
+```python
+from quickscraper_sdk import QuickScraper
+quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
+response = quickscraper_client.getHtml('http://httpbin.org/ip', parserSubscriptionId='PARSER_SUBSCRIPTION_ID')
+print(response._content)
+```
+
+### Webhook Addon
+
+```python
+from quickscraper_sdk import QuickScraper
+quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
+response = quickscraper_client.getHtml('http://httpbin.org/ip', webhookRequestId='WEBHOOK_ID')
+print(response._content)
+```
+### Get JSON from data
+
+```python
+from quickscraper_sdk import QuickScraper
+quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
+response = quickscraper_client.getData('http://httpbin.org/ip', parserSubscriptionId='PARSER_SUBSCRIPTION_ID')
+print(response._content)
+```
+### Write CSV, EXCEL to file from data
+
+```python
+from quickscraper_sdk import QuickScraper
+quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
+response = quickscraper_client.writeHtmlToFile('http://httpbin.org/ip', file_path='YOUR_FILE_PATH', parserSubscriptionId='PARSER_SUBSCRIPTION_ID')
+print(response._content)
+```
+
+### Add Dynamic Inputs With Parser
+
+```python
+from quickscraper_sdk import QuickScraper
+quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
+response = quickscraper_client.getData('http://httpbin.org/ip', parserSubscriptionId='PARSER_SUBSCRIPTION_ID', dynamicInputs= [ {'name': 'YOUR_INPUT_NAME', 'value': 'YOUR_INPUT_VALUE' } ])
+print(response._content)
+```
+
+### Scroll To Bottom Of the Page Feature
+
+```python
+from quickscraper_sdk import QuickScraper
+quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
+response = quickscraper_client.getHtml('http://httpbin.org/ip', isScroll=True, scrollTimeout=1000) # 1000 Consider as milliseconds for scroll after 1000 milliseconds
+print(response._content)
+```
+
+## Do you need an expert?
+
+Are you finding a developer for your world-class product? If yes, please contact here.
+Originally by [QuickScraper Developers - app@quickscraper.co](mailto:app@quickscraper.co).
+
```

