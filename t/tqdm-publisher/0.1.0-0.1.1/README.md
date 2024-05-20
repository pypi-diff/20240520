# Comparing `tmp/tqdm_publisher-0.1.0.tar.gz` & `tmp/tqdm_publisher-0.1.1.tar.gz`

## Comparing `tqdm_publisher-0.1.0.tar` & `tqdm_publisher-0.1.1.tar`

### file list

```diff
@@ -1,42 +1,45 @@
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/.coveragerc
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/license.txt
--rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/.github/workflows/add_issue_to_dashboard.yml
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/.github/workflows/add_pull_request_to_dashboard.yml
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/.github/workflows/assess-file-changes.yml
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/.github/workflows/auto-publish.yml
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/.github/workflows/codespell.yml
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/.github/workflows/dailies.yml
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/.github/workflows/deploy-tests.yml
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/.github/workflows/testing.yml
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/src/tqdm_publisher/__init__.py
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/src/tqdm_publisher/_handler.py
--rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/src/tqdm_publisher/_publisher.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/src/tqdm_publisher/_subscriber.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/src/tqdm_publisher/testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/src/tqdm_publisher/_demos/__init__.py
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/src/tqdm_publisher/_demos/_client.css
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/src/tqdm_publisher/_demos/_demo_command_line_interface.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/src/tqdm_publisher/_demos/_multiple_bars/_client.html
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/src/tqdm_publisher/_demos/_multiple_bars/_client.js
--rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/src/tqdm_publisher/_demos/_multiple_bars/_server.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/src/tqdm_publisher/_demos/_parallel_bars/_client.html
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/src/tqdm_publisher/_demos/_parallel_bars/_client.js
--rw-r--r--   0        0        0     8104 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/src/tqdm_publisher/_demos/_parallel_bars/_server.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/src/tqdm_publisher/_demos/_single_bar/_client.html
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/src/tqdm_publisher/_demos/_single_bar/_client.js
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/src/tqdm_publisher/_demos/_single_bar/_server.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/src/tqdm_publisher/_demos/utils/EventSourceManager.js
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/src/tqdm_publisher/_demos/utils/WebSocketManager.js
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/src/tqdm_publisher/_demos/utils/elements.js
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/tests/test_handler.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/tests/test_publisher.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/tests/test_subscriber.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/.gitignore
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/README.md
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5924 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/.coveragerc
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/license.txt
+-rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/.github/workflows/add_issue_to_dashboard.yml
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/.github/workflows/add_pull_request_to_dashboard.yml
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/.github/workflows/assess-file-changes.yml
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/.github/workflows/auto-publish.yml
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/.github/workflows/codespell.yml
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/.github/workflows/dailies.yml
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/.github/workflows/deploy-tests.yml
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/.github/workflows/testing.yml
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/src/tqdm_publisher/__init__.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/src/tqdm_publisher/_handler.py
+-rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/src/tqdm_publisher/_publisher.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/src/tqdm_publisher/_subscriber.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/src/tqdm_publisher/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/src/tqdm_publisher/_demos/__init__.py
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/src/tqdm_publisher/_demos/_client.css
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/src/tqdm_publisher/_demos/_demo_command_line_interface.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/src/tqdm_publisher/_demos/_multiple_bars/README.md
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/src/tqdm_publisher/_demos/_multiple_bars/_client.html
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/src/tqdm_publisher/_demos/_multiple_bars/_client.js
+-rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/src/tqdm_publisher/_demos/_multiple_bars/_server.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/src/tqdm_publisher/_demos/_parallel_bars/README.md
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/src/tqdm_publisher/_demos/_parallel_bars/_client.html
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/src/tqdm_publisher/_demos/_parallel_bars/_client.js
+-rw-r--r--   0        0        0     8106 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/src/tqdm_publisher/_demos/_parallel_bars/_server.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/src/tqdm_publisher/_demos/_single_bar/README.md
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/src/tqdm_publisher/_demos/_single_bar/_client.html
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/src/tqdm_publisher/_demos/_single_bar/_client.js
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/src/tqdm_publisher/_demos/_single_bar/_server.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/src/tqdm_publisher/_demos/utils/EventSourceManager.js
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/src/tqdm_publisher/_demos/utils/WebSocketManager.js
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/src/tqdm_publisher/_demos/utils/elements.js
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/tests/test_handler.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/tests/test_publisher.py
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/tests/test_subscriber.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/.gitignore
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/README.md
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5924 2020-02-02 00:00:00.000000 tqdm_publisher-0.1.1/PKG-INFO
```

