# Comparing `tmp/habits_txt-0.3.6.tar.gz` & `tmp/habits_txt-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "habits_txt-0.3.6.tar", max compression
+gzip compressed data, was "habits_txt-0.3.7.tar", max compression
```

## Comparing `habits_txt-0.3.6.tar` & `habits_txt-0.3.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     3184 2024-05-17 10:07:19.291761 habits_txt-0.3.6/README.md
--rwxr-xr-x   0        0        0      788 2024-05-15 17:43:14.132064 habits_txt-0.3.6/bin/hbtxt.py
--rw-r--r--   0        0        0        0 2024-05-14 20:25:35.415585 habits_txt-0.3.6/habits_txt/__init__.py
--rw-r--r--   0        0        0    13971 2024-05-15 17:43:14.132064 habits_txt-0.3.6/habits_txt/builder.py
--rw-r--r--   0        0        0     7980 2024-05-16 07:15:40.194208 habits_txt-0.3.6/habits_txt/cli.py
--rw-r--r--   0        0        0     2154 2024-05-14 20:25:35.415585 habits_txt-0.3.6/habits_txt/config.py
--rw-r--r--   0        0        0      224 2024-05-14 20:25:35.415585 habits_txt-0.3.6/habits_txt/defaults.py
--rw-r--r--   0        0        0     2323 2024-05-15 17:43:14.132064 habits_txt-0.3.6/habits_txt/directives.py
--rw-r--r--   0        0        0      380 2024-05-14 20:25:35.415585 habits_txt-0.3.6/habits_txt/exceptions.py
--rw-r--r--   0        0        0     8089 2024-05-17 13:06:12.645011 habits_txt-0.3.6/habits_txt/journal.py
--rw-r--r--   0        0        0     2940 2024-05-15 17:43:14.132064 habits_txt-0.3.6/habits_txt/models.py
--rw-r--r--   0        0        0     9037 2024-05-15 17:43:14.132064 habits_txt-0.3.6/habits_txt/parser.py
--rw-r--r--   0        0        0      952 2024-05-14 20:25:35.415585 habits_txt-0.3.6/habits_txt/records_query.py
--rw-r--r--   0        0        0      698 2024-05-17 13:06:12.645011 habits_txt-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     3558 1970-01-01 00:00:00.000000 habits_txt-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     3184 2024-05-17 10:07:19.291761 habits_txt-0.3.7/README.md
+-rwxr-xr-x   0        0        0      788 2024-05-15 17:43:14.132064 habits_txt-0.3.7/bin/hbtxt.py
+-rw-r--r--   0        0        0        0 2024-05-14 20:25:35.415585 habits_txt-0.3.7/habits_txt/__init__.py
+-rw-r--r--   0        0        0    13887 2024-05-20 07:58:20.155225 habits_txt-0.3.7/habits_txt/builder.py
+-rw-r--r--   0        0        0     7980 2024-05-16 07:15:40.194208 habits_txt-0.3.7/habits_txt/cli.py
+-rw-r--r--   0        0        0     2154 2024-05-14 20:25:35.415585 habits_txt-0.3.7/habits_txt/config.py
+-rw-r--r--   0        0        0      224 2024-05-14 20:25:35.415585 habits_txt-0.3.7/habits_txt/defaults.py
+-rw-r--r--   0        0        0     2325 2024-05-20 07:58:20.155225 habits_txt-0.3.7/habits_txt/directives.py
+-rw-r--r--   0        0        0      380 2024-05-14 20:25:35.415585 habits_txt-0.3.7/habits_txt/exceptions.py
+-rw-r--r--   0        0        0     8089 2024-05-20 07:46:21.587706 habits_txt-0.3.7/habits_txt/journal.py
+-rw-r--r--   0        0        0     3628 2024-05-20 07:58:20.155225 habits_txt-0.3.7/habits_txt/models.py
+-rw-r--r--   0        0        0     8729 2024-05-20 07:58:20.155225 habits_txt-0.3.7/habits_txt/parser.py
+-rw-r--r--   0        0        0      952 2024-05-14 20:25:35.415585 habits_txt-0.3.7/habits_txt/records_query.py
+-rw-r--r--   0        0        0      698 2024-05-20 07:58:20.155225 habits_txt-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     3558 1970-01-01 00:00:00.000000 habits_txt-0.3.7/PKG-INFO
```

### Comparing `habits_txt-0.3.6/README.md` & `habits_txt-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `habits_txt-0.3.6/bin/hbtxt.py` & `habits_txt-0.3.7/bin/hbtxt.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.3.6/habits_txt/builder.py` & `habits_txt-0.3.7/habits_txt/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,17 +32,17 @@
     Get the tracked habits at a given date.
 
     :param directives_: List of directives.
     :param date: Date to check.
     :return: List of tracked habits.
 
     Example:
-    >>> directive1 = directives.TrackDirective(dt.datetime(2024, 1, 1), "Habit 1", models.Frequency("*", "*", "*"))
-    >>> directive2 = directives.TrackDirective(dt.datetime(2024, 1, 2), "Habit 2", models.Frequency("*", "*", "*"))
-    >>> directive3 = directives.TrackDirective(dt.datetime(2024, 1, 3), "Habit 3", models.Frequency("*", "*", "*"))
+    >>> directive1 = directives.TrackDirective(dt.datetime(2024, 1, 1), "Habit 1", models.Frequency("* * *"))
+    >>> directive2 = directives.TrackDirective(dt.datetime(2024, 1, 2), "Habit 2", models.Frequency("* * *"))
+    >>> directive3 = directives.TrackDirective(dt.datetime(2024, 1, 3), "Habit 3", models.Frequency("* * *"))
     >>> tracked_habits = _get_tracked_habits_at_date([directive1, directive2, directive3], dt.datetime(2024, 1, 2))
     >>> print(tracked_habits)
     [Habit 1, Habit 2]
     """
     directives_before_date = [
         directive for directive in directives_ if directive.date <= date
     ]
@@ -68,17 +68,17 @@
     """
     Check if a track directive is valid.
 
     :param directive: Track directive.
     :param tracked_habits: Tracked habits.
 
     Example:
-    >>> directive1 = directives.TrackDirective(dt.datetime(2024, 1, 1), "Habit 1", models.Frequency("*", "*", "*"))
-    >>> directive2 = directives.TrackDirective(dt.datetime(2024, 1, 2), "Habit 2", models.Frequency("*", "*", "*"))
-    >>> tracked_habits = {models.Habit("Habit 1", models.Frequency("*", "*", "*"))}
+    >>> directive1 = directives.TrackDirective(dt.datetime(2024, 1, 1), "Habit 1", models.Frequency("* * *"))
+    >>> directive2 = directives.TrackDirective(dt.datetime(2024, 1, 2), "Habit 2", models.Frequency("* * *"))
+    >>> tracked_habits = {models.Habit("Habit 1", models.Frequency("* * *"))}
     >>> _check_track_directive_is_valid(directive2, tracked_habits)
     """
     if directive.habit_name in {habit.name for habit in tracked_habits}:
         raise exceptions.ConsistencyError(
             f"Several tracked habits with the same name: {directive.habit_name}",
             directive,
         )
@@ -91,15 +91,15 @@
     Check if an untrack directive is valid.
 
     :param directive: Untrack directive.
     :param tracked_habits: Tracked habits.
 
     Example:
     >>> directive = directives.UntrackDirective(dt.datetime(2024, 1, 1), "Habit 1")
-    >>> tracked_habits = {models.Habit("Habit 1", models.Frequency("*", "*", "*"))}
+    >>> tracked_habits = {models.Habit("Habit 1", models.Frequency("* * *"))}
     >>> _check_untrack_directive_is_valid(directive, tracked_habits)
     """
     if directive.habit_name not in {habit.name for habit in tracked_habits}:
         raise exceptions.ConsistencyError(
             f"Untracked habit without a corresponding track directive: {directive.habit_name}",
             directive,
         )
@@ -113,15 +113,15 @@
 
     :param habit_name: Name of the habit to remove.
     :param tracked_habits: Tracked habits.
     :return: Updated tracked habits.
 
     Example:
     >>> habit_name = "Habit 1"
-    >>> tracked_habits = {models.Habit("Habit 1", models.Frequency("*", "*", "*"))}
+    >>> tracked_habits = {models.Habit("Habit 1", models.Frequency("* * *"))}
     >>> updated_tracked_habits = _remove_habit_from_state(habit_name, tracked_habits)
     >>> print(updated_tracked_habits)
     []
     """
     return {habit for habit in tracked_habits if habit.name != habit_name}
 
 
@@ -131,15 +131,15 @@
     """
     Build a habit from a track directive.
 
     :param directive: Track directive.
     :return: Built habit.
 
     Example:
-    >>> directive = directives.TrackDirective(dt.datetime(2024, 1, 1), "Habit 1", models.Frequency("*", "*", "*"))
+    >>> directive = directives.TrackDirective(dt.datetime(2024, 1, 1), "Habit 1", models.Frequency("* * *"))
     >>> habit = _build_habit_from_track_directive(directive)
     >>> print(habit)
     Habit 1
     """
     return models.Habit(
         directive.habit_name, directive.frequency, directive.is_measurable
     )
@@ -208,15 +208,15 @@
 
     :param directive: Record directive.
     :param tracked_habits: Tracked habits.
     :param records: List of records.
 
     Example:
     >>> directive = directives.RecordDirective(dt.datetime(2024, 1, 1), "Habit 1", False)
-    >>> tracked_habits = {models.Habit("Habit 1", models.Frequency("*", "*", "*"))}
+    >>> tracked_habits = {models.Habit("Habit 1", models.Frequency("* * *"))}
     >>> records = [models.HabitRecord(dt.datetime(2024, 1, 1), "Habit 2", True)]
     >>> _check_record_directive_is_valid(directive, tracked_habits, records)
     """
     if directive.habit_name not in {habit.name for habit in tracked_habits}:
         raise exceptions.ConsistencyError(
             f"Recorded habit without a corresponding track directive: {directive.habit_name}",
             directive,
@@ -256,16 +256,16 @@
     Get the state of the habits at a given date.
 
     :param directives_: List of directives.
     :param date: Date to check.
     :return: List of tracked habits, list of records, list of matches.
 
     Example:
-    >>> directive1 = directives.TrackDirective(dt.datetime(2024, 1, 1), "Habit 1", models.Frequency("*", "*", "*"))
-    >>> directive2 = directives.TrackDirective(dt.datetime(2024, 1, 2), "Habit 2", models.Frequency("*", "*", "*"))
+    >>> directive1 = directives.TrackDirective(dt.datetime(2024, 1, 1), "Habit 1", models.Frequency("* * *"))
+    >>> directive2 = directives.TrackDirective(dt.datetime(2024, 1, 2), "Habit 2", models.Frequency("* * *"))
     >>> directive3 = directives.RecordDirective(dt.datetime(2024, 1, 1), "Habit 1", False)
     >>> tracked_habits, records, habits_records_matches = \
     get_state_at_date([directive1, directive2, directive3], dt.datetime(2024, 1, 1))
     >>> print(tracked_habits)
     [Habit 1]
     >>> print(records)
     [HabitRecord(Habit 1, False)]
@@ -309,17 +309,17 @@
     Get the matches of track, untrack, and record directives at a given date.
 
     :param directives_: List of directives.
     :param date: Date to check.
     :return: List of matches.
 
     Example:
-    >>> directive1 = directives.TrackDirective(dt.datetime(2024, 1, 1), "Habit 1", models.Frequency("*", "*", "*"))
+    >>> directive1 = directives.TrackDirective(dt.datetime(2024, 1, 1), "Habit 1", models.Frequency("* * *"))
     >>> directive2 = directives.UntrackDirective(dt.datetime(2024, 1, 2), "Habit 1")
-    >>> directive3 = directives.TrackDirective(dt.datetime(2024, 1, 2), "Habit 2", models.Frequency("*", "*", "*"))
+    >>> directive3 = directives.TrackDirective(dt.datetime(2024, 1, 2), "Habit 2", models.Frequency("* * *"))
     >>> directive4 = directives.RecordDirective(dt.datetime(2024, 1, 1), "Habit 1", False)
     >>> matches = get_track_untrack_record_matches_at_date(\
     [directive1, directive2, directive3, directive4], dt.datetime(2024, 2, 1))
     >>> print(matches)
     [(directive1, directive2, [directive4]), (directive3, None, [])]
     """
     directives_before_date = [
```

