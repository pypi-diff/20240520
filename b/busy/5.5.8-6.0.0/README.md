# Comparing `tmp/busy-5.5.8.tar.gz` & `tmp/busy-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "busy-5.5.8.tar", max compression
+gzip compressed data, was "busy-6.0.0.tar", max compression
```

## Comparing `busy-5.5.8.tar` & `busy-6.0.0.tar`

### file list

```diff
@@ -1,46 +1,36 @@
--rw-r--r--   0        0        0     1071 2023-11-06 05:10:07.073190 busy-5.5.8/LICENSE
--rw-r--r--   0        0        0    22370 2023-11-06 05:10:07.074190 busy-5.5.8/README.md
--rw-r--r--   0        0        0        0 2023-11-06 05:10:07.103191 busy-5.5.8/busy/__init__.py
--rw-r--r--   0        0        0       69 2023-11-06 05:10:07.074190 busy-5.5.8/busy/__main__.py
--rw-r--r--   0        0        0        0 2023-11-06 05:10:07.103191 busy-5.5.8/busy/command/__init__.py
--rw-r--r--   0        0        0     1641 2023-11-06 05:10:07.074190 busy-5.5.8/busy/command/activate_command.py
--rw-r--r--   0        0        0     1152 2023-11-06 05:10:07.074190 busy-5.5.8/busy/command/add_command.py
--rw-r--r--   0        0        0      293 2023-11-06 05:10:07.074190 busy-5.5.8/busy/command/base_command.py
--rw-r--r--   0        0        0     6878 2023-11-06 05:10:07.074190 busy-5.5.8/busy/command/command.py
--rw-r--r--   0        0        0      246 2023-11-06 05:10:07.074190 busy-5.5.8/busy/command/curses_command.py
--rw-r--r--   0        0        0     1714 2023-11-06 05:10:07.074190 busy-5.5.8/busy/command/defer_command.py
--rw-r--r--   0        0        0      965 2023-11-06 05:10:07.074190 busy-5.5.8/busy/command/delete_command.py
--rw-r--r--   0        0        0     1245 2023-11-06 05:10:07.074190 busy-5.5.8/busy/command/drop_and_pop_command.py
--rw-r--r--   0        0        0      683 2023-11-06 05:10:07.074190 busy-5.5.8/busy/command/edit_command.py
--rw-r--r--   0        0        0     1973 2023-11-06 05:10:07.074190 busy-5.5.8/busy/command/finish_command.py
--rw-r--r--   0        0        0      758 2023-11-06 05:10:07.074190 busy-5.5.8/busy/command/list_command.py
--rw-r--r--   0        0        0     1311 2023-11-06 05:10:07.074190 busy-5.5.8/busy/command/print_command.py
--rw-r--r--   0        0        0      272 2023-11-06 05:10:07.074190 busy-5.5.8/busy/command/queues_command.py
--rw-r--r--   0        0        0      284 2023-11-06 05:10:07.074190 busy-5.5.8/busy/command/resource_command.py
--rw-r--r--   0        0        0      256 2023-11-06 05:10:07.074190 busy-5.5.8/busy/command/show_command.py
--rw-r--r--   0        0        0     1040 2023-11-06 05:10:07.075190 busy-5.5.8/busy/command/switch_command.py
--rw-r--r--   0        0        0      334 2023-11-06 05:10:07.075190 busy-5.5.8/busy/command/tags_command.py
--rw-r--r--   0        0        0     3555 2023-11-06 05:10:07.075190 busy-5.5.8/busy/handler.py
--rw-r--r--   0        0        0        0 2023-11-06 05:10:07.104190 busy-5.5.8/busy/model/__init__.py
--rw-r--r--   0        0        0     5020 2023-11-06 05:10:07.075190 busy-5.5.8/busy/model/collection/__init__.py
--rw-r--r--   0        0        0      123 2023-11-06 05:10:07.075190 busy-5.5.8/busy/model/collection/done_collection.py
--rw-r--r--   0        0        0      123 2023-11-06 05:10:07.075190 busy-5.5.8/busy/model/collection/plan_collection.py
--rw-r--r--   0        0        0       81 2023-11-06 05:10:07.075190 busy-5.5.8/busy/model/collection/skip_collection.py
--rw-r--r--   0        0        0       81 2023-11-06 05:10:07.075190 busy-5.5.8/busy/model/collection/todo_collection.py
--rw-r--r--   0        0        0     3376 2023-11-06 05:10:07.075190 busy-5.5.8/busy/model/item.py
--rw-r--r--   0        0        0      237 2023-11-06 05:10:07.075190 busy-5.5.8/busy/storage/__init__.py
--rw-r--r--   0        0        0     2196 2023-11-06 05:10:07.075190 busy-5.5.8/busy/storage/file_storage.py
--rw-r--r--   0        0        0      133 2023-11-06 05:10:07.075190 busy-5.5.8/busy/ui/__init__.py
--rw-r--r--   0        0        0     9288 2023-11-06 05:10:07.075190 busy-5.5.8/busy/ui/curses_ui.py
--rw-r--r--   0        0        0     1499 2023-11-06 05:10:07.075190 busy-5.5.8/busy/ui/shell_ui.py
--rw-r--r--   0        0        0        0 2023-11-06 05:10:07.107190 busy-5.5.8/busy/ui/tcl_ui/__init__.py
--rw-r--r--   0        0        0      824 2023-11-06 05:10:07.075190 busy-5.5.8/busy/ui/tcl_ui/edit_task_widget.py
--rw-r--r--   0        0        0      701 2023-11-06 05:10:07.075190 busy-5.5.8/busy/ui/tcl_ui/get_item_widget.py
--rw-r--r--   0        0        0     5588 2023-11-06 05:10:07.075190 busy-5.5.8/busy/ui/ui.py
--rw-r--r--   0        0        0        0 2023-11-06 05:10:07.107190 busy-5.5.8/busy/util/__init__.py
--rw-r--r--   0        0        0     4443 2023-11-06 05:10:07.076190 busy-5.5.8/busy/util/checklist.py
--rw-r--r--   0        0        0     2844 2023-11-06 05:10:07.076190 busy-5.5.8/busy/util/date_util.py
--rw-r--r--   0        0        0      218 2023-11-06 05:10:07.076190 busy-5.5.8/busy/util/python_version.py
--rw-r--r--   0        0        0     2477 2023-11-06 05:10:07.076190 busy-5.5.8/busy/util/selector.py
--rw-r--r--   0        0        0      702 2023-11-06 05:10:24.727281 busy-5.5.8/pyproject.toml
--rw-r--r--   0        0        0    22924 1970-01-01 00:00:00.000000 busy-5.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-20 16:44:41.796714 busy-6.0.0/LICENSE
+-rw-r--r--   0        0        0    22370 2024-05-20 16:44:41.796714 busy-6.0.0/README.md
+-rw-r--r--   0        0        0      467 2024-05-20 16:44:41.796714 busy-6.0.0/busy/__init__.py
+-rw-r--r--   0        0        0       88 2024-05-20 16:44:41.796714 busy-6.0.0/busy/__main__.py
+-rw-r--r--   0        0        0     3879 2024-05-20 16:44:41.796714 busy-6.0.0/busy/command/__init__.py
+-rw-r--r--   0        0        0     1659 2024-05-20 16:44:41.796714 busy-6.0.0/busy/command/activate_command.py
+-rw-r--r--   0        0        0     1159 2024-05-20 16:44:41.797714 busy-6.0.0/busy/command/add_command.py
+-rw-r--r--   0        0        0      285 2024-05-20 16:44:41.797714 busy-6.0.0/busy/command/base_command.py
+-rw-r--r--   0        0        0     1709 2024-05-20 16:44:41.797714 busy-6.0.0/busy/command/defer_command.py
+-rw-r--r--   0        0        0      989 2024-05-20 16:44:41.797714 busy-6.0.0/busy/command/delete_command.py
+-rw-r--r--   0        0        0     1245 2024-05-20 16:44:41.797714 busy-6.0.0/busy/command/drop_and_pop_command.py
+-rw-r--r--   0        0        0      733 2024-05-20 16:44:41.797714 busy-6.0.0/busy/command/edit_command.py
+-rw-r--r--   0        0        0     1995 2024-05-20 16:44:41.797714 busy-6.0.0/busy/command/finish_command.py
+-rw-r--r--   0        0        0      750 2024-05-20 16:44:41.797714 busy-6.0.0/busy/command/list_command.py
+-rw-r--r--   0        0        0     1306 2024-05-20 16:44:41.797714 busy-6.0.0/busy/command/print_command.py
+-rw-r--r--   0        0        0      283 2024-05-20 16:44:41.797714 busy-6.0.0/busy/command/queues_command.py
+-rw-r--r--   0        0        0      276 2024-05-20 16:44:41.797714 busy-6.0.0/busy/command/resource_command.py
+-rw-r--r--   0        0        0      248 2024-05-20 16:44:41.798714 busy-6.0.0/busy/command/show_command.py
+-rw-r--r--   0        0        0      326 2024-05-20 16:44:41.798714 busy-6.0.0/busy/command/tags_command.py
+-rw-r--r--   0        0        0        0 2024-05-20 16:44:41.837714 busy-6.0.0/busy/model/__init__.py
+-rw-r--r--   0        0        0     5052 2024-05-20 16:44:41.798714 busy-6.0.0/busy/model/collection/__init__.py
+-rw-r--r--   0        0        0      123 2024-05-20 16:44:41.798714 busy-6.0.0/busy/model/collection/done_collection.py
+-rw-r--r--   0        0        0      123 2024-05-20 16:44:41.798714 busy-6.0.0/busy/model/collection/plan_collection.py
+-rw-r--r--   0        0        0       81 2024-05-20 16:44:41.798714 busy-6.0.0/busy/model/collection/skip_collection.py
+-rw-r--r--   0        0        0       81 2024-05-20 16:44:41.798714 busy-6.0.0/busy/model/collection/todo_collection.py
+-rw-r--r--   0        0        0     3376 2024-05-20 16:44:41.798714 busy-6.0.0/busy/model/item.py
+-rw-r--r--   0        0        0      342 2024-05-20 16:44:41.798714 busy-6.0.0/busy/storage/__init__.py
+-rw-r--r--   0        0        0     2147 2024-05-20 16:44:41.798714 busy-6.0.0/busy/storage/file_storage.py
+-rw-r--r--   0        0        0        0 2024-05-20 16:44:41.838714 busy-6.0.0/busy/util/__init__.py
+-rw-r--r--   0        0        0     3783 2024-05-20 16:44:41.798714 busy-6.0.0/busy/util/checklist.py
+-rw-r--r--   0        0        0     2844 2024-05-20 16:44:41.799714 busy-6.0.0/busy/util/date_util.py
+-rw-r--r--   0        0        0      795 2024-05-20 16:44:41.799714 busy-6.0.0/busy/util/edit.py
+-rw-r--r--   0        0        0      218 2024-05-20 16:44:41.799714 busy-6.0.0/busy/util/python_version.py
+-rw-r--r--   0        0        0     2477 2024-05-20 16:44:41.799714 busy-6.0.0/busy/util/selector.py
+-rw-r--r--   0        0        0      454 2024-05-20 16:44:52.986501 busy-6.0.0/pyproject.toml
+-rw-r--r--   0        0        0    22889 1970-01-01 00:00:00.000000 busy-6.0.0/PKG-INFO
```

### Comparing `busy-5.5.8/LICENSE` & `busy-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `busy-5.5.8/README.md` & `busy-6.0.0/README.md`

 * *Files identical despite different names*

