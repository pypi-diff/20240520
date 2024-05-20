# Comparing `tmp/pydantic_base_aiogram-1.0.98.tar.gz` & `tmp/pydantic_base_aiogram-1.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_base_aiogram-1.0.98.tar", max compression
+gzip compressed data, was "pydantic_base_aiogram-1.0.99.tar", max compression
```

## Comparing `pydantic_base_aiogram-1.0.98.tar` & `pydantic_base_aiogram-1.0.99.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     3089 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/README.md
--rw-r--r--   0        0        0       90 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/__init__.py
--rw-r--r--   0        0        0     1509 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/abstract_handler.py
--rw-r--r--   0        0        0      436 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/controller/__init__.py
--rw-r--r--   0        0        0      737 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/controller/abstract.py
--rw-r--r--   0        0        0     3918 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/controller/base.py
--rw-r--r--   0        0        0      486 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/controller/bool.py
--rw-r--r--   0        0        0       81 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/controller/cq_checkbox/__init__.py
--rw-r--r--   0        0        0     1681 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/controller/cq_checkbox/base.py
--rw-r--r--   0        0        0      251 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/controller/cq_checkbox/main.py
--rw-r--r--   0        0        0     2868 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/controller/cq_checkbox/multiple.py
--rw-r--r--   0        0        0      698 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/controller/cq_checkbox/single.py
--rw-r--r--   0        0        0       87 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/controller/custom_data_str/__init__.py
--rw-r--r--   0        0        0      204 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/controller/custom_data_str/base.py
--rw-r--r--   0        0        0      264 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/controller/custom_data_str/main.py
--rw-r--r--   0        0        0      247 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/controller/custom_data_str/multiple.py
--rw-r--r--   0        0        0      240 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/controller/custom_data_str/single.py
--rw-r--r--   0        0        0      978 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/controller/date_message_text.py
--rw-r--r--   0        0        0     1259 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/controller/factory.py
--rw-r--r--   0        0        0      877 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/controller/type_base_message_text.py
--rw-r--r--   0        0        0     2284 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/dialecsts.py
--rw-r--r--   0        0        0      583 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/dynamic/README.md
--rw-r--r--   0        0        0      160 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/dynamic/__init__.py
--rw-r--r--   0        0        0     2512 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/dynamic/builder.py
--rw-r--r--   0        0        0      307 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/dynamic/field_metadata.py
--rw-r--r--   0        0        0      100 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/dynamic_factory/README.md
--rw-r--r--   0        0        0        0 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/dynamic_factory/__init__.py
--rw-r--r--   0        0        0      584 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/dynamic_factory/enums.py
--rw-r--r--   0        0        0      190 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/dynamic_factory/handler.py
--rw-r--r--   0        0        0      531 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/dynamic_factory/schema.py
--rw-r--r--   0        0        0      449 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/exceptions.py
--rw-r--r--   0        0        0      169 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/field_factory/__init__.py
--rw-r--r--   0        0        0     1558 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/field_factory/base.py
--rw-r--r--   0        0        0      234 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/field_factory/enum.py
--rw-r--r--   0        0        0     1517 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/field_factory/main.py
--rw-r--r--   0        0        0     1872 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/field_factory/model.py
--rw-r--r--   0        0        0      596 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/field_factory/mult_single_splitter.py
--rw-r--r--   0        0        0     3010 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/field_factory/union.py
--rw-r--r--   0        0        0    10240 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/main.py
--rw-r--r--   0        0        0     1209 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/state_builder.py
--rw-r--r--   0        0        0     7292 2023-11-22 09:22:04.878181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/types.py
--rw-r--r--   0        0        0        0 2023-11-22 09:22:04.882181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/utils/__init__.py
--rw-r--r--   0        0        0      387 2023-11-22 09:22:04.882181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/utils/abstractions.py
--rw-r--r--   0        0        0     2140 2023-11-22 09:22:04.882181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/utils/add_more_handlers.py
--rw-r--r--   0        0        0        0 2023-11-22 09:22:04.882181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/utils/event_dialects/__init__.py
--rw-r--r--   0        0        0      222 2023-11-22 09:22:04.882181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/utils/event_dialects/base.py
--rw-r--r--   0        0        0      290 2023-11-22 09:22:04.882181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/utils/step.py
--rw-r--r--   0        0        0      321 2023-11-22 09:22:04.882181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/view/__init__.py
--rw-r--r--   0        0        0      749 2023-11-22 09:22:04.882181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/view/abstract.py
--rw-r--r--   0        0        0     5432 2023-11-22 09:22:04.882181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/view/base.py
--rw-r--r--   0        0        0      417 2023-11-22 09:22:04.882181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/view/bool.py
--rw-r--r--   0        0        0      888 2023-11-22 09:22:04.882181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/view/enum.py
--rw-r--r--   0        0        0     1626 2023-11-22 09:22:04.882181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/view/factory.py
--rw-r--r--   0        0        0      144 2023-11-22 09:22:04.882181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/view/float.py
--rw-r--r--   0        0        0      140 2023-11-22 09:22:04.882181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/view/int.py
--rw-r--r--   0        0        0     2543 2023-11-22 09:22:04.882181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/view/models.py
--rw-r--r--   0        0        0      809 2023-11-22 09:22:04.882181 pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/view/string.py
--rw-r--r--   0        0        0      451 2023-11-22 09:22:29.107960 pydantic_base_aiogram-1.0.98/pyproject.toml
--rw-r--r--   0        0        0     3691 1970-01-01 00:00:00.000000 pydantic_base_aiogram-1.0.98/PKG-INFO
+-rw-r--r--   0        0        0     3089 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/README.md
+-rw-r--r--   0        0        0       90 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/__init__.py
+-rw-r--r--   0        0        0     1509 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/abstract_handler.py
+-rw-r--r--   0        0        0      436 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/controller/__init__.py
+-rw-r--r--   0        0        0      737 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/controller/abstract.py
+-rw-r--r--   0        0        0     3918 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/controller/base.py
+-rw-r--r--   0        0        0      486 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/controller/bool.py
+-rw-r--r--   0        0        0       81 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/controller/cq_checkbox/__init__.py
+-rw-r--r--   0        0        0     1681 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/controller/cq_checkbox/base.py
+-rw-r--r--   0        0        0      251 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/controller/cq_checkbox/main.py
+-rw-r--r--   0        0        0     2868 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/controller/cq_checkbox/multiple.py
+-rw-r--r--   0        0        0      698 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/controller/cq_checkbox/single.py
+-rw-r--r--   0        0        0       87 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/controller/custom_data_str/__init__.py
+-rw-r--r--   0        0        0      204 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/controller/custom_data_str/base.py
+-rw-r--r--   0        0        0      264 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/controller/custom_data_str/main.py
+-rw-r--r--   0        0        0      247 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/controller/custom_data_str/multiple.py
+-rw-r--r--   0        0        0      240 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/controller/custom_data_str/single.py
+-rw-r--r--   0        0        0      978 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/controller/date_message_text.py
+-rw-r--r--   0        0        0     1259 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/controller/factory.py
+-rw-r--r--   0        0        0      877 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/controller/type_base_message_text.py
+-rw-r--r--   0        0        0     2284 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/dialecsts.py
+-rw-r--r--   0        0        0      583 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/dynamic/README.md
+-rw-r--r--   0        0        0      160 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/dynamic/__init__.py
+-rw-r--r--   0        0        0     2675 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/dynamic/builder.py
+-rw-r--r--   0        0        0      307 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/dynamic/field_metadata.py
+-rw-r--r--   0        0        0      100 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/dynamic_factory/README.md
+-rw-r--r--   0        0        0        0 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/dynamic_factory/__init__.py
+-rw-r--r--   0        0        0      584 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/dynamic_factory/enums.py
+-rw-r--r--   0        0        0      190 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/dynamic_factory/handler.py
+-rw-r--r--   0        0        0      531 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/dynamic_factory/schema.py
+-rw-r--r--   0        0        0      449 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/exceptions.py
+-rw-r--r--   0        0        0      169 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/field_factory/__init__.py
+-rw-r--r--   0        0        0     1558 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/field_factory/base.py
+-rw-r--r--   0        0        0      234 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/field_factory/enum.py
+-rw-r--r--   0        0        0     1517 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/field_factory/main.py
+-rw-r--r--   0        0        0     1872 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/field_factory/model.py
+-rw-r--r--   0        0        0      596 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/field_factory/mult_single_splitter.py
+-rw-r--r--   0        0        0     3010 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/field_factory/union.py
+-rw-r--r--   0        0        0    10240 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/main.py
+-rw-r--r--   0        0        0     1209 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/state_builder.py
+-rw-r--r--   0        0        0     7375 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/types.py
+-rw-r--r--   0        0        0        0 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/utils/__init__.py
+-rw-r--r--   0        0        0      387 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/utils/abstractions.py
+-rw-r--r--   0        0        0     2140 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/utils/add_more_handlers.py
+-rw-r--r--   0        0        0        0 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/utils/event_dialects/__init__.py
+-rw-r--r--   0        0        0      222 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/utils/event_dialects/base.py
+-rw-r--r--   0        0        0      290 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/utils/step.py
+-rw-r--r--   0        0        0      321 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/view/__init__.py
+-rw-r--r--   0        0        0      749 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/view/abstract.py
+-rw-r--r--   0        0        0     5432 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/view/base.py
+-rw-r--r--   0        0        0      417 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/view/bool.py
+-rw-r--r--   0        0        0      888 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/view/enum.py
+-rw-r--r--   0        0        0     1626 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/view/factory.py
+-rw-r--r--   0        0        0      144 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/view/float.py
+-rw-r--r--   0        0        0      140 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/view/int.py
+-rw-r--r--   0        0        0     2543 2023-11-24 02:17:39.886316 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/view/models.py
+-rw-r--r--   0        0        0      809 2023-11-24 02:17:39.890317 pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/view/string.py
+-rw-r--r--   0        0        0      451 2023-11-24 02:18:01.379847 pydantic_base_aiogram-1.0.99/pyproject.toml
+-rw-r--r--   0        0        0     3691 1970-01-01 00:00:00.000000 pydantic_base_aiogram-1.0.99/PKG-INFO
```

### Comparing `pydantic_base_aiogram-1.0.98/README.md` & `pydantic_base_aiogram-1.0.99/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/abstract_handler.py` & `pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/abstract_handler.py`

 * *Files identical despite different names*

### Comparing `pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/controller/abstract.py` & `pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/controller/abstract.py`

 * *Files identical despite different names*

### Comparing `pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/controller/base.py` & `pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/controller/base.py`

 * *Files identical despite different names*

### Comparing `pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/controller/cq_checkbox/base.py` & `pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/controller/cq_checkbox/base.py`

 * *Files identical despite different names*

### Comparing `pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/controller/cq_checkbox/multiple.py` & `pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/controller/cq_checkbox/multiple.py`

 * *Files identical despite different names*

### Comparing `pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/controller/cq_checkbox/single.py` & `pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/controller/cq_checkbox/single.py`

 * *Files identical despite different names*

### Comparing `pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/controller/date_message_text.py` & `pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/controller/date_message_text.py`

 * *Files identical despite different names*

### Comparing `pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/controller/factory.py` & `pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/controller/factory.py`

 * *Files identical despite different names*

### Comparing `pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/controller/type_base_message_text.py` & `pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/controller/type_base_message_text.py`

 * *Files identical despite different names*

### Comparing `pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/dialecsts.py` & `pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/dialecsts.py`

 * *Files identical despite different names*

### Comparing `pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/dynamic/README.md` & `pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/dynamic/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/dynamic/builder.py` & `pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/dynamic/builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,28 +4,31 @@
 from pydantic import BaseModel, Field
 from pydantic_base_aiogram.dynamic.field_metadata import FieldMetadata
 from pydantic_base_aiogram.main import SchemaBaseHandlersGroup
 
 
 class DynamicHandlersGroupBuilder:
     _DEFAULT_SCHEMA_NAME_POSTFIX = "Schema"
