# Comparing `tmp/paicorelib-1.1.1.tar.gz` & `tmp/paicorelib-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paicorelib-1.1.1.tar", max compression
+gzip compressed data, was "paicorelib-1.1.2.tar", max compression
```

## Comparing `paicorelib-1.1.1.tar` & `paicorelib-1.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      247 2024-05-18 06:43:21.852710 paicorelib-1.1.1/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2024-05-18 06:43:21.852710 paicorelib-1.1.1/LICENSE
--rw-r--r--   0        0        0      833 2024-05-18 06:43:21.852710 paicorelib-1.1.1/README.md
--rw-r--r--   0        0        0     1775 2024-05-18 06:43:21.852710 paicorelib-1.1.1/docs/Table-of-Terms.md
--rw-r--r--   0        0        0     1188 2024-05-18 06:43:21.852710 paicorelib-1.1.1/paicorelib/__init__.py
--rw-r--r--   0        0        0    15668 2024-05-18 06:43:21.852710 paicorelib-1.1.1/paicorelib/coordinate.py
--rw-r--r--   0        0        0       81 2024-05-18 06:43:21.852710 paicorelib-1.1.1/paicorelib/framelib/__init__.py
--rw-r--r--   0        0        0     5212 2024-05-18 06:43:21.852710 paicorelib-1.1.1/paicorelib/framelib/base.py
--rw-r--r--   0        0        0     7150 2024-05-18 06:43:21.852710 paicorelib-1.1.1/paicorelib/framelib/frame_defs.py
--rw-r--r--   0        0        0     9900 2024-05-18 06:43:21.852710 paicorelib-1.1.1/paicorelib/framelib/frame_gen.py
--rw-r--r--   0        0        0    22001 2024-05-18 06:43:21.852710 paicorelib-1.1.1/paicorelib/framelib/frames.py
--rw-r--r--   0        0        0      736 2024-05-18 06:43:21.852710 paicorelib-1.1.1/paicorelib/framelib/types.py
--rw-r--r--   0        0        0     4034 2024-05-18 06:43:21.852710 paicorelib-1.1.1/paicorelib/framelib/utils.py
--rw-r--r--   0        0        0     1532 2024-05-18 06:43:21.852710 paicorelib-1.1.1/paicorelib/hw_defs.py
--rw-r--r--   0        0        0     2312 2024-05-18 06:43:21.852710 paicorelib-1.1.1/paicorelib/hw_types.py
--rw-r--r--   0        0        0     7488 2024-05-18 06:43:21.852710 paicorelib-1.1.1/paicorelib/ram_model.py
--rw-r--r--   0        0        0     2618 2024-05-18 06:43:21.852710 paicorelib-1.1.1/paicorelib/ram_types.py
--rw-r--r--   0        0        0     5816 2024-05-18 06:43:21.852710 paicorelib-1.1.1/paicorelib/reg_model.py
--rw-r--r--   0        0        0     4265 2024-05-18 06:43:21.852710 paicorelib-1.1.1/paicorelib/reg_types.py
--rw-r--r--   0        0        0     5747 2024-05-18 06:43:21.852710 paicorelib-1.1.1/paicorelib/routing_defs.py
--rw-r--r--   0        0        0     1729 2024-05-18 06:43:21.852710 paicorelib-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     2097 1970-01-01 00:00:00.000000 paicorelib-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      308 2024-05-20 06:16:24.892903 paicorelib-1.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2024-05-20 06:16:24.892903 paicorelib-1.1.2/LICENSE
+-rw-r--r--   0        0        0      833 2024-05-20 06:16:24.892903 paicorelib-1.1.2/README.md
+-rw-r--r--   0        0        0     1775 2024-05-20 06:16:24.892903 paicorelib-1.1.2/docs/Table-of-Terms.md
+-rw-r--r--   0        0        0     1188 2024-05-20 06:16:24.892903 paicorelib-1.1.2/paicorelib/__init__.py
+-rw-r--r--   0        0        0    15668 2024-05-20 06:16:24.892903 paicorelib-1.1.2/paicorelib/coordinate.py
+-rw-r--r--   0        0        0       81 2024-05-20 06:16:24.892903 paicorelib-1.1.2/paicorelib/framelib/__init__.py
+-rw-r--r--   0        0        0     5212 2024-05-20 06:16:24.892903 paicorelib-1.1.2/paicorelib/framelib/base.py
+-rw-r--r--   0        0        0     7009 2024-05-20 06:16:24.892903 paicorelib-1.1.2/paicorelib/framelib/frame_defs.py
+-rw-r--r--   0        0        0     9900 2024-05-20 06:16:24.892903 paicorelib-1.1.2/paicorelib/framelib/frame_gen.py
+-rw-r--r--   0        0        0    22228 2024-05-20 06:16:24.892903 paicorelib-1.1.2/paicorelib/framelib/frames.py
+-rw-r--r--   0        0        0      736 2024-05-20 06:16:24.892903 paicorelib-1.1.2/paicorelib/framelib/types.py
+-rw-r--r--   0        0        0     4077 2024-05-20 06:16:24.892903 paicorelib-1.1.2/paicorelib/framelib/utils.py
+-rw-r--r--   0        0        0     1532 2024-05-20 06:16:24.892903 paicorelib-1.1.2/paicorelib/hw_defs.py
+-rw-r--r--   0        0        0     2312 2024-05-20 06:16:24.892903 paicorelib-1.1.2/paicorelib/hw_types.py
+-rw-r--r--   0        0        0     7488 2024-05-20 06:16:24.892903 paicorelib-1.1.2/paicorelib/ram_model.py
+-rw-r--r--   0        0        0     2618 2024-05-20 06:16:24.892903 paicorelib-1.1.2/paicorelib/ram_types.py
+-rw-r--r--   0        0        0     5816 2024-05-20 06:16:24.892903 paicorelib-1.1.2/paicorelib/reg_model.py
+-rw-r--r--   0        0        0     4265 2024-05-20 06:16:24.892903 paicorelib-1.1.2/paicorelib/reg_types.py
+-rw-r--r--   0        0        0     5747 2024-05-20 06:16:24.892903 paicorelib-1.1.2/paicorelib/routing_defs.py
+-rw-r--r--   0        0        0     1729 2024-05-20 06:16:24.892903 paicorelib-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2097 1970-01-01 00:00:00.000000 paicorelib-1.1.2/PKG-INFO
```

### Comparing `paicorelib-1.1.1/LICENSE` & `paicorelib-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `paicorelib-1.1.1/README.md` & `paicorelib-1.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 </div>
 
 <p align="center">
     <a href="https://github.com/PAICookers/PAIlib/blob/master/pyproject.toml">
         <img src="https://img.shields.io/pypi/pyversions/paicorelib">
     </a>
-    <a href="https://github.com/PAICookers/PAIlib/releases/tag/v1.1.1"
+    <a href="https://github.com/PAICookers/PAIlib/releases/tag/v1.1.2"
         <img src="https://img.shields.io/github/v/release/PAICookers/PAIlib?color=orange">
     </a>
     <a href="https://www.codefactor.io/repository/github/PAICookers/PAIlib">
       <img src="https://img.shields.io/codefactor/grade/github/PAICookers/PAIlib/master?color=red">
     </a>
     <a href="https://results.pre-commit.ci/latest/github/PAICookers/PAIlib/master">
 	   <img src="https://results.pre-commit.ci/badge/github/PAICookers/PAIlib/master.svg" alt="pre-commit.ci status">
```

