# Comparing `tmp/isic_metadata-1.9.1.tar.gz` & `tmp/isic_metadata-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isic_metadata-1.9.1.tar", last modified: Thu May 16 16:55:06 2024, max compression
+gzip compressed data, was "isic_metadata-2.0.0.tar", last modified: Mon May 20 18:31:10 2024, max compression
```

## Comparing `isic_metadata-1.9.1.tar` & `isic_metadata-2.0.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:55:06.295750 isic_metadata-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-16 16:54:53.000000 isic_metadata-1.9.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-16 16:54:53.000000 isic_metadata-1.9.1/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:55:06.287750 isic_metadata-1.9.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:55:06.291750 isic_metadata-1.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-16 16:54:53.000000 isic_metadata-1.9.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-16 16:54:53.000000 isic_metadata-1.9.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-16 16:54:53.000000 isic_metadata-1.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-16 16:54:53.000000 isic_metadata-1.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-16 16:55:06.295750 isic_metadata-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-16 16:54:53.000000 isic_metadata-1.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:55:06.291750 isic_metadata-1.9.1/isic_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-16 16:54:53.000000 isic_metadata-1.9.1/isic_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-05-16 16:54:53.000000 isic_metadata-1.9.1/isic_metadata/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    13589 2024-05-16 16:54:53.000000 isic_metadata-1.9.1/isic_metadata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:54:53.000000 isic_metadata-1.9.1/isic_metadata/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-16 16:54:53.000000 isic_metadata-1.9.1/isic_metadata/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:55:06.295750 isic_metadata-1.9.1/isic_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-16 16:55:06.000000 isic_metadata-1.9.1/isic_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-16 16:55:06.000000 isic_metadata-1.9.1/isic_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 16:55:06.000000 isic_metadata-1.9.1/isic_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-16 16:55:06.000000 isic_metadata-1.9.1/isic_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-16 16:55:06.000000 isic_metadata-1.9.1/isic_metadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-16 16:54:53.000000 isic_metadata-1.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 16:55:06.295750 isic_metadata-1.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-16 16:54:53.000000 isic_metadata-1.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:55:06.295750 isic_metadata-1.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:54:53.000000 isic_metadata-1.9.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-16 16:54:53.000000 isic_metadata-1.9.1/tests/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-05-16 16:54:53.000000 isic_metadata-1.9.1/tests/test_dependent_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-16 16:54:53.000000 isic_metadata-1.9.1/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-16 16:54:53.000000 isic_metadata-1.9.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-16 16:54:53.000000 isic_metadata-1.9.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:31:10.395531 isic_metadata-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-20 18:30:50.000000 isic_metadata-2.0.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-20 18:30:50.000000 isic_metadata-2.0.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:31:10.391531 isic_metadata-2.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:31:10.391531 isic_metadata-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-20 18:30:50.000000 isic_metadata-2.0.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-20 18:30:50.000000 isic_metadata-2.0.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-20 18:30:50.000000 isic_metadata-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-20 18:30:50.000000 isic_metadata-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-20 18:31:10.395531 isic_metadata-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-20 18:30:50.000000 isic_metadata-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:31:10.391531 isic_metadata-2.0.0/isic_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-20 18:30:50.000000 isic_metadata-2.0.0/isic_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-05-20 18:30:50.000000 isic_metadata-2.0.0/isic_metadata/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13639 2024-05-20 18:30:50.000000 isic_metadata-2.0.0/isic_metadata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 18:30:50.000000 isic_metadata-2.0.0/isic_metadata/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-20 18:30:50.000000 isic_metadata-2.0.0/isic_metadata/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:31:10.395531 isic_metadata-2.0.0/isic_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-20 18:31:10.000000 isic_metadata-2.0.0/isic_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-20 18:31:10.000000 isic_metadata-2.0.0/isic_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 18:31:10.000000 isic_metadata-2.0.0/isic_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-20 18:31:10.000000 isic_metadata-2.0.0/isic_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-20 18:31:10.000000 isic_metadata-2.0.0/isic_metadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-20 18:30:50.000000 isic_metadata-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 18:31:10.395531 isic_metadata-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-20 18:30:50.000000 isic_metadata-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:31:10.395531 isic_metadata-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 18:30:50.000000 isic_metadata-2.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-20 18:30:50.000000 isic_metadata-2.0.0/tests/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-05-20 18:30:50.000000 isic_metadata-2.0.0/tests/test_dependent_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-05-20 18:30:50.000000 isic_metadata-2.0.0/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-20 18:30:50.000000 isic_metadata-2.0.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-20 18:30:50.000000 isic_metadata-2.0.0/tox.ini
```

### Comparing `isic_metadata-1.9.1/.github/workflows/ci.yml` & `isic_metadata-2.0.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.9.1/.github/workflows/release.yml` & `isic_metadata-2.0.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.9.1/.gitignore` & `isic_metadata-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.9.1/LICENSE` & `isic_metadata-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.9.1/PKG-INFO` & `isic_metadata-2.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isic-metadata
-Version: 1.9.1
+Version: 2.0.0
 Home-page: https://github.com/ImageMarkup/isic-metadata
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/ImageMarkup/isic-metadata/issues
 Project-URL: Source, https://github.com/ImageMarkup/isic-metadata
 Keywords: requests
