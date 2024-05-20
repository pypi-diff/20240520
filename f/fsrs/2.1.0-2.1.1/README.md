# Comparing `tmp/fsrs-2.1.0.tar.gz` & `tmp/fsrs-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs-2.1.0.tar", last modified: Tue May  7 02:37:18 2024, max compression
+gzip compressed data, was "fsrs-2.1.1.tar", last modified: Mon May 20 14:37:54 2024, max compression
```

## Comparing `fsrs-2.1.0.tar` & `fsrs-2.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:37:18.028366 fsrs-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-07 02:37:13.000000 fsrs-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-05-07 02:37:18.028366 fsrs-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-07 02:37:13.000000 fsrs-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-07 02:37:13.000000 fsrs-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 02:37:18.028366 fsrs-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 02:37:13.000000 fsrs-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:37:18.024366 fsrs-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:37:18.028366 fsrs-2.1.0/src/fsrs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-07 02:37:13.000000 fsrs-2.1.0/src/fsrs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-07 02:37:13.000000 fsrs-2.1.0/src/fsrs/fsrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-05-07 02:37:13.000000 fsrs-2.1.0/src/fsrs/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:37:18.028366 fsrs-2.1.0/src/fsrs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-05-07 02:37:18.000000 fsrs-2.1.0/src/fsrs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-07 02:37:18.000000 fsrs-2.1.0/src/fsrs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 02:37:18.000000 fsrs-2.1.0/src/fsrs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-07 02:37:18.000000 fsrs-2.1.0/src/fsrs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:37:18.028366 fsrs-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-05-07 02:37:13.000000 fsrs-2.1.0/tests/test_fsrs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:37:54.184285 fsrs-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-20 14:37:49.000000 fsrs-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-05-20 14:37:54.184285 fsrs-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-20 14:37:49.000000 fsrs-2.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-20 14:37:49.000000 fsrs-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 14:37:54.184285 fsrs-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 14:37:49.000000 fsrs-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:37:54.180285 fsrs-2.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:37:54.180285 fsrs-2.1.1/src/fsrs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-20 14:37:49.000000 fsrs-2.1.1/src/fsrs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-20 14:37:49.000000 fsrs-2.1.1/src/fsrs/fsrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7051 2024-05-20 14:37:49.000000 fsrs-2.1.1/src/fsrs/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:37:54.184285 fsrs-2.1.1/src/fsrs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-05-20 14:37:54.000000 fsrs-2.1.1/src/fsrs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-20 14:37:54.000000 fsrs-2.1.1/src/fsrs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:37:54.000000 fsrs-2.1.1/src/fsrs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-20 14:37:54.000000 fsrs-2.1.1/src/fsrs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:37:54.184285 fsrs-2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-05-20 14:37:49.000000 fsrs-2.1.1/tests/test_fsrs.py
```

### Comparing `fsrs-2.1.0/LICENSE` & `fsrs-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fsrs-2.1.0/PKG-INFO` & `fsrs-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsrs
-Version: 2.1.0
+Version: 2.1.1
 Summary: Free Spaced Repetition Scheduler
 Author-email: Jarrett Ye <jarrett.ye@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Open Spaced Repetition
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `fsrs-2.1.0/README.md` & `fsrs-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fsrs-2.1.0/pyproject.toml` & `fsrs-2.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fsrs"
-version = "2.1.0"
+version = "2.1.1"
 description = "Free Spaced Repetition Scheduler"
 readme = "README.md"
 authors = [{ name = "Jarrett Ye", email = "jarrett.ye@outlook.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
```

### Comparing `fsrs-2.1.0/src/fsrs/fsrs.py` & `fsrs-2.1.1/src/fsrs/fsrs.py`

 * *Files identical despite different names*

### Comparing `fsrs-2.1.0/src/fsrs/models.py` & `fsrs-2.1.1/src/fsrs/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datetime import datetime, timedelta, UTC
+from datetime import datetime, timedelta, timezone
 import copy
 from typing import Tuple, Optional
 from enum import IntEnum
 
 
 class State(IntEnum):
     New = 0