### Comparing `habits_txt-0.3.6/habits_txt/cli.py` & `habits_txt-0.3.7/habits_txt/cli.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.3.6/habits_txt/config.py` & `habits_txt-0.3.7/habits_txt/config.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.3.6/habits_txt/directives.py` & `habits_txt-0.3.7/habits_txt/directives.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             and self.frequency == other.frequency
             and self.is_measurable == other.is_measurable
         )
 
     def __repr__(self):
         return (
             super().__repr__()
-            + f" {self.frequency} {defaults.MEASURABLE_KEYWORD if self.is_measurable else ''}"
+            + f" ({self.frequency}) {defaults.MEASURABLE_KEYWORD if self.is_measurable else ''}"
         )
 
 
 class UntrackDirective(Directive):
 
     directive_type = DirectiveType.UNTRACK
```

### Comparing `habits_txt-0.3.6/habits_txt/journal.py` & `habits_txt-0.3.7/habits_txt/journal.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.3.6/habits_txt/parser.py` & `habits_txt-0.3.7/habits_txt/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import datetime as dt
 import logging
 import re
 import typing
 from functools import wraps
 
-import croniter
-
 import habits_txt.defaults as defaults
 import habits_txt.directives as directives
 import habits_txt.exceptions as exceptions
 import habits_txt.models as models
 
 
 def parse_file(file_path: str) -> typing.Tuple[list[directives.Directive], list[str]]:
@@ -219,24 +217,19 @@
     res = re.search(r"\(.*\)", directive_line)
     if res is None:
         raise exceptions.ParseError(
             f"Could not find a frequency enclosed in parenthesis: {directive_line}"
         )
     frequency_str = res.group(0)
     frequency_str = frequency_str[1:-1]
-    frequency_parts = frequency_str.split(" ")
-    if len(frequency_parts) != 3:
-        raise exceptions.ParseError(f"Invalid frequency format: {frequency_str}")
-    day, month, day_of_week = frequency_parts
-    cron_expression = f"0 0 {day} {month} {day_of_week}"
     try:
-        croniter.croniter(cron_expression)
-        return models.Frequency(day, month, day_of_week)
+        frequency = models.Frequency(frequency_str)
+        return frequency
     except ValueError:
-        raise exceptions.ParseError(f"Invalid frequency format: {cron_expression}")
+        raise exceptions.ParseError(f"Invalid frequency format: {frequency_str}")
 
 
 @_handle_index_error_decorator(name="value")
 def _parse_value(directive_line: str) -> bool | float:
     """
     Parse the value from a directive line.
```

### Comparing `habits_txt-0.3.6/habits_txt/records_query.py` & `habits_txt-0.3.7/habits_txt/records_query.py`

 * *Files identical despite different names*

### Comparing `habits_txt-0.3.6/pyproject.toml` & `habits_txt-0.3.7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "habits.txt"
-version = "0.3.6"
+version = "0.3.7"
 description = ""
 authors = ["estebanthi <esteban.thilliez@gmail.com>"]
 readme = "README.md"
 packages = [
     {include = "habits_txt"}, {include = "bin"}
 ]
```

### Comparing `habits_txt-0.3.6/PKG-INFO` & `habits_txt-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: habits.txt
-Version: 0.3.6
+Version: 0.3.7
 Summary: 
 Author: estebanthi
 Author-email: esteban.thilliez@gmail.com
 Requires-Python: >=3.12,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
```

