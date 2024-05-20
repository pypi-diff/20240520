# Comparing `tmp/qpay_python-0.0.2.tar.gz` & `tmp/qpay_python-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qpay_python-0.0.2.tar", max compression
+gzip compressed data, was "qpay_python-0.0.3.tar", max compression
```

## Comparing `qpay_python-0.0.2.tar` & `qpay_python-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2802 2024-05-01 00:42:38.810092 qpay_python-0.0.2/README.md
--rw-r--r--   0        0        0     1490 2024-05-01 00:42:54.466278 qpay_python-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      107 2024-05-01 00:42:38.814092 qpay_python-0.0.2/qpay/__init__.py
--rw-r--r--   0        0        0     2954 2024-05-01 00:42:38.814092 qpay_python-0.0.2/qpay/auth.py
--rw-r--r--   0        0        0      496 2024-05-01 00:42:38.814092 qpay_python-0.0.2/qpay/exceptions.py
--rw-r--r--   0        0        0     4552 2024-05-01 00:42:38.814092 qpay_python-0.0.2/qpay/main.py
--rw-r--r--   0        0        0      371 2024-05-01 00:42:38.814092 qpay_python-0.0.2/qpay/singleton.py
--rw-r--r--   0        0        0     3833 1970-01-01 00:00:00.000000 qpay_python-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2802 2024-05-20 18:31:57.593273 qpay_python-0.0.3/README.md
+-rw-r--r--   0        0        0     1490 2024-05-20 18:32:03.653282 qpay_python-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      107 2024-05-20 18:31:57.597273 qpay_python-0.0.3/qpay/__init__.py
+-rw-r--r--   0        0        0     2954 2024-05-20 18:31:57.597273 qpay_python-0.0.3/qpay/auth.py
+-rw-r--r--   0        0        0      496 2024-05-20 18:31:57.597273 qpay_python-0.0.3/qpay/exceptions.py
+-rw-r--r--   0        0        0     4796 2024-05-20 18:31:57.597273 qpay_python-0.0.3/qpay/main.py
+-rw-r--r--   0        0        0      371 2024-05-20 18:31:57.597273 qpay_python-0.0.3/qpay/singleton.py
+-rw-r--r--   0        0        0     3833 1970-01-01 00:00:00.000000 qpay_python-0.0.3/PKG-INFO
```

### Comparing `qpay_python-0.0.2/README.md` & `qpay_python-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `qpay_python-0.0.2/pyproject.toml` & `qpay_python-0.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qpay-python"
-version = "0.0.2"
+version = "0.0.3"
 description = "QPay v2 SDK client for Python projects"
 authors = ["khasbilegt <khasbilegt.ts@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/khasbilegt/qpay-python"
 repository = "https://github.com/khasbilegt/qpay-python"
 keywords = ["python", "qpay", "sdk", "payment", "qr", "finance"]
```

### Comparing `qpay_python-0.0.2/qpay/auth.py` & `qpay_python-0.0.3/qpay/auth.py`

 * *Files identical despite different names*

### Comparing `qpay_python-0.0.2/qpay/main.py` & `qpay_python-0.0.3/qpay/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,24 @@
 logger = logging.getLogger(__name__)
 
 
 class Invoice(BaseModel):
     class URL(BaseModel):
         name: str = Field(description="Банкны нэр")
         description: str = Field(description="Утга")
+        logo: str = Field(description="Тухайн банкны лого")
         link: str = Field(description="Холбоос линк")
 
     id: str = Field(alias="invoice_id", description="Нэхэмжлэхийн дугаар")
     qr_text: str = Field(description="Данс болон картын гүйлгээ дэмжих QR утга")
     qr_image: str = Field(description="QPay лого голдоо агуулсан base64 зурган QR код")
+    short_url: str = Field(
+        alias="qPay_shortUrl",
+        description="QPay богино URL /Мессеж илгээхэд ашиглаж болно/",
+    )
     urls: list[URL] = Field(
         description="Аппликейшнээс банкны аппликейшнруу үсрэх Deeplink"
     )
 
 
 class Payment(BaseModel):
     id: str = Field(alias="payment_id", description="QPay-ээс үүссэн гүйлгээний дугаар")
```

### Comparing `qpay_python-0.0.2/PKG-INFO` & `qpay_python-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qpay-python
-Version: 0.0.2
+Version: 0.0.3
 Summary: QPay v2 SDK client for Python projects
 Home-page: https://github.com/khasbilegt/qpay-python
 License: MIT
 Keywords: python,qpay,sdk,payment,qr,finance
 Author: khasbilegt
 Author-email: khasbilegt.ts@gmail.com
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: qpay-python Version: 0.0.2 Summary: QPay v2 SDK
+Metadata-Version: 2.1 Name: qpay-python Version: 0.0.3 Summary: QPay v2 SDK
 client for Python projects Home-page: https://github.com/khasbilegt/qpay-python
 License: MIT Keywords: python,qpay,sdk,payment,qr,finance Author: khasbilegt
 Author-email: khasbilegt.ts@gmail.com Requires-Python: >=3.9,<4.0 Classifier:
 Framework :: Pydantic Classifier: Framework :: Pytest Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