@@ -61,15 +61,15 @@
         reps=0,
         lapses=0,
         state=State.New,
         last_review=None,
     ) -> None:
 
         if due is None:
-            self.due = datetime.now(UTC)
+            self.due = datetime.now(timezone.utc)
         else:
             self.due = due
 
         self.stability = stability
         self.difficulty = difficulty
         self.elapsed_days = elapsed_days
         self.scheduled_days = scheduled_days
```

### Comparing `fsrs-2.1.0/src/fsrs.egg-info/PKG-INFO` & `fsrs-2.1.1/src/fsrs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsrs
-Version: 2.1.0
+Version: 2.1.1
 Summary: Free Spaced Repetition Scheduler
 Author-email: Jarrett Ye <jarrett.ye@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Open Spaced Repetition
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `fsrs-2.1.0/tests/test_fsrs.py` & `fsrs-2.1.1/tests/test_fsrs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from fsrs import *
-from datetime import datetime, UTC
+from datetime import datetime, timezone
 import json
 import pytest
 
 
 def print_scheduling_cards(scheduling_cards):
     print("again.card:", scheduling_cards[Rating.Again].card.__dict__)
     print("again.review_log:", scheduling_cards[Rating.Again].review_log.__dict__)
@@ -36,15 +36,15 @@
             0.0179,
             0.3105,
             0.3976,
             0.0,
             2.0902,
         )
         card = Card()
-        now = datetime(2022, 11, 29, 12, 30, 0, 0, tzinfo=UTC)
+        now = datetime(2022, 11, 29, 12, 30, 0, 0, timezone.utc)
         scheduling_cards = f.repeat(card, now)
         print_scheduling_cards(scheduling_cards)
 
         ratings = (
             Rating.Good,
             Rating.Good,
             Rating.Good,
@@ -74,31 +74,31 @@
 
     def test_datetime(self):
 
         f = FSRS()
         card = Card()
 
         # new cards should be due immediately after creation
-        assert datetime.now(UTC) >= card.due
+        assert datetime.now(timezone.utc) >= card.due
 
         # comparing timezone aware cards with deprecated datetime.utcnow() should raise a TypeError
         with pytest.raises(TypeError):
             datetime.now() >= card.due
 
         # repeating a card with a non-utc, non-timezone-aware datetime object should raise a Value Error
         with pytest.raises(ValueError):
             f.repeat(card, datetime(2022, 11, 29, 12, 30, 0, 0))
 
         # repeat a card with rating good before next tests
-        scheduling_cards = f.repeat(card, datetime.now(UTC))
+        scheduling_cards = f.repeat(card, datetime.now(timezone.utc))
         card = scheduling_cards[Rating.Good].card
 
         # card object's due and last_review attributes must be timezone aware and UTC
-        assert card.due.tzinfo == UTC
-        assert card.last_review.tzinfo == UTC
+        assert card.due.tzinfo == timezone.utc
+        assert card.last_review.tzinfo == timezone.utc
         # card object's due datetime should be later than its last review
         assert card.due >= card.last_review
 
     def test_serialize(self):
 
         f = FSRS()
 
@@ -116,15 +116,15 @@
         card_dict = card.to_dict()
         copied_card = Card.from_dict(card_dict)
 
         assert vars(card) == vars(copied_card)
         assert card.to_dict() == copied_card.to_dict()
 
         # (x2) perform the above tests once more with a repeated card
-        scheduling_cards = f.repeat(card, datetime.now(UTC))
+        scheduling_cards = f.repeat(card, datetime.now(timezone.utc))
         repeated_card = scheduling_cards[Rating.Good].card
 
         with pytest.raises(TypeError):
             json.dumps(repeated_card.__dict__)
 
         assert type(json.dumps(repeated_card.to_dict())) == str
```