### Comparing `busy-5.5.8/busy/command/activate_command.py` & `busy-6.0.0/busy/command/activate_command.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-from dataclasses import dataclass
+from wizlib.parser import WizParser
 
-from busy.command.command import QueueCommand
+from busy.command import QueueCommand
 from busy.util import date_util
 
 
 def is_today_or_earlier(plan):
     return plan.plan_date <= date_util.today()
 
 
-@dataclass
 class ActivateCommand(QueueCommand):
 
     timing: str = ""
     yes: bool = None
     collection_state: str = 'plan'
     name = 'activate'
     key = 'c'
     default_criteria = [is_today_or_earlier]
 
     @classmethod
-    def set_parser(self, parser):
-        super().set_parser(parser)
+    def add_args(cls, parser: WizParser):
+        super().add_args(parser)
         # parser.add_argument('--timing', '-t', default='today')
-        self._add_confirmation_arg(parser)
+        cls.add_yes_arg(parser)
 
-    def clean_args(self):
+    def handle_vals(self):
+        super().handle_vals()
         # def update_timing():
-        #     self.timing = self.ui.get_string("Timing", "today")
-        super().clean_args()
+        #     self.timing = self.app.ui.get_text("Timing", "today")
+        super().handle_vals()
         # For now, handling criteria as normal
         if self.selection:
             if not self.provided('yes'):
                 items = self.collection.items(self.selection)
