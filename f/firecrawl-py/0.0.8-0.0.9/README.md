# Comparing `tmp/firecrawl-py-0.0.8.tar.gz` & `tmp/firecrawl-py-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firecrawl-py-0.0.8.tar", last modified: Thu May  9 00:30:33 2024, max compression
+gzip compressed data, was "firecrawl-py-0.0.9.tar", last modified: Mon May 20 16:40:27 2024, max compression
```

## Comparing `firecrawl-py-0.0.8.tar` & `firecrawl-py-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-05-09 00:30:33.635435 firecrawl-py-0.0.8/
--rw-r--r--   0 nicolascamara   (501) staff       (20)      196 2024-05-09 00:30:33.635318 firecrawl-py-0.0.8/PKG-INFO
--rw-r--r--   0 nicolascamara   (501) staff       (20)     3561 2024-04-26 21:23:35.000000 firecrawl-py-0.0.8/README.md
-drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-05-09 00:30:33.634452 firecrawl-py-0.0.8/firecrawl/
--rw-r--r--   0 nicolascamara   (501) staff       (20)       36 2024-04-15 21:00:54.000000 firecrawl-py-0.0.8/firecrawl/__init__.py
--rw-r--r--   0 nicolascamara   (501) staff       (20)     6932 2024-05-09 00:30:10.000000 firecrawl-py-0.0.8/firecrawl/firecrawl.py
-drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-05-09 00:30:33.635170 firecrawl-py-0.0.8/firecrawl_py.egg-info/
--rw-r--r--   0 nicolascamara   (501) staff       (20)      196 2024-05-09 00:30:33.000000 firecrawl-py-0.0.8/firecrawl_py.egg-info/PKG-INFO
--rw-r--r--   0 nicolascamara   (501) staff       (20)      242 2024-05-09 00:30:33.000000 firecrawl-py-0.0.8/firecrawl_py.egg-info/SOURCES.txt
--rw-r--r--   0 nicolascamara   (501) staff       (20)        1 2024-05-09 00:30:33.000000 firecrawl-py-0.0.8/firecrawl_py.egg-info/dependency_links.txt
--rw-r--r--   0 nicolascamara   (501) staff       (20)        9 2024-05-09 00:30:33.000000 firecrawl-py-0.0.8/firecrawl_py.egg-info/requires.txt
--rw-r--r--   0 nicolascamara   (501) staff       (20)       10 2024-05-09 00:30:33.000000 firecrawl-py-0.0.8/firecrawl_py.egg-info/top_level.txt
--rw-r--r--   0 nicolascamara   (501) staff       (20)       38 2024-05-09 00:30:33.635482 firecrawl-py-0.0.8/setup.cfg
--rw-r--r--   0 nicolascamara   (501) staff       (20)      342 2024-05-09 00:30:17.000000 firecrawl-py-0.0.8/setup.py
+drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-05-20 16:40:27.558237 firecrawl-py-0.0.9/
+-rw-r--r--   0 nicolascamara   (501) staff       (20)      196 2024-05-20 16:40:27.558106 firecrawl-py-0.0.9/PKG-INFO
+-rw-r--r--   0 nicolascamara   (501) staff       (20)     4278 2024-05-09 00:41:07.000000 firecrawl-py-0.0.9/README.md
+drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-05-20 16:40:27.557267 firecrawl-py-0.0.9/firecrawl/
+-rw-r--r--   0 nicolascamara   (501) staff       (20)       36 2024-04-15 21:00:54.000000 firecrawl-py-0.0.9/firecrawl/__init__.py
+-rw-r--r--   0 nicolascamara   (501) staff       (20)     6992 2024-05-20 16:39:18.000000 firecrawl-py-0.0.9/firecrawl/firecrawl.py
+drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-05-20 16:40:27.557911 firecrawl-py-0.0.9/firecrawl_py.egg-info/
+-rw-r--r--   0 nicolascamara   (501) staff       (20)      196 2024-05-20 16:40:27.000000 firecrawl-py-0.0.9/firecrawl_py.egg-info/PKG-INFO
+-rw-r--r--   0 nicolascamara   (501) staff       (20)      242 2024-05-20 16:40:27.000000 firecrawl-py-0.0.9/firecrawl_py.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolascamara   (501) staff       (20)        1 2024-05-20 16:40:27.000000 firecrawl-py-0.0.9/firecrawl_py.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolascamara   (501) staff       (20)        9 2024-05-20 16:40:27.000000 firecrawl-py-0.0.9/firecrawl_py.egg-info/requires.txt
+-rw-r--r--   0 nicolascamara   (501) staff       (20)       10 2024-05-20 16:40:27.000000 firecrawl-py-0.0.9/firecrawl_py.egg-info/top_level.txt
+-rw-r--r--   0 nicolascamara   (501) staff       (20)       38 2024-05-20 16:40:27.558286 firecrawl-py-0.0.9/setup.cfg
+-rw-r--r--   0 nicolascamara   (501) staff       (20)      342 2024-05-20 16:40:00.000000 firecrawl-py-0.0.9/setup.py
```

### Comparing `firecrawl-py-0.0.8/firecrawl/firecrawl.py` & `firecrawl-py-0.0.9/firecrawl/firecrawl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import os
 from typing import Any, Dict, Optional
 import requests
 import time
 
 class FirecrawlApp:
-    def __init__(self, api_key=None):
+    def __init__(self, api_key=None, api_url='https://api.firecrawl.dev'):
         self.api_key = api_key or os.getenv('FIRECRAWL_API_KEY')
         if self.api_key is None:
             raise ValueError('No API key provided')
+        self.api_url = api_url or os.getenv('FIRECRAWL_API_URL')
     
     
 
     def scrape_url(self, url: str, params: Optional[Dict[str, Any]] = None) -> Any:
         headers = {
             'Content-Type': 'application/json',
             'Authorization': f'Bearer {self.api_key}'
@@ -34,40 +35,40 @@
             
             # Include any other params directly at the top level of scrape_params
             for key, value in params.items():
                 if key != 'extractorOptions':
                     scrape_params[key] = value
         # Make the POST request with the prepared headers and JSON data
         response = requests.post(
-            'https://api.firecrawl.dev/v0/scrape',
+            f'{self.api_url}/v0/scrape',
             headers=headers,
             json=scrape_params
         )
         if response.status_code == 200:
             response = response.json()
             if response['success']:
                 return response['data']
             else:
                 raise Exception(f'Failed to scrape URL. Error: {response["error"]}')
-        elif response.status_code in [402, 409, 500]:
+        elif response.status_code in [402, 408, 409, 500]:
             error_message = response.json().get('error', 'Unknown error occurred')
             raise Exception(f'Failed to scrape URL. Status code: {response.status_code}. Error: {error_message}')
         else:
             raise Exception(f'Failed to scrape URL. Status code: {response.status_code}')
         
     def search(self, query, params=None):
         headers = {
             'Content-Type': 'application/json',
             'Authorization': f'Bearer {self.api_key}'
         }
         json_data = {'query': query}
         if params:
             json_data.update(params)
         response = requests.post(
-            'https://api.firecrawl.dev/v0/search',
+            f'{self.api_url}/v0/search',
             headers=headers,
             json=json_data
         )
         if response.status_code == 200:
             response = response.json()
             if response['success'] == True:
                 return response['data']
@@ -81,27 +82,27 @@
             raise Exception(f'Failed to search. Status code: {response.status_code}')
 
     def crawl_url(self, url, params=None, wait_until_done=True, timeout=2):
         headers = self._prepare_headers()
         json_data = {'url': url}
         if params:
             json_data.update(params)
-        response = self._post_request('https://api.firecrawl.dev/v0/crawl', json_data, headers)
+        response = self._post_request(f'{self.api_url}/v0/crawl', json_data, headers)
         if response.status_code == 200:
             job_id = response.json().get('jobId')
             if wait_until_done:
                 return self._monitor_job_status(job_id, headers, timeout)
             else:
                 return {'jobId': job_id}
         else:
             self._handle_error(response, 'start crawl job')
 
     def check_crawl_status(self, job_id):
         headers = self._prepare_headers()
-        response = self._get_request(f'https://api.firecrawl.dev/v0/crawl/status/{job_id}', headers)
+        response = self._get_request(f'{self.api_url}/v0/crawl/status/{job_id}', headers)
         if response.status_code == 200:
             return response.json()
         else:
             self._handle_error(response, 'check crawl status')
 
     def _prepare_headers(self):
         return {
@@ -126,15 +127,15 @@
             else:
                 return response
         return response
 
     def _monitor_job_status(self, job_id, headers, timeout):
         import time
         while True:
-            status_response = self._get_request(f'https://api.firecrawl.dev/v0/crawl/status/{job_id}', headers)
+            status_response = self._get_request(f'{self.api_url}/v0/crawl/status/{job_id}', headers)
             if status_response.status_code == 200:
                 status_data = status_response.json()
                 if status_data['status'] == 'completed':
                     if 'data' in status_data:
                         return status_data['data']
                     else:
                         raise Exception('Crawl job completed but no data was returned')
@@ -144,12 +145,12 @@
                     time.sleep(timeout)  # Wait for the specified timeout before checking again
                 else:
                     raise Exception(f'Crawl job failed or was stopped. Status: {status_data["status"]}')
             else:
                 self._handle_error(status_response, 'check crawl status')
 
     def _handle_error(self, response, action):
-        if response.status_code in [402, 409, 500]:
+        if response.status_code in [402, 408, 409, 500]:
             error_message = response.json().get('error', 'Unknown error occurred')
             raise Exception(f'Failed to {action}. Status code: {response.status_code}. Error: {error_message}')
         else:
             raise Exception(f'Unexpected error occurred while trying to {action}. Status code: {response.status_code}')
```

