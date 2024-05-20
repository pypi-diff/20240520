# Comparing `tmp/deltachat_rpc_client-1.139.2.tar.gz` & `tmp/deltachat_rpc_client-1.139.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltachat_rpc_client-1.139.2.tar", last modified: Sat May 18 21:06:20 2024, max compression
+gzip compressed data, was "deltachat_rpc_client-1.139.3.tar", last modified: Mon May 20 18:41:23 2024, max compression
```

## Comparing `deltachat_rpc_client-1.139.2.tar` & `deltachat_rpc_client-1.139.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:06:20.384030 deltachat_rpc_client-1.139.2/
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-05-18 21:06:11.000000 deltachat_rpc_client-1.139.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-18 21:06:20.384030 deltachat_rpc_client-1.139.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-18 21:06:11.000000 deltachat_rpc_client-1.139.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-18 21:06:11.000000 deltachat_rpc_client-1.139.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 21:06:20.384030 deltachat_rpc_client-1.139.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:06:20.380030 deltachat_rpc_client-1.139.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:06:20.384030 deltachat_rpc_client-1.139.2/src/deltachat_rpc_client/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-18 21:06:11.000000 deltachat_rpc_client-1.139.2/src/deltachat_rpc_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-18 21:06:11.000000 deltachat_rpc_client-1.139.2/src/deltachat_rpc_client/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13369 2024-05-18 21:06:11.000000 deltachat_rpc_client-1.139.2/src/deltachat_rpc_client/account.py
--rw-r--r--   0 runner    (1001) docker     (127)    10659 2024-05-18 21:06:11.000000 deltachat_rpc_client-1.139.2/src/deltachat_rpc_client/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-18 21:06:11.000000 deltachat_rpc_client-1.139.2/src/deltachat_rpc_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-05-18 21:06:11.000000 deltachat_rpc_client-1.139.2/src/deltachat_rpc_client/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-18 21:06:11.000000 deltachat_rpc_client-1.139.2/src/deltachat_rpc_client/contact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-18 21:06:11.000000 deltachat_rpc_client-1.139.2/src/deltachat_rpc_client/deltachat.py
--rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-05-18 21:06:11.000000 deltachat_rpc_client-1.139.2/src/deltachat_rpc_client/direct_imap.py
--rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-05-18 21:06:11.000000 deltachat_rpc_client-1.139.2/src/deltachat_rpc_client/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-18 21:06:11.000000 deltachat_rpc_client-1.139.2/src/deltachat_rpc_client/message.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-18 21:06:11.000000 deltachat_rpc_client-1.139.2/src/deltachat_rpc_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-05-18 21:06:11.000000 deltachat_rpc_client-1.139.2/src/deltachat_rpc_client/pytestplugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-18 21:06:11.000000 deltachat_rpc_client-1.139.2/src/deltachat_rpc_client/rpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:06:20.384030 deltachat_rpc_client-1.139.2/src/deltachat_rpc_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-18 21:06:20.000000 deltachat_rpc_client-1.139.2/src/deltachat_rpc_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-18 21:06:20.000000 deltachat_rpc_client-1.139.2/src/deltachat_rpc_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 21:06:20.000000 deltachat_rpc_client-1.139.2/src/deltachat_rpc_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-18 21:06:20.000000 deltachat_rpc_client-1.139.2/src/deltachat_rpc_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-18 21:06:20.000000 deltachat_rpc_client-1.139.2/src/deltachat_rpc_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-18 21:06:20.000000 deltachat_rpc_client-1.139.2/src/deltachat_rpc_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:06:20.384030 deltachat_rpc_client-1.139.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-05-18 21:06:11.000000 deltachat_rpc_client-1.139.2/tests/test_chatlist_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    24172 2024-05-18 21:06:11.000000 deltachat_rpc_client-1.139.2/tests/test_securejoin.py
--rw-r--r--   0 runner    (1001) docker     (127)    22129 2024-05-18 21:06:11.000000 deltachat_rpc_client-1.139.2/tests/test_something.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-18 21:06:11.000000 deltachat_rpc_client-1.139.2/tests/test_vcard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-18 21:06:11.000000 deltachat_rpc_client-1.139.2/tests/test_webxdc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:41:23.576413 deltachat_rpc_client-1.139.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-05-20 18:41:17.000000 deltachat_rpc_client-1.139.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-20 18:41:23.576413 deltachat_rpc_client-1.139.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-20 18:41:17.000000 deltachat_rpc_client-1.139.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-20 18:41:17.000000 deltachat_rpc_client-1.139.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 18:41:23.576413 deltachat_rpc_client-1.139.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:41:23.572414 deltachat_rpc_client-1.139.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:41:23.572414 deltachat_rpc_client-1.139.3/src/deltachat_rpc_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-20 18:41:17.000000 deltachat_rpc_client-1.139.3/src/deltachat_rpc_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-20 18:41:17.000000 deltachat_rpc_client-1.139.3/src/deltachat_rpc_client/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13612 2024-05-20 18:41:17.000000 deltachat_rpc_client-1.139.3/src/deltachat_rpc_client/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10659 2024-05-20 18:41:17.000000 deltachat_rpc_client-1.139.3/src/deltachat_rpc_client/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-20 18:41:17.000000 deltachat_rpc_client-1.139.3/src/deltachat_rpc_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-05-20 18:41:17.000000 deltachat_rpc_client-1.139.3/src/deltachat_rpc_client/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-20 18:41:17.000000 deltachat_rpc_client-1.139.3/src/deltachat_rpc_client/contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-20 18:41:17.000000 deltachat_rpc_client-1.139.3/src/deltachat_rpc_client/deltachat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-05-20 18:41:17.000000 deltachat_rpc_client-1.139.3/src/deltachat_rpc_client/direct_imap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-05-20 18:41:17.000000 deltachat_rpc_client-1.139.3/src/deltachat_rpc_client/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-20 18:41:17.000000 deltachat_rpc_client-1.139.3/src/deltachat_rpc_client/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-20 18:41:17.000000 deltachat_rpc_client-1.139.3/src/deltachat_rpc_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-05-20 18:41:17.000000 deltachat_rpc_client-1.139.3/src/deltachat_rpc_client/pytestplugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-20 18:41:17.000000 deltachat_rpc_client-1.139.3/src/deltachat_rpc_client/rpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:41:23.576413 deltachat_rpc_client-1.139.3/src/deltachat_rpc_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-20 18:41:23.000000 deltachat_rpc_client-1.139.3/src/deltachat_rpc_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-20 18:41:23.000000 deltachat_rpc_client-1.139.3/src/deltachat_rpc_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 18:41:23.000000 deltachat_rpc_client-1.139.3/src/deltachat_rpc_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-20 18:41:23.000000 deltachat_rpc_client-1.139.3/src/deltachat_rpc_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-20 18:41:23.000000 deltachat_rpc_client-1.139.3/src/deltachat_rpc_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 18:41:23.000000 deltachat_rpc_client-1.139.3/src/deltachat_rpc_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:41:23.576413 deltachat_rpc_client-1.139.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7409 2024-05-20 18:41:17.000000 deltachat_rpc_client-1.139.3/tests/test_chatlist_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24172 2024-05-20 18:41:17.000000 deltachat_rpc_client-1.139.3/tests/test_securejoin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22129 2024-05-20 18:41:17.000000 deltachat_rpc_client-1.139.3/tests/test_something.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-20 18:41:17.000000 deltachat_rpc_client-1.139.3/tests/test_vcard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-20 18:41:17.000000 deltachat_rpc_client-1.139.3/tests/test_webxdc.py
```

### Comparing `deltachat_rpc_client-1.139.2/LICENSE` & `deltachat_rpc_client-1.139.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.2/PKG-INFO` & `deltachat_rpc_client-1.139.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltachat-rpc-client
-Version: 1.139.2
+Version: 1.139.3
 Summary: Python client for Delta Chat core JSON-RPC interface
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
```

### Comparing `deltachat_rpc_client-1.139.2/README.md` & `deltachat_rpc_client-1.139.3/README.md`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.2/pyproject.toml` & `deltachat_rpc_client-1.139.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=45"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "deltachat-rpc-client"
-version = "1.139.2"
+version = "1.139.3"
 description = "Python client for Delta Chat core JSON-RPC interface"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS :: MacOS X",
```

