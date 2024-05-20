# Comparing `tmp/py-netty-1.0.0.tar.gz` & `tmp/py-netty-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-netty-1.0.0.tar", last modified: Fri Apr  5 02:09:41 2024, max compression
+gzip compressed data, was "py-netty-1.0.1.tar", last modified: Mon May 20 06:11:18 2024, max compression
```

## Comparing `py-netty-1.0.0.tar` & `py-netty-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 haoru      (501) staff       (20)        0 2024-04-05 02:09:41.393479 py-netty-1.0.0/
--rw-r--r--   0 haoru      (501) staff       (20)     1065 2023-09-15 14:42:10.000000 py-netty-1.0.0/LICENSE
--rw-r--r--   0 haoru      (501) staff       (20)     8762 2024-04-05 02:09:41.392754 py-netty-1.0.0/PKG-INFO
--rw-r--r--   0 haoru      (501) staff       (20)     7757 2024-02-07 07:00:46.000000 py-netty-1.0.0/README.md
-drwxr-xr-x   0 haoru      (501) staff       (20)        0 2024-04-05 02:09:41.388625 py-netty-1.0.0/py_netty/
--rw-r--r--   0 haoru      (501) staff       (20)      218 2024-02-02 09:16:04.000000 py-netty-1.0.0/py_netty/__init__.py
--rw-r--r--   0 haoru      (501) staff       (20)     3758 2024-03-25 01:49:53.000000 py-netty-1.0.0/py_netty/bootstrap.py
--rw-r--r--   0 haoru      (501) staff       (20)      487 2024-02-18 05:21:21.000000 py-netty-1.0.0/py_netty/bytebuf.py
--rw-r--r--   0 haoru      (501) staff       (20)    16684 2024-03-24 15:54:43.000000 py-netty-1.0.0/py_netty/channel.py
--rw-r--r--   0 haoru      (501) staff       (20)     3861 2023-09-16 01:26:45.000000 py-netty-1.0.0/py_netty/eventfd.py
--rw-r--r--   0 haoru      (501) staff       (20)    15905 2024-03-25 01:53:25.000000 py-netty-1.0.0/py_netty/eventloop.py
--rw-r--r--   0 haoru      (501) staff       (20)     3138 2023-09-22 05:47:29.000000 py-netty-1.0.0/py_netty/handler.py
--rw-r--r--   0 haoru      (501) staff       (20)     1922 2024-02-07 06:26:51.000000 py-netty-1.0.0/py_netty/utils.py
-drwxr-xr-x   0 haoru      (501) staff       (20)        0 2024-04-05 02:09:41.392117 py-netty-1.0.0/py_netty.egg-info/
--rw-r--r--   0 haoru      (501) staff       (20)     8762 2024-04-05 02:09:41.000000 py-netty-1.0.0/py_netty.egg-info/PKG-INFO
--rw-r--r--   0 haoru      (501) staff       (20)      358 2024-04-05 02:09:41.000000 py-netty-1.0.0/py_netty.egg-info/SOURCES.txt
--rw-r--r--   0 haoru      (501) staff       (20)        1 2024-04-05 02:09:41.000000 py-netty-1.0.0/py_netty.egg-info/dependency_links.txt
--rw-r--r--   0 haoru      (501) staff       (20)        6 2024-04-05 02:09:41.000000 py-netty-1.0.0/py_netty.egg-info/requires.txt
--rw-r--r--   0 haoru      (501) staff       (20)        9 2024-04-05 02:09:41.000000 py-netty-1.0.0/py_netty.egg-info/top_level.txt
--rw-r--r--   0 haoru      (501) staff       (20)      186 2024-04-05 02:09:41.394118 py-netty-1.0.0/setup.cfg
--rw-r--r--   0 haoru      (501) staff       (20)     1524 2024-04-05 02:08:40.000000 py-netty-1.0.0/setup.py
+drwxr-xr-x   0 haoru      (501) staff       (20)        0 2024-05-20 06:11:18.265058 py-netty-1.0.1/
+-rw-r--r--   0 haoru      (501) staff       (20)     1065 2023-09-15 14:42:10.000000 py-netty-1.0.1/LICENSE
+-rw-r--r--   0 haoru      (501) staff       (20)     8762 2024-05-20 06:11:18.264668 py-netty-1.0.1/PKG-INFO
+-rw-r--r--   0 haoru      (501) staff       (20)     7757 2024-02-07 07:00:46.000000 py-netty-1.0.1/README.md
+drwxr-xr-x   0 haoru      (501) staff       (20)        0 2024-05-20 06:11:18.259568 py-netty-1.0.1/py_netty/
+-rw-r--r--   0 haoru      (501) staff       (20)      218 2024-02-02 09:16:04.000000 py-netty-1.0.1/py_netty/__init__.py
+-rw-r--r--   0 haoru      (501) staff       (20)     4485 2024-05-20 05:40:17.000000 py-netty-1.0.1/py_netty/bootstrap.py
+-rw-r--r--   0 haoru      (501) staff       (20)      487 2024-02-18 05:21:21.000000 py-netty-1.0.1/py_netty/bytebuf.py
+-rw-r--r--   0 haoru      (501) staff       (20)    16684 2024-03-24 15:54:43.000000 py-netty-1.0.1/py_netty/channel.py
+-rw-r--r--   0 haoru      (501) staff       (20)     3861 2023-09-16 01:26:45.000000 py-netty-1.0.1/py_netty/eventfd.py
+-rw-r--r--   0 haoru      (501) staff       (20)    15905 2024-03-25 01:53:25.000000 py-netty-1.0.1/py_netty/eventloop.py
+-rw-r--r--   0 haoru      (501) staff       (20)     3138 2023-09-22 05:47:29.000000 py-netty-1.0.1/py_netty/handler.py
+-rw-r--r--   0 haoru      (501) staff       (20)     1922 2024-02-07 06:26:51.000000 py-netty-1.0.1/py_netty/utils.py
+drwxr-xr-x   0 haoru      (501) staff       (20)        0 2024-05-20 06:11:18.263658 py-netty-1.0.1/py_netty.egg-info/
+-rw-r--r--   0 haoru      (501) staff       (20)     8762 2024-05-20 06:11:18.000000 py-netty-1.0.1/py_netty.egg-info/PKG-INFO
+-rw-r--r--   0 haoru      (501) staff       (20)      358 2024-05-20 06:11:18.000000 py-netty-1.0.1/py_netty.egg-info/SOURCES.txt
+-rw-r--r--   0 haoru      (501) staff       (20)        1 2024-05-20 06:11:18.000000 py-netty-1.0.1/py_netty.egg-info/dependency_links.txt
+-rw-r--r--   0 haoru      (501) staff       (20)        6 2024-05-20 06:11:18.000000 py-netty-1.0.1/py_netty.egg-info/requires.txt
+-rw-r--r--   0 haoru      (501) staff       (20)        9 2024-05-20 06:11:18.000000 py-netty-1.0.1/py_netty.egg-info/top_level.txt
+-rw-r--r--   0 haoru      (501) staff       (20)      186 2024-05-20 06:11:18.266190 py-netty-1.0.1/setup.cfg
+-rw-r--r--   0 haoru      (501) staff       (20)     1524 2024-05-20 06:09:31.000000 py-netty-1.0.1/setup.py
```

### Comparing `py-netty-1.0.0/LICENSE` & `py-netty-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py-netty-1.0.0/PKG-INFO` & `py-netty-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-netty
-Version: 1.0.0
+Version: 1.0.1
 Summary: TCP framework in flavor of Netty
 Home-page: https://github.com/ruanhao/py-netty
 Author: Hao Ruan
 Author-email: ruanhao1116@gmail.com
 License: MIT
 Keywords: network,tcp,non-blocking,epoll,nio,netty
 Classifier: Intended Audience :: Developers