### Comparing `tqdm_publisher-0.1.0/license.txt` & `tqdm_publisher-0.1.1/license.txt`

 * *Files identical despite different names*

### Comparing `tqdm_publisher-0.1.0/.github/CODE_OF_CONDUCT.md` & `tqdm_publisher-0.1.1/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `tqdm_publisher-0.1.0/.github/ISSUE_TEMPLATE/bug_report.yml` & `tqdm_publisher-0.1.1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `tqdm_publisher-0.1.0/.github/workflows/assess-file-changes.yml` & `tqdm_publisher-0.1.1/.github/workflows/assess-file-changes.yml`

 * *Files identical despite different names*

### Comparing `tqdm_publisher-0.1.0/.github/workflows/auto-publish.yml` & `tqdm_publisher-0.1.1/.github/workflows/auto-publish.yml`

 * *Files identical despite different names*

### Comparing `tqdm_publisher-0.1.0/.github/workflows/dailies.yml` & `tqdm_publisher-0.1.1/.github/workflows/dailies.yml`

 * *Files identical despite different names*

### Comparing `tqdm_publisher-0.1.0/.github/workflows/deploy-tests.yml` & `tqdm_publisher-0.1.1/.github/workflows/deploy-tests.yml`

 * *Files identical despite different names*

### Comparing `tqdm_publisher-0.1.0/.github/workflows/testing.yml` & `tqdm_publisher-0.1.1/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `tqdm_publisher-0.1.0/src/tqdm_publisher/_handler.py` & `tqdm_publisher-0.1.1/src/tqdm_publisher/_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,29 +13,29 @@
 
     def listen(self) -> queue.Queue:
         new_queue = self._queue(maxsize=0)
         self.listeners.append(new_queue)
         return new_queue
 
     def create_progress_subscriber(
-        self, iterable: Iterable[Any], additional_metadata: dict = dict(), **tqdm_kwargs
+        self, *tqdm_args, additional_metadata: dict = dict(), **tqdm_kwargs
     ) -> TQDMProgressSubscriber:
 
         def on_progress_update(progress_update: dict):
             """
             This is the injection called on every update of the progress bar.
 
             It triggers the announcement event over all listeners on each update of the progress bar.
 
             It must be defined inside this local scope to communicate the `additional_metadata` from the level above
             without including it in the method signature.
             """
             self.announce(message=dict(**progress_update, **additional_metadata))
 