### Comparing `deltachat_rpc_client-1.139.2/src/deltachat_rpc_client/__init__.py` & `deltachat_rpc_client-1.139.3/src/deltachat_rpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.2/src/deltachat_rpc_client/_utils.py` & `deltachat_rpc_client-1.139.3/src/deltachat_rpc_client/_utils.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.2/src/deltachat_rpc_client/account.py` & `deltachat_rpc_client-1.139.3/src/deltachat_rpc_client/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,14 +293,20 @@
     def wait_for_incoming_msg_event(self):
         """Wait for incoming message event and return it."""
         while True:
             event = self.wait_for_event()
             if event.kind == EventType.INCOMING_MSG:
                 return event
 
+    def wait_for_incoming_msg(self):
+        """Wait for incoming message and return it.
+
+        Consumes all events before the next incoming message event."""
+        return self.get_message_by_id(self.wait_for_incoming_msg_event().msg_id)
+
     def wait_for_securejoin_inviter_success(self):
         while True:
             event = self.wait_for_event()
             if event["kind"] == "SecurejoinInviterProgress" and event["progress"] == 1000:
                 break
 
     def wait_for_securejoin_joiner_success(self):
```

### Comparing `deltachat_rpc_client-1.139.2/src/deltachat_rpc_client/chat.py` & `deltachat_rpc_client-1.139.3/src/deltachat_rpc_client/chat.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.2/src/deltachat_rpc_client/client.py` & `deltachat_rpc_client-1.139.3/src/deltachat_rpc_client/client.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.2/src/deltachat_rpc_client/const.py` & `deltachat_rpc_client-1.139.3/src/deltachat_rpc_client/const.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.2/src/deltachat_rpc_client/contact.py` & `deltachat_rpc_client-1.139.3/src/deltachat_rpc_client/contact.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.2/src/deltachat_rpc_client/deltachat.py` & `deltachat_rpc_client-1.139.3/src/deltachat_rpc_client/deltachat.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.2/src/deltachat_rpc_client/direct_imap.py` & `deltachat_rpc_client-1.139.3/src/deltachat_rpc_client/direct_imap.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.2/src/deltachat_rpc_client/events.py` & `deltachat_rpc_client-1.139.3/src/deltachat_rpc_client/events.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.2/src/deltachat_rpc_client/message.py` & `deltachat_rpc_client-1.139.3/src/deltachat_rpc_client/message.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.2/src/deltachat_rpc_client/pytestplugin.py` & `deltachat_rpc_client-1.139.3/src/deltachat_rpc_client/pytestplugin.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.2/src/deltachat_rpc_client/rpc.py` & `deltachat_rpc_client-1.139.3/src/deltachat_rpc_client/rpc.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.2/src/deltachat_rpc_client.egg-info/PKG-INFO` & `deltachat_rpc_client-1.139.3/src/deltachat_rpc_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltachat-rpc-client
-Version: 1.139.2
+Version: 1.139.3
 Summary: Python client for Delta Chat core JSON-RPC interface
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
```

### Comparing `deltachat_rpc_client-1.139.2/src/deltachat_rpc_client.egg-info/SOURCES.txt` & `deltachat_rpc_client-1.139.3/src/deltachat_rpc_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.2/tests/test_chatlist_events.py` & `deltachat_rpc_client-1.139.3/tests/test_chatlist_events.py`

 * *Files 10% similar despite different names*

```diff
@@ -122,30 +122,31 @@
     bob_addr = bob.get_config("addr")
     alice_contact_bob = alice.create_contact(bob_addr, "Bob")
     alice_chat_bob = alice_contact_bob.create_chat()
     alice_chat_bob.send_text("hi")
 
     alice.set_config("download_limit", "1")
 