```

### Comparing `py-netty-1.0.0/README.md` & `py-netty-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `py-netty-1.0.0/py_netty/bootstrap.py` & `py-netty-1.0.1/py_netty/bootstrap.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,27 +36,40 @@
 
 @define(slots=True)
 class Bootstrap:
     eventloop_group: EventLoopGroup = field(factory=EventLoopGroup)
     handler_initializer: typing.Callable = field(default=_handler_initializer)
     tls: bool = False
     verify: bool = True
+    ssl_context_cb: typing.Callable = None
+
+    def _create_ssl_context(self):
+        ctx = _client_ssl_context(self.verify)
+        if self.ssl_context_cb:
+            try:
+                self.ssl_context_cb(ctx)
+            except Exception as e:
+                logger.error("Error in ssl_context_cb(client): %s", e)
+        return ctx
+
+    def _wrap_ssl_socket(self, sock, server_hostname_or_address):
+        return self._create_ssl_context().wrap_socket(sock, server_hostname=server_hostname_or_address)
 
     def connect(self, address, port, ensure_connected: bool = False) -> ChannelFuture:
         sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         # if ensure_connected or self.tls:
         if ensure_connected:
             sock.connect((address, port))
             if self.tls:
-                sock = _client_ssl_context(self.verify).wrap_socket(sock, server_hostname=address)
+                sock = self._wrap_ssl_socket(sock, address)
             sock.setblocking(False)
         else:
             sock.setblocking(False)
             if self.tls:
-                sock = _client_ssl_context(self.verify).wrap_socket(sock, server_hostname=address)
+                sock = self._wrap_ssl_socket(sock, address)
             sock.connect_ex((address, port))  # non blocking
         return NioSocketChannel(
             self.eventloop_group.get_eventloop(),
             sock,
             handler_initializer=self.handler_initializer
         ).register()
 
@@ -64,21 +77,28 @@
 @define(slots=True)
 class ServerBootstrap:
     parant_group: EventLoopGroup = field(factory=EventLoopGroup)
     child_group: EventLoopGroup = field(factory=EventLoopGroup)
     child_handler_initializer: typing.Callable = field(default=_handler_initializer)
     certfile: str = None
     keyfile: str = None
+    ssl_context_cb: typing.Callable = None
 
     def bind(self, address='localhost', port=-1) -> ChannelFuture:
         assert port > 0
         assert ((self.certfile is not None) ^ (self.keyfile is not None)) is False, "Both certfile and keyfile must be specified"
         server_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         if self.certfile and self.keyfile:
-            server_socket = _server_ssl_context(self.certfile, self.keyfile).wrap_socket(server_socket, server_side=True)
+            ssl_ctx = _server_ssl_context(self.certfile, self.keyfile)
+            if self.ssl_context_cb:
+                try:
+                    self.ssl_context_cb(ssl_ctx)
+                except Exception as e:
+                    logger.error("Error in ssl_context_cb(server): %s", e)
+            server_socket = ssl_ctx.wrap_socket(server_socket, server_side=True)
         server_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         server_socket.bind((address, port))
         server_socket.listen(128)
         server_socket.setblocking(0)
         eventloop = self.parant_group.get_eventloop()
 
         class _ChannelInitializer(ChannelHandlerAdapter):
```

