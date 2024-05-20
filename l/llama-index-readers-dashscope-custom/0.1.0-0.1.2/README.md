# Comparing `tmp/llama_index_readers_dashscope_custom-0.1.0.tar.gz` & `tmp/llama_index_readers_dashscope_custom-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_dashscope_custom-0.1.0.tar", max compression
+gzip compressed data, was "llama_index_readers_dashscope_custom-0.1.2.tar", max compression
```

## Comparing `llama_index_readers_dashscope_custom-0.1.0.tar` & `llama_index_readers_dashscope_custom-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,13 @@
--rw-r--r--   0        0        0     2177 2024-05-04 10:30:27.278670 llama_index_readers_dashscope_custom-0.1.0/README.md
--rw-r--r--   0        0        0      118 2024-05-04 09:51:00.252095 llama_index_readers_dashscope_custom-0.1.0/llama_index/readers/dashscope/__init__.py
--rw-r--r--   0        0        0    15199 2024-05-04 10:35:58.306766 llama_index_readers_dashscope_custom-0.1.0/llama_index/readers/dashscope/base.py
--rw-r--r--   0        0        0      113 2024-05-04 09:51:00.302352 llama_index_readers_dashscope_custom-0.1.0/llama_index/readers/dashscope/domain/base_domains.py
--rw-r--r--   0        0        0    10372 2024-05-04 10:39:20.482785 llama_index_readers_dashscope_custom-0.1.0/llama_index/readers/dashscope/domain/lease_domains.py
--rw-r--r--   0        0        0     5140 2024-05-04 10:41:18.894794 llama_index_readers_dashscope_custom-0.1.0/llama_index/readers/dashscope/utils.py
--rw-r--r--   0        0        0     1665 2024-05-08 05:43:43.768010 llama_index_readers_dashscope_custom-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2873 1970-01-01 00:00:00.000000 llama_index_readers_dashscope_custom-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2255 2024-05-10 12:30:42.022898 llama_index_readers_dashscope_custom-0.1.2/README.md
+-rw-r--r--   0        0        0      118 2024-04-28 01:35:31.434766 llama_index_readers_dashscope_custom-0.1.2/llama_index/readers/dashscope/__init__.py
+-rw-r--r--   0        0        0      346 2024-04-28 01:39:45.405826 llama_index_readers_dashscope_custom-0.1.2/llama_index/readers/dashscope/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    11809 2024-05-10 11:51:37.947843 llama_index_readers_dashscope_custom-0.1.2/llama_index/readers/dashscope/__pycache__/base.cpython-38.pyc
+-rw-r--r--   0        0        0     5197 2024-05-02 06:36:55.115398 llama_index_readers_dashscope_custom-0.1.2/llama_index/readers/dashscope/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0        0        0    15418 2024-05-10 11:51:34.400632 llama_index_readers_dashscope_custom-0.1.2/llama_index/readers/dashscope/base.py
+-rw-r--r--   0        0        0      593 2024-04-26 07:43:04.724789 llama_index_readers_dashscope_custom-0.1.2/llama_index/readers/dashscope/domain/__pycache__/base_domains.cpython-38.pyc
+-rw-r--r--   0        0        0     8945 2024-05-01 13:04:52.659556 llama_index_readers_dashscope_custom-0.1.2/llama_index/readers/dashscope/domain/__pycache__/lease_domains.cpython-38.pyc
+-rw-r--r--   0        0        0      113 2024-04-26 07:16:03.221786 llama_index_readers_dashscope_custom-0.1.2/llama_index/readers/dashscope/domain/base_domains.py
+-rw-r--r--   0        0        0    10453 2024-05-01 08:02:45.812805 llama_index_readers_dashscope_custom-0.1.2/llama_index/readers/dashscope/domain/lease_domains.py
+-rw-r--r--   0        0        0     4977 2024-05-02 05:57:05.710066 llama_index_readers_dashscope_custom-0.1.2/llama_index/readers/dashscope/utils.py
+-rw-r--r--   0        0        0     1647 2024-05-20 06:26:12.665787 llama_index_readers_dashscope_custom-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2951 1970-01-01 00:00:00.000000 llama_index_readers_dashscope_custom-0.1.2/PKG-INFO
```

### Comparing `llama_index_readers_dashscope_custom-0.1.0/README.md` & `llama_index_readers_dashscope_custom-0.1.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 # LlamaIndex Readers Integration: Dashscope
 
 ## Usage
 
-```python
+```
 from llama_index.readers.dashscope.base import DashScopeParse
 from llama_index.readers.dashscope.utils import ResultType
 
-file_list = [
-    # your files (accept doc, docx, pdf)
-]
+file_list = ['./aiayn.pdf', './aiayn.abc']
 
 parse = DashScopeParse(result_type=ResultType.DASHCOPE_DOCMIND)
 documents = parse.load_data(file_path=file_list)
 ```
 
 ## Reader Setting:
 
 A full list of retriever settings/kwargs is below:
 
 - api_key: Optional[str] -- Your dashscope API key, which can be passed in through environment variables or parameters.
   The parameter settings will override the results from the environment variables
 - workspace_id: Optional[str] -- Your dashscope workspace_id, which can be passed in through environment variables or
   parameters. The parameter settings will override the results from the environment variables
+- category_id: Optional[str] -- The category_id for the parser. The default value is "default".
 - base_url: Optional[str] -- The base url for the Dashscope API. The default value is "https://dashscope.aliyuncs.com".
   The parameter settings will override the results from the environment variables.
 - result_type: Optional[ResultType] -- The result type for the parser. The default value is ResultType.DASHCOPE_DOCMIND.
 - num_workers: Optional[int] -- The number of workers to use sending API requests for parsing. The default value is 4,
   greater than 0, less than 10.
-- check_interval: Optional[int] -- The interval in seconds to check if the parsing is done. The default value is 2.
-- max_timeout: Optional[int] -- The maximum timeout in seconds to wait for the parsing to finish. The default value is 20000.
+- check_interval: Optional[int] -- The interval in seconds to check if the parsing is done. The default value is 5.
+- max_timeout: Optional[int] -- The maximum timeout in seconds to wait for the parsing to finish. The default value is
+    3600.
 - verbose: Optional[bool] -- Whether to print the progress of the parsing. The default value is True.
 - show_progress: Optional[bool] -- Show progress when parsing multiple files. The default value is True.
 - ignore_errors: Optional[bool] -- Whether or not to ignore and skip errors raised during parsing. The default value is
   True.
 
 ## Reader Input:
 
 - file_path: Union[str, List[str]] -- The file path or list of file paths to parse.
 
 ## Reader Output:
 
 - List[llama_index.core.schema.Document] -- The list of documents parsed from the file.
-  - text: str -- The text of the document from DASHCOPE_DOCMIND.
+  - text: str -- The text of the document from DASHCOPE_DOCMIND.
```