-    event = bob.wait_for_incoming_msg_event()
-    msg = bob.get_message_by_id(event.msg_id)
+    msg = bob.wait_for_incoming_msg()
     chat_id = msg.get_snapshot().chat_id
     msg.get_snapshot().chat.accept()
     bob.get_chat_by_id(chat_id).send_message(
         "Hello World, this message is bigger than 5 bytes",
         html=base64.b64encode(os.urandom(300000)).decode("utf-8"),
     )
 
-    msg_id = alice.wait_for_incoming_msg_event().msg_id
-
-    assert alice.get_message_by_id(msg_id).get_snapshot().download_state == const.DownloadState.AVAILABLE
+    message = alice.wait_for_incoming_msg()
+    snapshot = message.get_snapshot()
+    assert snapshot.download_state == const.DownloadState.AVAILABLE
 
     alice.clear_all_events()
-    chat_id = alice.get_message_by_id(msg_id).get_snapshot().chat_id
-    alice._rpc.download_full_message(alice.id, msg_id)
+
+    snapshot = message.get_snapshot()
+    chat_id = snapshot.chat_id
+    alice._rpc.download_full_message(alice.id, message.id)
 
     wait_for_chatlist_specific_item(alice, chat_id)
 
 
 def get_multi_account_test_setup(acfactory: ACFactory) -> [Account, Account, Account]:
     alice, bob = acfactory.get_online_accounts(2)
 
@@ -173,28 +174,26 @@
     Test that chatlist changed events are emitted for the second device
     when the message is marked as read on the first device
     """
     alice, alice_second_device, bob, alice_chat_bob = get_multi_account_test_setup(acfactory)
 
     alice_chat_bob.send_text("hello")
 
-    event = bob.wait_for_incoming_msg_event()
-    msg = bob.get_message_by_id(event.msg_id)
+    msg = bob.wait_for_incoming_msg()
     bob_chat_id = msg.get_snapshot().chat_id
     msg.get_snapshot().chat.accept()
 
     alice.clear_all_events()
     alice_second_device.clear_all_events()
     bob.get_chat_by_id(bob_chat_id).send_text("hello")
 
     # make sure alice_second_device already received the message
     alice_second_device.wait_for_incoming_msg_event()
 
-    event = alice.wait_for_incoming_msg_event()
-    msg = alice.get_message_by_id(event.msg_id)
+    msg = alice.wait_for_incoming_msg()
     alice_second_device.clear_all_events()
     msg.mark_seen()
 
     wait_for_chatlist_specific_item(bob, bob_chat_id)
     wait_for_chatlist_specific_item(alice, alice_chat_bob.id)
```

### Comparing `deltachat_rpc_client-1.139.2/tests/test_securejoin.py` & `deltachat_rpc_client-1.139.3/tests/test_securejoin.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.2/tests/test_something.py` & `deltachat_rpc_client-1.139.3/tests/test_something.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.2/tests/test_vcard.py` & `deltachat_rpc_client-1.139.3/tests/test_vcard.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.139.2/tests/test_webxdc.py` & `deltachat_rpc_client-1.139.3/tests/test_webxdc.py`

 * *Files identical despite different names*