+    _DEFAULT_TBASEMODEL = BaseModel
 
     def __init__(
         self, 
         field_metadas: list[FieldMetadata], 
         getters: Optional[dict[str, Callable]] = None,
         extra_schema: Optional[list[BaseModel]] = None,
         extra_types: Optional[dict[str, type]] = None,
         schema_name_postfix: Optional[str] = None,
+        TBaseModel: Optional[Type[BaseModel]] = None,
     ) -> None:
         self._field_metadas = field_metadas
         self._getters = getters or {}
         self._extra_types = extra_types or {}
         self._schemas = extra_schema.copy() if extra_schema else []
         self._schema_name_postfix = schema_name_postfix or self._DEFAULT_SCHEMA_NAME_POSTFIX
+        self._TBaseModel = TBaseModel or self._DEFAULT_TBASEMODEL
         self._check_getters()
 
     def _check_getters(self):
         for meta in self._field_metadas:
             assert (
                 not meta._getter_name 
                 or meta._getter_name in self._getters
@@ -53,15 +56,15 @@
             field = Field(view_text=meta._view_text, getter=getter)
             property_name = str(uuid4())
             properties[property_name] = field
             types[property_name] = self._load_type(meta._type)
 
         properties['__annotations__'] = types
 
-        return type(schema_name, (BaseModel,), properties)
+        return type(schema_name, (self._TBaseModel,), properties)
     
     def _load_type(self, name: str) -> type:
         try:
             return eval(name)
         except (NameError, TypeError):
             return self._extra_types.get(name)  # type: ignore
```

### Comparing `pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/dynamic_factory/enums.py` & `pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/dynamic_factory/enums.py`

 * *Files identical despite different names*

### Comparing `pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/dynamic_factory/schema.py` & `pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/dynamic_factory/schema.py`

 * *Files identical despite different names*

### Comparing `pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/field_factory/base.py` & `pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/field_factory/base.py`

 * *Files identical despite different names*

### Comparing `pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/field_factory/main.py` & `pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/field_factory/main.py`

 * *Files identical despite different names*

### Comparing `pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/field_factory/model.py` & `pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/field_factory/model.py`

 * *Files identical despite different names*

### Comparing `pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/field_factory/mult_single_splitter.py` & `pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/field_factory/mult_single_splitter.py`

 * *Files identical despite different names*

### Comparing `pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/field_factory/union.py` & `pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/field_factory/union.py`

 * *Files identical despite different names*

### Comparing `pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/main.py` & `pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/main.py`

 * *Files identical despite different names*

### Comparing `pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/state_builder.py` & `pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/state_builder.py`

 * *Files identical despite different names*

### Comparing `pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/types.py` & `pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,16 @@
                     parent = {}
 
                 parent_elem[parent_name] = parent
 
             if isinstance(parent, list):
                 if len(parent) < 1:
                     parent.append({})
+                elif data_key in parent[-1]:
+                    parent.append({})
 
                 parent = parent[-1]
 
             parent_elem = parent
 
         if not is_list_type(self.field.outer_type_):
             parent_elem[data_key] = value
```

### Comparing `pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/utils/add_more_handlers.py` & `pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/utils/add_more_handlers.py`

 * *Files identical despite different names*

### Comparing `pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/view/abstract.py` & `pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/view/abstract.py`

 * *Files identical despite different names*

### Comparing `pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/view/base.py` & `pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/view/base.py`

 * *Files identical despite different names*

### Comparing `pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/view/enum.py` & `pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/view/enum.py`

 * *Files identical despite different names*

### Comparing `pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/view/factory.py` & `pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/view/factory.py`

 * *Files identical despite different names*

### Comparing `pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/view/models.py` & `pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/view/models.py`

 * *Files identical despite different names*

### Comparing `pydantic_base_aiogram-1.0.98/pydantic_base_aiogram/view/string.py` & `pydantic_base_aiogram-1.0.99/pydantic_base_aiogram/view/string.py`

 * *Files identical despite different names*

### Comparing `pydantic_base_aiogram-1.0.98/PKG-INFO` & `pydantic_base_aiogram-1.0.99/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-base-aiogram
-Version: 1.0.98
+Version: 1.0.99
 Summary: This code simplifies the conversion of Pydantic schemas into Aiogram handler groups, making it easy to create form-filling handlers.
 Author: axdjuraev
 Author-email: axdjuraev@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

