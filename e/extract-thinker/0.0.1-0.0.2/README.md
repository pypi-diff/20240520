# Comparing `tmp/extract_thinker-0.0.1.tar.gz` & `tmp/extract_thinker-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extract_thinker-0.0.1.tar", max compression
+gzip compressed data, was "extract_thinker-0.0.2.tar", max compression
```

## Comparing `extract_thinker-0.0.1.tar` & `extract_thinker-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,29 @@
--rw-r--r--   0        0        0      718 2024-05-14 10:18:46.906985 extract_thinker-0.0.1/extract_thinker/__init__.py
--rw-r--r--   0        0        0     2434 2024-05-14 10:46:55.894659 extract_thinker-0.0.1/extract_thinker/app.py
--rw-r--r--   0        0        0      377 2024-04-26 13:59:04.968309 extract_thinker-0.0.1/extract_thinker/document_loader/azure_form_recognizer_loader.py
--rw-r--r--   0        0        0      665 2024-04-30 13:13:19.923447 extract_thinker-0.0.1/extract_thinker/document_loader/cached_document_loader.py
--rw-r--r--   0        0        0      331 2024-04-26 13:59:02.293295 extract_thinker-0.0.1/extract_thinker/document_loader/doctr_loader.py
--rw-r--r--   0        0        0     4220 2024-05-07 15:55:35.728302 extract_thinker-0.0.1/extract_thinker/document_loader/document_loader.py
--rw-r--r--   0        0        0     3880 2024-05-14 10:56:49.373743 extract_thinker-0.0.1/extract_thinker/document_loader/document_loader_tesseract.py
--rw-r--r--   0        0        0      167 2024-04-29 14:18:11.677749 extract_thinker-0.0.1/extract_thinker/document_loader/llm_interceptor.py
--rw-r--r--   0        0        0      185 2024-04-29 14:18:16.411423 extract_thinker-0.0.1/extract_thinker/document_loader/loader_interceptor.py
--rw-r--r--   0        0        0      349 2024-04-26 13:59:29.461620 extract_thinker-0.0.1/extract_thinker/document_loader/text_extract_loader.py
--rw-r--r--   0        0        0     8256 2024-05-14 10:57:22.725354 extract_thinker-0.0.1/extract_thinker/extractor.py
--rw-r--r--   0        0        0     3208 2024-05-14 10:23:22.251477 extract_thinker-0.0.1/extract_thinker/image_splitter.py
--rw-r--r--   0        0        0      638 2024-05-09 17:02:38.377337 extract_thinker-0.0.1/extract_thinker/llm.py
--rw-r--r--   0        0        0      262 2024-05-10 10:44:16.996625 extract_thinker-0.0.1/extract_thinker/models/classification.py
--rw-r--r--   0        0        0      154 2024-05-10 09:41:25.611114 extract_thinker-0.0.1/extract_thinker/models/classification_response.py
--rw-r--r--   0        0        0       74 2024-05-10 09:41:21.888560 extract_thinker-0.0.1/extract_thinker/models/contract.py
--rw-r--r--   0        0        0      275 2024-05-13 12:38:21.612076 extract_thinker-0.0.1/extract_thinker/models/doc_group.py
--rw-r--r--   0        0        0      177 2024-05-10 11:59:29.851609 extract_thinker-0.0.1/extract_thinker/models/doc_groups.py
--rw-r--r--   0        0        0      396 2024-05-10 14:49:55.747887 extract_thinker-0.0.1/extract_thinker/models/doc_groups2.py
--rw-r--r--   0        0        0     8759 2024-05-14 10:57:04.716256 extract_thinker-0.0.1/extract_thinker/process.py
--rw-r--r--   0        0        0     1446 2024-05-13 12:17:03.224421 extract_thinker-0.0.1/extract_thinker/splitter.py
--rw-r--r--   0        0        0     1708 2024-04-24 22:59:58.384108 extract_thinker-0.0.1/extract_thinker/text_splitter.py
--rw-r--r--   0        0        0     2554 2024-05-14 10:49:29.665042 extract_thinker-0.0.1/extract_thinker/utils.py
--rw-r--r--   0        0        0    11558 2024-02-02 12:09:16.119169 extract_thinker-0.0.1/LICENSE
--rw-r--r--   0        0        0      753 2024-05-13 14:01:16.417041 extract_thinker-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2642 2024-04-03 17:06:52.613249 extract_thinker-0.0.1/README.md
--rw-r--r--   0        0        0     3602 1970-01-01 00:00:00.000000 extract_thinker-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-20 11:34:05.110381 extract_thinker-0.0.2/LICENSE
+-rw-r--r--   0        0        0     4927 2024-05-20 11:34:05.110381 extract_thinker-0.0.2/README.md
+-rw-r--r--   0        0        0      929 2024-05-20 11:34:05.110381 extract_thinker-0.0.2/extract_thinker/__init__.py
+-rw-r--r--   0        0        0     2367 2024-05-20 11:34:05.110381 extract_thinker-0.0.2/extract_thinker/app.py
+-rw-r--r--   0        0        0      366 2024-05-20 11:34:05.110381 extract_thinker-0.0.2/extract_thinker/document_loader/azure_form_recognizer_loader.py
+-rw-r--r--   0        0        0      646 2024-05-20 11:34:05.110381 extract_thinker-0.0.2/extract_thinker/document_loader/cached_document_loader.py
+-rw-r--r--   0        0        0      320 2024-05-20 11:34:05.110381 extract_thinker-0.0.2/extract_thinker/document_loader/doctr_loader.py
+-rw-r--r--   0        0        0     4107 2024-05-20 11:34:05.110381 extract_thinker-0.0.2/extract_thinker/document_loader/document_loader.py
+-rw-r--r--   0        0        0     1270 2024-05-20 11:34:05.110381 extract_thinker-0.0.2/extract_thinker/document_loader/document_loader_spreadsheet.py
+-rw-r--r--   0        0        0     3794 2024-05-20 11:34:05.110381 extract_thinker-0.0.2/extract_thinker/document_loader/document_loader_tesseract.py
+-rw-r--r--   0        0        0      918 2024-05-20 11:34:05.110381 extract_thinker-0.0.2/extract_thinker/document_loader/document_loader_text.py
+-rw-r--r--   0        0        0      160 2024-05-20 11:34:05.114381 extract_thinker-0.0.2/extract_thinker/document_loader/llm_interceptor.py
+-rw-r--r--   0        0        0      178 2024-05-20 11:34:05.114381 extract_thinker-0.0.2/extract_thinker/document_loader/loader_interceptor.py
+-rw-r--r--   0        0        0      338 2024-05-20 11:34:05.114381 extract_thinker-0.0.2/extract_thinker/document_loader/text_extract_loader.py
+-rw-r--r--   0        0        0     8820 2024-05-20 11:34:05.114381 extract_thinker-0.0.2/extract_thinker/extractor.py
+-rw-r--r--   0        0        0     3130 2024-05-20 11:34:05.114381 extract_thinker-0.0.2/extract_thinker/image_splitter.py
+-rw-r--r--   0        0        0      617 2024-05-20 11:34:05.114381 extract_thinker-0.0.2/extract_thinker/llm.py
+-rw-r--r--   0        0        0      263 2024-05-20 11:34:05.114381 extract_thinker-0.0.2/extract_thinker/models/classification.py
+-rw-r--r--   0        0        0      146 2024-05-20 11:34:05.114381 extract_thinker-0.0.2/extract_thinker/models/classification_response.py
+-rw-r--r--   0        0        0       69 2024-05-20 11:34:05.114381 extract_thinker-0.0.2/extract_thinker/models/contract.py
+-rw-r--r--   0        0        0      264 2024-05-20 11:34:05.114381 extract_thinker-0.0.2/extract_thinker/models/doc_group.py
+-rw-r--r--   0        0        0      168 2024-05-20 11:34:05.114381 extract_thinker-0.0.2/extract_thinker/models/doc_groups.py
+-rw-r--r--   0        0        0      379 2024-05-20 11:34:05.114381 extract_thinker-0.0.2/extract_thinker/models/doc_groups2.py
+-rw-r--r--   0        0        0     8546 2024-05-20 11:34:05.114381 extract_thinker-0.0.2/extract_thinker/process.py
+-rw-r--r--   0        0        0     1410 2024-05-20 11:34:05.114381 extract_thinker-0.0.2/extract_thinker/splitter.py
+-rw-r--r--   0        0        0     1671 2024-05-20 11:34:05.114381 extract_thinker-0.0.2/extract_thinker/text_splitter.py
+-rw-r--r--   0        0        0     2598 2024-05-20 11:34:05.114381 extract_thinker-0.0.2/extract_thinker/utils.py
+-rw-r--r--   0        0        0      742 2024-05-20 11:34:05.118381 extract_thinker-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5992 1970-01-01 00:00:00.000000 extract_thinker-0.0.2/PKG-INFO
```

### Comparing `extract_thinker-0.0.1/extract_thinker/app.py` & `extract_thinker-0.0.2/extract_thinker/app.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-import os
-from dotenv import load_dotenv
-
-from extract_thinker.document_loader.document_loader_tesseract import DocumentLoaderTesseract
-from extract_thinker.process import Process
-from extract_thinker.image_splitter import ImageSplitter
-from extractor import Extractor
-from extract_thinker.models.classification import Classification
-from tests.models.invoice import InvoiceContract
-from tests.models.driver_license import DriverLicense
-
-load_dotenv()
-
-# Usage
-extractor = Extractor()
-extractor.load_document_loader(DocumentLoaderTesseract(os.getenv("TESSERACT_PATH")))
-extractor.load_llm("gpt-3.5-turbo")
-
-classifications = [
-    Classification(name="Driver License", description="This is a driver license", contract=DriverLicense, extractor=extractor),
-    Classification(name="Invoice", description="This is an invoice", contract=InvoiceContract, extractor=extractor)
-]
-
-process = Process()
-process.load_document_loader(DocumentLoaderTesseract(os.getenv("TESSERACT_PATH")))
-process.load_splitter(ImageSplitter())
-
-path = "C:\\Users\\Lopez\\Desktop\\MagniFinance\\examples\\outputTestOne.pdf"
-other_path = "C:\\Users\\Lopez\\Desktop\\MagniFinance\\examples\\SingleInvoiceTests\\FT63O.pdf"
-
-split_content = process.load_file(path)\
-    .split(classifications)\
-    .extract()
-
-# extractor.loadSplitter(ImageSplitter())
-# extractor.loadfile(
-#     "C:\\Users\\Lopez\\Desktop\\MagniFinance\\examples\\outputTestOne.pdf"
-# )
-# extractor.split(classifications)
-
-# extractor.loadfile("C:\\Users\\Lopez\\Desktop\\MagniFinance\\examples\\outputTestOne.pdf").split(classifications)
-
-extractor.load_document_loader(
-    DocumentLoaderTesseract("C:\\Program Files\\Tesseract-OCR\\tesseract.exe")
-)
-extractor.load_llm("claude-3-haiku-20240307")
-
-# extractor.classify_from_path(
-#     "C:\\Users\\Lopez\\Desktop\\ExtractThinker\\driverLicense.jpg",
-#     classifications
-# )
-
-# extractor.loadfile(
-#     "C:\\Users\\Lopez\\Desktop\\ExtractThinker\\driverLicense.jpg"
-#     )\
-#     .split(classifications)\
-#     .extract()\
-#     .where(lambda x: x.name == "Driver License")\
-
-# user_info = extractor.extract_from_file(
-#     'C:\\Users\\Lopez\\Desktop\\ExtractThinker\\driverLicense.jpg', UserContract, vision=True)
-
-# print(user_info.name)
-# print(user_info.age)
-
-# the equivalent of this for the instructor:
-
+import os
+from dotenv import load_dotenv
+
+from extract_thinker.document_loader.document_loader_tesseract import DocumentLoaderTesseract
+from extract_thinker.process import Process
+from extract_thinker.image_splitter import ImageSplitter
+from extractor import Extractor
+from extract_thinker.models.classification import Classification
+from tests.models.invoice import InvoiceContract
+from tests.models.driver_license import DriverLicense
+
+load_dotenv()
+
+# Usage
+extractor = Extractor()
+extractor.load_document_loader(DocumentLoaderTesseract(os.getenv("TESSERACT_PATH")))
+extractor.load_llm("gpt-3.5-turbo")
+
+classifications = [
+    Classification(name="Driver License", description="This is a driver license", contract=DriverLicense, extractor=extractor),
+    Classification(name="Invoice", description="This is an invoice", contract=InvoiceContract, extractor=extractor)
+]
+
+process = Process()
+process.load_document_loader(DocumentLoaderTesseract(os.getenv("TESSERACT_PATH")))
+process.load_splitter(ImageSplitter())
+
+path = "C:\\Users\\Lopez\\Desktop\\MagniFinance\\examples\\outputTestOne.pdf"
+other_path = "C:\\Users\\Lopez\\Desktop\\MagniFinance\\examples\\SingleInvoiceTests\\FT63O.pdf"
+
+split_content = process.load_file(path)\
+    .split(classifications)\
+    .extract()
+
+# extractor.loadSplitter(ImageSplitter())
+# extractor.loadfile(
+#     "C:\\Users\\Lopez\\Desktop\\MagniFinance\\examples\\outputTestOne.pdf"
+# )
+# extractor.split(classifications)
+
+# extractor.loadfile("C:\\Users\\Lopez\\Desktop\\MagniFinance\\examples\\outputTestOne.pdf").split(classifications)
+
+extractor.load_document_loader(
+    DocumentLoaderTesseract("C:\\Program Files\\Tesseract-OCR\\tesseract.exe")
+)
+extractor.load_llm("claude-3-haiku-20240307")
+
+# extractor.classify_from_path(
+#     "C:\\Users\\Lopez\\Desktop\\ExtractThinker\\driverLicense.jpg",
+#     classifications
+# )
+
+# extractor.loadfile(
+#     "C:\\Users\\Lopez\\Desktop\\ExtractThinker\\driverLicense.jpg"
+#     )\
+#     .split(classifications)\
+#     .extract()\
+#     .where(lambda x: x.name == "Driver License")\
+
+# user_info = extractor.extract_from_file(
+#     'C:\\Users\\Lopez\\Desktop\\ExtractThinker\\driverLicense.jpg', UserContract, vision=True)
+
+# print(user_info.name)
+# print(user_info.age)
+
+# the equivalent of this for the instructor:
+
 # equivalent for this, inside instructor: json.loads(json_string)