```

### Comparing `isic_metadata-1.9.1/isic_metadata/__init__.py` & `isic_metadata-2.0.0/isic_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.9.1/isic_metadata/fields.py` & `isic_metadata-2.0.0/isic_metadata/fields.py`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.9.1/isic_metadata/metadata.py` & `isic_metadata-2.0.0/isic_metadata/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 from collections import defaultdict
+from decimal import Decimal
 from typing import Annotated, Any, Literal
 
 from annotated_types import Ge  # noqa: TCH002
 from pydantic import (
     AfterValidator,
     BaseModel,
     BeforeValidator,
@@ -43,15 +44,15 @@
 """
 IGNORE_RCM_MODEL_CHECKS = "_ignore_rcm_model_checks"
 
 CUSTOM_MESSAGES = {
     "enum": "Unsupported value for {loc}: '{value}'.",
     "int_parsing": "Unable to parse value as an integer.",
     "bool_parsing": "Unable to parse value as a boolean.",
-    "float_parsing": "Unable to parse value as a number.",
+    "decimal_parsing": "Unable to parse value as a number.",
     "greater_than_equal": "Number must be greater than or equal to {ge}.",
 }
 
 
 def convert_errors(e: ValidationError) -> list[ErrorDetails]:
     new_errors: list[ErrorDetails] = []
     for error in e.errors():
@@ -204,23 +205,25 @@
     anatom_site_general: AnatomSiteGeneralEnum | None = None
     benign_malignant: BenignMalignantEnum | None = None
     diagnosis: DiagnosisEnum | None = None
     diagnosis_confirm_type: DiagnosisConfirmTypeEnum | None = None
     personal_hx_mm: bool | None = None
     family_hx_mm: bool | None = None
     clin_size_long_diam_mm: (
-        Annotated[float, BeforeValidator(ClinSizeLongDiamMm.parse_measurement_str)] | None
+        Annotated[Decimal, BeforeValidator(ClinSizeLongDiamMm.parse_measurement_str)] | None
     ) = None
     fitzpatrick_skin_type: FitzpatrickSkinType | None = None
     melanocytic: bool | None = None
     concomitant_biopsy: bool | None = None
 
     mel_class: MelClassEnum | None = None
     mel_mitotic_index: MelMitoticIndexEnum | None = None
-    mel_thick_mm: Annotated[float, BeforeValidator(MelThickMm.parse_measurement_str)] | None = None
+    mel_thick_mm: Annotated[Decimal, BeforeValidator(MelThickMm.parse_measurement_str)] | None = (
+        None
+    )
     mel_type: MelTypeEnum | None = None
     mel_ulcer: bool | None = None
 
     patient_id: str | None = None
     lesion_id: str | None = None
     acquisition_day: int | None = None
```

### Comparing `isic_metadata-1.9.1/isic_metadata.egg-info/PKG-INFO` & `isic_metadata-2.0.0/isic_metadata.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isic-metadata
-Version: 1.9.1
+Version: 2.0.0
 Home-page: https://github.com/ImageMarkup/isic-metadata
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/ImageMarkup/isic-metadata/issues
 Project-URL: Source, https://github.com/ImageMarkup/isic-metadata
 Keywords: requests
```

### Comparing `isic_metadata-1.9.1/isic_metadata.egg-info/SOURCES.txt` & `isic_metadata-2.0.0/isic_metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.9.1/pyproject.toml` & `isic_metadata-2.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,17 @@
   "TD002", # Missing author in TODO
   "TD003", # Missing issue link on the line following this TODO
   "TRY003", # Avoid specifying long messages outside the exception class
 
   # Excessive
   "RET503", # implict return
   "PLR2004", # magic value used in comparison
