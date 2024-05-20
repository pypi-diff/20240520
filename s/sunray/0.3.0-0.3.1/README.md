# Comparing `tmp/sunray-0.3.0-py3-none-any.whl.zip` & `tmp/sunray-0.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 21932 bytes, number of entries: 16
+Zip file size: 21950 bytes, number of entries: 16
 -rw-r--r--  2.0 unx     2272 b- defN 80-Jan-01 00:00 sunray/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 sunray/_internal/__init__.py
 -rw-r--r--  2.0 unx    25396 b- defN 80-Jan-01 00:00 sunray/_internal/actor_mixin.py
 -rw-r--r--  2.0 unx    65315 b- defN 80-Jan-01 00:00 sunray/_internal/callable.py
--rw-r--r--  2.0 unx    15322 b- defN 80-Jan-01 00:00 sunray/_internal/core.py
+-rw-r--r--  2.0 unx    15339 b- defN 80-Jan-01 00:00 sunray/_internal/core.py
 -rw-r--r--  2.0 unx    10468 b- defN 80-Jan-01 00:00 sunray/_internal/dag.py
 -rw-r--r--  2.0 unx      658 b- defN 80-Jan-01 00:00 sunray/_internal/io.py
 -rw-r--r--  2.0 unx    11074 b- defN 80-Jan-01 00:00 sunray/_internal/remote.py
--rw-r--r--  2.0 unx    11210 b- defN 80-Jan-01 00:00 sunray/_internal/typing.py
+-rw-r--r--  2.0 unx    11288 b- defN 80-Jan-01 00:00 sunray/_internal/typing.py
 -rw-r--r--  2.0 unx      807 b- defN 80-Jan-01 00:00 sunray/_internal/util.py
 -rw-r--r--  2.0 unx      430 b- defN 80-Jan-01 00:00 sunray/dag.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 sunray/py.typed
--rw-r--r--  2.0 unx     1068 b- defN 80-Jan-01 00:00 sunray-0.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     8833 b- defN 80-Jan-01 00:00 sunray-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 sunray-0.3.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1249 b- defN 16-Jan-01 00:00 sunray-0.3.0.dist-info/RECORD
-16 files, 154190 bytes uncompressed, 19902 bytes compressed:  87.1%
+-rw-r--r--  2.0 unx     1068 b- defN 80-Jan-01 00:00 sunray-0.3.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8848 b- defN 80-Jan-01 00:00 sunray-0.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 sunray-0.3.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1249 b- defN 16-Jan-01 00:00 sunray-0.3.1.dist-info/RECORD
+16 files, 154300 bytes uncompressed, 19920 bytes compressed:  87.1%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: sunray/dag.py
 Comment: 
 
 Filename: sunray/py.typed
 Comment: 
 
-Filename: sunray-0.3.0.dist-info/LICENSE
+Filename: sunray-0.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: sunray-0.3.0.dist-info/METADATA
+Filename: sunray-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: sunray-0.3.0.dist-info/WHEEL
+Filename: sunray-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: sunray-0.3.0.dist-info/RECORD
+Filename: sunray-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sunray/__init__.py

```diff
@@ -1,12 +1,12 @@
 # ruff: noqa: E402, F401
 from __future__ import annotations
 
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 __authors__ = [
     "ZhengYu, Xu <zen-xu@outlook.com>",
 ]
 
 # re-exports from ray
 from ray._private.worker import LOCAL_MODE as LOCAL_MODE
 from ray._private.worker import RESTORE_WORKER_MODE as RESTORE_WORKER_MODE
```

## sunray/_internal/core.py

```diff
@@ -452,15 +452,15 @@
         dashboard_port: int | None = None,
         job_config: JobConfig | None = None,
         configure_logging: bool = True,
         logging_level: int = ...,
         logging_format: str | None = None,
         log_to_driver: bool = True,
         namespace: str | None = None,
-        runtime_env: RuntimeEnv | None = None,
+        runtime_env: RuntimeEnv | dict[str, Any] | None = None,
         storage: str | None = None,
         **kwargs,
     ) -> BaseContext: ...
 
     def is_initialized() -> bool: ...
 
     def shutdown(_exiting_interpreter: bool = False) -> None: ...
```

## sunray/_internal/typing.py