```

### Comparing `extract_thinker-0.0.1/extract_thinker/document_loader/cached_document_loader.py` & `extract_thinker-0.0.2/extract_thinker/document_loader/cached_document_loader.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-
-
-from io import BytesIO
-from typing import Any, Union
-
-from cachetools import TTLCache
-from extract_thinker.document_loader.document_loader import DocumentLoader
-
-
-class CachedDocumentLoader(DocumentLoader):
-    def __init__(self, content: Any = None, cache_ttl: int = 300):
-        super().__init__(content)
-        self.cache = TTLCache(maxsize=100, ttl=cache_ttl)
-
-    def cached_load_content_from_file(self, file_path: str) -> Union[str, object]:
-        return self.load_content_from_file(file_path)
-
-    def cached_load_content_from_stream(self, stream: BytesIO) -> Union[str, object]:
-        return self.load_content_from_stream(stream)
+
+
+from io import BytesIO
+from typing import Any, Union
+
+from cachetools import TTLCache
+from extract_thinker.document_loader.document_loader import DocumentLoader
+
+
+class CachedDocumentLoader(DocumentLoader):
+    def __init__(self, content: Any = None, cache_ttl: int = 300):
+        super().__init__(content)
+        self.cache = TTLCache(maxsize=100, ttl=cache_ttl)
+
+    def cached_load_content_from_file(self, file_path: str) -> Union[str, object]:
+        return self.load_content_from_file(file_path)
+
+    def cached_load_content_from_stream(self, stream: BytesIO) -> Union[str, object]:
+        return self.load_content_from_stream(stream)
```

### Comparing `extract_thinker-0.0.1/extract_thinker/document_loader/document_loader_tesseract.py` & `extract_thinker-0.0.2/extract_thinker/document_loader/document_loader_tesseract.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-from io import BytesIO
-from operator import attrgetter
-import os
-from typing import Any, List, Union
-from PIL import Image
-import pytesseract
-
-from extract_thinker.document_loader.cached_document_loader import CachedDocumentLoader
-from extract_thinker.utils import get_image_type
-
-from cachetools import cachedmethod
-from cachetools.keys import hashkey
-import concurrent.futures
-
-SUPPORTED_IMAGE_FORMATS = ["jpeg", "png", "bmp", "tiff"]
-
-
-class DocumentLoaderTesseract(CachedDocumentLoader):
-    def __init__(self, tesseract_cmd, isContainer=False, content=None, cache_ttl=300):
-        super().__init__(content, cache_ttl)
-        self.tesseract_cmd = tesseract_cmd
-        if isContainer:
-            # docker path to tesseract
-            self.tesseract_cmd = os.environ.get("TESSERACT_PATH", "tesseract")
-        pytesseract.pytesseract.tesseract_cmd = self.tesseract_cmd
-        if not os.path.isfile(self.tesseract_cmd):
-            raise Exception(f"Tesseract not found at {self.tesseract_cmd}")
-
-    @cachedmethod(cache=attrgetter('cache'), key=lambda self, file_path: hashkey(file_path))
-    def load_content_from_file(self, file_path: str) -> Union[str, object]:
-        try:
-            file_type = get_image_type(file_path)
-            if file_type in SUPPORTED_IMAGE_FORMATS:
-                image = Image.open(file_path)
-                raw_text = str(pytesseract.image_to_string(image))
-                self.content = raw_text
-                return self.content
-            else:
-                raise Exception(f"Unsupported file type: {file_path}")
-        except Exception as e:
-            raise Exception(f"Error processing file: {e}") from e
-
-    @cachedmethod(cache=attrgetter('cache'), key=lambda self, stream: hashkey(id(stream)))
-    def load_content_from_stream(self, stream: Union[BytesIO, str]) -> Union[str, object]:
-        try:
-            file_type = get_image_type(stream)
-            if file_type in SUPPORTED_IMAGE_FORMATS:
-                image = Image.open(stream)
-                raw_text = str(pytesseract.image_to_string(image))
-                self.content = raw_text
-                return self.content
-            else:
-                raise Exception(f"Unsupported stream type: {stream}")
-        except Exception as e:
-            raise Exception(f"Error processing stream: {e}") from e
-
-    def process_image(self, image):
-        for attempt in range(3):
-            raw_text = str(pytesseract.image_to_string(Image.open(BytesIO(image))))
-            if raw_text:
-                return raw_text
-            raise Exception("Failed to process image after 3 attempts")
-
-    @cachedmethod(cache=attrgetter('cache'), key=lambda self, stream: hashkey(id(stream)))
-    def load_content_from_stream_list(self, stream: BytesIO) -> List[Any]:
-        images = self.convert_to_images(stream)
-
-        with concurrent.futures.ThreadPoolExecutor() as executor:
-            futures = {i: executor.submit(self.process_image, image[i]) for i, image in enumerate(images.values())}
-
-        contents = []
-        for i, future in futures.items():
-            contents.append({"image": images[i], "content": future.result()})
-
-        return contents
-
-    @cachedmethod(cache=attrgetter('cache'), key=lambda self, input_list: hashkey(id(input_list)))
-    def load_content_from_file_list(self, input: List[Union[str, BytesIO]]) -> List[Any]:
-        images = self.convert_to_images(input)
-
-        with concurrent.futures.ThreadPoolExecutor() as executor:
-            futures = {i: executor.submit(self.process_image, image[i]) for i, image in enumerate(images.values())}
-
-        contents = []
-        for i, future in futures.items():
-            contents.append({"image": Image.open(BytesIO(images[i][i])), "content": future.result()})
-
-        return contents
+from io import BytesIO
+from operator import attrgetter
+import os
+from typing import Any, List, Union
+from PIL import Image
+import pytesseract
+
+from extract_thinker.document_loader.cached_document_loader import CachedDocumentLoader
+from extract_thinker.utils import get_image_type
+
+from cachetools import cachedmethod
+from cachetools.keys import hashkey
+import concurrent.futures
+
+SUPPORTED_IMAGE_FORMATS = ["jpeg", "png", "bmp", "tiff"]
+
+
+class DocumentLoaderTesseract(CachedDocumentLoader):
+    def __init__(self, tesseract_cmd, isContainer=False, content=None, cache_ttl=300):
+        super().__init__(content, cache_ttl)
+        self.tesseract_cmd = tesseract_cmd
+        if isContainer:
+            # docker path to tesseract
+            self.tesseract_cmd = os.environ.get("TESSERACT_PATH", "tesseract")
+        pytesseract.pytesseract.tesseract_cmd = self.tesseract_cmd
+        if not os.path.isfile(self.tesseract_cmd):
+            raise Exception(f"Tesseract not found at {self.tesseract_cmd}")
+
+    @cachedmethod(cache=attrgetter('cache'), key=lambda self, file_path: hashkey(file_path))
+    def load_content_from_file(self, file_path: str) -> Union[str, object]:
+        try:
+            file_type = get_image_type(file_path)
+            if file_type in SUPPORTED_IMAGE_FORMATS:
+                image = Image.open(file_path)
+                raw_text = str(pytesseract.image_to_string(image))
+                self.content = raw_text
+                return self.content
+            else:
+                raise Exception(f"Unsupported file type: {file_path}")
+        except Exception as e:
+            raise Exception(f"Error processing file: {e}") from e
+
+    @cachedmethod(cache=attrgetter('cache'), key=lambda self, stream: hashkey(id(stream)))
+    def load_content_from_stream(self, stream: Union[BytesIO, str]) -> Union[str, object]:
+        try:
+            file_type = get_image_type(stream)
+            if file_type in SUPPORTED_IMAGE_FORMATS:
+                image = Image.open(stream)
+                raw_text = str(pytesseract.image_to_string(image))
+                self.content = raw_text
+                return self.content
+            else:
+                raise Exception(f"Unsupported stream type: {stream}")
+        except Exception as e:
+            raise Exception(f"Error processing stream: {e}") from e
+
+    def process_image(self, image):
+        for attempt in range(3):
+            raw_text = str(pytesseract.image_to_string(Image.open(BytesIO(image))))
+            if raw_text:
+                return raw_text
+            raise Exception("Failed to process image after 3 attempts")
+
+    @cachedmethod(cache=attrgetter('cache'), key=lambda self, stream: hashkey(id(stream)))
+    def load_content_from_stream_list(self, stream: BytesIO) -> List[Any]:
+        images = self.convert_to_images(stream)
+
+        with concurrent.futures.ThreadPoolExecutor() as executor:
+            futures = {i: executor.submit(self.process_image, image[i]) for i, image in enumerate(images.values())}
+
+        contents = []
+        for i, future in futures.items():
+            contents.append({"image": images[i], "content": future.result()})
+
+        return contents
+
+    @cachedmethod(cache=attrgetter('cache'), key=lambda self, input_list: hashkey(id(input_list)))
+    def load_content_from_file_list(self, input: List[Union[str, BytesIO]]) -> List[Any]:
+        images = self.convert_to_images(input)
+
+        with concurrent.futures.ThreadPoolExecutor() as executor:
+            futures = {i: executor.submit(self.process_image, image[i]) for i, image in enumerate(images.values())}
+
+        contents = []
+        for i, future in futures.items():
+            contents.append({"image": Image.open(BytesIO(images[i][i])), "content": future.result()})
+
+        return contents
```

### Comparing `extract_thinker-0.0.1/extract_thinker/extractor.py` & `extract_thinker-0.0.2/extract_thinker/extractor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,197 +1,210 @@
-import asyncio
-from typing import Any, Dict, List, Optional, IO, Union
-
-from pydantic import BaseModel
-from extract_thinker.document_loader.document_loader import DocumentLoader
-from extract_thinker.models.classification import Classification
-from extract_thinker.models.classification_response import (
-    ClassificationResponse,
-)
-from extract_thinker.llm import LLM
-import os
-
-from extract_thinker.document_loader.loader_interceptor import LoaderInterceptor
-from extract_thinker.document_loader.llm_interceptor import LlmInterceptor
-
-from extract_thinker.utils import get_image_type
-
-
-SUPPORTED_IMAGE_FORMATS = ["jpeg", "png", "bmp", "tiff"]
-
-
-class Extractor:
-    def __init__(
-        self, processor: Optional[DocumentLoader] = None, llm: Optional[LLM] = None
-    ):
-        self.document_loader: Optional[DocumentLoader] = processor
-        self.llm: Optional[LLM] = llm
-        self.file: Optional[str] = None
-        self.document_loaders_by_file_type: Dict[str, DocumentLoader] = {}
-        self.loader_interceptors: List[LoaderInterceptor] = []
-        self.llm_interceptors: List[LlmInterceptor] = []
-
-    def add_interceptor(
-        self, interceptor: Union[LoaderInterceptor, LlmInterceptor]
-    ) -> None:
-        if isinstance(interceptor, LoaderInterceptor):
-            self.loader_interceptors.append(interceptor)
-        elif isinstance(interceptor, LlmInterceptor):
-            self.llm_interceptors.append(interceptor)
-        else:
-            raise ValueError(
-                "Interceptor must be an instance of LoaderInterceptor or LlmInterceptor"
-            )
-
-    def set_document_loader_for_file_type(
-        self, file_type: str, document_loader: DocumentLoader
-    ):
-        self.document_loaders_by_file_type[file_type] = document_loader
-
-    def get_document_loader_for_file(self, file: str) -> DocumentLoader:
-        _, ext = os.path.splitext(file)
-        return self.document_loaders_by_file_type.get(ext, self.document_loader)
-
-    def load_document_loader(self, document_loader: DocumentLoader) -> None:
-        self.document_loader = document_loader
-
-    def load_llm(self, model: str) -> None:
-        self.llm = LLM(model)
-
-    def extract(self, source: Union[str, IO, list], response_model: type[BaseModel], vision: bool = False) -> str:
-        if not issubclass(response_model, BaseModel):
-            raise ValueError("response_model must be a subclass of Pydantic's BaseModel.")
-
-        if isinstance(source, str):  # if it's a file path
-            return self.extract_from_file(source, response_model, vision)
-        elif isinstance(source, IO):  # if it's a stream
-            return self.extract_from_stream(source, response_model, vision)
-        elif isinstance(source, list) and all(isinstance(item, dict) for item in source):  # if it's a list of dictionaries
-            return self.extract_from_list(source, response_model, vision)
-        else:
-            raise ValueError("Source must be a file path, a stream, or a list of dictionaries")
-
-    async def extract_async(self, source: Union[str, IO, list], response_model: type[BaseModel], vision: bool = False) -> str:
-        return await asyncio.to_thread(self.extract, source, response_model, vision)
-
-    def extract_from_list(self, data: List[Dict[Any, Any]], response_model: type[BaseModel], vision: bool) -> str:
-        # check if document_loader is None, raise error
-        if self.document_loader is None:
-            raise ValueError("Document loader is not set")
-
-        content = "\n".join([f"#{k}:\n{v}" for d in data for k, v in d.items() if k != "image"])
-        return self._extract(content, data, response_model, vision, is_stream=False)
-
-    def extract_from_file(
-        self, file: str, response_model: str, vision: bool = False
-    ) -> str:
-        if self.document_loader is not None:
-            content = self.document_loader.load_content_from_file(file)
-        else:
-            document_loader = self.get_document_loader_for_file(file)
-            if document_loader is None:
-                raise ValueError("No suitable document loader found for file type")
-            content = document_loader.load_content_from_file(file)
-        return self._extract(content, file, response_model, vision)
-
-    def extract_from_stream(
-        self, stream: IO, response_model: str, vision: bool = False
-    ) -> str:
-        # check if document_loader is None, raise error
-        if self.document_loader is None:
-            raise ValueError("Document loader is not set")
-
-        content = self.document_loader.load(stream)
-        return self._extract(content, stream, response_model, vision, is_stream=True)
-
-    def classify_from_path(self, path: str, classifications: List[Classification]):
-        content = self.document_loader.load_content_from_file(path)
-        return self._classify(content, classifications)
-
-    def classify_from_stream(self, stream: IO, classifications: List[Classification]):
-        content = self.document_loader.load_content_from_stream(stream)
-        self._classify(content, classifications)
-
-    def _classify(self, content: str, classifications: List[Classification]):
-        messages = [
-            {
-                "role": "system",
-                "content": "You are a server API that receives document information "
-                "and returns specific fields in JSON format.",
-            },
-        ]
-
-        input_data = (
-            f"##Content\n{content}\n##Classifications\n"
-            + "\n".join([f"{c.name}: {c.description}" for c in classifications])
-            + "\n\n##JSON Output\n"
-        )
-
-        messages.append({"role": "user", "content": input_data})
-
-        response = self.llm.request(messages, ClassificationResponse)
-
-        return response
-
-    def classify(self, input: Union[str, IO], classifications: List[Classification]):
-        if isinstance(input, str):
-            # Check if the input is a valid file path
-            if os.path.isfile(input):
-                file_type = get_image_type(input)
-                if file_type in SUPPORTED_IMAGE_FORMATS:
-                    return self.classify_from_path(input, classifications)
-                else:
-                    raise ValueError(f"Unsupported file type: {input}")
-            else:
-                raise ValueError(f"No such file: {input}")
-        elif hasattr(input, 'read'):
-            # Check if the input is a stream (like a file object)
-            return self.classify_from_stream(input, classifications)
-        else:
-            raise ValueError("Input must be a file path or a stream.")
-
-    def _extract(
-        self, content, file_or_stream, response_model, vision=False, is_stream=False
-    ):
-        # call all the llm interceptors before calling the llm
-        for interceptor in self.llm_interceptors:
-            interceptor.intercept(self.llm)
-
-        messages = [
-            {
-                "role": "system",
-                "content": "You are a server API that receives document information "
-                "and returns specific fields in JSON format.",
-            },
-        ]
-
-        if vision:
-            base64_encoded_image = self._encode_image_to_base64(
-                file_or_stream, is_stream
-            )
-
-            messages = [
-                {
-                    "role": "user",
-                    "content": [
-                        {"type": "text", "text": "Whats in this image?"},
-                        {
-                            "type": "image_url",
-                            "image_url": {
-                                "url": "data:image/jpeg;base64," + base64_encoded_image
-                            },
-                        },
-                    ],
-                }
-            ]
-        else:
-            messages.append({"role": "user", "content": "##Content\n\n" + content})
-
-        response = self.llm.request(messages, response_model)
-        return response
-
-    def loadfile(self, file):
-        self.file = file
-        return self
-
-    def loadstream(self, stream):
-        return self
+import asyncio
+from typing import Any, Dict, List, Optional, IO, Union
+
+from pydantic import BaseModel
+from extract_thinker.document_loader.document_loader import DocumentLoader
+from extract_thinker.models.classification import Classification
+from extract_thinker.models.classification_response import (
+    ClassificationResponse,
+)
+from extract_thinker.llm import LLM
+import os
+
+from extract_thinker.document_loader.loader_interceptor import LoaderInterceptor
+from extract_thinker.document_loader.llm_interceptor import LlmInterceptor
+
+from extract_thinker.utils import get_file_extension
+
+
+SUPPORTED_IMAGE_FORMATS = ["jpeg", "png", "bmp", "tiff"]
+SUPPORTED_EXCEL_FORMATS = ['.xls', '.xlsx', '.xlsm', '.xlsb', '.odf', '.ods', '.odt', '.csv']
+
+
+class Extractor:
+    def __init__(
+        self, processor: Optional[DocumentLoader] = None, llm: Optional[LLM] = None
+    ):
+        self.document_loader: Optional[DocumentLoader] = processor
+        self.llm: Optional[LLM] = llm
+        self.file: Optional[str] = None
+        self.document_loaders_by_file_type: Dict[str, DocumentLoader] = {}
+        self.loader_interceptors: List[LoaderInterceptor] = []
+        self.llm_interceptors: List[LlmInterceptor] = []
+
+    def add_interceptor(
+        self, interceptor: Union[LoaderInterceptor, LlmInterceptor]
+    ) -> None:
+        if isinstance(interceptor, LoaderInterceptor):
+            self.loader_interceptors.append(interceptor)
+        elif isinstance(interceptor, LlmInterceptor):
+            self.llm_interceptors.append(interceptor)
+        else:
+            raise ValueError(
+                "Interceptor must be an instance of LoaderInterceptor or LlmInterceptor"
+            )
+
+    def set_document_loader_for_file_type(
+        self, file_type: str, document_loader: DocumentLoader
+    ):
+        self.document_loaders_by_file_type[file_type] = document_loader
+
+    def get_document_loader_for_file(self, file: str) -> DocumentLoader:
+        _, ext = os.path.splitext(file)
+        return self.document_loaders_by_file_type.get(ext, self.document_loader)
+
+    def load_document_loader(self, document_loader: DocumentLoader) -> None:
+        self.document_loader = document_loader
+
+    def load_llm(self, model: str) -> None:
+        self.llm = LLM(model)
+
+    def extract(self, source: Union[str, IO, list], response_model: type[BaseModel], vision: bool = False) -> str:
+        if not issubclass(response_model, BaseModel):
+            raise ValueError("response_model must be a subclass of Pydantic's BaseModel.")
+
+        if isinstance(source, str):  # if it's a file path
+            return self.extract_from_file(source, response_model, vision)
+        elif isinstance(source, IO):  # if it's a stream
+            return self.extract_from_stream(source, response_model, vision)
+        elif isinstance(source, list) and all(isinstance(item, dict) for item in source):  # if it's a list of dictionaries
+            return self.extract_from_list(source, response_model, vision)
+        else:
+            raise ValueError("Source must be a file path, a stream, or a list of dictionaries")
+
+    async def extract_async(self, source: Union[str, IO, list], response_model: type[BaseModel], vision: bool = False) -> str:
+        return await asyncio.to_thread(self.extract, source, response_model, vision)
+
+    def extract_from_list(self, data: List[Dict[Any, Any]], response_model: type[BaseModel], vision: bool) -> str:
+        # check if document_loader is None, raise error
+        if self.document_loader is None:
+            raise ValueError("Document loader is not set")
+
+        content = "\n".join([f"#{k}:\n{v}" for d in data for k, v in d.items() if k != "image"])
+        return self._extract(content, data, response_model, vision, is_stream=False)
+
+    def extract_from_file(
+        self, file: str, response_model: str, vision: bool = False
+    ) -> str:
+        if self.document_loader is not None:
+            content = self.document_loader.load_content_from_file(file)
+        else:
+            document_loader = self.get_document_loader_for_file(file)
+            if document_loader is None:
+                raise ValueError("No suitable document loader found for file type")
+            content = document_loader.load_content_from_file(file)
+        return self._extract(content, file, response_model, vision)
+
+    def extract_from_stream(
+        self, stream: IO, response_model: str, vision: bool = False
+    ) -> str:
+        # check if document_loader is None, raise error
+        if self.document_loader is None:
+            raise ValueError("Document loader is not set")
+
+        content = self.document_loader.load(stream)
+        return self._extract(content, stream, response_model, vision, is_stream=True)
+
+    def classify_from_path(self, path: str, classifications: List[Classification]):
+        content = self.document_loader.load_content_from_file(path)
+        return self._classify(content, classifications)
+
+    def classify_from_stream(self, stream: IO, classifications: List[Classification]):
+        content = self.document_loader.load_content_from_stream(stream)
+        self._classify(content, classifications)
+
+    def classify_from_excel(self, path: Union[str, IO], classifications: List[Classification]):
+        if isinstance(path, str):
+            content = self.document_loader.load_content_from_file(path)
+        else:
+            content = self.document_loader.load_content_from_stream(path)
+        return self._classify(content, classifications)
+
+    def _classify(self, content: str, classifications: List[Classification]):
+        messages = [
+            {
+                "role": "system",
+                "content": "You are a server API that receives document information "
+                "and returns specific fields in JSON format.",
+            },
+        ]
+
+        input_data = (
+            f"##Content\n{content}\n##Classifications\n"
+            + "\n".join([f"{c.name}: {c.description}" for c in classifications])
+            + "\n\n##JSON Output\n"
+        )
+
+        messages.append({"role": "user", "content": input_data})
+
+        response = self.llm.request(messages, ClassificationResponse)
+
+        return response
+
+    def classify(self, input: Union[str, IO], classifications: List[Classification]):
+        if isinstance(input, str):
+            # Check if the input is a valid file path
+            if os.path.isfile(input):
+                file_type = get_file_extension(input)
+                if file_type in SUPPORTED_IMAGE_FORMATS:
+                    return self.classify_from_path(input, classifications)
+                elif file_type in SUPPORTED_EXCEL_FORMATS:
+                    return self.classify_from_excel(input, classifications)
+                else:
+                    raise ValueError(f"Unsupported file type: {input}")
+            else:
+                raise ValueError(f"No such file: {input}")
+        elif hasattr(input, 'read'):
+            # Check if the input is a stream (like a file object)
+            return self.classify_from_stream(input, classifications)
+        else:
+            raise ValueError("Input must be a file path or a stream.")
+
+    async def classify_async(self, input: Union[str, IO], classifications: List[Classification]):
+        return await asyncio.to_thread(self.classify, input, classifications)
+
+    def _extract(
+        self, content, file_or_stream, response_model, vision=False, is_stream=False
+    ):
+        # call all the llm interceptors before calling the llm
+        for interceptor in self.llm_interceptors:
+            interceptor.intercept(self.llm)
+
+        messages = [
+            {
+                "role": "system",
+                "content": "You are a server API that receives document information "
+                "and returns specific fields in JSON format.",
+            },
+        ]
+
+        if vision:
+            base64_encoded_image = self._encode_image_to_base64(
+                file_or_stream, is_stream
+            )
+
+            messages = [
+                {
+                    "role": "user",
+                    "content": [
+                        {"type": "text", "text": "Whats in this image?"},
+                        {
+                            "type": "image_url",
+                            "image_url": {
+                                "url": "data:image/jpeg;base64," + base64_encoded_image
+                            },
+                        },
+                    ],
+                }
+            ]
+        else:
+            messages.append({"role": "user", "content": "##Content\n\n" + content})
+
+        response = self.llm.request(messages, response_model)
+        return response
+
+    def loadfile(self, file):
+        self.file = file
+        return self
+
+    def loadstream(self, stream):
+        return self
```

### Comparing `extract_thinker-0.0.1/extract_thinker/image_splitter.py` & `extract_thinker-0.0.2/extract_thinker/image_splitter.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-import base64
-import litellm
-from io import BytesIO
-from typing import List, Any
-from extract_thinker.models.classification import Classification
-from extract_thinker.models.doc_groups2 import DocGroups2
-from extract_thinker.splitter import Splitter
-from extract_thinker.utils import extract_json
-
-
-class ImageSplitter(Splitter):
-
-    def encode_image(self, image):
-        buffered = BytesIO()
-        image.save(buffered, format=image.format)
-        img_byte = buffered.getvalue()
-        return base64.b64encode(img_byte).decode("utf-8")
-
-    def belongs_to_same_document(self,
-                                 obj1: Any,
-                                 obj2: Any,
-                                 classifications: List[Classification]
-                                 ) -> DocGroups2:
-
-        if 'image' not in obj1 or 'image' not in obj2:
-            raise ValueError("Input objects must have an 'image' key")
-
-        page1 = obj1['image']
-        page2 = obj2['image']
-
-        assistantPrompt = 'What you are an API that extracts information. You receive as input: \r\n1. two pages \r\n2. a group of classifications\r\n output:\r\nA JSON with the classification of each document and if belongs to the same document\r\n\r\n//Example 1\r\n//can be null if belongsToSamePage is true\r\n{\r\n    "belongs_to_same_document": true,\r\n    "classification_page1": "LLC",\r\n    "classification_page2": "LLC"\r\n}\r\n//Example 2\r\n{\r\n    "belongs_to_same_document": false,\r\n    "classification_page1": "LLC",\r\n    "classification_page2": "Invoice"\r\n}'
-
-        base64_image1 = self.encode_image(page1)
-        base64_image2 = self.encode_image(page2)
-
-        classifications_text = (
-            "##Classifications\n"
-            + "\n".join([f"{c.name}: {c.description}" for c in classifications])
-            + "\n\n##JSON Output\n"
-        )
-
-        resp = litellm.completion(
-            model="claude-3-sonnet-20240229",
-            messages=[
-                {
-                    "role": "system",
-                    "content": assistantPrompt,
-                },
-                {
-                    "role": "user",
-                    "content": [
-                        {"type": "text", "text": classifications_text},
-                        {
-                            "type": "image_url",
-                            "image_url": {
-                                "url": "data:image/jpeg;base64," + base64_image1
-                            },
-                        },
-                        {
-                            "type": "image_url",
-                            "image_url": {
-                                "url": "data:image/jpeg;base64," + base64_image2
-                            },
-                        },
-                        {"type": "text", "text": "###JSON Output\n"},
-                    ],
-                },
-            ],
-        )
-
-        jsonText = resp.choices[0].message.content
-
-        jsonText = extract_json(jsonText)
-
-        # TODO: eventually will be done in a more robust way
-        validated_obj = DocGroups2(**jsonText)
-
-        return validated_obj
+import base64
+import litellm
+from io import BytesIO
+from typing import List, Any
+from extract_thinker.models.classification import Classification
+from extract_thinker.models.doc_groups2 import DocGroups2
+from extract_thinker.splitter import Splitter
+from extract_thinker.utils import extract_json
+
+
+class ImageSplitter(Splitter):
+
+    def encode_image(self, image):
+        buffered = BytesIO()
+        image.save(buffered, format=image.format)
+        img_byte = buffered.getvalue()
+        return base64.b64encode(img_byte).decode("utf-8")
+
+    def belongs_to_same_document(self,
+                                 obj1: Any,
+                                 obj2: Any,
+                                 classifications: List[Classification]
+                                 ) -> DocGroups2:
+
+        if 'image' not in obj1 or 'image' not in obj2:
+            raise ValueError("Input objects must have an 'image' key")
+
+        page1 = obj1['image']
+        page2 = obj2['image']
+
+        assistantPrompt = 'What you are an API that extracts information. You receive as input: \r\n1. two pages \r\n2. a group of classifications\r\n output:\r\nA JSON with the classification of each document and if belongs to the same document\r\n\r\n//Example 1\r\n//can be null if belongsToSamePage is true\r\n{\r\n    "belongs_to_same_document": true,\r\n    "classification_page1": "LLC",\r\n    "classification_page2": "LLC"\r\n}\r\n//Example 2\r\n{\r\n    "belongs_to_same_document": false,\r\n    "classification_page1": "LLC",\r\n    "classification_page2": "Invoice"\r\n}'
+
+        base64_image1 = self.encode_image(page1)
+        base64_image2 = self.encode_image(page2)
+
+        classifications_text = (
+            "##Classifications\n"
+            + "\n".join([f"{c.name}: {c.description}" for c in classifications])
+            + "\n\n##JSON Output\n"
+        )
+
+        resp = litellm.completion(
+            model="claude-3-sonnet-20240229",
+            messages=[
+                {
+                    "role": "system",
+                    "content": assistantPrompt,
+                },
+                {
+                    "role": "user",
+                    "content": [
+                        {"type": "text", "text": classifications_text},
+                        {
+                            "type": "image_url",
+                            "image_url": {
+                                "url": "data:image/jpeg;base64," + base64_image1
+                            },
+                        },
+                        {
+                            "type": "image_url",
+                            "image_url": {
+                                "url": "data:image/jpeg;base64," + base64_image2
+                            },
+                        },
+                        {"type": "text", "text": "###JSON Output\n"},
+                    ],
+                },
+            ],
+        )
+
+        jsonText = resp.choices[0].message.content
+
+        jsonText = extract_json(jsonText)
+
+        # TODO: eventually will be done in a more robust way
+        validated_obj = DocGroups2(**jsonText)
+
+        return validated_obj
```

### Comparing `extract_thinker-0.0.1/extract_thinker/llm.py` & `extract_thinker-0.0.2/extract_thinker/llm.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-import instructor
-import litellm
-from extract_thinker.utils import num_tokens_from_string
-
-
-class LLM:
-    def __init__(self, model):
-        self.client = instructor.from_litellm(litellm.completion)
-        self.model = model
-
-    def request(self, messages, response_model):
-
-        contents = map(lambda message: message['content'], messages)
-
-        all_contents = ' '.join(contents)
-        return self.client.chat.completions.create(
-            model=self.model,
-            max_tokens=num_tokens_from_string(all_contents),
-            messages=messages,
-            response_model=response_model,
-        )
+import instructor
+import litellm
+from extract_thinker.utils import num_tokens_from_string
+
+
+class LLM:
+    def __init__(self, model):
+        self.client = instructor.from_litellm(litellm.completion)
+        self.model = model
+
+    def request(self, messages, response_model):
+
+        contents = map(lambda message: message['content'], messages)
+
+        all_contents = ' '.join(contents)
+        return self.client.chat.completions.create(
+            model=self.model,
+            max_tokens=num_tokens_from_string(all_contents),
+            messages=messages,
+            response_model=response_model,
+        )
```

### Comparing `extract_thinker-0.0.1/extract_thinker/process.py` & `extract_thinker-0.0.2/extract_thinker/process.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,213 +1,213 @@
-import asyncio
-from typing import IO, Any, Dict, List, Optional
-from extract_thinker.extractor import Extractor
-from extract_thinker.models.classification import Classification
-from extract_thinker.document_loader.document_loader import DocumentLoader
-from extract_thinker.models.doc_group import DocGroup
-from extract_thinker.models.doc_groups2 import DocGroups2
-from extract_thinker.splitter import Splitter
-from extract_thinker.models.doc_groups import (
-    DocGroups,
-)
-from extract_thinker.utils import get_image_type
-
-
-class Process:
-    def __init__(self):
-        # self.extractors: List[Extractor] = []
-        self.doc_groups: Optional[DocGroups] = None
-        self.split_classifications: List[Classification] = []
-        self.extractor_groups: List[List[Extractor]] = []  # for classication
-        self.document_loaders_by_file_type: Dict[str, DocumentLoader] = {}
-        self.document_loader: Optional[DocumentLoader] = None
-        self.file_path: Optional[str] = None
-        self.file_stream: Optional[IO] = None
-        self.splitter: Optional[Splitter] = None
-
-    def set_document_loader_for_file_type(self, file_type: str, document_loader: DocumentLoader):
-        if self.document_loader is not None:
-            raise ValueError("Cannot set a document loader for a specific file type when a default loader is already set.")
-        self.document_loaders_by_file_type[file_type] = document_loader
-
-    def load_document_loader(self, document_loader: DocumentLoader):
-        if self.document_loaders_by_file_type:
-            raise ValueError("Cannot set a default document loader when specific loaders are already set.")
-        self.document_loader = document_loader
-        return self
-
-    def load_splitter(self, splitter: Splitter):
-        self.splitter = splitter
-        return self
-
-    def add_classifyExtractor(self, extractor_groups: List[List[Extractor]]):
-        for extractors in extractor_groups:
-            self.extractor_groups.append(extractors)
-        return self
-
-    async def _classify_async(self, extractor, file, classifications):
-        loop = asyncio.get_event_loop()
-        return await loop.run_in_executor(None, extractor.classify, file, classifications)
-
-    async def classify_async(self, file: str, classifications) -> Optional[Classification]:
-        for extractor_group in self.extractor_groups:
-            group_classifications = await asyncio.gather(*(self._classify_async(extractor, file, classifications) for extractor in extractor_group))
-
-            # Check if all classifications in the group are the same
-            if len(set(group_classifications)) == 1:
-                return group_classifications[0]
-
-        # If no agreement was found, return None
-        return None
-
-    async def classify_extractor(self, session, extractor, file):
-        return await session.run(extractor.classify, file)
-
-    # check if there is only the default one, if not, get from the file type. if none is present, raise an error
-    def get_document_loader(self, file):
-        if self.document_loader is not None:
-            return self.document_loader
-
-        filetype = get_image_type(file)
-        return self.document_loaders_by_file_type.get(filetype, None)
-
-    def load_file(self, file):
-        self.file_path = file
-        return self
-
-    def split(self, classifications: List[Classification]):
-
-        self.split_classifications = classifications
-
-        documentLoader = self.get_document_loader(self.file_path)
-
-        if documentLoader is None:
-            raise ValueError("No suitable document loader found for file type")
-
-        if self.file_path:
-            content = documentLoader.load_content_from_file_list(self.file_path)
-        elif self.file_stream:
-            content = documentLoader.load_content_from_stream_list(self.file_stream)
-        else:
-            raise ValueError("No file or stream available")
-
-        if len(content) == 1:
-            raise ValueError("Document must have at least 2 pages")
-
-        groups = self.splitter.split_document_into_groups(content)
-
-        loop = asyncio.get_event_loop()
-        processedGroups = loop.run_until_complete(
-            self.splitter.process_split_groups(groups, classifications)
-        )
-
-        doc_groups = self.aggregate_split_documents_2(processedGroups)
-
-        # doc_groups = DocGroups()
-        # doc_groups.doc_groups.append(DocGroup(pages=[1], classification='Invoice'))
-        # doc_groups.doc_groups.append(DocGroup(pages=[2], classification='Invoice'))
-        # doc_groups.doc_groups.append(DocGroup(pages=[3], classification='Invoice'))
-        # doc_groups.doc_groups.append(DocGroup(pages=[4, 5], classification='Invoice'))
-
-        self.doc_groups = doc_groups
-
-        return self
-
-    def aggregate_split_documents_2(self, doc_groups_tasks: List[DocGroups2]) -> DocGroups:
-        doc_groups = DocGroups()
-        current_group = DocGroup()
-        page_number = 1
-
-        # do the first group outside of the loop
-        doc_group = doc_groups_tasks[0]
-
-        if doc_group.belongs_to_same_document:
-            current_group.pages = [1, 2]
-            current_group.classification = doc_group.classification_page1
-        else:
-            current_group.pages = [1]
-            current_group.classification = doc_group.classification_page1
-
-            doc_groups.doc_groups.append(current_group)
-
-            current_group = DocGroup()
-            current_group.pages = [2]
-            current_group.classification = doc_group.classification_page2
-
-        page_number += 1
-
-        for index in range(1, len(doc_groups_tasks)):
-            doc_group_2 = doc_groups_tasks[index]
-
-            if doc_group_2.belongs_to_same_document:
-                current_group.pages.append(page_number + 1)
-            else:
-                doc_groups.doc_groups.append(current_group)
-
-                current_group = DocGroup()
-                current_group.classification = doc_group_2.classification_page2
-                current_group.pages = [page_number + 1]
-
-            page_number += 1
-
-        doc_groups.doc_groups.append(current_group)  # the last group
-
-        return doc_groups
-
-    def where(self, condition):
-        pass
-
-    def extract(self) -> List[Any]:
-        if self.doc_groups is None:
-            raise ValueError("Document groups have not been initialized")
-
-        async def _extract(doc_group):
-            classificationStr = doc_group.classification  # str
-
-            for classification in self.split_classifications:
-                if classification.name == classificationStr:
-                    extractor = classification.extractor
-                    contract = classification.contract
-                    break
-
-            if extractor is None:
-                raise ValueError("Extractor not found for classification")
-
-            documentLoader = self.get_document_loader(self.file_path)
-
-            if documentLoader is None:
-                raise ValueError("No suitable document loader found for file type")
-
-            if self.file_path:
-                content = documentLoader.load_content_from_file_list(self.file_path)
-            elif self.file_stream:
-                content = documentLoader.load_content_from_stream_list(self.file_stream)
-            else:
-                raise ValueError("No file or stream available")
-
-            # doc_groups contains e.g [1,2], [3], [4,5] and doc_group is e.g [1,2]
-            # content is a list of pages with the content of each page
-            # get the content of the pages, add them together and extract the data
-
-            pages_content = [content[i - 1] for i in doc_group.pages]
-            return await extractor.extract_async(pages_content, contract)
-
-        doc_groups = self.doc_groups.doc_groups
-
-        async def process_doc_groups(groups: List[Any]) -> List[Any]:
-            # Create asynchronous tasks for processing each group
-            tasks = [_extract(group) for group in groups]
-            try:
-                # Execute all tasks concurrently and wait for all to complete
-                processedGroups = await asyncio.gather(*tasks)
-                return processedGroups
-            except Exception as e:
-                # Handle possible exceptions that might occur during task execution
-                print(f"An error occurred: {e}")
-                raise
-
-        loop = asyncio.get_event_loop()
-        processedGroups = loop.run_until_complete(
-            process_doc_groups(doc_groups)
-        )
-
-        return processedGroups
+import asyncio
+from typing import IO, Any, Dict, List, Optional
+from extract_thinker.extractor import Extractor
+from extract_thinker.models.classification import Classification
+from extract_thinker.document_loader.document_loader import DocumentLoader
+from extract_thinker.models.doc_group import DocGroup
+from extract_thinker.models.doc_groups2 import DocGroups2
+from extract_thinker.splitter import Splitter
+from extract_thinker.models.doc_groups import (
+    DocGroups,
+)
+from extract_thinker.utils import get_image_type
+
+
+class Process:
+    def __init__(self):
+        # self.extractors: List[Extractor] = []
+        self.doc_groups: Optional[DocGroups] = None
+        self.split_classifications: List[Classification] = []
+        self.extractor_groups: List[List[Extractor]] = []  # for classication
+        self.document_loaders_by_file_type: Dict[str, DocumentLoader] = {}
+        self.document_loader: Optional[DocumentLoader] = None
+        self.file_path: Optional[str] = None
+        self.file_stream: Optional[IO] = None
+        self.splitter: Optional[Splitter] = None
+
+    def set_document_loader_for_file_type(self, file_type: str, document_loader: DocumentLoader):
+        if self.document_loader is not None:
+            raise ValueError("Cannot set a document loader for a specific file type when a default loader is already set.")
+        self.document_loaders_by_file_type[file_type] = document_loader
+
+    def load_document_loader(self, document_loader: DocumentLoader):
+        if self.document_loaders_by_file_type:
+            raise ValueError("Cannot set a default document loader when specific loaders are already set.")
+        self.document_loader = document_loader
+        return self
+
+    def load_splitter(self, splitter: Splitter):
+        self.splitter = splitter
+        return self
+
+    def add_classifyExtractor(self, extractor_groups: List[List[Extractor]]):
+        for extractors in extractor_groups:
+            self.extractor_groups.append(extractors)
+        return self
+
+    async def _classify_async(self, extractor, file, classifications):
+        loop = asyncio.get_event_loop()
+        return await loop.run_in_executor(None, extractor.classify, file, classifications)
+
+    async def classify_async(self, file: str, classifications) -> Optional[Classification]:
+        for extractor_group in self.extractor_groups:
+            group_classifications = await asyncio.gather(*(self._classify_async(extractor, file, classifications) for extractor in extractor_group))
+
+            # Check if all classifications in the group are the same
+            if len(set(group_classifications)) == 1:
+                return group_classifications[0]
+
+        # If no agreement was found, return None
+        return None
+
+    async def classify_extractor(self, session, extractor, file):
+        return await session.run(extractor.classify, file)
+
+    # check if there is only the default one, if not, get from the file type. if none is present, raise an error
+    def get_document_loader(self, file):
+        if self.document_loader is not None:
+            return self.document_loader
+
+        filetype = get_image_type(file)
+        return self.document_loaders_by_file_type.get(filetype, None)
+
+    def load_file(self, file):
+        self.file_path = file
+        return self
+
+    def split(self, classifications: List[Classification]):
+
+        self.split_classifications = classifications
+
+        documentLoader = self.get_document_loader(self.file_path)
+
+        if documentLoader is None:
+            raise ValueError("No suitable document loader found for file type")
+
+        if self.file_path:
+            content = documentLoader.load_content_from_file_list(self.file_path)
+        elif self.file_stream:
+            content = documentLoader.load_content_from_stream_list(self.file_stream)
+        else:
+            raise ValueError("No file or stream available")
+
+        if len(content) == 1:
+            raise ValueError("Document must have at least 2 pages")
+
+        groups = self.splitter.split_document_into_groups(content)
+
+        loop = asyncio.get_event_loop()
+        processedGroups = loop.run_until_complete(
+            self.splitter.process_split_groups(groups, classifications)
+        )
+
+        doc_groups = self.aggregate_split_documents_2(processedGroups)
+
+        # doc_groups = DocGroups()
+        # doc_groups.doc_groups.append(DocGroup(pages=[1], classification='Invoice'))
+        # doc_groups.doc_groups.append(DocGroup(pages=[2], classification='Invoice'))
+        # doc_groups.doc_groups.append(DocGroup(pages=[3], classification='Invoice'))
+        # doc_groups.doc_groups.append(DocGroup(pages=[4, 5], classification='Invoice'))
+
+        self.doc_groups = doc_groups
+
+        return self
+
+    def aggregate_split_documents_2(self, doc_groups_tasks: List[DocGroups2]) -> DocGroups:
+        doc_groups = DocGroups()
+        current_group = DocGroup()
+        page_number = 1
+
+        # do the first group outside of the loop
+        doc_group = doc_groups_tasks[0]
+
+        if doc_group.belongs_to_same_document:
+            current_group.pages = [1, 2]
+            current_group.classification = doc_group.classification_page1
+        else:
+            current_group.pages = [1]
+            current_group.classification = doc_group.classification_page1
+
+            doc_groups.doc_groups.append(current_group)
+
+            current_group = DocGroup()
+            current_group.pages = [2]
+            current_group.classification = doc_group.classification_page2
+
+        page_number += 1
+
+        for index in range(1, len(doc_groups_tasks)):
+            doc_group_2 = doc_groups_tasks[index]
+
+            if doc_group_2.belongs_to_same_document:
+                current_group.pages.append(page_number + 1)
+            else:
+                doc_groups.doc_groups.append(current_group)
+
+                current_group = DocGroup()
+                current_group.classification = doc_group_2.classification_page2
+                current_group.pages = [page_number + 1]
+
+            page_number += 1
+
+        doc_groups.doc_groups.append(current_group)  # the last group
+
+        return doc_groups
+
+    def where(self, condition):
+        pass
+
+    def extract(self) -> List[Any]:
+        if self.doc_groups is None:
+            raise ValueError("Document groups have not been initialized")
+
+        async def _extract(doc_group):
+            classificationStr = doc_group.classification  # str
+
+            for classification in self.split_classifications:
+                if classification.name == classificationStr:
+                    extractor = classification.extractor
+                    contract = classification.contract
+                    break
+
+            if extractor is None:
+                raise ValueError("Extractor not found for classification")
+
+            documentLoader = self.get_document_loader(self.file_path)
+
+            if documentLoader is None:
+                raise ValueError("No suitable document loader found for file type")
+
+            if self.file_path:
+                content = documentLoader.load_content_from_file_list(self.file_path)
+            elif self.file_stream:
+                content = documentLoader.load_content_from_stream_list(self.file_stream)
+            else:
+                raise ValueError("No file or stream available")
+
+            # doc_groups contains e.g [1,2], [3], [4,5] and doc_group is e.g [1,2]
+            # content is a list of pages with the content of each page
+            # get the content of the pages, add them together and extract the data
+
+            pages_content = [content[i - 1] for i in doc_group.pages]
+            return await extractor.extract_async(pages_content, contract)
+
+        doc_groups = self.doc_groups.doc_groups
+
+        async def process_doc_groups(groups: List[Any]) -> List[Any]:
+            # Create asynchronous tasks for processing each group
+            tasks = [_extract(group) for group in groups]
+            try:
+                # Execute all tasks concurrently and wait for all to complete
+                processedGroups = await asyncio.gather(*tasks)
+                return processedGroups
+            except Exception as e:
+                # Handle possible exceptions that might occur during task execution
+                print(f"An error occurred: {e}")
+                raise
+
+        loop = asyncio.get_event_loop()
+        processedGroups = loop.run_until_complete(
+            process_doc_groups(doc_groups)
+        )
+
+        return processedGroups
```

### Comparing `extract_thinker-0.0.1/extract_thinker/splitter.py` & `extract_thinker-0.0.2/extract_thinker/splitter.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import asyncio
-from typing import Any, List
-from abc import ABC, abstractmethod
-from extract_thinker.models.doc_groups2 import DocGroups2
-
-
-class Splitter(ABC):
-    @abstractmethod
-    def belongs_to_same_document(self, page1: Any, page2: Any, contract: str) -> DocGroups2:
-        pass
-
-    def split_document_into_groups(self, document: List[Any]) -> List[List[Any]]:
-        page_per_split = 2
-        split = []
-        if len(document) == 1:
-            return [document]
-        for i in range(0, len(document) - 1):
-            group = document[i: i + page_per_split]
-            split.append(group)
-        return split
-
-    async def process_split_groups(self, split: List[List[Any]], contract: str) -> List[DocGroups2]:
-        # Create asynchronous tasks for processing each group
-        tasks = [self.process_group(x, contract) for x in split]
-        try:
-            # Execute all tasks concurrently and wait for all to complete
-            doc_groups = await asyncio.gather(*tasks)
-            return doc_groups
-        except Exception as e:
-            # Handle possible exceptions that might occur during task execution
-            print(f"An error occurred: {e}")
-            raise
-
-    async def process_group(self, group: List[Any], contract: str) -> DocGroups2:
-        page2 = group[1] if len(group) > 1 else None
-        return self.belongs_to_same_document(group[0], page2, contract)
+import asyncio
+from typing import Any, List
+from abc import ABC, abstractmethod
+from extract_thinker.models.doc_groups2 import DocGroups2
+
+
+class Splitter(ABC):
+    @abstractmethod
+    def belongs_to_same_document(self, page1: Any, page2: Any, contract: str) -> DocGroups2:
+        pass
+
+    def split_document_into_groups(self, document: List[Any]) -> List[List[Any]]:
+        page_per_split = 2
+        split = []
+        if len(document) == 1:
+            return [document]
+        for i in range(0, len(document) - 1):
+            group = document[i: i + page_per_split]
+            split.append(group)
+        return split
+
+    async def process_split_groups(self, split: List[List[Any]], contract: str) -> List[DocGroups2]:
+        # Create asynchronous tasks for processing each group
+        tasks = [self.process_group(x, contract) for x in split]
+        try:
+            # Execute all tasks concurrently and wait for all to complete
+            doc_groups = await asyncio.gather(*tasks)
+            return doc_groups
+        except Exception as e:
+            # Handle possible exceptions that might occur during task execution
+            print(f"An error occurred: {e}")
+            raise
+
+    async def process_group(self, group: List[Any], contract: str) -> DocGroups2:
+        page2 = group[1] if len(group) > 1 else None
+        return self.belongs_to_same_document(group[0], page2, contract)
```

### Comparing `extract_thinker-0.0.1/extract_thinker/text_splitter.py` & `extract_thinker-0.0.2/extract_thinker/text_splitter.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from splitter import Splitter
-
-
-from typing import IO, Union
-
-
-class TextSplitter(Splitter):
-    def belongs_to_same_document(self,
-                                 page1: Union[str, IO],
-                                 page2: Union[str, IO]) -> bool:
-        # assistantPrompt = 'What you are an API that extracts information. You receive as input: \r\n1. two pages \r\n2. a group of classifications\r\n output:\r\nA JSON with the classification of each document and if belongs to the same document\r\n\r\n//Example 1\r\n//can be null if belongsToSamePage is true\r\n{\r\n    "belongsToSameDocument": true,\r\n    "classificationPage1": "LLC",\r\n    "classificationPage2": "LLC"\r\n}\r\n//Example 2\r\n{\r\n    "belongsToSameDocument": false,\r\n    "classificationPage1": "LLC",\r\n    "classificationPage2": "Invoice"\r\n}'
-
-        # classifications_text = (
-        #     "##Classifications\n"
-        #     + "\n".join([f"{c.name}: {c.description}" for c in classifications])
-        #     + "\n\n##JSON Output\n"
-        # )
-
-        # resp = litellm.completion(
-        #     model="claude-3-sonnet-20240229",
-        #     messages=[
-        #         {
-        #             "role": "system",
-        #             "content": assistantPrompt,
-        #         },
-        #         {
-        #             "role": "user",
-        #             "content": [
-        #                 {"type": "text", "text": classifications_text},
-        #                 {"type": "text", "text": page1},
-        #                 {"type": "text", "text": page2},
-        #             ],
-        #         },
-        #     ],
-        # )
-
-        # return resp
+from splitter import Splitter
+
+
+from typing import IO, Union
+
+
+class TextSplitter(Splitter):
+    def belongs_to_same_document(self,
+                                 page1: Union[str, IO],
+                                 page2: Union[str, IO]) -> bool:
+        # assistantPrompt = 'What you are an API that extracts information. You receive as input: \r\n1. two pages \r\n2. a group of classifications\r\n output:\r\nA JSON with the classification of each document and if belongs to the same document\r\n\r\n//Example 1\r\n//can be null if belongsToSamePage is true\r\n{\r\n    "belongsToSameDocument": true,\r\n    "classificationPage1": "LLC",\r\n    "classificationPage2": "LLC"\r\n}\r\n//Example 2\r\n{\r\n    "belongsToSameDocument": false,\r\n    "classificationPage1": "LLC",\r\n    "classificationPage2": "Invoice"\r\n}'
+
+        # classifications_text = (
+        #     "##Classifications\n"
+        #     + "\n".join([f"{c.name}: {c.description}" for c in classifications])
+        #     + "\n\n##JSON Output\n"
+        # )
+
+        # resp = litellm.completion(
+        #     model="claude-3-sonnet-20240229",
+        #     messages=[
+        #         {
+        #             "role": "system",
+        #             "content": assistantPrompt,
+        #         },
+        #         {
+        #             "role": "user",
+        #             "content": [
+        #                 {"type": "text", "text": classifications_text},
+        #                 {"type": "text", "text": page1},
+        #                 {"type": "text", "text": page2},
+        #             ],
+        #         },
+        #     ],
+        # )
+
+        # return resp
         pass
```

### Comparing `extract_thinker-0.0.1/LICENSE` & `extract_thinker-0.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