### Comparing `py-netty-1.0.0/py_netty/channel.py` & `py-netty-1.0.1/py_netty/channel.py`

 * *Files identical despite different names*

### Comparing `py-netty-1.0.0/py_netty/eventfd.py` & `py-netty-1.0.1/py_netty/eventfd.py`

 * *Files identical despite different names*

### Comparing `py-netty-1.0.0/py_netty/eventloop.py` & `py-netty-1.0.1/py_netty/eventloop.py`

 * *Files identical despite different names*

### Comparing `py-netty-1.0.0/py_netty/handler.py` & `py-netty-1.0.1/py_netty/handler.py`

 * *Files identical despite different names*

### Comparing `py-netty-1.0.0/py_netty/utils.py` & `py-netty-1.0.1/py_netty/utils.py`

 * *Files identical despite different names*

### Comparing `py-netty-1.0.0/py_netty.egg-info/PKG-INFO` & `py-netty-1.0.1/py_netty.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-netty
-Version: 1.0.0
+Version: 1.0.1
 Summary: TCP framework in flavor of Netty
 Home-page: https://github.com/ruanhao/py-netty
 Author: Hao Ruan
 Author-email: ruanhao1116@gmail.com
 License: MIT
 Keywords: network,tcp,non-blocking,epoll,nio,netty
 Classifier: Intended Audience :: Developers
```

### Comparing `py-netty-1.0.0/setup.py` & `py-netty-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 # install_requires = (this_directory / 'requirements.txt').read_text().splitlines()
 
-version = '1.0.0'
+version = '1.0.1'
 
 config = {
     'name': 'py-netty',
     'url': 'https://github.com/ruanhao/py-netty',
     'license': 'MIT',
     "long_description": long_description,
     "long_description_content_type": 'text/markdown',
```