-                self.ui.output('\n'.join([str(i) for i in items]))
+                self.app.ui.send('\n'.join([str(i) for i in items]))
                 intro = f"Activate {self.count()}"
                 # self.confirm(intro, update_timing)
                 self.confirm(intro)
 
     @QueueCommand.wrap
     def execute(self):
         if not self.selection:
             self.status = "Activated nothing"
         elif self.yes is False:
             self.status = "Activate command canceled"
         else:
-            todos = self.storage.get_collection(self.queue)
+            todos = self.app.storage.get_collection(self.queue)
             activated = self.collection.delete(self.selection)
             for item in activated:
                 item.state = 'todo'
             todos[0:0] = activated
             self.status = f"Activated {self.count()}"
```

### Comparing `busy-5.5.8/busy/command/add_command.py` & `busy-6.0.0/busy/command/add_command.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-from dataclasses import dataclass
+from wizlib.parser import WizParser
 
-from busy.command.command import QueueCommand
+from busy.command import QueueCommand
 from busy.model.item import Item
 
 
-@dataclass
 class AddCommand(QueueCommand):
 
     description: str = ""
     name = 'add'
     key = 'a'
 
     @classmethod
-    def set_parser(self, parser):
-        super().set_parser(parser)
+    def add_args(cls, parser: WizParser):
+        super().add_args(parser)
         parser.add_argument('--description', '-d', nargs='?')
 
