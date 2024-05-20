# Comparing `tmp/llama_index_readers_sec_filings-0.1.3.tar.gz` & `tmp/llama_index_readers_sec_filings-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_sec_filings-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_readers_sec_filings-0.1.4.tar", max compression
```

## Comparing `llama_index_readers_sec_filings-0.1.3.tar` & `llama_index_readers_sec_filings-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3533 2024-02-13 13:53:01.868462 llama_index_readers_sec_filings-0.1.3/README.md
--rw-r--r--   0        0        0       98 2024-02-13 13:53:01.868651 llama_index_readers_sec_filings-0.1.3/llama_index/readers/sec_filings/__init__.py
--rw-r--r--   0        0        0     3760 2024-02-13 13:53:01.868708 llama_index_readers_sec_filings-0.1.3/llama_index/readers/sec_filings/base.py
--rw-r--r--   0        0        0        0 2024-02-13 13:53:01.868808 llama_index_readers_sec_filings-0.1.3/llama_index/readers/sec_filings/prepline_sec_filings/__init__.py
--rw-r--r--   0        0        0        0 2024-02-13 13:53:01.868917 llama_index_readers_sec_filings-0.1.3/llama_index/readers/sec_filings/prepline_sec_filings/api/__init__.py
--rw-r--r--   0        0        0     1384 2024-02-13 13:53:01.868986 llama_index_readers_sec_filings-0.1.3/llama_index/readers/sec_filings/prepline_sec_filings/api/app.py
--rw-r--r--   0        0        0    14201 2024-02-13 13:53:01.869229 llama_index_readers_sec_filings-0.1.3/llama_index/readers/sec_filings/prepline_sec_filings/api/section.py
--rw-r--r--   0        0        0     8717 2024-02-20 18:45:10.313599 llama_index_readers_sec_filings-0.1.3/llama_index/readers/sec_filings/prepline_sec_filings/fetch.py
--rw-r--r--   0        0        0    18812 2024-02-20 18:45:10.313777 llama_index_readers_sec_filings-0.1.3/llama_index/readers/sec_filings/prepline_sec_filings/sec_document.py
--rw-r--r--   0        0        0     6323 2024-02-13 13:53:01.869489 llama_index_readers_sec_filings-0.1.3/llama_index/readers/sec_filings/prepline_sec_filings/sections.py
--rw-r--r--   0        0        0    11025 2024-02-20 18:45:10.313997 llama_index_readers_sec_filings-0.1.3/llama_index/readers/sec_filings/sec_filings.py
--rw-r--r--   0        0        0     6607 2024-02-13 13:53:01.869653 llama_index_readers_sec_filings-0.1.3/llama_index/readers/sec_filings/utils.py
--rw-r--r--   0        0        0     1537 2024-02-21 20:48:40.316855 llama_index_readers_sec_filings-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4210 1970-01-01 00:00:00.000000 llama_index_readers_sec_filings-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     3537 2024-05-20 02:26:38.103739 llama_index_readers_sec_filings-0.1.4/README.md
+-rw-r--r--   0        0        0       98 2024-05-20 02:26:38.103739 llama_index_readers_sec_filings-0.1.4/llama_index/readers/sec_filings/__init__.py
+-rw-r--r--   0        0        0     3760 2024-05-20 02:26:38.103739 llama_index_readers_sec_filings-0.1.4/llama_index/readers/sec_filings/base.py
+-rw-r--r--   0        0        0        0 2024-05-20 02:26:38.103739 llama_index_readers_sec_filings-0.1.4/llama_index/readers/sec_filings/prepline_sec_filings/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 02:26:38.107740 llama_index_readers_sec_filings-0.1.4/llama_index/readers/sec_filings/prepline_sec_filings/api/__init__.py
+-rw-r--r--   0        0        0     1384 2024-05-20 02:26:38.107740 llama_index_readers_sec_filings-0.1.4/llama_index/readers/sec_filings/prepline_sec_filings/api/app.py
+-rw-r--r--   0        0        0    14201 2024-05-20 02:26:38.107740 llama_index_readers_sec_filings-0.1.4/llama_index/readers/sec_filings/prepline_sec_filings/api/section.py
+-rw-r--r--   0        0        0     8717 2024-05-20 02:26:38.107740 llama_index_readers_sec_filings-0.1.4/llama_index/readers/sec_filings/prepline_sec_filings/fetch.py
+-rw-r--r--   0        0        0    18812 2024-05-20 02:26:38.107740 llama_index_readers_sec_filings-0.1.4/llama_index/readers/sec_filings/prepline_sec_filings/sec_document.py
+-rw-r--r--   0        0        0     6323 2024-05-20 02:26:38.107740 llama_index_readers_sec_filings-0.1.4/llama_index/readers/sec_filings/prepline_sec_filings/sections.py
+-rw-r--r--   0        0        0    11065 2024-05-20 02:26:38.107740 llama_index_readers_sec_filings-0.1.4/llama_index/readers/sec_filings/sec_filings.py
+-rw-r--r--   0        0        0     6607 2024-05-20 02:26:38.107740 llama_index_readers_sec_filings-0.1.4/llama_index/readers/sec_filings/utils.py
+-rw-r--r--   0        0        0     1537 2024-05-20 02:26:38.107740 llama_index_readers_sec_filings-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4163 1970-01-01 00:00:00.000000 llama_index_readers_sec_filings-0.1.4/PKG-INFO
```

### Comparing `llama_index_readers_sec_filings-0.1.3/README.md` & `llama_index_readers_sec_filings-0.1.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # SEC DATA DOWNLOADER
 