### Comparing `paicorelib-1.1.1/docs/Table-of-Terms.md` & `paicorelib-1.1.2/docs/Table-of-Terms.md`

 * *Files identical despite different names*

### Comparing `paicorelib-1.1.1/paicorelib/__init__.py` & `paicorelib-1.1.2/paicorelib/__init__.py`

 * *Files identical despite different names*

### Comparing `paicorelib-1.1.1/paicorelib/coordinate.py` & `paicorelib-1.1.2/paicorelib/coordinate.py`

 * *Files identical despite different names*

### Comparing `paicorelib-1.1.1/paicorelib/framelib/base.py` & `paicorelib-1.1.2/paicorelib/framelib/base.py`

 * *Files identical despite different names*

### Comparing `paicorelib-1.1.1/paicorelib/framelib/frame_defs.py` & `paicorelib-1.1.2/paicorelib/framelib/frame_defs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from enum import IntEnum, unique
 
 
+def _mask(mask_bit: int) -> int:
+    return (1 << mask_bit) - 1
+
+
 @unique
 class FrameType(IntEnum):
     """Types of Frames"""
 
     FRAME_CONFIG = 0
     FRAME_TEST = 0x1
     FRAME_WORK = 0x2
@@ -37,71 +41,71 @@
     WORK_TYPE4 = 0b1011
     """Type IV, init"""
 
 
 class FrameFormat:
     """General frame mask & offset."""
 