### Comparing `llama_index_readers_dashscope_custom-0.1.0/llama_index/readers/dashscope/base.py` & `llama_index_readers_dashscope_custom-0.1.2/llama_index/readers/dashscope/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,48 @@
 import os
 import asyncio
 import httpx
 import time
 from pathlib import Path
 from tenacity import (
-    retry,
-    wait_exponential,
-    before_sleep_log,
-    after_log,
-    retry_if_exception_type,
-    stop_after_delay,
+    retry, wait_exponential, before_sleep_log, after_log, retry_if_exception_type, stop_after_delay
 )
 from typing import List, Optional, Union
 
 from llama_index.core.async_utils import run_jobs
 from llama_index.core.bridge.pydantic import Field, validator
 from llama_index.core.readers.base import BasePydanticReader
 from llama_index.core.schema import Document
 from llama_index.readers.dashscope.utils import *
 
 from llama_index.readers.dashscope.domain.lease_domains import (
-    DownloadFileLeaseResult,
-    UploadFileLeaseResult,
-    AddFileResult,
-    QueryFileResult,
-    DatahubDataStatusEnum,
-)
+    DownloadFileLeaseResult, UploadFileLeaseResult, AddFileResult, QueryFileResult, DatahubDataStatusEnum)
 
 DASHSCOPE_DEFAULT_BASE_URL = "https://dashscope.aliyuncs.com"
-DASHSCOPE_DEFAULT_DC_CATEGORY = os.getenv(
-    "DASHSCOPE_DEFAULT_DC_CATEGORY", default="default"
-)
+DASHSCOPE_DEFAULT_DC_CATEGORY = os.getenv("DASHSCOPE_DEFAULT_DC_CATEGORY", default="default")
 
 logger = get_stream_logger(name=__name__)
 
 
 class DashScopeParse(BasePydanticReader):
     """A smart-parser for files."""
 
     api_key: str = Field(default="", description="The API key for the DashScope API.")
-    workspace_id: str = Field(
-        default="",
-        description="The Workspace  for the DashScope API.If not set, "
-        "it will use the default workspace.",
-    )
+    workspace_id: str = Field(default="",
+                              description="The Workspace  for the DashScope API.If not set, "
+                                          "it will use the default workspace.")
+    category_id: str = Field(default=DASHSCOPE_DEFAULT_DC_CATEGORY,
+                             description="The dc category for the DashScope API.If not set, "
+                                         "it will use the default dc category.")
     base_url: str = Field(
         default=DASHSCOPE_DEFAULT_BASE_URL,
         description="The base URL of the DashScope Parsing API.",
     )
     result_type: ResultType = Field(
-        default=ResultType.DASHSCOPE_DOCMIND,
-        description="The result type for the parser.",
+        default=ResultType.DASHSCOPE_DOCMIND, description="The result type for the parser."
     )
     num_workers: int = Field(
         default=4,
         gt=0,
         lt=10,
         description="The number of workers to use sending API requests for parsing.",
     )
@@ -96,189 +84,166 @@
 
     @validator("workspace_id", pre=True, always=True)
     def validate_workspace_id(cls, v: str) -> str:
         """Validate the Workspace."""
         if not v:
             import os
 
-            return os.getenv("DASHSCOPE_WORKSPACE_ID", "")
+            workspace = os.getenv("DASHSCOPE_WORKSPACE_ID", "")
+            return workspace
+
+        return v
+
+    @validator("category_id", pre=True, always=True)
+    def validate_category_id(cls, v: str) -> str:
+        """Validate the category."""
+        if not v:
+            import os
+
+            category_id = os.getenv("DASHSCOPE_CATEGORY_ID", DASHSCOPE_DEFAULT_DC_CATEGORY)
+            return category_id
 
         return v
 
     @validator("base_url", pre=True, always=True)
     def validate_base_url(cls, v: str) -> str:
         """Validate the base URL."""
-        if v and v != DASHSCOPE_DEFAULT_BASE_URL:
+        if v and DASHSCOPE_DEFAULT_BASE_URL != v:
             return v
         else:
-            url = (
-                os.getenv("DASHSCOPE_BASE_URL", None)
-                or "https://dashscope.aliyuncs.com"
-            )
-            if url and not url.startswith(("http://", "https://")):
-                raise ValueError(
-                    "The DASHSCOPE_BASE_URL must start with http or https. "
-                )
+            url = os.getenv("DASHSCOPE_BASE_URL", None) or 'https://dashscope.aliyuncs.com'
+            if url and not (url.startswith("http://") or url.startswith("https://")):
+                raise ValueError("The DASHSCOPE_BASE_URL must start with http or https. ")
             return url or DASHSCOPE_DEFAULT_BASE_URL
 
     def _get_dashscope_header(self):
         return {
             "Authorization": f"Bearer {self.api_key}",
             "Content-Type": "application/json",
             "X-DashScope-WorkSpace": f"{self.workspace_id}",
-            "X-DashScope-OpenAPISource": "CloudSDK",
+            "X-DashScope-OpenAPISource": "CloudSDK"
         }
 
     # upload a document and get back a job_id
     async def _create_job(
-        self, file_path: str, extra_info: Optional[dict] = None
+            self, file_path: str, extra_info: Optional[dict] = None
     ) -> str:
         file_path = str(file_path)
         UploadFileLeaseResult.is_file_valid(file_path=file_path)
 
         headers = self._get_dashscope_header()
 
         # load data
         with open(file_path, "rb") as f:
             upload_file_lease_result = self.__upload_lease(file_path, headers)
 
             upload_file_lease_result.upload(file_path, f)
 