+```bash
+pip install llama-index-readers-sec-filings
+```
+
 Please checkout this repo that I am building on SEC Question Answering Agent [SEC-QA](https://github.com/Athe-kunal/SEC-QA-Agent)
 
 This repository downloads all the texts from SEC documents (10-K and 10-Q). Currently, it is not supporting documents that are amended, but that will be added in the near futures.
 
 Install the required dependencies
 
 ```
@@ -17,17 +21,15 @@
 - filing_type: 10-K or 10-Q filing type
 - num_workers: It is for multithreading and multiprocessing. We have multi-threading at the ticker level and multi-processing at the year level for a given ticker
 - include_amends: To include amendments or not.
 
 ## Usage
 
 ```python
-from llama_index import download_loader
-
-SECFilingsLoader = download_loader("SECFilingsLoader")
+from llama_index.readers.sec_filings import SECFilingsLoader
 
 loader = SECFilingsLoader(tickers=["TSLA"], amount=3, filing_type="10-K")
 loader.load_data()
 ```
 
 It will download the data in the following directories and sub-directories
 
@@ -91,37 +93,36 @@
 ## EXAMPLES
 
 This loader is can be used with both Langchain and LlamaIndex.
 
 ### LlamaIndex
 
 ```python
-from llama_index import VectorStoreIndex, download_loader
-from llama_index import SimpleDirectoryReader
+from llama_index.core import VectorStoreIndex, download_loader
+from llama_index.core import SimpleDirectoryReader
 
-SECFilingsLoader = download_loader("SECFilingsLoader")
+from llama_index.readers.sec_filings import SECFilingsLoader
 
 loader = SECFilingsLoader(tickers=["TSLA"], amount=3, filing_type="10-K")
 loader.load_data()
 
 documents = SimpleDirectoryReader("data\TSLA\2022").load_data()
 index = VectorStoreIndex.from_documents(documents)
 index.query("What are the risk factors of Tesla for the year 2022?")
 ```
 
 ### Langchain
 
 ```python
-from llama_index import download_loader
 from langchain.llms import OpenAI
 from langchain.chains import RetrievalQA
 from langchain.document_loaders import DirectoryLoader
 from langchain.indexes import VectorstoreIndexCreator
 
-SECFilingsLoader = download_loader("SECFilingsLoader")
+from llama_index.readers.sec_filings import SECFilingsLoader
 
 loader = SECFilingsLoader(tickers=["TSLA"], amount=3, filing_type="10-K")
 loader.load_data()
 
 dir_loader = DirectoryLoader("data\TSLA\2022")
 
 index = VectorstoreIndexCreator().from_loaders([dir_loader])
```

### Comparing `llama_index_readers_sec_filings-0.1.3/llama_index/readers/sec_filings/base.py` & `llama_index_readers_sec_filings-0.1.4/llama_index/readers/sec_filings/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_sec_filings-0.1.3/llama_index/readers/sec_filings/prepline_sec_filings/api/app.py` & `llama_index_readers_sec_filings-0.1.4/llama_index/readers/sec_filings/prepline_sec_filings/api/app.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_sec_filings-0.1.3/llama_index/readers/sec_filings/prepline_sec_filings/api/section.py` & `llama_index_readers_sec_filings-0.1.4/llama_index/readers/sec_filings/prepline_sec_filings/api/section.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_sec_filings-0.1.3/llama_index/readers/sec_filings/prepline_sec_filings/fetch.py` & `llama_index_readers_sec_filings-0.1.4/llama_index/readers/sec_filings/prepline_sec_filings/fetch.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_sec_filings-0.1.3/llama_index/readers/sec_filings/prepline_sec_filings/sec_document.py` & `llama_index_readers_sec_filings-0.1.4/llama_index/readers/sec_filings/prepline_sec_filings/sec_document.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_sec_filings-0.1.3/llama_index/readers/sec_filings/prepline_sec_filings/sections.py` & `llama_index_readers_sec_filings-0.1.4/llama_index/readers/sec_filings/prepline_sec_filings/sections.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_sec_filings-0.1.3/llama_index/readers/sec_filings/sec_filings.py` & `llama_index_readers_sec_filings-0.1.4/llama_index/readers/sec_filings/sec_filings.py`

 * *Files 0% similar despite different names*

```diff
@@ -328,10 +328,11 @@
         assert company
         assert email
         session = requests.Session()
         session.headers.update(
             {
                 "User-Agent": f"{company} {email}",
                 "Content-Type": "text/html",
+                "Host": "www.sec.gov",
             }
         )
         return session
```

### Comparing `llama_index_readers_sec_filings-0.1.3/llama_index/readers/sec_filings/utils.py` & `llama_index_readers_sec_filings-0.1.4/llama_index/readers/sec_filings/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_sec_filings-0.1.3/pyproject.toml` & `llama_index_readers_sec_filings-0.1.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 description = "llama-index readers sec_filings integration"
 exclude = ["**/BUILD"]
 keywords = ["10-K", "10-Q", "SEC Filings", "finance"]
 license = "MIT"
 maintainers = ["Athe-kunal"]
 name = "llama-index-readers-sec-filings"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
```

### Comparing `llama_index_readers_sec_filings-0.1.3/PKG-INFO` & `llama_index_readers_sec_filings-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: llama-index-readers-sec-filings
-Version: 0.1.3
+Version: 0.1.4
 Summary: llama-index readers sec_filings integration
 License: MIT
 Keywords: 10-K,10-Q,SEC Filings,finance
 Author: Your Name
 Author-email: you@example.com
 Maintainer: Athe-kunal
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Description-Content-Type: text/markdown
 
 # SEC DATA DOWNLOADER
 
+```bash
+pip install llama-index-readers-sec-filings
+```
+
 Please checkout this repo that I am building on SEC Question Answering Agent [SEC-QA](https://github.com/Athe-kunal/SEC-QA-Agent)
 
 This repository downloads all the texts from SEC documents (10-K and 10-Q). Currently, it is not supporting documents that are amended, but that will be added in the near futures.
 
 Install the required dependencies
 
 ```
@@ -36,17 +39,15 @@
 - filing_type: 10-K or 10-Q filing type
 - num_workers: It is for multithreading and multiprocessing. We have multi-threading at the ticker level and multi-processing at the year level for a given ticker
 - include_amends: To include amendments or not.
 
 ## Usage
 
 ```python
-from llama_index import download_loader
-
-SECFilingsLoader = download_loader("SECFilingsLoader")
+from llama_index.readers.sec_filings import SECFilingsLoader
 
 loader = SECFilingsLoader(tickers=["TSLA"], amount=3, filing_type="10-K")
 loader.load_data()
 ```
 
 It will download the data in the following directories and sub-directories
 
@@ -110,37 +111,36 @@
 ## EXAMPLES
 
 This loader is can be used with both Langchain and LlamaIndex.
 
 ### LlamaIndex
 
 ```python
-from llama_index import VectorStoreIndex, download_loader
-from llama_index import SimpleDirectoryReader
+from llama_index.core import VectorStoreIndex, download_loader
+from llama_index.core import SimpleDirectoryReader
 
-SECFilingsLoader = download_loader("SECFilingsLoader")
+from llama_index.readers.sec_filings import SECFilingsLoader
 
 loader = SECFilingsLoader(tickers=["TSLA"], amount=3, filing_type="10-K")
 loader.load_data()
 
 documents = SimpleDirectoryReader("data\TSLA\2022").load_data()
 index = VectorStoreIndex.from_documents(documents)
 index.query("What are the risk factors of Tesla for the year 2022?")
 ```
 
 ### Langchain
 
 ```python
-from llama_index import download_loader
 from langchain.llms import OpenAI
 from langchain.chains import RetrievalQA
 from langchain.document_loaders import DirectoryLoader
 from langchain.indexes import VectorstoreIndexCreator
 
-SECFilingsLoader = download_loader("SECFilingsLoader")
+from llama_index.readers.sec_filings import SECFilingsLoader
 
 loader = SECFilingsLoader(tickers=["TSLA"], amount=3, filing_type="10-K")
 loader.load_data()
 
 dir_loader = DirectoryLoader("data\TSLA\2022")
 
 index = VectorstoreIndexCreator().from_loaders([dir_loader])
```