-        return TQDMProgressSubscriber(iterable=iterable, on_progress_update=on_progress_update, **tqdm_kwargs)
+        return TQDMProgressSubscriber(*tqdm_args, on_progress_update=on_progress_update, **tqdm_kwargs)
 
     def announce(self, message: Dict[Any, Any]):
         """
         Announce a message to all listeners.
 
         This message can be any dictionary. But, when used internally, is
         expected to contain the progress_bar_id and format_dict of the TQDMProgressSubscriber update function,
```

### Comparing `tqdm_publisher-0.1.0/src/tqdm_publisher/_publisher.py` & `tqdm_publisher-0.1.1/src/tqdm_publisher/_publisher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Union
 from uuid import uuid4
 
 from tqdm import tqdm as base_tqdm
 
 
 class TQDMProgressPublisher(base_tqdm):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(self, *tqdm_args, **tqdm_kwargs):
+        super().__init__(*tqdm_args, **tqdm_kwargs)
         self.progress_bar_id = str(uuid4())
         self.callbacks = dict()
 
     # Override the update method to run callbacks
     def update(self, n: int = 1) -> Union[bool, None]:
         displayed = super().update(n)
```

### Comparing `tqdm_publisher-0.1.0/src/tqdm_publisher/_subscriber.py` & `tqdm_publisher-0.1.1/src/tqdm_publisher/_subscriber.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from typing import Any, Dict, Iterable
+from typing import Any, Dict, Iterable, Optional
 
 from ._publisher import TQDMProgressPublisher
 
 
 class TQDMProgressSubscriber(TQDMProgressPublisher):
-    def __init__(self, iterable: Iterable[Any], on_progress_update: callable, **tqdm_kwargs):
-        super().__init__(iterable=iterable, **tqdm_kwargs)
+    def __init__(self, *tqdm_args, on_progress_update: callable, **tqdm_kwargs):
+
+        super().__init__(*tqdm_args, **tqdm_kwargs)
 
         def run_on_progress_update(format_dict: Dict[str, Any]):
             """
             This is the injection called on every update of the progress bar.
 
             It calls the `on_progress_update` function, which must take a dictionary
             containing the progress bar ID and `format_dict`.
```

### Comparing `tqdm_publisher-0.1.0/src/tqdm_publisher/_demos/_client.css` & `tqdm_publisher-0.1.1/src/tqdm_publisher/_demos/_client.css`

 * *Files identical despite different names*

### Comparing `tqdm_publisher-0.1.0/src/tqdm_publisher/_demos/_demo_command_line_interface.py` & `tqdm_publisher-0.1.1/src/tqdm_publisher/_demos/_demo_command_line_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     "demo_single": dict(subpath="_single_bar", server=run_single_bar_demo),
     "demo_multiple": dict(subpath="_multiple_bars", server=run_multiple_bar_demo),
     "demo_parallel": dict(subpath="_parallel_bars", server=run_parallel_bar_demo),
 }
 
 DEMO_BASE_FOLDER_PATH = Path(__file__).parent
 
+
 def _command_line_interface():
     """A simple command line interface for running the demo for TQDM Publisher."""
     if len(sys.argv) <= 1:
         print("No input provided. Please specify a command (e.g. 'demo').")
         return
 
     command = sys.argv[1]
```

### Comparing `tqdm_publisher-0.1.0/src/tqdm_publisher/_demos/_multiple_bars/_client.html` & `tqdm_publisher-0.1.1/src/tqdm_publisher/_demos/_multiple_bars/_client.html`

 * *Files identical despite different names*

### Comparing `tqdm_publisher-0.1.0/src/tqdm_publisher/_demos/_multiple_bars/_client.js` & `tqdm_publisher-0.1.1/src/tqdm_publisher/_demos/_multiple_bars/_client.js`

 * *Files identical despite different names*

### Comparing `tqdm_publisher-0.1.0/src/tqdm_publisher/_demos/_multiple_bars/_server.py` & `tqdm_publisher-0.1.1/src/tqdm_publisher/_demos/_multiple_bars/_server.py`

 * *Files identical despite different names*

### Comparing `tqdm_publisher-0.1.0/src/tqdm_publisher/_demos/_parallel_bars/_client.html` & `tqdm_publisher-0.1.1/src/tqdm_publisher/_demos/_parallel_bars/_client.html`

 * *Files identical despite different names*

### Comparing `tqdm_publisher-0.1.0/src/tqdm_publisher/_demos/_parallel_bars/_client.js` & `tqdm_publisher-0.1.1/src/tqdm_publisher/_demos/_parallel_bars/_client.js`

 * *Files identical despite different names*

### Comparing `tqdm_publisher-0.1.0/src/tqdm_publisher/_demos/_parallel_bars/_server.py` & `tqdm_publisher-0.1.1/src/tqdm_publisher/_demos/_parallel_bars/_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,19 +211,20 @@
 @cross_origin()
 def update():
     data = json.loads(request.data) if request.data else {}
     request_id = data["request_id"]
     progress_bar_id = data["id"]
     format_dict = data["data"]
 