-            url = f"{self.base_url}/api/v1/datacenter/category/{DASHSCOPE_DEFAULT_DC_CATEGORY}/add_file"
+            url = f"{self.base_url}/api/v1/datacenter/category/{self.category_id}/add_file"
             async with httpx.AsyncClient(timeout=self.max_timeout) as client:
-                response = await client.post(
-                    url,
-                    headers=headers,
-                    json={
-                        "lease_id": upload_file_lease_result.lease_id,
-                        "parser": ResultType.DASHSCOPE_DOCMIND.value,
-                    },
-                )
-            add_file_result = dashscope_response_handler(
-                response, "add_file", AddFileResult, url=url
-            )
+                response = await client.post(url, headers=headers, json={
+                    "lease_id": upload_file_lease_result.lease_id,
+                    "parser": ResultType.DASHSCOPE_DOCMIND.value
+                })
+            add_file_result = dashscope_response_handler(response, "add_file", AddFileResult, url=url)
 
         return add_file_result.file_id
 
-    @retry(
-        stop=stop_after_delay(60),
-        wait=wait_exponential(multiplier=5, max=60),
-        before_sleep=before_sleep_log(logger, logging.INFO),
-        after=after_log(logger, logging.INFO),
-        reraise=True,
-        retry=retry_if_exception_type(RetryException),
-    )
+    @retry(stop=stop_after_delay(60), wait=wait_exponential(multiplier=5, max=60),
+           before_sleep=before_sleep_log(logger, logging.INFO), after=after_log(logger, logging.INFO), reraise=True,
+           retry=retry_if_exception_type(RetryException))
     def __upload_lease(self, file_path, headers):
-        url = f"{self.base_url}/api/v1/datacenter/category/{DASHSCOPE_DEFAULT_DC_CATEGORY}/upload_lease"
+        url = f"{self.base_url}/api/v1/datacenter/category/{self.category_id}/upload_lease"
         try:
             with httpx.Client(timeout=self.max_timeout) as client:
-                response = client.post(
-                    url,
-                    headers=headers,
-                    json={
-                        "file_name": os.path.basename(file_path),
-                        "size_bytes": os.path.getsize(file_path),
-                        "content_md5": get_file_md5(file_path),
-                    },
-                )
+                response = client.post(url, headers=headers, json={
+                    "file_name": os.path.basename(file_path),
+                    "size_bytes": os.path.getsize(file_path),
+                    "content_md5": get_file_md5(file_path)
+                })
         except httpx.ConnectTimeout:
             raise RetryException("Connect timeout")
         except httpx.ReadTimeout:
             raise RetryException("Read timeout")
         except httpx.NetworkError:
             raise RetryException("Network error")
 
-        upload_file_lease_result = dashscope_response_handler(
-            response, "upload_lease", UploadFileLeaseResult, url=url
-        )
-        logger.info(
-            f"{file_path} upload lease result: {upload_file_lease_result.lease_id}"
-        )
+        upload_file_lease_result = dashscope_response_handler(response, "upload_lease",
+                                                              UploadFileLeaseResult, url=url)
+        logger.info(f"{file_path} upload lease result: {upload_file_lease_result.lease_id}")
         return upload_file_lease_result
 
     async def _get_job_result(
-        self, data_id: str, result_type: str, verbose: bool = False
+            self, data_id: str, result_type: str, verbose: bool = False
     ) -> dict:
-        result_url = f"{self.base_url}/api/v1/datacenter/category/{DASHSCOPE_DEFAULT_DC_CATEGORY}/file/{data_id}/download_lease"
-        status_url = f"{self.base_url}/api/v1/datacenter/category/{DASHSCOPE_DEFAULT_DC_CATEGORY}/file/{data_id}/query"
+        result_url = f"{self.base_url}/api/v1/datacenter/category/{self.category_id}/file/{data_id}/download_lease"
+        status_url = f"{self.base_url}/api/v1/datacenter/category/{self.category_id}/file/{data_id}/query"
 
         headers = self._get_dashscope_header()
 
         start = time.time()
         tries = 0
         while True:
             await asyncio.sleep(1)
             tries += 1
-            query_file_result = await self._dashscope_query(
-                data_id, headers, status_url
-            )
+            query_file_result = await self._dashscope_query(data_id, headers, status_url)
 
             status = query_file_result.status
             if DatahubDataStatusEnum.PARSE_SUCCESS.value == status:
                 async with httpx.AsyncClient(timeout=self.max_timeout) as client:
-                    response = await client.post(
-                        result_url, headers=headers, json={"file_id": data_id}
-                    )
-                    down_file_lease_result = dashscope_response_handler(
-                        response,
-                        "download_lease",
-                        DownloadFileLeaseResult,
-                        url=result_url,
-                    )
+                    response = await client.post(result_url, headers=headers, json={
+                        "file_id": data_id
+                    })
+                    down_file_lease_result = dashscope_response_handler(response, "download_lease",
+                                                                        DownloadFileLeaseResult, url=result_url)
                     if self.parse_result:
                         return {
                             result_type: down_file_lease_result.download(escape=True),
-                            "job_id": data_id,
+                            "job_id": data_id
                         }
                     else:
-                        return {result_type: "{}", "job_id": data_id}
-            elif (
-                DatahubDataStatusEnum.PARSING.value == status
-                or DatahubDataStatusEnum.INIT.value == status
-            ):
+                        return {
+                            result_type: "{}",
+                            "job_id": data_id
+                        }
+            elif DatahubDataStatusEnum.PARSING.value == status or DatahubDataStatusEnum.INIT.value == status:
                 end = time.time()
                 if end - start > self.max_timeout:
                     raise Exception(f"Timeout while parsing the file: {data_id}")
                 if verbose and tries % 5 == 0:
                     print(".", end="", flush=True)
 
                 await asyncio.sleep(self.check_interval)
 
                 continue
             else:
                 raise Exception(
                     f"Failed to parse the file: {data_id}, status: {status}"
                 )
 
-    @retry(
-        stop=stop_after_delay(60),
-        wait=wait_exponential(multiplier=5, max=60),
-        before_sleep=before_sleep_log(logger, logging.INFO),
-        after=after_log(logger, logging.INFO),
-        reraise=True,
-        retry=retry_if_exception_type(RetryException),
-    )
+    @retry(stop=stop_after_delay(60), wait=wait_exponential(multiplier=5, max=60),
+           before_sleep=before_sleep_log(logger, logging.INFO), after=after_log(logger, logging.INFO), reraise=True,
+           retry=retry_if_exception_type(RetryException))
     async def _dashscope_query(self, data_id, headers, status_url):
         try:
             async with httpx.AsyncClient(timeout=self.max_timeout) as client:
-                response = await client.post(
-                    status_url, headers=headers, json={"file_id": data_id}
-                )
-                return dashscope_response_handler(
-                    response, "query", QueryFileResult, url=status_url
-                )
+                response = await client.post(status_url, headers=headers, json={
+                    "file_id": data_id
+                })
+                query_file_result = dashscope_response_handler(response, "query", QueryFileResult, url=status_url)
+                return query_file_result
         except httpx.ConnectTimeout:
             raise RetryException("Connect timeout")
         except httpx.ReadTimeout:
             raise RetryException("Read timeout")
         except httpx.NetworkError:
             raise RetryException("Network error")
 
     async def _aload_data(
-        self, file_path: str, extra_info: Optional[dict] = None, verbose: bool = False
+            self, file_path: str, extra_info: Optional[dict] = None, verbose: bool = False
     ) -> List[Document]:
         """Load data from the input path."""
         try:
             data_id = await self._create_job(file_path, extra_info=extra_info)
             logger.info(f"Started parsing the file [{file_path}] under [{data_id}]")
 
             result = await self._get_job_result(
@@ -287,25 +252,27 @@
 
             document = Document(
                 text=result[self.result_type.value],
                 metadata=extra_info or {},
             )
             document.id_ = data_id
 
-            return [document]
+            return [
+                document
+            ]
 
         except Exception as e:
-            logger.error(f"Error while parsing the file '{file_path}':{e!s}")
+            logger.error(f"Error while parsing the file '{file_path}':{str(e)}")
             if self.ignore_errors:
                 return []
             else:
-                raise
+                raise e
 
     async def aload_data(
-        self, file_path: Union[List[str], str], extra_info: Optional[dict] = None
+            self, file_path: Union[List[str], str], extra_info: Optional[dict] = None
     ) -> List[Document]:
         """Load data from the input path."""
         if isinstance(file_path, (str, Path)):
             return await self._aload_data(
                 file_path, extra_info=extra_info, verbose=self.verbose
             )
         elif isinstance(file_path, list):
@@ -327,58 +294,56 @@
 
                 # return flattened results
                 return [item for sublist in results for item in sublist]
             except RuntimeError as e:
                 if nest_asyncio_err in str(e):
                     raise RuntimeError(nest_asyncio_msg)
                 else:
-                    raise
+                    raise e
         else:
             raise ValueError(
                 "The input file_path must be a string or a list of strings."
             )
 
     def load_data(
-        self, file_path: Union[List[str], str], extra_info: Optional[dict] = None
+            self, file_path: Union[List[str], str], extra_info: Optional[dict] = None
     ) -> List[Document]:
         extra_info = {"parse_fmt_type": ResultType.DASHSCOPE_DOCMIND.value}
         """Load data from the input path."""
         try:
             return asyncio.run(self.aload_data(file_path, extra_info))
         except RuntimeError as e:
             if nest_asyncio_err in str(e):
                 raise RuntimeError(nest_asyncio_msg)
             else:
-                raise
+                raise e
 
     async def _aget_json(
-        self, file_path: str, extra_info: Optional[dict] = None
+            self, file_path: str, extra_info: Optional[dict] = None
     ) -> List[dict]:
         """Load data from the input path."""
         try:
             job_id = await self._create_job(file_path, extra_info=extra_info)
             if self.verbose:
                 logger.info("Started parsing the file under job_id %s" % job_id)
 
-            result = await self._get_job_result(
-                job_id, ResultType.DASHSCOPE_DOCMIND.value
-            )
+            result = await self._get_job_result(job_id, ResultType.DASHSCOPE_DOCMIND.value)
             result["job_id"] = job_id
             result["file_path"] = file_path
             return [result]
 
         except Exception as e:
             logger.info(f"Error while parsing the file '{file_path}':", e)
             if self.ignore_errors:
                 return []
             else:
-                raise
+                raise e
 
     async def aget_json(
-        self, file_path: Union[List[str], str], extra_info: Optional[dict] = None
+            self, file_path: Union[List[str], str], extra_info: Optional[dict] = None
     ) -> List[dict]:
         """Load data from the input path."""
         if isinstance(file_path, (str, Path)):
             return await self._aget_json(file_path, extra_info=extra_info)
         elif isinstance(file_path, list):
             jobs = [self._aget_json(f, extra_info=extra_info) for f in file_path]
             try:
@@ -391,28 +356,28 @@
 
                 # return flattened results
                 return [item for sublist in results for item in sublist]
             except RuntimeError as e:
                 if nest_asyncio_err in str(e):
                     raise RuntimeError(nest_asyncio_msg)
                 else:
-                    raise
+                    raise e
         else:
             raise ValueError(
                 "The input file_path must be a string or a list of strings."
             )
 
     def get_json_result(
-        self, file_path: Union[List[str], str], extra_info: Optional[dict] = None
+            self, file_path: Union[List[str], str], extra_info: Optional[dict] = None
     ) -> List[dict]:
         extra_info = {"parse_fmt_type": ResultType.DASHSCOPE_DOCMIND.value}
         """Parse the input path."""
         try:
             return asyncio.run(self.aget_json(file_path, extra_info))
         except RuntimeError as e:
             if nest_asyncio_err in str(e):
                 raise RuntimeError(nest_asyncio_msg)
             else:
-                raise
+                raise e
 
     def get_images(self, json_result: List[dict], download_path: str) -> List[dict]:
         raise NotImplementedError
```

### Comparing `llama_index_readers_dashscope_custom-0.1.0/llama_index/readers/dashscope/domain/lease_domains.py` & `llama_index_readers_dashscope_custom-0.1.2/llama_index/readers/dashscope/domain/lease_domains.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import json
 import requests
 from enum import Enum
 from llama_index.readers.dashscope.domain.base_domains import DictToObject
-from llama_index.readers.dashscope.utils import get_stream_logger
+from llama_index.readers.dashscope.utils import SUPPORTED_FILE_TYPES, get_stream_logger
 
 logger = get_stream_logger(name=__name__)
 
 
 class FileUploadMethod(Enum):
     OSS_PreSignedUrl = "OSS.PreSignedUrl"
 
@@ -15,95 +15,92 @@
     def from_value(cls, value):
         for member in cls:
             if member.value == value:
                 return member
         raise ValueError(f"No enum member found for value '{value}'")
 
 
-class UploadFileParameter:
+class UploadFileParameter(object):
     def upload(self, file_name: str, file: object):
         pass
 
 
 class OssPreSignedUrlParameter(UploadFileParameter, DictToObject):
     def __init__(self, url: str, method: str, headers: dict):
         self.url = url
         self.method = method
         self.headers = headers
 
     @classmethod
     def from_dict(cls, data: dict) -> "OssPreSignedUrlParameter":
-        if "method" not in data:
+        if "method" not in data.keys():
             raise ValueError("OssPreSignedUrlParameter method key is required")
-        if "headers" not in data:
+        if "headers" not in data.keys():
             raise ValueError("OssPreSignedUrlParameter headers key is required")
-        if "url" not in data:
+        if "url" not in data.keys():
             raise ValueError("OssPreSignedUrlParameter url key is required")
         else:
-            return OssPreSignedUrlParameter(
-                data["url"], data["method"], data["headers"]
-            )
+            return OssPreSignedUrlParameter(data["url"], data["method"], data["headers"])
 
     def upload(self, file_name: str, file: object):
         logger.info(f"Start upload {file_name}.")
         try:
-            if self.method == "PUT":
+            if "PUT" == self.method:
                 response = requests.put(self.url, data=file, headers=self.headers)
-            elif self.method == "POST":
+            elif "POST" == self.method:
                 response = requests.post(self.url, data=file, headers=self.headers)
             else:
                 raise Exception(f"Upload {file_name} unsupported method: {self.method}")
             if response.status_code != 200:
                 raise Exception(
-                    f"Upload {file_name} failed with status code: {response.status_code} \n {self.url} \n {self.headers} \n {response.text}"
-                )
+                    f"Upload {file_name} failed with status code: {response.status_code} \n {self.url} \n {self.headers} \n {response.text}")
             logger.info(f"Upload {file_name} success.")
         except requests.ConnectionError as ce:
             logger.info(f"Upload {file_name} Error connecting to {self.url}: {ce}")
             raise
         except requests.RequestException as e:
-            logger.info(
-                f"Upload {file_name} An error occurred while uploading to {self.url}: {e}"
-            )
+            logger.info(f"Upload {file_name} An error occurred while uploading to {self.url}: {e}")
             raise
         except Exception as e:
-            logger.info(
-                f"Upload {file_name} An error occurred while uploading to {self.url}: {e}"
-            )
+            logger.info(f"Upload {file_name} An error occurred while uploading to {self.url}: {e}")
             raise
 
 
 class UploadFileLeaseResult(DictToObject):
     def __init__(self, type: str, param: UploadFileParameter, lease_id: str):
         self.type: str = type
         self.param: UploadFileParameter = param
         self.lease_id: str = lease_id
 
     @classmethod
     def from_dict(cls, data: dict) -> "UploadFileLeaseResult":
-        if "lease_id" not in data:
+        if "lease_id" not in data.keys():
             raise ValueError("UploadFileLeaseResult lease_id key is required")
-        if "param" not in data:
+
+        if "param" not in data.keys():
             raise ValueError("UploadFileLeaseResult param key is required")
-        if "type" not in data:
+
+        if "type" not in data.keys():
             raise ValueError("UploadFileLeaseResult type key is required")
         else:
             if data["type"] == FileUploadMethod.OSS_PreSignedUrl.value:
                 return cls(
                     data["type"],
                     OssPreSignedUrlParameter.from_dict(data["param"]),
-                    data["lease_id"],
+                    data["lease_id"]
                 )
             else:
                 raise ValueError(f"Unsupported upload type: {data['type']}")
 
     @staticmethod
     def is_file_valid(file_path: str) -> None:
-        if file_path is None or file_path.strip() == "":
-            raise ValueError(f"file_path can't blank.")
+        if file_path is None or '' == file_path.strip():
+            raise ValueError(
+                f"file_path can't blank."
+            )
         file_path = str(file_path)
 
         # file_ext = os.path.splitext(file_path)[1]
         # if file_ext not in SUPPORTED_FILE_TYPES:
         #     raise ValueError(
         #         f"Currently, only the following file types are supported: {SUPPORTED_FILE_TYPES} "
         #         f"Current file type: {file_ext}"