-    def clean_args(self):
-        super().clean_args()
+    def handle_vals(self):
+        super().handle_vals()
         if not self.provided('description'):
-            self.description = self.ui.edit_text("")
+            self.description = self.app.ui.get_text('Description: ')
             # edited = self.ui.edit_items(self.collection, self.selection)
 
     @QueueCommand.wrap
     def execute(self):
         if self.description:
             item = Item(self.description)
             self.collection.insert(0, item)
```

### Comparing `busy-5.5.8/busy/command/defer_command.py` & `busy-6.0.0/busy/command/defer_command.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from dataclasses import dataclass
+from wizlib.parser import WizParser
 
-from busy.command.command import QueueCommand
+from busy.command import QueueCommand
 from busy.util import date_util
 
 
-@dataclass
 class DeferCommand(QueueCommand):
 
     timing: str = ""
     yes: bool = None
     name = 'defer'
     key = 'f'
 
     @classmethod
-    def set_parser(self, parser):
-        super().set_parser(parser)
+    def add_args(cls, parser: WizParser):
+        super().add_args(parser)
         parser.add_argument('--timing', '-t', default='tomorrow')
-        self._add_confirmation_arg(parser)
+        cls.add_yes_arg(parser)
+
+    def handle_vals(self):
+        super().handle_vals()
 
-    def clean_args(self):
         def update_deferral():