+
+  "TCH003",  # type checking blocks
+
 ]
 
 [tool.ruff.lint.per-file-ignores]
 "tests/**" = [
   "PLR0913", # Too many arguments to function call
   "PLR2004", # Magic value used in comparison
   "S", # flake8-bandit
```

### Comparing `isic_metadata-1.9.1/setup.py` & `isic_metadata-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.9.1/tests/test_batch.py` & `isic_metadata-2.0.0/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.9.1/tests/test_dependent_fields.py` & `isic_metadata-2.0.0/tests/test_dependent_fields.py`

 * *Files identical despite different names*

### Comparing `isic_metadata-1.9.1/tests/test_fields.py` & `isic_metadata-2.0.0/tests/test_fields.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from decimal import Decimal
 from typing import Any
 
 from hypothesis import given
 from hypothesis import strategies as st
 from pydantic import ValidationError
 import pytest
 
@@ -11,16 +12,16 @@
 @pytest.mark.parametrize(
     ("field", "str_value", "parsed_value", "dependent_fields"),
     # dependent_fields is a dict of field names to values are there just to satisfy
     # the field validators.
     [
         ("age", "54", 54, {}),
         ("melanocytic", "True", True, {}),
-        ("clin_size_long_diam_mm", "4mm", 4.0, {}),
-        ("mel_thick_mm", ".33mm", 0.33, {"diagnosis": "melanoma"}),
+        ("clin_size_long_diam_mm", "4mm", Decimal("4.0"), {}),
+        ("mel_thick_mm", ".33mm", Decimal("0.33"), {"diagnosis": "melanoma"}),
         ("mel_ulcer", "false", False, {"diagnosis": "melanoma"}),
         ("family_hx_mm", "False", False, {}),
         ("personal_hx_mm", "0", False, {}),
         ("acquisition_day", "142", 142, {}),
     ],
 )
 def test_non_str_types(
@@ -78,19 +79,19 @@
 def test_nevus_diagnosis():
     MetadataRow.model_validate({"diagnosis": "nevus", "nevus_type": "blue"})
 
 
 @pytest.mark.parametrize(
     ("raw", "parsed"),
     [
-        ("4.5 mm", 4.5),
-        ("14.2   mm", 14.2),
-        ("4.5mm", 4.5),
-        ("1mm", 1.0),
-        ("3.25", 3.25),
+        ("4.5 mm", Decimal("4.5")),
+        ("14.2   mm", Decimal("14.2")),
+        ("4.5mm", Decimal("4.5")),
+        ("1mm", Decimal("1.0")),
+        ("3.25", Decimal("3.25")),
     ],
 )
 def test_mel_thick_mm(raw: str, parsed: float):
     metadata = MetadataRow.model_validate({"diagnosis": "melanoma", "mel_thick_mm": raw})
     assert metadata.mel_thick_mm == parsed
 
 
@@ -98,21 +99,24 @@
     with pytest.raises(ValidationError) as excinfo:
         MetadataRow.model_validate({"mel_thick_mm": "foo"})
     assert len(excinfo.value.errors()) == 1
     assert "Unable to parse value as a number" in convert_errors(excinfo.value)[0]["msg"]
 
 
 @given(
-    clin_size=st.one_of(st.floats(min_value=0, exclude_min=True), st.integers(min_value=1)).map(
-        lambda x: f"{x} mm"
-    )
+    clin_size=st.one_of(
+        # keep max values bounded so they don't generate larger than representable decimals.
+        # disallow infinity to avoid the string 'inf'.
+        st.floats(min_value=0, max_value=1_000_000, exclude_min=True, allow_infinity=False),
+        st.integers(min_value=1, max_value=1_000),
+    ).map(lambda x: f"{x} mm")
 )
 def test_clin_size_long_diam_mm_always_rounded(clin_size: str):
     metadata = MetadataRow.model_validate({"clin_size_long_diam_mm": clin_size})
-    assert isinstance(metadata.clin_size_long_diam_mm, float)
+    assert isinstance(metadata.clin_size_long_diam_mm, Decimal)
     assert metadata.clin_size_long_diam_mm == round(metadata.clin_size_long_diam_mm, ndigits=1)
 
 
 def test_clin_size_long_diam_mm_invalid():
     with pytest.raises(ValidationError) as excinfo:
         MetadataRow.model_validate({"clin_size_long_diam_mm": "foo"})
     assert len(excinfo.value.errors()) == 1
```

### Comparing `isic_metadata-1.9.1/tox.ini` & `isic_metadata-2.0.0/tox.ini`

 * *Files identical despite different names*

