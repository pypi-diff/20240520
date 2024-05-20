# Comparing `tmp/ftmq-0.6.4.tar.gz` & `tmp/ftmq-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftmq-0.6.4.tar", max compression
+gzip compressed data, was "ftmq-0.6.5.tar", max compression
```

## Comparing `ftmq-0.6.4.tar` & `ftmq-0.6.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1077 2023-04-04 14:31:45.930293 ftmq-0.6.4/LICENSE
--rw-r--r--   0        0        0     4741 2024-01-31 02:14:30.592540 ftmq-0.6.4/README.md
--rw-r--r--   0        0        0       72 2024-05-17 10:45:05.608660 ftmq-0.6.4/ftmq/__init__.py
--rw-r--r--   0        0        0     2011 2024-01-03 16:54:37.194210 ftmq-0.6.4/ftmq/aggregate.py
--rw-r--r--   0        0        0     4790 2024-03-14 08:37:57.172570 ftmq-0.6.4/ftmq/aggregations.py
--rw-r--r--   0        0        0     4059 2024-03-14 17:13:11.419765 ftmq-0.6.4/ftmq/aleph.py
--rw-r--r--   0        0        0    10790 2024-04-04 12:20:24.054303 ftmq-0.6.4/ftmq/cli.py
--rw-r--r--   0        0        0      580 2024-02-23 20:01:04.717383 ftmq-0.6.4/ftmq/dedupe.py
--rw-r--r--   0        0        0     2517 2024-02-24 16:21:44.983220 ftmq-0.6.4/ftmq/enums.py
--rw-r--r--   0        0        0       93 2023-10-14 09:45:57.814196 ftmq-0.6.4/ftmq/exceptions.py
--rw-r--r--   0        0        0     7069 2023-10-14 09:45:57.814196 ftmq-0.6.4/ftmq/filters.py
--rw-r--r--   0        0        0     2807 2024-02-24 16:21:02.863390 ftmq-0.6.4/ftmq/io.py
--rw-r--r--   0        0        0      292 2024-03-13 18:50:42.659003 ftmq-0.6.4/ftmq/model/__init__.py
--rw-r--r--   0        0        0     4090 2024-03-13 19:40:59.788009 ftmq-0.6.4/ftmq/model/coverage.py
--rw-r--r--   0        0        0     5051 2024-05-17 10:17:43.525455 ftmq-0.6.4/ftmq/model/dataset.py
--rw-r--r--   0        0        0      482 2024-02-26 10:46:34.773368 ftmq-0.6.4/ftmq/model/mixins.py
--rw-r--r--   0        0        0     1866 2024-04-04 13:32:02.291870 ftmq-0.6.4/ftmq/model/proxy.py
--rw-r--r--   0        0        0    10276 2024-03-14 08:34:41.217377 ftmq-0.6.4/ftmq/query.py
--rw-r--r--   0        0        0    12223 2024-03-14 07:39:24.177208 ftmq-0.6.4/ftmq/sql.py
--rw-r--r--   0        0        0     2054 2024-03-14 05:58:47.124786 ftmq-0.6.4/ftmq/store/__init__.py
--rw-r--r--   0        0        0     1310 2024-02-24 16:21:45.719217 ftmq-0.6.4/ftmq/store/aleph.py
--rw-r--r--   0        0        0     3362 2024-03-14 08:35:41.593130 ftmq-0.6.4/ftmq/store/base.py
--rw-r--r--   0        0        0      768 2024-02-24 16:21:45.719217 ftmq-0.6.4/ftmq/store/level.py
--rw-r--r--   0        0        0      550 2024-03-13 18:57:03.036638 ftmq-0.6.4/ftmq/store/memory.py
--rw-r--r--   0        0        0      441 2024-02-23 20:01:36.309188 ftmq-0.6.4/ftmq/store/redis.py
--rw-r--r--   0        0        0     4878 2024-03-13 18:57:03.036638 ftmq-0.6.4/ftmq/store/sql.py
--rw-r--r--   0        0        0     1118 2024-04-04 12:11:45.481029 ftmq-0.6.4/ftmq/types.py
--rw-r--r--   0        0        0     5963 2024-04-04 12:14:29.656166 ftmq-0.6.4/ftmq/util.py
--rw-r--r--   0        0        0     1755 2024-05-17 10:45:05.608660 ftmq-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     6197 1970-01-01 00:00:00.000000 ftmq-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-04 14:31:45.930293 ftmq-0.6.5/LICENSE
+-rw-r--r--   0        0        0     4741 2024-05-18 23:30:42.996434 ftmq-0.6.5/README.md
+-rw-r--r--   0        0        0       72 2024-05-20 17:33:22.484001 ftmq-0.6.5/ftmq/__init__.py
+-rw-r--r--   0        0        0     2011 2024-01-03 16:54:37.194210 ftmq-0.6.5/ftmq/aggregate.py
+-rw-r--r--   0        0        0     4790 2024-05-18 23:30:42.996434 ftmq-0.6.5/ftmq/aggregations.py
+-rw-r--r--   0        0        0     4059 2024-05-18 23:30:42.996434 ftmq-0.6.5/ftmq/aleph.py
+-rw-r--r--   0        0        0    10790 2024-05-18 23:30:42.996434 ftmq-0.6.5/ftmq/cli.py
+-rw-r--r--   0        0        0      580 2024-05-18 23:30:43.000434 ftmq-0.6.5/ftmq/dedupe.py
+-rw-r--r--   0        0        0     2517 2024-05-18 23:30:43.000434 ftmq-0.6.5/ftmq/enums.py
+-rw-r--r--   0        0        0       93 2023-10-14 09:45:57.814196 ftmq-0.6.5/ftmq/exceptions.py
+-rw-r--r--   0        0        0     7069 2023-10-14 09:45:57.814196 ftmq-0.6.5/ftmq/filters.py
+-rw-r--r--   0        0        0     2807 2024-05-18 23:30:43.000434 ftmq-0.6.5/ftmq/io.py
+-rw-r--r--   0        0        0      292 2024-05-18 23:30:43.000434 ftmq-0.6.5/ftmq/model/__init__.py
+-rw-r--r--   0        0        0     4090 2024-05-18 23:30:43.000434 ftmq-0.6.5/ftmq/model/coverage.py
+-rw-r--r--   0        0        0     5051 2024-05-18 23:30:43.000434 ftmq-0.6.5/ftmq/model/dataset.py
+-rw-r--r--   0        0        0      482 2024-05-18 23:30:43.000434 ftmq-0.6.5/ftmq/model/mixins.py
+-rw-r--r--   0        0        0     1866 2024-05-18 23:30:43.000434 ftmq-0.6.5/ftmq/model/proxy.py
+-rw-r--r--   0        0        0    10276 2024-05-18 23:30:43.000434 ftmq-0.6.5/ftmq/query.py
+-rw-r--r--   0        0        0    12497 2024-05-19 02:10:21.045339 ftmq-0.6.5/ftmq/sql.py
+-rw-r--r--   0        0        0     2354 2024-05-20 17:29:43.689193 ftmq-0.6.5/ftmq/store/__init__.py
+-rw-r--r--   0        0        0     1310 2024-05-18 23:30:43.000434 ftmq-0.6.5/ftmq/store/aleph.py
+-rw-r--r--   0        0        0     3550 2024-05-20 16:56:14.420840 ftmq-0.6.5/ftmq/store/base.py
+-rw-r--r--   0        0        0      768 2024-05-18 23:30:43.000434 ftmq-0.6.5/ftmq/store/level.py
+-rw-r--r--   0        0        0      550 2024-05-18 23:30:43.000434 ftmq-0.6.5/ftmq/store/memory.py
+-rw-r--r--   0        0        0      441 2024-05-18 23:30:43.000434 ftmq-0.6.5/ftmq/store/redis.py
+-rw-r--r--   0        0        0     5161 2024-05-19 02:10:21.045339 ftmq-0.6.5/ftmq/store/sql.py
+-rw-r--r--   0        0        0     1118 2024-05-18 23:30:43.000434 ftmq-0.6.5/ftmq/types.py
+-rw-r--r--   0        0        0     6147 2024-05-20 16:54:27.350737 ftmq-0.6.5/ftmq/util.py
+-rw-r--r--   0        0        0     1828 2024-05-20 17:33:22.484001 ftmq-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0     6193 1970-01-01 00:00:00.000000 ftmq-0.6.5/PKG-INFO
```

### Comparing `ftmq-0.6.4/LICENSE` & `ftmq-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.4/README.md` & `ftmq-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.4/ftmq/aggregate.py` & `ftmq-0.6.5/ftmq/aggregate.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.4/ftmq/aggregations.py` & `ftmq-0.6.5/ftmq/aggregations.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.4/ftmq/aleph.py` & `ftmq-0.6.5/ftmq/aleph.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.4/ftmq/cli.py` & `ftmq-0.6.5/ftmq/cli.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.4/ftmq/dedupe.py` & `ftmq-0.6.5/ftmq/dedupe.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.4/ftmq/enums.py` & `ftmq-0.6.5/ftmq/enums.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.4/ftmq/filters.py` & `ftmq-0.6.5/ftmq/filters.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.4/ftmq/io.py` & `ftmq-0.6.5/ftmq/io.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.4/ftmq/model/coverage.py` & `ftmq-0.6.5/ftmq/model/coverage.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.4/ftmq/model/dataset.py` & `ftmq-0.6.5/ftmq/model/dataset.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.4/ftmq/model/proxy.py` & `ftmq-0.6.5/ftmq/model/proxy.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.4/ftmq/query.py` & `ftmq-0.6.5/ftmq/query.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.4/ftmq/sql.py` & `ftmq-0.6.5/ftmq/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -309,14 +309,16 @@
     def aggregations(self) -> Select:
         qs = []
         for agg in self.q.aggregations:
             sql_agg = getattr(func, agg.func)
             sql_agg_value = self.table.c.value
             if agg.func == Aggregations.count:
                 sql_agg_value = distinct(sql_agg_value)