-            self.timing = self.ui.get_string("Timing", "tomorrow")
-        super().clean_args()
+            self.timing = self.app.ui.get_text("Timing: ", [], "tomorrow")
         if self.selection:
             items = self.collection.items(self.selection)
-            self.ui.output('\n'.join([str(i) for i in items]))
+            self.app.ui.send('\n'.join([str(i) for i in items]))
             if not self.provided('timing'):
                 self.timing = 'tomorrow'
             while not self.provided('yes'):
                 intro = f"Defer {self.count()} to {self.date}"
                 self.confirm(intro, update_deferral)
 
     @property
@@ -40,14 +40,14 @@
     @QueueCommand.wrap
     def execute(self):
         if not self.selection:
             self.status = "Deferred nothing"
         elif self.yes is False:
             self.status = "Defer operation unconfirmed"
         else:
-            plans = self.storage.get_collection(self.queue, 'plan')
+            plans = self.app.storage.get_collection(self.queue, 'plan')
             deferred = self.collection.delete(self.selection)
             for item in deferred:
                 item.plan_date = self.date
                 item.state = 'plan'
             plans.extend(deferred)
             self.status = f"Deferred {self.count(deferred)} to {self.date}"
```

### Comparing `busy-5.5.8/busy/command/delete_command.py` & `busy-6.0.0/busy/command/delete_command.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-from dataclasses import dataclass
 
-from busy.command.command import CollectionCommand
+from wizlib.parser import WizParser
+
+from busy.command import CollectionCommand
 
 
-@dataclass
 class DeleteCommand(CollectionCommand):
 
     yes: bool = None
     name = 'delete'
     key = 'd'
     default_criteria = [1]
 
     @classmethod
-    def set_parser(self, parser):
-        super().set_parser(parser)
+    def add_args(cls, parser: WizParser):
+        super().add_args(parser)
         parser.add_argument('--yes', action='store_true', default=None)
 
-    def clean_args(self):
-        super().clean_args()
+    def handle_vals(self):
+        super().handle_vals()
+        super().handle_vals()
         if self.selection:
             items = self.collection.items(self.selection)
-            self.ui.output('\n'.join([str(i) for i in items]))
+            self.app.ui.send('\n'.join([str(i) for i in items]))
             self.confirm(f"Delete {self.count()}")
 
     # Assume the indices have been already set, before confirmation.
 
     @CollectionCommand.wrap
     def execute(self):
         if self.yes:
```

### Comparing `busy-5.5.8/busy/command/drop_and_pop_command.py` & `busy-6.0.0/busy/command/drop_and_pop_command.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from busy.command.command import QueueCommand
+from busy.command import QueueCommand
 
 
 class DropCommand(QueueCommand):
     """Move an item to the end of the todo collection of a queue"""
 
     name = 'drop'
     key = 'r'
     default_criteria = [1]
 
     @QueueCommand.wrap
     def execute(self):
-        collection = self.storage.get_collection(self.queue)
+        collection = self.app.storage.get_collection(self.queue)
         lolist, hilist = self.collection.split(self.selection)
         self.collection.data = hilist + lolist
         if len(lolist) == 1:
             self.status = f"Dropped: {str(lolist[0])}"
         elif lolist:
             self.status = f"Dropped {str(len(lolist))} Items"
         else:
@@ -26,15 +26,15 @@
 
     name = 'pop'
     key = 'o'
     default_criteria = ['-']
 
     @QueueCommand.wrap
     def execute(self):
-        collection = self.storage.get_collection(self.queue)
+        collection = self.app.storage.get_collection(self.queue)
         hilist, lolist = self.collection.split(self.selection)
         self.collection.data = hilist + lolist
         if len(hilist) == 1:
             self.status = f"Popped: {str(hilist[0])}"
         elif hilist:
             self.status = f"Popped {str(len(hilist))} Items"
         else:
```

### Comparing `busy-5.5.8/busy/command/edit_command.py` & `busy-6.0.0/busy/command/edit_command.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from dataclasses import dataclass
 
