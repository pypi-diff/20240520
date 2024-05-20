# Comparing `tmp/html_elements-0.2.0.tar.gz` & `tmp/html_elements-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html_elements-0.2.0.tar", max compression
+gzip compressed data, was "html_elements-0.2.1.tar", max compression
```

## Comparing `html_elements-0.2.0.tar` & `html_elements-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1076 2024-03-22 09:26:50.620238 html_elements-0.2.0/LICENSE
--rw-r--r--   0        0        0     1555 2024-03-22 09:23:20.750337 html_elements-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-02-14 14:26:35.458394 html_elements-0.2.0/html_elements/__init__.py
--rw-r--r--   0        0        0    11310 2024-04-29 18:00:53.216948 html_elements-0.2.0/html_elements/base.py
--rw-r--r--   0        0        0    34848 2024-04-04 18:09:24.887636 html_elements-0.2.0/html_elements/elements.py
--rw-r--r--   0        0        0     4159 2024-03-01 08:37:04.759557 html_elements-0.2.0/html_elements/extensions.py
--rw-r--r--   0        0        0        0 2024-04-03 17:56:10.211171 html_elements-0.2.0/html_elements/py.typed
--rw-r--r--   0        0        0      941 2024-04-29 18:02:19.722588 html_elements-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2185 1970-01-01 00:00:00.000000 html_elements-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-03-22 09:26:50.620238 html_elements-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1555 2024-03-22 09:23:20.750337 html_elements-0.2.1/README.md
+-rw-r--r--   0        0        0      102 2024-05-20 13:22:28.820541 html_elements-0.2.1/html_elements/__init__.py
+-rw-r--r--   0        0        0    11455 2024-05-20 13:23:59.721552 html_elements-0.2.1/html_elements/base.py
+-rw-r--r--   0        0        0    34848 2024-05-20 13:23:59.722813 html_elements-0.2.1/html_elements/elements.py
+-rw-r--r--   0        0        0     4194 2024-05-20 13:23:59.721560 html_elements-0.2.1/html_elements/extensions.py
+-rw-r--r--   0        0        0        0 2024-04-03 17:56:10.211171 html_elements-0.2.1/html_elements/py.typed
+-rw-r--r--   0        0        0      945 2024-05-20 13:23:57.095172 html_elements-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2185 1970-01-01 00:00:00.000000 html_elements-0.2.1/PKG-INFO
```

### Comparing `html_elements-0.2.0/LICENSE` & `html_elements-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `html_elements-0.2.0/README.md` & `html_elements-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `html_elements-0.2.0/html_elements/base.py` & `html_elements-0.2.1/html_elements/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 import html
 from abc import ABC, ABCMeta
-from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Dict, List,
-                    Literal, Tuple, Type, TypedDict, Union)
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    ClassVar,
+    Dict,
+    List,
+    Literal,
+    Tuple,
+    Type,
+    TypedDict,
+    Union,
+)
 
 from typing_extensions import dataclass_transform
 
 Undefined = object()
 HtmlAttributeType = Literal["attribute", "content"]
 
 
@@ -253,28 +264,40 @@
     def __str__(self) -> str:
         return self.to_html()
 
     def __repr__(self) -> str:
         return f"<{self.__html_config__['tag']}> field"
 
 
-def format_attribute(key: str, value: Any, attribute: HtmlAttributeInfo, inner_multi: bool = False, escape: bool = True) -> str:
+def format_attribute(
+    key: str,
+    value: Any,
+    attribute: HtmlAttributeInfo,
+    inner_multi: bool = False,
+    escape: bool = True,
+) -> str:
     """
     Formats the attribute to add to the html attributes.
     Depending on the value and attribute config, this can add zero, one or more attributes
     Returns the attribute to add e.g. `selected`, `type="button"` or `aria-type="button" aria-checked="false"`
     """
     html_attribute = attribute.html_attribute or key if not inner_multi else key
     html_attribute = html.escape(html_attribute, quote=True) if escape else html_attribute
     if value is None:
         return ""
     if not inner_multi and attribute.multi_attribute:
         # For an aria dict, treat each value as
         formatted = [
-            format_attribute(f"{html_attribute}-{sub_key}", sub_value, attribute, inner_multi=True, escape=escape)
+            format_attribute(
+                f"{html_attribute}-{sub_key}",
+                sub_value,
+                attribute,
+                inner_multi=True,
+                escape=escape,
+            )
             for sub_key, sub_value in value.items()
         ]
         # Don't add empty attributes
         return " ".join(i for i in formatted if i)
     if isinstance(value, bool):
         # for e.g. disabled. Only set if true
         if value:
```

### Comparing `html_elements-0.2.0/html_elements/elements.py` & `html_elements-0.2.1/html_elements/elements.py`

 * *Files identical despite different names*

### Comparing `html_elements-0.2.0/html_elements/extensions.py` & `html_elements-0.2.1/html_elements/extensions.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,24 @@
     #TODO Allow for proper typing of extensions
     """
     for subcls in base.__html_subclasses__:
         subcls.__html_attributes__.update(extension.__html_attributes__)
 
 
 TrueFalse = Literal["true", "false"]
-HxSwap = Literal["innerHTML", "outerHTML", "beforebegin", "afterbegin", "beforeend", "afterend", "delete", "none"]
+HxSwap = Literal[
+    "innerHTML",
+    "outerHTML",
+    "beforebegin",
+    "afterbegin",
+    "beforeend",
+    "afterend",
+    "delete",
+    "none",
+]
 
 
 class HtmxExtension(BaseHtmlElement, ABC):
     # Core attributes
     hx_get: Union[str, None] = HtmlAttribute(default=None, html_attribute="hx-get")
     hx_post: Union[str, None] = HtmlAttribute(default=None, html_attribute="hx-post")
     hx_on: Dict[str, str] = HtmlAttribute(default_factory=dict, html_attribute="hx-on", multi_attribute=True)
```

### Comparing `html_elements-0.2.0/pyproject.toml` & `html_elements-0.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "html-elements"
-version = "0.2.0"
+version = "0.2.1"
 description = "HTML element objects to use in pure Python server side rendering"
 authors = ["Anton De Meester <antondemeester@gmail.com>"]
 readme = "README.md"
 packages = [{include = "html_elements"}]
 license = "MIT"
 
 [project.urls]
@@ -25,16 +25,16 @@
 mkdocs-material = "^9.5.11"
 pytest-cov = "^4.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.black]
+[tool.ruff]
 line-length = 128
-exclude = "docs_code|local"
+exclude = ["docs_code", "local"]
 
 [tool.pyright]
 exclude = ["local", "site"]
 
 [tool.mypy]
 exclude = "site|local"
```

### Comparing `html_elements-0.2.0/PKG-INFO` & `html_elements-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html-elements
-Version: 0.2.0
+Version: 0.2.1
 Summary: HTML element objects to use in pure Python server side rendering
 License: MIT
 Author: Anton De Meester
 Author-email: antondemeester@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