@@ -122,34 +119,35 @@
 class AddFileResult(DictToObject):
     def __init__(self, file_id: str, parser: str):
         self.file_id = file_id
         self.parser = parser
 
     @classmethod
     def from_dict(cls, data: dict):
-        default_values = {"file_id": "", "parser": ""}
+        default_values = {
+            "file_id": "",
+            "parser": ""
+        }
 
         file_id = data.get("file_id", default_values["file_id"])
         parser = data.get("parser", default_values["parser"])
 
         return cls(file_id, parser)
 
 
 class QueryFileResult(DictToObject):
-    def __init__(
-        self,
-        file_id: str,
-        status: str,
-        file_name: str,
-        file_type: str,
-        parser: str,
-        size_bytes: int,
-        upload_time: str,
-        category: str,
-    ):
+    def __init__(self,
+                 file_id: str,
+                 status: str,
+                 file_name: str,
+                 file_type: str,
+                 parser: str,
+                 size_bytes: int,
+                 upload_time: str,
+                 category: str):
         self.file_id = file_id
         self.status = status
         self.file_name = file_name
         self.file_type = file_type
         self.parser = parser
         self.size_bytes = size_bytes
         self.upload_time = upload_time
@@ -170,26 +168,26 @@
             "file_id": "",
             "status": "",
             "file_name": "",
             "file_type": "",
             "parser": "",
             "size_bytes": 0,
             "upload_time": "",
-            "category": "",
+            "category": ""
         }
 
         return cls(
             file_id=data.get("file_id", default_values["file_id"]),
             status=data.get("status", default_values["status"]),
             file_name=data.get("file_name", default_values["file_name"]),
             file_type=data.get("file_type", default_values["file_type"]),
             parser=data.get("parser", default_values["parser"]),
             size_bytes=data.get("size_bytes", default_values["size_bytes"]),
             upload_time=data.get("upload_time", default_values["upload_time"]),
-            category=data.get("category", default_values["category"]),
+            category=data.get("category", default_values["category"])
         )
 
 
 class FileDownloadType(Enum):
     HTTP = "HTTP"
 
     @classmethod
@@ -197,15 +195,15 @@
         for member in cls:
             if member.value == value:
                 return member
         raise ValueError(f"No enum member found for value '{value}'")
 
 
 class HttpDownloadParameter(DictToObject):
-    def __init__(self, url, method, headers) -> None:
+    def __init__(self, url, method, headers):
         self.url = url
         self.method = method
         self.headers = headers
 
     @classmethod
     def from_dict(cls, data: dict):
         """
@@ -213,25 +211,29 @@
 
         Args:
             data (dict): A dictionary containing the necessary keys and values corresponding to the class attributes.
 
         Returns:
             QueryFileResult: An instance of `QueryFileResult` populated with data from the input dictionary.
         """
-        default_values = {"url": "", "method": "GET", "headers": {}}
+        default_values = {
+            "url": "",
+            "method": "GET",
+            "headers": {}
+        }
 
         return cls(
             url=data.get("url", default_values["url"]),
             method=data.get("method", default_values["method"]),
-            headers=data.get("headers", default_values["headers"]),
+            headers=data.get("headers", default_values["headers"])
         )
 
 
 class DownloadFileLeaseResult(DictToObject):
-    def __init__(self, file_id, lease_id, file_name, type, param) -> None:
+    def __init__(self, file_id, lease_id, file_name, type, param):
         self.file_id = file_id
         self.lease_id = lease_id
         self.file_name = file_name
         self.type = type
         self.param = param
 
     @classmethod