-    GENERAL_MASK = (1 << 64) - 1
+    GENERAL_MASK = _mask(64)
 
     # Header
     GENERAL_HEADER_OFFSET = 60
-    GENERAL_HEADER_MASK = (1 << 4) - 1
+    GENERAL_HEADER_MASK = _mask(4)
 
     GENERAL_FRAME_TYPE_OFFSET = GENERAL_HEADER_OFFSET
     GENERAL_FRAME_TYPE_MASK = GENERAL_HEADER_MASK
 
     # Chip address
     GENERAL_CHIP_ADDR_OFFSET = 50
-    GENERAL_CHIP_ADDR_MASK = (1 << 10) - 1
+    GENERAL_CHIP_ADDR_MASK = _mask(10)
     # Chip X/Y address
     GENERAL_CHIP_X_ADDR_OFFSET = 55
-    GENERAL_CHIP_X_ADDR_MASK = (1 << 5) - 1
+    GENERAL_CHIP_X_ADDR_MASK = _mask(5)
     GENERAL_CHIP_Y_ADDR_OFFSET = GENERAL_CHIP_ADDR_OFFSET
-    GENERAL_CHIP_Y_ADDR_MASK = (1 << 5) - 1
+    GENERAL_CHIP_Y_ADDR_MASK = _mask(5)
 
     # Core address
     GENERAL_CORE_ADDR_OFFSET = 40
-    GENERAL_CORE_ADDR_MASK = (1 << 10) - 1
+    GENERAL_CORE_ADDR_MASK = _mask(10)
     # Core X/Y address
     GENERAL_CORE_X_ADDR_OFFSET = 45
-    GENERAL_CORE_X_ADDR_MASK = (1 << 5) - 1
+    GENERAL_CORE_X_ADDR_MASK = _mask(5)
     GENERAL_CORE_Y_ADDR_OFFSET = GENERAL_CORE_ADDR_OFFSET
-    GENERAL_CORE_Y_ADDR_MASK = (1 << 5) - 1
+    GENERAL_CORE_Y_ADDR_MASK = _mask(5)
 
     # Core* address
     GENERAL_CORE_EX_ADDR_OFFSET = 30
-    GENERAL_CORE_EX_ADDR_MASK = (1 << 10) - 1
+    GENERAL_CORE_EX_ADDR_MASK = _mask(10)
     # Core* X/Y address
     GENERAL_CORE_X_EX_ADDR_OFFSET = 35
-    GENERAL_CORE_X_EX_ADDR_MASK = (1 << 5) - 1
+    GENERAL_CORE_X_EX_ADDR_MASK = _mask(5)
     GENERAL_CORE_Y_EX_ADDR_OFFSET = GENERAL_CORE_EX_ADDR_OFFSET
-    GENERAL_CORE_Y_EX_ADDR_MASK = (1 << 5) - 1
+    GENERAL_CORE_Y_EX_ADDR_MASK = _mask(5)
 
     # Global core = Chip address + core address
     GENERAL_CORE_GLOBAL_ADDR_OFFSET = GENERAL_CORE_ADDR_OFFSET
-    GENERAL_CORE_GLOBAL_ADDR_MASK = (1 << 20) - 1
+    GENERAL_CORE_GLOBAL_ADDR_MASK = _mask(20)
 
     # Frame 前34位
     GENERAL_FRAME_PRE_OFFSET = 30
-    GENERAL_FRAME_PRE_MASK = (1 << 34) - 1
+    GENERAL_FRAME_PRE_MASK = _mask(34)
 
     # 通用数据帧LOAD掩码
     GENERAL_PAYLOAD_OFFSET = 0
-    GENERAL_PAYLOAD_MASK = (1 << 30) - 1
+    GENERAL_PAYLOAD_MASK = _mask(30)
 
     # 通用数据包LOAD掩码
     GENERAL_PACKAGE_SRAM_ADDR_OFFSET = 20
-    GENERAL_PACKAGE_SRAM_ADDR_MASK = (1 << 10) - 1
+    GENERAL_PACKAGE_SRAM_ADDR_MASK = _mask(10)
 
     GENERAL_PACKAGE_TYPE_OFFSET = 19
-    GENERAL_PACKAGE_TYPE_MASK = 1
+    GENERAL_PACKAGE_TYPE_MASK = _mask(1)
 
     GENERAL_PACKAGE_NUM_OFFSET = 0
-    GENERAL_PACKAGE_NUM_MASK = (1 << 19) - 1
+    GENERAL_PACKAGE_NUM_MASK = _mask(19)
 
 
 class OfflineFrameFormat(FrameFormat):
     """Basic offline frame format"""
 
     pass
 