-from busy.command.command import CollectionCommand
+
+from busy.command import CollectionCommand
+from busy.util.edit import edit_items
 
 
-@dataclass
 class EditorCommandBase(CollectionCommand):
 
     @CollectionCommand.wrap
     def execute(self):
         if not self.selection:
             self.status = "Edited nothing"
         else:
-            edited = self.ui.edit_items(self.collection, self.selection)
+            command = self.app.config.get('editor') or 'emacs'
+            edited = edit_items(self.collection, self.selection, command)
             self.status = f"Edited {self.count(edited)}"
 
 
 class EditOneItemCommand(EditorCommandBase):
     """Edit items; default to just one"""
 
     name = "edit"
```

### Comparing `busy-5.5.8/busy/command/finish_command.py` & `busy-6.0.0/busy/command/finish_command.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,49 @@
-from dataclasses import dataclass
 
-from busy.command.command import QueueCommand
+
+from wizlib.parser import WizParser
+
+from busy.command import QueueCommand
 from busy.model.item import Item
 from busy.util import date_util
 from busy.util.date_util import relative_date
 
 
-@dataclass
 class FinishCommand(QueueCommand):
     """Mark a task as finished by moving it to the done queue"""
 
     yes: bool = None
     name = 'finish'
     key = 'n'
 
     @classmethod
-    def set_parser(self, parser):
-        super().set_parser(parser)
-        self._add_confirmation_arg(parser)
-
-    def clean_args(self):
-        super().clean_args()
+    def add_args(cls, parser: WizParser):
+        super().add_args(parser)
+        cls.add_yes_arg(parser)
+
+    def handle_vals(self):
+        super().handle_vals()
+        super().handle_vals()
         if self.selection:
             if not self.provided('yes'):
                 items = self.collection.items(self.selection)
-                self.ui.output('\n'.join([str(i) for i in items]))
+                self.app.ui.send('\n'.join([str(i) for i in items]))
                 intro = f"Finish {self.count()}"
                 self.confirm(intro)
 
     @QueueCommand.wrap
     def execute(self):
         if not self.selection:
             self.status = "Finished nothing"
         elif self.yes is False:
             self.status = "Finish operation unconfirmed"
         else:
             date = date_util.today()
