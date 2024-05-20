# Comparing `tmp/sentier_glossary-0.1.0.tar.gz` & `tmp/sentier_glossary-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentier_glossary-0.1.0.tar", last modified: Sun May 19 22:47:49 2024, max compression
+gzip compressed data, was "sentier_glossary-0.2.0.tar", last modified: Mon May 20 13:30:02 2024, max compression
```

## Comparing `sentier_glossary-0.1.0.tar` & `sentier_glossary-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:47:49.149914 sentier_glossary-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-19 22:47:45.000000 sentier_glossary-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 22:47:45.000000 sentier_glossary-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-19 22:47:49.145913 sentier_glossary-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-19 22:47:45.000000 sentier_glossary-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-19 22:47:45.000000 sentier_glossary-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:47:49.145913 sentier_glossary-0.1.0/sentier_glossary/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-19 22:47:45.000000 sentier_glossary-0.1.0/sentier_glossary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-05-19 22:47:45.000000 sentier_glossary-0.1.0/sentier_glossary/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-19 22:47:45.000000 sentier_glossary-0.1.0/sentier_glossary/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:47:49.145913 sentier_glossary-0.1.0/sentier_glossary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-19 22:47:49.000000 sentier_glossary-0.1.0/sentier_glossary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-19 22:47:49.000000 sentier_glossary-0.1.0/sentier_glossary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 22:47:49.000000 sentier_glossary-0.1.0/sentier_glossary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-19 22:47:49.000000 sentier_glossary-0.1.0/sentier_glossary.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-19 22:47:49.000000 sentier_glossary-0.1.0/sentier_glossary.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 22:47:49.149914 sentier_glossary-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:30:02.686800 sentier_glossary-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-20 13:29:59.000000 sentier_glossary-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 13:29:59.000000 sentier_glossary-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-20 13:30:02.686800 sentier_glossary-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-20 13:29:59.000000 sentier_glossary-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-20 13:29:59.000000 sentier_glossary-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:30:02.686800 sentier_glossary-0.2.0/sentier_glossary/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-20 13:29:59.000000 sentier_glossary-0.2.0/sentier_glossary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-05-20 13:29:59.000000 sentier_glossary-0.2.0/sentier_glossary/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-20 13:29:59.000000 sentier_glossary-0.2.0/sentier_glossary/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:30:02.686800 sentier_glossary-0.2.0/sentier_glossary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-20 13:30:02.000000 sentier_glossary-0.2.0/sentier_glossary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-20 13:30:02.000000 sentier_glossary-0.2.0/sentier_glossary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:30:02.000000 sentier_glossary-0.2.0/sentier_glossary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-20 13:30:02.000000 sentier_glossary-0.2.0/sentier_glossary.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-20 13:30:02.000000 sentier_glossary-0.2.0/sentier_glossary.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 13:30:02.686800 sentier_glossary-0.2.0/setup.cfg
```

### Comparing `sentier_glossary-0.1.0/LICENSE` & `sentier_glossary-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sentier_glossary-0.1.0/PKG-INFO` & `sentier_glossary-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentier_glossary
-Version: 0.1.0
+Version: 0.2.0
 Summary: Client interface to sentier.dev sustainability assessment glossary
 Author-email: João Gonçalves <jsvgoncalves@gmail.com>, Chris Mutel <cmutel@gmail.com>
 Maintainer-email: João Gonçalves <jsvgoncalves@gmail.com>, Chris Mutel <cmutel@gmail.com>
 Project-URL: source, https://github.com/Depart-de-Sentier/sentier_glossary
 Project-URL: homepage, https://github.com/Depart-de-Sentier/sentier_glossary
 Project-URL: tracker, https://github.com/Depart-de-Sentier/sentier_glossary/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sentier_glossary-0.1.0/README.md` & `sentier_glossary-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sentier_glossary-0.1.0/pyproject.toml` & `sentier_glossary-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sentier_glossary-0.1.0/sentier_glossary/main.py` & `sentier_glossary-0.2.0/sentier_glossary/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import locale
 from enum import Enum
-from urllib.parse import urljoin, urlparse
+from functools import reduce
+from urllib.parse import urljoin
 
 import requests
 import torch
-from sentence_transformers import SentenceTransformer, util # type: ignore
+from sentence_transformers import SentenceTransformer, util  # type: ignore
 
 from sentier_glossary.settings import Settings
 
 
 class CommonSchemes(Enum):
     cn2024 = "http://data.europa.eu/xsp/cn2024/cn2024"
     nace21 = "http://data.europa.eu/ux2/nace2.1/nace2.1"
@@ -21,27 +22,61 @@
 DEFAULT_COMPONENTS = {
     "process": CommonSchemes.cn2024,
     "product": CommonSchemes.nace21,
     "unit": None,
     "place": None,
 }
 