@@ -241,40 +243,38 @@
 
         Args:
             data (dict): A dictionary containing the necessary keys and values corresponding to the class attributes.
 
         Returns:
             QueryFileResult: An instance of `QueryFileResult` populated with data from the input dictionary.
         """
-        if "param" not in data:
+        if "param" not in data.keys():
             raise ValueError("download_lease result param is required")
 
         default_values = {
             "file_id": "",
             "lease_id": "",
             "file_name": "",
             "type": FileDownloadType.HTTP.value,
-            "param": HttpDownloadParameter.from_dict(data["param"]),
+            "param": HttpDownloadParameter.from_dict(data["param"])
         }
 
         return cls(
             file_id=data.get("file_id", default_values["file_id"]),
             lease_id=data.get("lease_id", default_values["lease_id"]),
             file_name=data.get("file_name", default_values["file_name"]),
             type=FileDownloadType.from_value(data.get("type", default_values["type"])),
-            param=default_values["param"],
+            param=default_values["param"]
         )
 
     def download(self, escape: bool = False):
-        if self.type == FileDownloadType.HTTP:
-            if self.param.method == "GET":
-                json_bytes = requests.get(
-                    url=self.param.url, headers=self.param.headers
-                ).content
-                json_str = json_bytes.decode("utf-8")
+        if FileDownloadType.HTTP == self.type:
+            if "GET" == self.param.method:
+                json_bytes = requests.get(url=self.param.url, headers=self.param.headers).content
+                json_str = json_bytes.decode('utf-8')
                 if escape:
                     return json.dumps(json_str, ensure_ascii=False)
                 else:
                     return json_str
             else:
                 raise ValueError(f"Invalid download method: {self.param.method}")
         else:
```

### Comparing `llama_index_readers_dashscope_custom-0.1.0/llama_index/readers/dashscope/utils.py` & `llama_index_readers_dashscope_custom-0.1.2/llama_index/readers/dashscope/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,36 +2,36 @@
 import logging
 
 from enum import Enum
 from httpx._models import Response
 from typing import Dict, Any, Type, TypeVar
 from llama_index.readers.dashscope.domain.base_domains import DictToObject
 
-T = TypeVar("T", bound=DictToObject)
+T = TypeVar('T', bound=DictToObject)
 
 # Asyncio error messages
 nest_asyncio_err = "cannot be called from a running event loop"
 nest_asyncio_msg = "The event loop is already running. Add `import nest_asyncio; nest_asyncio.apply()` to your code to fix this issue."
 
 
-def get_stream_logger(name="dashscope-parser", level=logging.INFO, format_string=None):
+def get_stream_logger(name='dashscope-parser', level=logging.INFO, format_string=None):
     if not format_string:
         format_string = "%(asctime)s %(name)s [%(levelname)s] %(thread)d : %(message)s"
     logger = logging.getLogger(name)
     logger.setLevel(level)
     formatter = logging.Formatter(format_string)
     fh = logging.StreamHandler()
     fh.setLevel(level)
     fh.setFormatter(formatter)
     logger.addHandler(fh)
     return logger
 
 
 def get_file_md5(file_path):
-    with open(file_path, "rb") as f:
+    with open(file_path, 'rb') as f:
         md5 = hashlib.md5()
         while chunk := f.read(8192):
             md5.update(chunk)
     return md5.hexdigest()
 
 
 def generate_request_id():
@@ -39,17 +39,15 @@
     import uuid
 
     return str(uuid.uuid4())
 
 
 def __is_response_successful(response_data: Dict[str, Any]) -> bool:
     """Check if the response data indicates a successful operation."""
-    return ("code" in response_data) and (
-        response_data["code"] == "Success" or response_data["code"] == "success"
-    )
+    return ("code" in response_data) and ("Success" == response_data["code"] or "success" == response_data["code"])
 
 
 def __raise_exception(response: Response, process: str) -> None:
     """Log the error and raise a specific exception based on the response."""
     error_message = f"Failed to {process}: {response.text}"
     raise ValueError(error_message)
 
@@ -58,27 +56,25 @@
     """
     Custom exception class to indicate a situation where an operation needs to be retried.
 
     This exception should be raised when an operation fails due to anticipated recoverable reasons,
     suggesting to the caller that a retry logic might be appropriate.
     """
 
-    def __init__(
-        self, message="Operation failed, requiring a retry", cause=None
-    ) -> None:
+    def __init__(self, message="Operation failed, requiring a retry", cause=None):
         """
         Initialize a RetryException instance.
 
         :param message: Detailed information about the exception, a string by default set as "Operation failed, requiring a retry"
         :param cause: The original exception object that caused this exception, optional
         """
         super().__init__(message)
         self.cause = cause
 
-    def __str__(self) -> str:
+    def __str__(self):
         """
         Return a string representation of the exception, including the original exception information if present.
 
         :return: String representation of the exception details
         """
         if self.cause:
             return f"{super().__str__()} caused by: {self.cause}"
@@ -91,61 +87,51 @@
     error_message = f"Failed to {process}: {response.text}"
     raise RetryException(cause=error_message)
 
 
 logger = get_stream_logger(name="DashScopeResponseHandler")
 
 
-def dashscope_response_handler(
-    response: Response, process: str, result_class: Type[T], url: str = ""
-) -> T:
+def dashscope_response_handler(response: Response, process: str, result_class: Type[T], url: str = "") -> T:
     """Handle the response from the DashScope API."""
     if response is None:
-        raise ValueError(
-            f"DashScopeParse {process} [URL:{url}] http response object is none."
-        )
+        raise ValueError(f"DashScopeParse {process} [URL:{url}] http response object is none.")
 
     if not isinstance(process, str) or not process:
-        raise ValueError(
-            "DashScopeParse func [dashscope_response_handler] process parameter is empty."
-        )
+        raise ValueError("DashScopeParse func [dashscope_response_handler] process parameter is empty.")
 
     if response.status_code != 200:
         logger.error(
-            f"DashScopeParse {process} [URL:{url}] response http status code is not 200: [{response.status_code}:{response.text}]"
-        )
-        if response.status_code == 429:
+            f"DashScopeParse {process} [URL:{url}] response http status code is not 200: [{response.status_code}:{response.text}]")
+        if 429 == response.status_code:
             __raise_exception_for_retry(response, process)
         __raise_exception(response, process)
     try:
         response_data = response.json()
     except Exception as e:
-        logger.error(
-            f"DashScopeParse {process} [URL:{url}] response data is not json: {response.text}."
-        )
+        logger.error(f"DashScopeParse {process} [URL:{url}] response data is not json: {response.text}.")
         __raise_exception(response, process)
 
     if not __is_response_successful(response_data):
-        logger.error(
-            f"DashScopeParse {process} [URL:{url}] response fail: {response.text}."
-        )
+        logger.error(f"DashScopeParse {process} [URL:{url}] response fail: {response.text}.")
         __raise_exception(response, process)
 
-    if "data" not in response_data:
+    if 'data' not in response_data:
         logger.error(
-            f"DashScopeParse {process} [URL:{url}] response data does not contain 'data' key: {response_data}."
-        )
+            f"DashScopeParse {process} [URL:{url}] response data does not contain 'data' key: {response_data}.")
         __raise_exception(response, process)
-    if "request_id" in response_data and process != "query":
-        logger.info(
-            f"DashScopeParse {process} [URL:{url}] request_id: {response_data['request_id']}."
-        )
-    return result_class.from_dict(response_data["data"])
+    if "request_id" in response_data and "query" != process:
+        logger.info(f"DashScopeParse {process} [URL:{url}] request_id: {response_data['request_id']}.")
+    return result_class.from_dict(response_data['data'])
 
 
 class ResultType(Enum):
     """The result type for the parser."""
 
     DASHSCOPE_DOCMIND = "DASHSCOPE_DOCMIND"
 
 
-SUPPORTED_FILE_TYPES = [".pdf", ".doc", ".docx"]
+SUPPORTED_FILE_TYPES = [
+    ".pdf",
+    ".doc",
+    ".docx"
+]
```

### Comparing `llama_index_readers_dashscope_custom-0.1.0/pyproject.toml` & `llama_index_readers_dashscope_custom-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 [build-system]
-build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
 
 [tool.codespell]
 check-filenames = true
 check-hidden = true
 # Feel free to un-skip examples, and experimental, you will just need to
 # work through many typos (--write-changes and --interactive will help)
 skip = "*.csv,*.html,*.json,*.jsonl,*.pdf,*.txt,*.ipynb"
 
-[tool.llamahub]
-contains_example = false
-import_path = "llama_index.readers.dashscope.base"
+# [tool.llamahub]
+# contains_example = false
+# import_path = "<import-path>"
 
-[tool.llamahub.class_authors]
-DashScopeEmbedding = "phantomgrapes"
+# [tool.llamahub.class_authors]
+# CLASS = "github-username"
 
 [tool.mypy]
 disallow_untyped_defs = true
 # Remove venv skip when integrated with pre-commit
 exclude = ["_static", "build", "examples", "notebooks", "venv"]
 ignore_missing_imports = true
 python_version = "3.8"
 
 [tool.poetry]
-authors = ["Your Name <you@example.com>"]
+name = "llama-index-readers-dashscope-custom"
+version = "0.1.2"
 description = "llama-index readers dashscope integration"
+authors = ["Your Name <you@example.com>"]
 license = "MIT"
-name = "llama-index-readers-dashscope-custom"
-packages = [{include = "llama_index/"}]
 readme = "README.md"
-version = "0.1.0"
+packages = [{ include = "llama_index/" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.0"
-oss2 = "^2.18.4"
+oss2 = "^2.18.5"
 retrying = "^1.3.4"
 
 [tool.poetry.group.dev.dependencies]
-black = {extras = ["jupyter"], version = "<=23.9.1,>=23.7.0"}
-codespell = {extras = ["toml"], version = ">=v2.2.6"}
-flask = "3.0.3"
+black = { extras = ["jupyter"], version = "<=23.9.1,>=23.7.0" }
+codespell = { extras = ["toml"], version = ">=v2.2.6" }
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
 pytest = "7.2.1"
 pytest-mock = "3.11.1"
-reportlab = "4.2.0"
 ruff = "0.0.292"
 tree-sitter-languages = "^1.8.0"
 types-Deprecated = ">=0.1.0"
 types-PyYAML = "^6.0.12.12"
 types-protobuf = "^4.24.0.4"
 types-redis = "4.5.5.0"
-types-requests = "2.28.11.8"  # TODO: unpin when mypy>0.991
+types-requests = "2.28.11.8" # TODO: unpin when mypy>0.991
 types-setuptools = "67.1.0.0"
+flask = "3.0.3"
+reportlab = "4.2.0"
```

### Comparing `llama_index_readers_dashscope_custom-0.1.0/PKG-INFO` & `llama_index_readers_dashscope_custom-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,64 +1,63 @@
 Metadata-Version: 2.1
 Name: llama-index-readers-dashscope-custom
-Version: 0.1.0
+Version: 0.1.2
 Summary: llama-index readers dashscope integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: llama-index-core (>=0.10.0,<0.11.0)
-Requires-Dist: oss2 (>=2.18.4,<3.0.0)
+Requires-Dist: oss2 (>=2.18.5,<3.0.0)
 Requires-Dist: retrying (>=1.3.4,<2.0.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Readers Integration: Dashscope
 
 ## Usage
 
-```python
+```
 from llama_index.readers.dashscope.base import DashScopeParse
 from llama_index.readers.dashscope.utils import ResultType
 
-file_list = [
-    # your files (accept doc, docx, pdf)
-]
+file_list = ['./aiayn.pdf', './aiayn.abc']
 
 parse = DashScopeParse(result_type=ResultType.DASHCOPE_DOCMIND)
 documents = parse.load_data(file_path=file_list)
 ```
 
 ## Reader Setting:
 
 A full list of retriever settings/kwargs is below:
 
 - api_key: Optional[str] -- Your dashscope API key, which can be passed in through environment variables or parameters.
   The parameter settings will override the results from the environment variables
 - workspace_id: Optional[str] -- Your dashscope workspace_id, which can be passed in through environment variables or
   parameters. The parameter settings will override the results from the environment variables
+- category_id: Optional[str] -- The category_id for the parser. The default value is "default".
 - base_url: Optional[str] -- The base url for the Dashscope API. The default value is "https://dashscope.aliyuncs.com".
   The parameter settings will override the results from the environment variables.
 - result_type: Optional[ResultType] -- The result type for the parser. The default value is ResultType.DASHCOPE_DOCMIND.
 - num_workers: Optional[int] -- The number of workers to use sending API requests for parsing. The default value is 4,
   greater than 0, less than 10.
-- check_interval: Optional[int] -- The interval in seconds to check if the parsing is done. The default value is 2.
-- max_timeout: Optional[int] -- The maximum timeout in seconds to wait for the parsing to finish. The default value is 20000.
+- check_interval: Optional[int] -- The interval in seconds to check if the parsing is done. The default value is 5.
+- max_timeout: Optional[int] -- The maximum timeout in seconds to wait for the parsing to finish. The default value is
+    3600.
 - verbose: Optional[bool] -- Whether to print the progress of the parsing. The default value is True.
 - show_progress: Optional[bool] -- Show progress when parsing multiple files. The default value is True.
 - ignore_errors: Optional[bool] -- Whether or not to ignore and skip errors raised during parsing. The default value is
   True.
 
 ## Reader Input:
 
 - file_path: Union[str, List[str]] -- The file path or list of file paths to parse.
 
 ## Reader Output:
 
 - List[llama_index.core.schema.Document] -- The list of documents parsed from the file.
   - text: str -- The text of the document from DASHCOPE_DOCMIND.
-
```