@@ -119,136 +123,136 @@
 
 
 class OfflineConfigFrame2Format(OfflineFrameFormat):
     """Offline config frame type II, parameter REG"""
 
     # Frame #1
     WEIGHT_WIDTH_OFFSET = 28
-    WEIGHT_WIDTH_MASK = (1 << 2) - 1
+    WEIGHT_WIDTH_MASK = _mask(2)
 
     LCN_OFFSET = 24
-    LCN_MASK = (1 << 4) - 1
+    LCN_MASK = _mask(4)
 
     INPUT_WIDTH_OFFSET = 23
     INPUT_WIDTH_MASK = 1
 
     SPIKE_WIDTH_OFFSET = 22
     SPIKE_WIDTH_MASK = 1
 
     NEURON_NUM_OFFSET = 9
-    NEURON_NUM_MASK = (1 << 13) - 1
+    NEURON_NUM_MASK = _mask(13)
 
     POOL_MAX_OFFSET = 8
-    POOL_MAX_MASK = 1
+    POOL_MAX_MASK = _mask(1)
 
     TICK_WAIT_START_HIGH8_OFFSET = 0
     TICK_WAIT_START_COMBINATION_OFFSET = 7
-    TICK_WAIT_START_HIGH8_MASK = (1 << 8) - 1
+    TICK_WAIT_START_HIGH8_MASK = _mask(8)
 
     # Frame #2
     TICK_WAIT_START_LOW7_OFFSET = 23
-    TICK_WAIT_START_LOW7_MASK = (1 << 7) - 1
+    TICK_WAIT_START_LOW7_MASK = _mask(7)
 
     TICK_WAIT_END_OFFSET = 8
-    TICK_WAIT_END_MASK = (1 << 15) - 1
+    TICK_WAIT_END_MASK = _mask(15)
 
     SNN_EN_OFFSET = 7
-    SNN_EN_MASK = 1
+    SNN_EN_MASK = _mask(1)
 
     TARGET_LCN_OFFSET = 3
-    TARGET_LCN_MASK = (1 << 4) - 1
+    TARGET_LCN_MASK = _mask(4)
 
     # 用于配置帧2型test_chip_addr
     TEST_CHIP_ADDR_HIGH3_OFFSET = 0
     TEST_CHIP_ADDR_LOW7_OFFSET = 7
-    TEST_CHIP_ADDR_HIGH3_MASK = (1 << 3) - 1
+    TEST_CHIP_ADDR_HIGH3_MASK = _mask(3)
 
     # Frame #3
     TEST_CHIP_ADDR_LOW7_OFFSET = 23
-    TEST_CHIP_ADDR_LOW7_MASK = (1 << 7) - 1
+    TEST_CHIP_ADDR_LOW7_MASK = _mask(7)
 
 
 class OfflineConfigFrame3Format(OfflineFrameFormat):
     """Offline config frame type III, param RAM"""
 
     # Frame #1
     VJT_PRE_OFFSET = 0
-    VJT_PRE_MASK = (1 << 30) - 1
+    VJT_PRE_MASK = _mask(30)
 
     BIT_TRUNCATE_OFFSET = 30
-    BIT_TRUNCATE_MASK = (1 << 5) - 1
+    BIT_TRUNCATE_MASK = _mask(5)
 
     WEIGHT_DET_STOCH_OFFSET = 35
-    WEIGHT_DET_STOCH_MASK = (1 << 1) - 1
+    WEIGHT_DET_STOCH_MASK = _mask(1)
 
     LEAK_V_LOW28_OFFSET = 36
-    LEAK_V_LOW28_MASK = (1 << 28) - 1
+    LEAK_V_LOW28_MASK = _mask(28)
 
     # Frame #2
     LEAK_V_HIGH2_OFFSET = 0
-    LEAK_V_HIGH2_MASK = (1 << 2) - 1
+    LEAK_V_HIGH2_MASK = _mask(2)
 
     LEAK_DET_STOCH_OFFSET = 2
-    LEAK_DET_STOCH_MASK = (1 << 1) - 1
+    LEAK_DET_STOCH_MASK = _mask(1)
 
     LEAK_REVERSAL_FLAG_OFFSET = 3
-    LEAK_REVERSAL_FLAG_MASK = (1 << 1) - 1
+    LEAK_REVERSAL_FLAG_MASK = _mask(1)
 
     THRESHOLD_POS_OFFSET = 4