-cfg = Settings()
 
 class GlossaryAPI:
-    def __init__(self, base_url: str = cfg.base_url, default_language: str | None = None):
-        self.base_url = base_url
-        if not self.base_url.endswith("/"):
-            self.base_url += "/"
+    def __init__(self, cfg: Settings | None = None, default_language: str | None = None):
+        self._cfg = cfg if cfg is not None else Settings()
+        if not self._cfg.base_url.endswith("/"):
+            self._cfg.base_url += "/"
 
         self._semantic_search = False
         # self._catalogues = {}
         self.language_code = self.get_language_code()
         print(f"Using language code '{self.language_code}'; change with `set_language_code()`")
 
+    def _requests_get(self, url: str, params: dict | None = None) -> dict:
+        """Perform a `requests.get(api_url, …)` with given parameters.
+
+        Args:
+            url: The API endpoint.
+            params: Any additional parameters to pass.
+
+        Returns:
+            dict: A dictionary containing the parsed JSON response.
+
+        Raises:
+            requests.exceptions.RequestException: If there is an error with the request,
+            such as a connection error or an invalid URL.
+
+        """
+        params = self._params | params if params is not None else self._params
+        response = requests.get(
+            reduce(urljoin, [self._cfg.base_url, f"{self._cfg.api_version}/", url]),
+            params=params,
+        )
+        try:
+            response.raise_for_status()
+        except requests.exceptions.RequestException as error:
+            msg = f"Error fetching data: {error}"
+            if response is not None:
+                status_code = response.status_code
+                msg += f"\nHTTP {status_code}"
+                if 400 <= status_code < 600:
+                    try:
+                        error_data = response.json()
+                        msg += f"\nResponse: {error_data}"
+                    except ValueError:
+                        msg += f"\nResponse: {response.text}"
+            raise requests.exceptions.RequestException(msg) from error
+        return response.json()
 
     @property
     def _params(self) -> dict:
         """Default parameters for every request."""
         return {"lang": self.language_code}
 
     def get_language_code(self, default: str = "en") -> str:
@@ -65,45 +100,35 @@
         components: dict[str, CommonSchemes | None] = DEFAULT_COMPONENTS,
     ) -> None:
         """Download data and metadata to perform semantic search queries"""
         self.embedder = SentenceTransformer("all-MiniLM-L6-v2")
 
     def schemes(self) -> list:
         """Get all concept schemes, regardless of type"""
-        return requests.get(urljoin(self.base_url, "schemes"), params=self._params).json()[
-            "concept_schemes"
-        ]
+        return self._requests_get("schemes")["concept_schemes"]
 
     def concepts_for_scheme(self, scheme_iri: str | Enum) -> list:
         if isinstance(scheme_iri, Enum):
             scheme_iri = scheme_iri.value
         # TBD: Validate input arg
-        data = requests.get(
-            urljoin(self.base_url, "concepts"),
-            params=self._params | {"concept_scheme_iri": scheme_iri},
-        ).json()["concepts"]
+        data = self._requests_get("concepts", {"concept_scheme_iri": scheme_iri})["concepts"]
         if not data and scheme_iri not in {obj["iri"] for obj in self.schemes()}:
             raise KeyError(f"Given concept scheme IRI '{scheme_iri}' not present in glossary")
         return data
 
     def search(self, query: str) -> str:
         """Search the the whole concept library
 
         Args:
             query (str): the search query string
 
         Returns:
             list of results
         """
-        print(requests.get(
-            urljoin(self.base_url, "search"), params=self._params | {"search_term": query}
-        ).json())
-        return requests.get(
-            urljoin(self.base_url, "search"), params=self._params | {"search_term": query}
-        ).json()["concepts"]
+        return self._requests_get("search", {"search_term": query})["concepts"]
 
 
 # # Corpus with example sentences
 # corpus = [
 #     "A man is eating food.",
 #     "A man is eating a piece of bread.",
 #     "The girl is carrying a baby.",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sentier_glossary-0.1.0/sentier_glossary.egg-info/PKG-INFO` & `sentier_glossary-0.2.0/sentier_glossary.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentier_glossary
-Version: 0.1.0
+Version: 0.2.0
 Summary: Client interface to sentier.dev sustainability assessment glossary
 Author-email: João Gonçalves <jsvgoncalves@gmail.com>, Chris Mutel <cmutel@gmail.com>
 Maintainer-email: João Gonçalves <jsvgoncalves@gmail.com>, Chris Mutel <cmutel@gmail.com>
 Project-URL: source, https://github.com/Depart-de-Sentier/sentier_glossary
 Project-URL: homepage, https://github.com/Depart-de-Sentier/sentier_glossary
 Project-URL: tracker, https://github.com/Depart-de-Sentier/sentier_glossary/issues
 Classifier: Development Status :: 4 - Beta
```