-    # Forward updates over Sever-Side Events
+    # Forward updates over Server-Sent Events
     progress_handler.announce(dict(request_id=request_id, progress_bar_id=progress_bar_id, format_dict=format_dict))
 
     return jsonify({"status": "success"})
 
+
 @app.route("/events", methods=["GET"])
 @cross_origin()
 def events():
     return Response(listen_to_events(), mimetype="text/event-stream")
 
 
 async def start_server(port):
```

### Comparing `tqdm_publisher-0.1.0/src/tqdm_publisher/_demos/_single_bar/_client.html` & `tqdm_publisher-0.1.1/src/tqdm_publisher/_demos/_single_bar/_client.html`

 * *Files identical despite different names*

### Comparing `tqdm_publisher-0.1.0/src/tqdm_publisher/_demos/_single_bar/_client.js` & `tqdm_publisher-0.1.1/src/tqdm_publisher/_demos/_single_bar/_client.js`

 * *Files identical despite different names*

### Comparing `tqdm_publisher-0.1.0/src/tqdm_publisher/_demos/_single_bar/_server.py` & `tqdm_publisher-0.1.1/src/tqdm_publisher/_demos/_single_bar/_server.py`

 * *Files identical despite different names*

### Comparing `tqdm_publisher-0.1.0/src/tqdm_publisher/_demos/utils/EventSourceManager.js` & `tqdm_publisher-0.1.1/src/tqdm_publisher/_demos/utils/EventSourceManager.js`

 * *Files identical despite different names*

### Comparing `tqdm_publisher-0.1.0/src/tqdm_publisher/_demos/utils/WebSocketManager.js` & `tqdm_publisher-0.1.1/src/tqdm_publisher/_demos/utils/WebSocketManager.js`

 * *Files identical despite different names*

### Comparing `tqdm_publisher-0.1.0/src/tqdm_publisher/_demos/utils/elements.js` & `tqdm_publisher-0.1.1/src/tqdm_publisher/_demos/utils/elements.js`

 * *Files identical despite different names*

### Comparing `tqdm_publisher-0.1.0/tests/test_handler.py` & `tqdm_publisher-0.1.1/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `tqdm_publisher-0.1.0/tests/test_publisher.py` & `tqdm_publisher-0.1.1/tests/test_publisher.py`

 * *Files identical despite different names*

### Comparing `tqdm_publisher-0.1.0/tests/test_subscriber.py` & `tqdm_publisher-0.1.1/tests/test_subscriber.py`

 * *Files 21% similar despite different names*

```diff
@@ -26,14 +26,53 @@
         assert str(UUID(identifier, version=4)) == identifier
 
         assert "format_dict" in data
         format = data["format_dict"]
         assert "n" in format and "total" in format
 
     tasks = create_tasks()
-    subscriber = TQDMProgressSubscriber(asyncio.as_completed(tasks), test_callback, total=len(tasks))
+    total = len(tasks)
+    subscriber = TQDMProgressSubscriber(
+        asyncio.as_completed(tasks),
+        total=total,
+        mininterval=0,
+        on_progress_update=test_callback,
+    )
 
     # Simulate an update to trigger the callback
     for f in subscriber:
         await f
 
-    assert n_callback_executions > 1
+    assert n_callback_executions == total + 1
+
+
+# Test manual update management
+@pytest.mark.asyncio
+async def test_manual_updates():
+    n_callback_executions = 0
+
+    def test_callback(data):
+        nonlocal n_callback_executions
+        n_callback_executions += 1
+
+        print(data)
+
+        assert "progress_bar_id" in data
+        identifier = data["progress_bar_id"]
+        assert str(UUID(identifier, version=4)) == identifier
+
+        assert "format_dict" in data
+        format = data["format_dict"]
+        assert "n" in format and "total" in format
+
+    tasks = create_tasks(10)
+    total = len(tasks)
+    subscriber = TQDMProgressSubscriber(on_progress_update=test_callback, total=total, mininterval=0)
+
+    # Simulate updatse to trigger the callback
+    for task in asyncio.as_completed(tasks):
+        await task
+        subscriber.update(1)  # Update by 1 iteration
+
+    assert n_callback_executions == total + 1
+
+    subscriber.close()
```