-    THRESHOLD_POS_MASK = (1 << 29) - 1
+    THRESHOLD_POS_MASK = _mask(29)
 
     THRESHOLD_NEG_OFFSET = 33
-    THRESHOLD_NEG_MASK = (1 << 29) - 1
+    THRESHOLD_NEG_MASK = _mask(29)
 
     THRESHOLD_NEG_MODE_OFFSET = 62
-    THRESHOLD_NEG_MODE_MASK = (1 << 1) - 1
+    THRESHOLD_NEG_MODE_MASK = _mask(1)
 
     THRESHOLD_MASK_CTRL_LOW1_OFFSET = 63
-    THRESHOLD_MASK_CTRL_LOW1_MASK = (1 << 1) - 1
+    THRESHOLD_MASK_CTRL_LOW1_MASK = _mask(1)
 
     # Frame #3
     THRESHOLD_MASK_CTRL_HIGH4_OFFSET = 0
-    THRESHOLD_MASK_CTRL_HIGH4_MASK = (1 << 4) - 1
+    THRESHOLD_MASK_CTRL_HIGH4_MASK = _mask(4)
 
     LEAK_POST_OFFSET = 4
-    LEAK_POST_MASK = (1 << 1) - 1
+    LEAK_POST_MASK = _mask(1)
 
     RESET_V_OFFSET = 5
-    RESET_V_MASK = (1 << 30) - 1
+    RESET_V_MASK = _mask(30)
 
     RESET_MODE_OFFSET = 35
-    RESET_MODE_MASK = (1 << 2) - 1
+    RESET_MODE_MASK = _mask(2)
 
     ADDR_CHIP_Y_OFFSET = 37
-    ADDR_CHIP_Y_MASK = (1 << 5) - 1
+    ADDR_CHIP_Y_MASK = _mask(5)
 
     ADDR_CHIP_X_OFFSET = 42
-    ADDR_CHIP_X_MASK = (1 << 5) - 1
+    ADDR_CHIP_X_MASK = _mask(5)
 
     ADDR_CORE_Y_EX_OFFSET = 47
-    ADDR_CORE_Y_EX_MASK = (1 << 5) - 1
+    ADDR_CORE_Y_EX_MASK = _mask(5)
 
     ADDR_CORE_X_EX_OFFSET = 52
-    ADDR_CORE_X_EX_MASK = (1 << 5) - 1
+    ADDR_CORE_X_EX_MASK = _mask(5)
 
     ADDR_CORE_Y_OFFSET = 57
-    ADDR_CORE_Y_MASK = (1 << 5) - 1
+    ADDR_CORE_Y_MASK = _mask(5)
 
     ADDR_CORE_X_LOW2_OFFSET = 62
-    ADDR_CORE_X_LOW2_MASK = (1 << 2) - 1
+    ADDR_CORE_X_LOW2_MASK = _mask(2)
 
     # Frame #4
     ADDR_CORE_X_HIGH3_OFFSET = 0
-    ADDR_CORE_X_HIGH3_MASK = (1 << 3) - 1
+    ADDR_CORE_X_HIGH3_MASK = _mask(3)
 
     ADDR_AXON_OFFSET = 3
-    ADDR_AXON_MASK = (1 << 11) - 1
+    ADDR_AXON_MASK = _mask(11)
 
     TICK_RELATIVE_OFFSET = 14
-    TICK_RELATIVE_MASK = (1 << 8) - 1
+    TICK_RELATIVE_MASK = _mask(8)
 
 
 class OfflineConfigFrame4Format(OfflineFrameFormat):
     """Offline config frame type IV, weight RAM"""
 
     pass
 
@@ -259,48 +263,48 @@
 WeightRAMFormat = OfflineConfigFrame4Format
 
 
 class OfflineWorkFrame1Format(OfflineFrameFormat):
     """Work frame type I"""
 
     RESERVED_OFFSET = 27
-    RESERVED_MASK = (1 << 3) - 1
+    RESERVED_MASK = _mask(3)
 
     AXON_OFFSET = 16
-    AXON_MASK = (1 << 11) - 1
+    AXON_MASK = _mask(11)
 
     TIMESLOT_OFFSET = 8
-    TIMESLOT_MASK = (1 << 8) - 1
+    TIMESLOT_MASK = _mask(8)
 
     DATA_OFFSET = 0
-    DATA_MASK = (1 << 8) - 1
+    DATA_MASK = _mask(8)
 
 
 class OfflineWorkFrame2Format(OfflineFrameFormat):
     """Work frame type II"""
 
     RESERVED_OFFSET = 30