-            dones = self.storage.get_collection(self.queue, 'done')
-            plans = self.storage.get_collection(self.queue, 'plan')
+            dones = self.app.storage.get_collection(self.queue, 'done')
+            plans = self.app.storage.get_collection(self.queue, 'plan')
             items = self.collection.delete(self.selection)
             finished = [Item(i.current, state='done',
                              done_date=date_util.today()) for i in items]
             nexts = [Item(i.next, state='todo') for i in items
                      if (i.next and not i.repeat)]
             repeats = [Item(i.description, state='plan',
                             plan_date=i.repeat_date)
```

### Comparing `busy-5.5.8/busy/command/list_command.py` & `busy-6.0.0/busy/command/list_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from busy.command.command import CollectionCommand
+from busy.command import CollectionCommand
 
 
 class ListCommand(CollectionCommand):
     """Show the descriptions with selection numbers, default to all"""
 
     name = 'list'
     # key = "l"
```

### Comparing `busy-5.5.8/busy/model/collection/__init__.py` & `busy-6.0.0/busy/model/collection/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     schema = ['description']
 
     def validate_item(self, item):
         if item.state != self.state:
             raise CollectionError(
                 f"Incorrect state {item.state} for {self.state} collection")
         if '|' in item.description:
-            raise CollectionError(
-                f"Pipe symbol not permitted in item description '{item.description}'")
+            raise CollectionError(f"Pipe symbol not permitted in item " +
+                                  f"description '{item.description}'")
 
     def validate(self, value):
         for item in value if isinstance(value, Iterable) else [value]:
             self.validate_item(item)
 
     # Override list methods to make sure we've got Items of the right state.
     # There might be some methods missing here. Also set changed.
@@ -85,15 +85,16 @@
             super().__init__(value)
         self.changed = False
 
     # Methods related to selection and maniuplation by "criteria"
     # Numbers in "criteria" start with 1.
 
     def select(self, *criteria):
-        """Take "criteria" (such as tags, ranges of numbers, etc) and return the
+        """
+        Take 'criteria' (such as tags, ranges of numbers, etc) and return the
         indices of the resulting items. In other parts of the class and
         subclasses, operations need to know what items to act on.
         """
         selector = Selector(criteria)
         return [i for i in selector.indices(self.data)]
 
     def items(self, indices: list[int] = None):
@@ -102,16 +103,16 @@
             return self.data
         else:
             return [self[i] for i in indices]
 
     def replace(self, indices: list, newvalues: list):
         """Replace existing items at the select provided.
 
-        Also inserts if the indices run out. Does not create items; expects them
-        to already exist. Does not return anything since the calling code
+        Also inserts if the indices run out. Does not create items; expects
+        them to already exist. Does not return anything since the calling code
         already has the new items.
         """
         _indices = sorted(indices)
         _newvalues = newvalues.copy()
         max = (_indices[-1] + 1) if _indices else 0
         while _newvalues and _indices:
             self[_indices.pop(0)] = _newvalues.pop(0)
```

### Comparing `busy-5.5.8/busy/model/item.py` & `busy-6.0.0/busy/model/item.py`

 * *Files identical despite different names*

### Comparing `busy-5.5.8/busy/storage/file_storage.py` & `busy-6.0.0/busy/storage/file_storage.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,24 +11,23 @@
 RE_QUEUE = re.compile(f"([a-zA-Z0-9\\-]+)\\.({'|'.join(STATES)})\\.psv")
 
 
 class FileStorage(Storage):
 
     def __init__(self, path: str = ''):
         if path:
-            self.root = Path(path) if isinstance(path, str) else path
+            self.directory = Path(path) if isinstance(path, str) else path
         else:
-            env_var = os.environ.get('BUSY_ROOT')
-            self.root = Path(env_var if env_var else Path.home() / '.busy')
-            self.root.mkdir(parents=True, exist_ok=True)
-        assert isinstance(self.root, Path) and self.root.is_dir()
+            self.directory = Path.home() / '.busy'
+        self.directory.mkdir(parents=True, exist_ok=True)
+        assert isinstance(self.directory, Path) and self.directory.is_dir()
         self.cache = {}
 
     def filepath(self, queue: str, state: str) -> str:
-        return self.root / f"{queue}.{state}.psv"
+        return self.directory / f"{queue}.{state}.psv"
 
     def get_collection(self, queue: str, state: str = 'todo'):
         id = (queue, state)
         if id not in self.cache:
             collection = Collection.family_member('state', state)()
             path = self.filepath(queue, state)
             if path.is_file():
@@ -42,15 +41,15 @@
         collections = [self.get_collection(queue, s) for s in STATES]
         return any(len(c) for c in collections)
 
     @property
     def queue_names(self):
         """Return names of queues. Cache nothing."""
         result = set()
-        for path in self.root.iterdir():
+        for path in self.directory.iterdir():
             if path.is_file() and (match := RE_QUEUE.match(path.name)):
                 queue = match.groups()[0]
                 if (queue not in result) and path.stat().st_size:
                     result.add(queue)
         return result
 
     def save(self):
```

### Comparing `busy-5.5.8/busy/util/checklist.py` & `busy-6.0.0/busy/util/checklist.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from reportlab.lib.pagesizes import letter as LETTER
 from reportlab.lib.units import inch as INCH
 from reportlab.pdfgen.canvas import Canvas
 from reportlab.pdfbase import pdfmetrics
 
 
 @dataclass
-class Checklist:
+class Checklist:  # pragma: nocover
 
     filenamestem: str = None
     pagesize: tuple = LETTER
     margin: float = 1.0 * INCH
     fontname_items: str = "Helvetica"
     fontname_heading: str = "Helvetica-Bold"
     fontsize_items: float = 12.0
@@ -95,31 +95,7 @@
             canvas.drawString(self.margin, self.topy, heading)
             y = self.topy - self.fontsize_heading - self.paragap
             for item in items:
                 y = self.print(canvas, item.capitalize(), y)
             canvas.save()
             run(['open', filepath.absolute()])
             sleep(1)  # A hack to give Preview time to open the temp file
-
-
-if __name__ == '__main__':
-
-    items = [
-        "welcome mat",
-        "wall patch kit",
-        "ReportLab can handle word wrap and text flow in generated PDF docs",
-        "brooms (2)",
-        "bins",
-        """
-        When using ReportLab, you have fine-grained control over the layout and
-        formatting of text. You can specify the width of text areas and enable
-        automatic word wrapping within those areas. This ensures that the text
-        flows naturally within the defined boundaries, wrapping to the next
-        line when necessary.
-        """,
-        "Bananas"
-    ] * 8
-
-    title = "Shopping"
-
-    p = Checklist()
-    p.generate(title, items)
```

### Comparing `busy-5.5.8/busy/util/date_util.py` & `busy-6.0.0/busy/util/date_util.py`

 * *Files identical despite different names*

### Comparing `busy-5.5.8/busy/util/selector.py` & `busy-6.0.0/busy/util/selector.py`

 * *Files identical despite different names*

### Comparing `busy-5.5.8/PKG-INFO` & `busy-6.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: busy
-Version: 5.5.8
+Version: 6.0.0
 Summary: Personal time management for techies
 License: MIT
 Author: Steampunk Wizard
 Author-email: busy@steampunkwizard.ca
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: platformdirs (>=3.10.0,<4.0.0)
-Requires-Dist: punkeditor (>=0.2,<0.3)
 Requires-Dist: reportlab (>=4.0.4,<5.0.0)
-Requires-Dist: wizlib (>=1.1,<1.2)
+Requires-Dist: wizlib (>=3.1.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 Busy
 ====
 
 Personal time management for techies
 ------------------------------------
```

#### html2text {}

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 2.1 Name: busy Version: 5.5.8 Summary: Personal time
+Metadata-Version: 2.1 Name: busy Version: 6.0.0 Summary: Personal time
 management for techies License: MIT Author: Steampunk Wizard Author-email:
 busy@steampunkwizard.ca Requires-Python: >=3.11,<3.12 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: platformdirs
-(>=3.10.0,<4.0.0) Requires-Dist: punkeditor (>=0.2,<0.3) Requires-Dist:
-reportlab (>=4.0.4,<5.0.0) Requires-Dist: wizlib (>=1.1,<1.2) Description-
-Content-Type: text/markdown Busy ==== Personal time management for techies ----
--------------------------------- Buzz through crazy busy days with as little
-stress as possible. Stay focused by seeing only one task at a time. Use this
-simple, fast, and fun tool all day with the keyboard in a familiar terminal
-environment.
+(>=3.10.0,<4.0.0) Requires-Dist: reportlab (>=4.0.4,<5.0.0) Requires-Dist:
+wizlib (>=3.1.0,<4.0.0) Description-Content-Type: text/markdown Busy ====
+Personal time management for techies ------------------------------------ Buzz
+through crazy busy days with as little stress as possible. Stay focused by
+seeing only one task at a time. Use this simple, fast, and fun tool all day
+with the keyboard in a familiar terminal environment.
 [https://gitlab.com/uploads/-/system/project/avatar/6521273/
 bee.png?width=64]_B_e_e_ _i_c_o_n_ _c_r_e_a_t_e_d_ _b_y_ _F_r_e_e_p_i_k_ _-_ _F_l_a_t_i_c_o_n Using Busy? [Contact
 us!](mailto:busy@steampunkwizard.ca)_ Usage ===== tl;dr: ```bash pipx install
 busy ``` ```bash busy ``` Principles ---------- Busy is built with the
 following usage principles in mind: - *Monotasking*: We each focus better when
 we work on exactly one task at a time. So busy only shows you one task. -
 *Keyboard-driven*: Productive people use the keyboard effectively, because
```