+            elif agg.func in (Aggregations.sum, Aggregations.avg):
+                sql_agg_value = func.cast(sql_agg_value, NUMERIC)
             aggregator = sql_agg(sql_agg_value)
             qs.append(
                 select(
                     text(f"'{agg.prop}'"),
                     text(f"'{agg.func}'"),
                     aggregator,
                 ).where(
@@ -350,14 +352,16 @@
                 if agg.prop in self.META_COLUMNS:
                     sql_agg_value = self._get_lookup_column(agg.prop)
                 else:
                     sql_agg_value = self.table.c.value
                 sql_agg = getattr(func, agg.func)
                 if agg.func == Aggregations.count:
                     sql_agg_value = distinct(sql_agg_value)
+                elif agg.func in (Aggregations.sum, Aggregations.avg):
+                    sql_agg_value = func.cast(sql_agg_value, NUMERIC)
                 aggregator = sql_agg(sql_agg_value)
 
                 inner = select(self.table.c.canonical_id.distinct()).where(
                     *self._get_grouping_where(grouper, group)
                 )
 
                 qs.append(
```

### Comparing `ftmq-0.6.4/ftmq/store/__init__.py` & `ftmq-0.6.5/ftmq/store/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,21 @@
     if parsed.scheme == "redis":
         try:
             from ftmq.store.redis import RedisStore
 
             return RedisStore(catalog, dataset, path=path, resolver=resolver)
         except ImportError:
             raise ImportError("Can not load RedisStore. Install `redis`")
+    if parsed.scheme == "clickhouse":
+        try:
+            from ftm_columnstore import get_store as get_cstore
+
+            return get_cstore(catalog, dataset, resolver=resolver)
+        except ImportError:
+            raise ImportError("Can not load ClickhouseStore. Install `ftm-columnstore`")
     if "sql" in parsed.scheme:
         get_metadata.cache_clear()
         return SQLStore(catalog, dataset, uri=uri, resolver=resolver)
     if "aleph" in parsed.scheme:
         return AlephStore.from_uri(
             uri, catalog=catalog, dataset=dataset, resolver=resolver
         )
```

### Comparing `ftmq-0.6.4/ftmq/store/aleph.py` & `ftmq-0.6.5/ftmq/store/aleph.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.4/ftmq/store/base.py` & `ftmq-0.6.5/ftmq/store/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from nomenklatura.resolver import Resolver
 
 from ftmq.aggregations import AggregatorResult
 from ftmq.model.coverage import Collector, DatasetStats
 from ftmq.model.dataset import C, Dataset
 from ftmq.query import Q
 from ftmq.types import CE, CEGenerator
-from ftmq.util import DefaultDataset, make_dataset
+from ftmq.util import DefaultDataset, ensure_dataset, make_dataset
 
 log = logging.getLogger(__name__)
 
 
 class Store(nk.Store):
     def __init__(
         self,
@@ -32,17 +32,21 @@
             dataset = DefaultDataset
         super().__init__(dataset=dataset, resolver=resolver or Resolver(), **kwargs)
 
     def get_catalog(self) -> C:
         # return implicit catalog computed from current datasets in store
         raise NotImplementedError
 
-    def iterate(self) -> CEGenerator:
-        catalog = self.get_catalog()
-        view = self.view(catalog.get_scope())
+    def iterate(self, dataset: str | Dataset | None = None) -> CEGenerator:
+        dataset = ensure_dataset(dataset)
+        if dataset is not None:
+            view = self.view(dataset)
+        else:
+            catalog = self.get_catalog()
+            view = self.view(catalog.get_scope())
         yield from view.entities()
 
     def resolve(self, dataset: str | Dataset | None = None) -> None:
         if not self.resolver.edges:
             return
         if dataset is not None:
             if isinstance(dataset, str):
```

### Comparing `ftmq-0.6.4/ftmq/store/level.py` & `ftmq-0.6.5/ftmq/store/level.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.4/ftmq/store/memory.py` & `ftmq-0.6.5/ftmq/store/memory.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.4/ftmq/store/sql.py` & `ftmq-0.6.5/ftmq/store/sql.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 import os
 from collections import defaultdict
 from datetime import date
+from decimal import Decimal
 
 from anystore.util import clean_dict
 from nomenklatura import store as nk
 from nomenklatura.dataset import DS
 from sqlalchemy import select
 
 from ftmq.aggregations import AggregatorResult
 from ftmq.enums import Fields
 from ftmq.exceptions import ValidationError
 from ftmq.model.coverage import Collector, DatasetStats
 from ftmq.model.dataset import Catalog
 from ftmq.query import Q, Query
 from ftmq.store.base import Store, View
 from ftmq.types import CEGenerator
+from ftmq.util import to_numeric
 
 MAX_SQL_AGG_GROUPS = int(os.environ.get("MAX_SQL_AGG_GROUPS", 10))
 
 
+def clean_agg_value(value: str | Decimal) -> str | float | int | None:
+    if isinstance(value, Decimal):
+        return to_numeric(value)
+    return value
+
+
 class SQLQueryView(View, nk.sql.SQLView):
     def ensure_scoped_query(self, query: Q) -> Q:
         if not query.datasets:
             return query.where(dataset__in=self.dataset_names)
         if query.dataset_names - self.dataset_names:
             raise ValidationError("Query datasets outside view scope")
         return query
@@ -54,17 +62,17 @@
         for country, count in self.store._execute(
             query.sql.intervals_countries, stream=False
         ):
             if country is not None:
                 c.intervals_countries[country] = count
         stats = c.export()
         for start, end in self.store._execute(query.sql.date_range, stream=False):
-            if start is not None:
+            if start:
                 stats.coverage.start = date.fromisoformat(start)
-            if end is not None:
+            if end:
                 stats.coverage.end = date.fromisoformat(end)
             break
 
         for res in self.store._execute(query.sql.countries, stream=False):
             stats.coverage.countries.append(res)
 
         for res in self.store._execute(query.sql.count, stream=False):
@@ -82,15 +90,15 @@
         if key in self._cache:
             return self._cache[key]
         res: AggregatorResult = defaultdict(dict)
 
         for prop, func, value in self.store._execute(
             query.sql.aggregations, stream=False
         ):
-            res[func][prop] = value
+            res[func][prop] = clean_agg_value(value)
 
         if query.sql.group_props:
             res["groups"] = defaultdict(lambda: defaultdict(lambda: defaultdict(dict)))
             for prop in query.sql.group_props:
                 if prop == Fields.year:
                     start, end = self.stats(query).coverage.years
                     if start or end:
@@ -105,15 +113,17 @@
                             stream=False,
                         )
                     ]
                 for group in groups:
                     for agg_prop, func, value in self.store._execute(
                         query.sql.get_group_aggregations(prop, group), stream=False
                     ):
-                        res["groups"][prop][func][agg_prop][group] = value
+                        res["groups"][prop][func][agg_prop][group] = clean_agg_value(
+                            value
+                        )
         res = clean_dict(res)
         self._cache[key] = res
         return res
 
 
 class SQLStore(Store, nk.SQLStore):
     def get_catalog(self) -> Catalog:
```

### Comparing `ftmq-0.6.4/ftmq/types.py` & `ftmq-0.6.5/ftmq/types.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.4/ftmq/util.py` & `ftmq-0.6.5/ftmq/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,23 @@
 
 
 @cache
 def make_dataset(name: str) -> Dataset:
     return Dataset.make({"name": name, "title": name})
 
 
+@cache
+def ensure_dataset(ds: str | Dataset | None = None) -> Dataset | None:
+    if not ds:
+        return
+    if isinstance(ds, str):
+        return make_dataset(ds)
+    return ds
+
+
 DefaultDataset = make_dataset("default")
 
 
 def parse_comparator(key: str) -> tuple[str, Comparators]:
     key, *comparator = key.split("__", 1)
     if comparator:
         comparator = Comparators[comparator[0]]
```

### Comparing `ftmq-0.6.4/pyproject.toml` & `ftmq-0.6.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ftmq"
-version = "0.6.4"
+version = "0.6.5"
 description = "followthemoney query dsl and io helpers"
 authors = ["Simon Wörpel <simon.woerpel@pm.me>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/investigativedata/ftmq"
 repository = "https://github.com/investigativedata/ftmq"
 documentation = "https://github.com/investigativedata/ftmq"
@@ -34,15 +34,15 @@
 cryptography = "^42.0.7"
 certifi = ">=2024.2.2"
 pydantic = "^2.7.1"
 sqlalchemy = "^2.0.30"
 alephclient = "^2.4.1"
 pycountry = "^23.12.11"
 urllib3 = "<3"
-nomenklatura = "^3.10.6"
+nomenklatura = ">3.10,<3.11"
 anystore = "^0.1.3"
 pantomime = "^0.6.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.4.3,<9.0.0"
 pytest-cov = ">=4.1,<6.0"
 black = ">=23.11,<25.0"
@@ -52,20 +52,20 @@
 flake8 = ">=6.1,<8.0"
 ipdb = "^0.13.13"
 bump2version = "^1.0.1"
 cloudpickle = ">=2.2.1,<4.0.0"
 pytest-env = "^1.1.1"
 bump-pydantic = ">=0.7,<0.9"
 
-
+[tool.poetry.group.clickhouse.dependencies]
+ftm-columnstore = "^0.3.0"
 
 [tool.poetry.group.level.dependencies]
 plyvel = "^1.5.1"
 
-
 [tool.poetry.group.redis.dependencies]
 redis = "^5.0.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ftmq-0.6.4/PKG-INFO` & `ftmq-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftmq
-Version: 0.6.4
+Version: 0.6.5
 Summary: followthemoney query dsl and io helpers
 Home-page: https://github.com/investigativedata/ftmq
 License: MIT
 Author: Simon Wörpel
 Author-email: simon.woerpel@pm.me
 Requires-Python: >=3.11,<3.12
 Classifier: Intended Audience :: Developers
@@ -18,15 +18,15 @@
 Requires-Dist: anystore (>=0.1.3,<0.2.0)
 Requires-Dist: banal (>=1.0.6,<2.0.0)
 Requires-Dist: certifi (>=2024.2.2)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: click-default-group (>=1.2.4,<2.0.0)
 Requires-Dist: cryptography (>=42.0.7,<43.0.0)
 Requires-Dist: followthemoney (>=3.6.0,<4.0.0)
-Requires-Dist: nomenklatura (>=3.10.6,<4.0.0)
+Requires-Dist: nomenklatura (>3.10,<3.11)
 Requires-Dist: orjson (>=3.10.3,<4.0.0)
 Requires-Dist: pantomime (>=0.6.1,<0.7.0)
 Requires-Dist: pycountry (>=23.12.11,<24.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: sqlalchemy (>=2.0.30,<3.0.0)
 Requires-Dist: urllib3 (<3)
 Project-URL: Bug Tracker, https://github.com/investigativedata/ftmq/issues
```