-    RESERVED_MASK = (1 << 20) - 1
+    RESERVED_MASK = _mask(20)
 
     TIME_OFFSET = 0
-    TIME_MASK = (1 << 30) - 1
+    TIME_MASK = _mask(30)
 
 
 class OfflineWorkFrame3Format(OfflineFrameFormat):
     """Work frame type III"""
 
     RESERVED_OFFSET = 0
-    RESERVED_MASK = (1 << 50) - 1
+    RESERVED_MASK = _mask(50)
 
 
 class OfflineWorkFrame4Format(OfflineFrameFormat):
     """Work frame type IV"""
 
     RESERVED_OFFSET = 0
-    RESERVED_MASK = (1 << 50) - 1
+    RESERVED_MASK = _mask(50)
 
 
 SpikeFrameFormat = OfflineWorkFrame1Format
 SyncFrameFormat = OfflineWorkFrame2Format
 ClearFrameFormat = OfflineWorkFrame3Format
 InitFrameFormat = OfflineWorkFrame4Format
```

### Comparing `paicorelib-1.1.1/paicorelib/framelib/frame_gen.py` & `paicorelib-1.1.2/paicorelib/framelib/frame_gen.py`

 * *Files identical despite different names*

### Comparing `paicorelib-1.1.1/paicorelib/framelib/frames.py` & `paicorelib-1.1.2/paicorelib/framelib/frames.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import warnings
-from typing import Any, ClassVar, Dict, Optional, Union
+from typing import Any, ClassVar, Dict, Literal, Optional, Union
 
 import numpy as np
 from numpy.typing import NDArray
 
 from paicorelib import Coord, CoordLike
 from paicorelib import ReplicationId as RId
 from paicorelib import RIdLike, to_coord, to_rid
@@ -18,14 +18,15 @@
 from .frame_defs import ParameterRegFormat as RegF
 from .frame_defs import SpikeFrameFormat as WF1F
 from .types import FRAME_DTYPE, ArrayType, DataType, FrameArrayType
 from .utils import (
     OUT_OF_RANGE_WARNING,
     ShapeError,
     TruncationWarning,
+    _mask,
     bin_split,
     params_check,
     params_check2,
 )
 
 __all__ = [
     "OfflineConfigFrame1",
@@ -43,14 +44,18 @@
     "OfflineWorkFrame1",
     "OfflineWorkFrame2",
     "OfflineWorkFrame3",
     "OfflineWorkFrame4",
 ]
 
 
+_L_PACKAGE_TYPE_CONF_TESTOUT = 0  # Literal value of package type for conf & test out
+_L_PACKAGE_TYPE_TESTIN = 1  # Literal value of package type for test in.
+
+
 class _RandomSeedFrame(Frame):
     """For reusing the method of splitting the random seed."""
 
     def __init__(
         self,
         header: FH,
         chip_coord: Coord,
@@ -70,15 +75,15 @@
         super().__init__(header, chip_coord, core_coord, rid, payload)
 
     def _random_seed_split(self) -> FrameArrayType:
         return np.asarray(
             [
                 (self._random_seed >> 34) & FF.GENERAL_PAYLOAD_MASK,
                 (self._random_seed >> 4) & FF.GENERAL_PAYLOAD_MASK,
-                (self._random_seed & ((1 << 4) - 1)) << 26,
+                (self._random_seed & _mask(4)) << 26,
             ],
             dtype=FRAME_DTYPE,
         )
 
     @property
     def random_seed(self) -> int:
         return self._random_seed
@@ -169,15 +174,17 @@
         sram_start_addr: int,
         neuron_num: int,
         neuron_attrs: Dict[str, Any],
         neuron_dest_info: Dict[str, Any],
         repeat: int,
     ) -> None:
         n_package = 4 * neuron_num * repeat
-        payload = _package_arg_check(sram_start_addr, n_package, 0)
+        payload = _package_arg_check(
+            sram_start_addr, n_package, _L_PACKAGE_TYPE_CONF_TESTOUT
+        )
         packages = self._packages_reorganized(
             neuron_attrs,
             neuron_dest_info,
             neuron_num,
             repeat,
         )
 
@@ -328,15 +335,17 @@
         core_coord: Coord,
         rid: RId,
         /,
         sram_start_addr: int,
         data_package_num: int,
         weight_ram: FrameArrayType,
     ) -> None:
-        payload = _package_arg_check(sram_start_addr, data_package_num, 0)
+        payload = _package_arg_check(
+            sram_start_addr, data_package_num, _L_PACKAGE_TYPE_CONF_TESTOUT
+        )
         _weight_ram = weight_ram.flatten()
 
         super().__init__(header, chip_coord, core_coord, rid, payload, _weight_ram)
 
 
 class OfflineConfigFrame1(_RandomSeedFrame):
     """Offline config frame type I"""
@@ -470,15 +479,17 @@
         chip_coord: Coord,
         core_coord: Coord,
         rid: RId,
         /,
         sram_start_addr: int,
         data_package_num: int,
     ) -> None:
-        payload = _package_arg_check(sram_start_addr, data_package_num, 1)
+        payload = _package_arg_check(
+            sram_start_addr, data_package_num, _L_PACKAGE_TYPE_TESTIN
+        )
 
         super().__init__(self.header, chip_coord, core_coord, rid, payload)
 
 
 class OfflineTestOutFrame3(_NeuronRAMFrame):
     header: ClassVar[FH] = FH.CONFIG_TYPE4
 
@@ -515,15 +526,17 @@
         chip_coord: Coord,
         core_coord: Coord,
         rid: RId,
         /,
         sram_start_addr: int,
         data_package_num: int,
     ):
-        payload = _package_arg_check(sram_start_addr, data_package_num, 1)
+        payload = _package_arg_check(
+            sram_start_addr, data_package_num, _L_PACKAGE_TYPE_TESTIN
+        )
 
         super().__init__(self.header, chip_coord, core_coord, rid, payload)
 
 
 class OfflineTestOutFrame4(_WeightRAMFrame):
     header: ClassVar[FH] = FH.TEST_TYPE4
 
@@ -676,38 +689,26 @@
         )
 
 
 class OfflineWorkFrame3(Frame):
     header: ClassVar[FH] = FH.WORK_TYPE3
 
     def __init__(self, chip_coord: Coord) -> None:
-        super().__init__(
-            self.header,
-            chip_coord,
-            Coord(0, 0),
-            RId(0, 0),
-            0,
-        )
+        super().__init__(self.header, chip_coord, Coord(0, 0), RId(0, 0), 0)
 
 
 class OfflineWorkFrame4(Frame):
     header: ClassVar[FH] = FH.WORK_TYPE4
 
     def __init__(self, chip_coord: Coord) -> None:
-        super().__init__(
-            self.header,
-            chip_coord,
-            Coord(0, 0),
-            RId(0, 0),
-            0,
-        )
+        super().__init__(self.header, chip_coord, Coord(0, 0), RId(0, 0), 0)
 
 
 def _package_arg_check(
-    sram_start_addr: int, data_package_num: int, package_type: int
+    sram_start_addr: int, data_package_num: int, package_type: Literal[0, 1]
 ) -> FRAME_DTYPE:
     if sram_start_addr > RAMF.GENERAL_PACKAGE_SRAM_ADDR_MASK or sram_start_addr < 0:
         raise ValueError(f"SRAM start address out of range, {sram_start_addr}.")
 
     if data_package_num > RAMF.GENERAL_PACKAGE_NUM_MASK or data_package_num < 0:
         raise ValueError(
             f"the numeber of data package out of range, {data_package_num}."
```

### Comparing `paicorelib-1.1.1/paicorelib/framelib/types.py` & `paicorelib-1.1.2/paicorelib/framelib/types.py`

 * *Files identical despite different names*

### Comparing `paicorelib-1.1.1/paicorelib/framelib/utils.py` & `paicorelib-1.1.2/paicorelib/framelib/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import numpy as np
 from pydantic import TypeAdapter
 
 from .frame_defs import FrameFormat as FF
 from .frame_defs import FrameHeader as FH
 from .frame_defs import FrameType as FT
+from .frame_defs import _mask
 from .types import FRAME_DTYPE, BasicFrameArray, FrameArrayType
 
 
 class FrameIllegalError(ValueError):
     """Frame is illegal."""
 
     pass
@@ -100,31 +101,31 @@
 
 def np2txt(fp: Path, d: np.ndarray) -> None:
     with open(fp, "w") as f:
         for i in range(d.size):
             f.write("{:064b}\n".format(d[i]))
 
 
-def bin_split(x: int, pos: int, high_mask: Optional[int] = None) -> Tuple[int, int]:
+def bin_split(x: int, pos: int, high_mask_bit: Optional[int] = None) -> Tuple[int, int]:
     """Split an integer, return the high and low part.
 
     Argument:
         - x: the integer
         - pos: the position (LSB) to split the binary.
         - high_mask: mask for the high part. Optional.
 
     Example::
 
         >>> bin_split(0b1100001001, 3)
         97(0b1100001), 1
     """
-    low = x & ((1 << pos) - 1)
+    low = x & _mask(pos)
 
-    if isinstance(high_mask, int):
-        high = (x >> pos) & high_mask
+    if isinstance(high_mask_bit, int):
+        high = (x >> pos) & _mask(high_mask_bit)
     else:
         high = x >> pos
 
     return high, low
 
 
 def params_check(checker: TypeAdapter):
```

### Comparing `paicorelib-1.1.1/paicorelib/hw_defs.py` & `paicorelib-1.1.2/paicorelib/hw_defs.py`

 * *Files identical despite different names*

### Comparing `paicorelib-1.1.1/paicorelib/hw_types.py` & `paicorelib-1.1.2/paicorelib/hw_types.py`

 * *Files identical despite different names*

### Comparing `paicorelib-1.1.1/paicorelib/ram_model.py` & `paicorelib-1.1.2/paicorelib/ram_model.py`

 * *Files identical despite different names*

### Comparing `paicorelib-1.1.1/paicorelib/ram_types.py` & `paicorelib-1.1.2/paicorelib/ram_types.py`

 * *Files identical despite different names*

### Comparing `paicorelib-1.1.1/paicorelib/reg_model.py` & `paicorelib-1.1.2/paicorelib/reg_model.py`

 * *Files identical despite different names*

### Comparing `paicorelib-1.1.1/paicorelib/reg_types.py` & `paicorelib-1.1.2/paicorelib/reg_types.py`

 * *Files identical despite different names*

### Comparing `paicorelib-1.1.1/paicorelib/routing_defs.py` & `paicorelib-1.1.2/paicorelib/routing_defs.py`

 * *Files identical despite different names*

### Comparing `paicorelib-1.1.1/pyproject.toml` & `paicorelib-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "paicorelib"
-version = "1.1.1"
+version = "1.1.2"
 description = "Library of PAICORE 2.0"
 authors = ["Ziru Pan <zrpan@stu.pku.edu.cn>"]
 maintainers = [
     "Hongtu Xia <hongtux@pku.edu.cn>",
     "Siyuan Gao <siyuan-gao@outlook.com>",
     "Zhaoyang Hao <hzyang2218@gmail.com>",
     "Ziru Pan <zrpan@stu.pku.edu.cn>",
```

### Comparing `paicorelib-1.1.1/PKG-INFO` & `paicorelib-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paicorelib
-Version: 1.1.1
+Version: 1.1.2
 Summary: Library of PAICORE 2.0
 Home-page: https://github.com/PAICookers/PAIlib
 License: GPL-3.0-or-later
 Keywords: PAICORE 2.0,PAICORE library,PAILib
 Author: Ziru Pan
 Author-email: zrpan@stu.pku.edu.cn
 Maintainer: Hongtu Xia
@@ -34,15 +34,15 @@
 
 </div>
 
 <p align="center">
     <a href="https://github.com/PAICookers/PAIlib/blob/master/pyproject.toml">
         <img src="https://img.shields.io/pypi/pyversions/paicorelib">
     </a>
-    <a href="https://github.com/PAICookers/PAIlib/releases/tag/v1.1.1"
+    <a href="https://github.com/PAICookers/PAIlib/releases/tag/v1.1.2"
         <img src="https://img.shields.io/github/v/release/PAICookers/PAIlib?color=orange">
     </a>
     <a href="https://www.codefactor.io/repository/github/PAICookers/PAIlib">
       <img src="https://img.shields.io/codefactor/grade/github/PAICookers/PAIlib/master?color=red">
     </a>
     <a href="https://results.pre-commit.ci/latest/github/PAICookers/PAIlib/master">
 	   <img src="https://results.pre-commit.ci/badge/github/PAICookers/PAIlib/master.svg" alt="pre-commit.ci status">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: paicorelib Version: 1.1.1 Summary: Library of
+Metadata-Version: 2.1 Name: paicorelib Version: 1.1.2 Summary: Library of
 PAICORE 2.0 Home-page: https://github.com/PAICookers/PAIlib License: GPL-3.0-
 or-later Keywords: PAICORE 2.0,PAICORE library,PAILib Author: Ziru Pan Author-
 email: zrpan@stu.pku.edu.cn Maintainer: Hongtu Xia Maintainer-email:
 hongtux@pku.edu.cn Requires-Python: >=3.8,<4.0 Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