### Comparing `tqdm_publisher-0.1.0/.gitignore` & `tqdm_publisher-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tqdm_publisher-0.1.0/README.md` & `tqdm_publisher-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # tqdm-publisher
-[![PyPI version](https://badge.fury.io/py/tqdm_publisher.svg)](https://badge.fury.io/py/tqdm_publisher.svg)
+[![PyPI version](https://badge.fury.io/py/tqdm-publisher.svg)](https://badge.fury.io/py/tqdm-publisher.svg)
 [![codecov](https://codecov.io/github/catalystneuro/tqdm_publisher/coverage.svg?branch=main)](https://codecov.io/github/catalystneuro/tqdm_publisher?branch=main)
 [![License](https://img.shields.io/pypi/l/tqdm_publisher.svg)](https://github.com/catalystneuro/tqdm_publisher/blob/main/license.txt)
 
 `tqdm_publisher` is a small Python package that allows you to subscribe to updates from `tqdm` progress bars with arbitrary callback functions.
 
 This is useful if you want to use `tqdm` to track the progress of a long-running task, but you also want to do something else with the progress information (e.g., forward it to a user interface, log it to a file, etc.).
```

### Comparing `tqdm_publisher-0.1.0/pyproject.toml` & `tqdm_publisher-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.version]
 source = "vcs"
 
 [project]
 name = "tqdm_publisher"
-version="0.1.0"
+version="0.1.1"
 authors = [
   { name="Garrett Flynn", email="garrett.flynn@catalystneuro.com" },
   { name="Cody Baker", email="cody.baker@catalystneuro.com" },
 ]
 description = "Extends the base tqdm progress bar with a subscribe method that can expose updates to external (potentially non-Python) processes."
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `tqdm_publisher-0.1.0/PKG-INFO` & `tqdm_publisher-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tqdm_publisher
-Version: 0.1.0
+Version: 0.1.1
 Summary: Extends the base tqdm progress bar with a subscribe method that can expose updates to external (potentially non-Python) processes.
 Project-URL: Homepage, https://github.com/catalystneuro/tqdm_publisher
 Project-URL: Bug Tracker, https://github.com/catalystneuro/tqdm_publisher/issues
 Author-email: Garrett Flynn <garrett.flynn@catalystneuro.com>, Cody Baker <cody.baker@catalystneuro.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, CatalystNeuro
@@ -55,15 +55,15 @@
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-asyncio; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Description-Content-Type: text/markdown
 
 # tqdm-publisher
-[![PyPI version](https://badge.fury.io/py/tqdm_publisher.svg)](https://badge.fury.io/py/tqdm_publisher.svg)
+[![PyPI version](https://badge.fury.io/py/tqdm-publisher.svg)](https://badge.fury.io/py/tqdm-publisher.svg)
 [![codecov](https://codecov.io/github/catalystneuro/tqdm_publisher/coverage.svg?branch=main)](https://codecov.io/github/catalystneuro/tqdm_publisher?branch=main)
 [![License](https://img.shields.io/pypi/l/tqdm_publisher.svg)](https://github.com/catalystneuro/tqdm_publisher/blob/main/license.txt)
 
 `tqdm_publisher` is a small Python package that allows you to subscribe to updates from `tqdm` progress bars with arbitrary callback functions.
 
 This is useful if you want to use `tqdm` to track the progress of a long-running task, but you also want to do something else with the progress information (e.g., forward it to a user interface, log it to a file, etc.).
```