```diff
@@ -2,14 +2,15 @@
 
 from typing import TYPE_CHECKING
 
 
 if TYPE_CHECKING:
     import types
 
+    from typing import Any
     from typing import Union
 
     from ray import runtime_env
     from ray.util import scheduling_strategies
     from typing_extensions import Literal
     from typing_extensions import NotRequired
     from typing_extensions import Required
@@ -33,35 +34,35 @@
         max_restarts: int
         max_task_retries: int
         max_pending_calls: int
         max_concurrency: int
         name: str
         namespace: str
         lifetime: Literal["detached"] | None
-        runtime_env: RuntimeEnv
+        runtime_env: RuntimeEnv | dict[str, Any]
         concurrency_groups: dict[str, int]
         scheduling_strategy: SchedulingStrategy
 
     class FunctionRemoteOptions(TypedDict, total=False):
         num_cpus: float
         num_gpus: float
         resources: dict[str, float]
         accelerator_type: str
         memory: float
         object_store_memory: float
         max_calls: int
         max_retries: int
-        runtime_env: RuntimeEnv
+        runtime_env: RuntimeEnv | dict[str, Any]
         retry_exceptions: list[type[Exception]]
         scheduling_strategy: SchedulingStrategy
 
     class RayInitOpts(TypedDict, total=False):
         labels: dict[str, str]
         namespace: str
-        runtime_env: RuntimeEnv
+        runtime_env: RuntimeEnv | dict[str, Any]
 
     class RuntimeEnv(TypedDict, total=False):
         working_dir: str
         """
         Specifies the working directory for the Ray workers. This must either be (1) an local existing directory with total size at most 100 MiB, (2) a local existing zipped file with total unzipped size at most 100 MiB (Note: ``excludes`` has no effect), or (3) a URI to a remotely-stored zip file containing the working directory for your job (no file size limit is enforced by Ray). See :ref:`remote-uris` for details.
         The specified directory will be downloaded to each node on the cluster, and Ray workers will be started in their node's copy of this directory.
```

## Comparing `sunray-0.3.0.dist-info/LICENSE` & `sunray-0.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sunray-0.3.0.dist-info/METADATA` & `sunray-0.3.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sunray
-Version: 0.3.0
-Summary: 
+Version: 0.3.1
+Summary: More robust ray
 Author: ZhengYu, Xu
 Author-email: zen-xu@outlook.com
 Requires-Python: >=3.7,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

## Comparing `sunray-0.3.0.dist-info/RECORD` & `sunray-0.3.1.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-sunray/__init__.py,sha256=2NZbK6w7bnGNC_jPVPMokLlQotKBC3-ezjVKHIxTjOU,2272
+sunray/__init__.py,sha256=BC6dHW_8DWiM8jTvZopm3Q_11MLmvHC17yu2mLX2eIw,2272
 sunray/_internal/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sunray/_internal/actor_mixin.py,sha256=zhtKOKSdrMURT2cTf3Bq-WqVyrpiemSVt5uAToZxNBI,25396
 sunray/_internal/callable.py,sha256=eVi_mmJjOsZzVwqaP1DTfWBDF3nRMXhacBC6yT_fPpM,65315
-sunray/_internal/core.py,sha256=QE5Vgx1e50Z4N4jc6w4JnutKgtlIJTXeWQ_7xAx8ck0,15322
+sunray/_internal/core.py,sha256=eENxf9dMS5Y23saeEB1Ah3PGzYIraoRq3Sh7gAx_-bc,15339
 sunray/_internal/dag.py,sha256=B3g-Z0zVGfv7zWj2jO7eTrYsHdvzdxSel54UF_IeKU0,10468
 sunray/_internal/io.py,sha256=44YKqLW-oeKI8ehhGtc8ZhJ2yk4jx2Zrfh4pa3trNPs,658
 sunray/_internal/remote.py,sha256=Qsrql1NiiW26E_O6euuZ3U-E_RY_vz-6uqY6KdObsok,11074
-sunray/_internal/typing.py,sha256=jpgUvdGXrDN62G_fS3Ta_4l7cALlpNr5h3FcDZ58i5U,11210
+sunray/_internal/typing.py,sha256=brz_CAx45m8-28JTTqpT-5OKT3OU0N53KwF8-CyoS44,11288
 sunray/_internal/util.py,sha256=WQ6WLD_b2uY1d_6nyf24R7SbP1nqZ1CmUnzS5NMaiLA,807
 sunray/dag.py,sha256=ydCtgNVf_E2K0AFABzRhPkvlLPPUq6HQLR7QXswODJM,430
 sunray/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sunray-0.3.0.dist-info/LICENSE,sha256=4ix-bYe2BfMr6RchyTiQ2g18h5fXPTdVrjB6LLsxoaQ,1068
-sunray-0.3.0.dist-info/METADATA,sha256=XzmIGicc3y0Z5xNjzasGaJgdMQzOo2QsEcO2dWk0I2Y,8833
-sunray-0.3.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-sunray-0.3.0.dist-info/RECORD,,
+sunray-0.3.1.dist-info/LICENSE,sha256=4ix-bYe2BfMr6RchyTiQ2g18h5fXPTdVrjB6LLsxoaQ,1068
+sunray-0.3.1.dist-info/METADATA,sha256=d5q-9naDnhf9_UVjOM1l6sNw4AROtP7QOOf8Lmwnstw,8848
+sunray-0.3.1.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+sunray-0.3.1.dist-info/RECORD,,
```

