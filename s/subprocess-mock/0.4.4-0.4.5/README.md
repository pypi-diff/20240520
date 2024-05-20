# Comparing `tmp/subprocess-mock-0.4.4.tar.gz` & `tmp/subprocess_mock-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subprocess-mock-0.4.4.tar", last modified: Mon Feb 19 07:52:06 2024, max compression
+gzip compressed data, was "subprocess_mock-0.4.5.tar", last modified: Mon May 20 10:41:53 2024, max compression
```

## Comparing `subprocess-mock-0.4.4.tar` & `subprocess_mock-0.4.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 07:52:06.031970 subprocess-mock-0.4.4/
--rw-rw-rw-   0 root         (0) root         (0)     1075 2024-02-19 07:51:53.000000 subprocess-mock-0.4.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4114 2024-02-19 07:52:06.031970 subprocess-mock-0.4.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1444 2024-02-19 07:51:53.000000 subprocess-mock-0.4.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1586 2024-02-19 07:51:53.000000 subprocess-mock-0.4.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-19 07:52:06.031970 subprocess-mock-0.4.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 07:52:06.024970 subprocess-mock-0.4.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 07:52:06.028970 subprocess-mock-0.4.4/src/subprocess_mock/
--rw-rw-rw-   0 root         (0) root         (0)      901 2024-02-19 07:51:53.000000 subprocess-mock-0.4.4/src/subprocess_mock/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2024-02-19 07:51:53.000000 subprocess-mock-0.4.4/src/subprocess_mock/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)    13618 2024-02-19 07:51:53.000000 subprocess-mock-0.4.4/src/subprocess_mock/child.py
--rw-rw-rw-   0 root         (0) root         (0)     3560 2024-02-19 07:51:53.000000 subprocess-mock-0.4.4/src/subprocess_mock/commandline.py
--rw-rw-rw-   0 root         (0) root         (0)      940 2024-02-19 07:51:53.000000 subprocess-mock-0.4.4/src/subprocess_mock/commons.py
--rw-rw-rw-   0 root         (0) root         (0)     3000 2024-02-19 07:51:53.000000 subprocess-mock-0.4.4/src/subprocess_mock/functions.py
--rw-rw-rw-   0 root         (0) root         (0)    36338 2024-02-19 07:51:53.000000 subprocess-mock-0.4.4/src/subprocess_mock/parent.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-19 07:51:53.000000 subprocess-mock-0.4.4/src/subprocess_mock/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    18196 2024-02-19 07:51:53.000000 subprocess-mock-0.4.4/src/subprocess_mock/streams.py
--rw-rw-rw-   0 root         (0) root         (0)    12729 2024-02-19 07:51:53.000000 subprocess-mock-0.4.4/src/subprocess_mock/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 07:52:06.030970 subprocess-mock-0.4.4/src/subprocess_mock.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4114 2024-02-19 07:52:06.000000 subprocess-mock-0.4.4/src/subprocess_mock.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      632 2024-02-19 07:52:06.000000 subprocess-mock-0.4.4/src/subprocess_mock.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-19 07:52:06.000000 subprocess-mock-0.4.4/src/subprocess_mock.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-02-19 07:52:06.000000 subprocess-mock-0.4.4/src/subprocess_mock.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 07:52:06.030970 subprocess-mock-0.4.4/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1880 2024-02-19 07:51:53.000000 subprocess-mock-0.4.4/tests/test_commandline.py
--rw-rw-rw-   0 root         (0) root         (0)     1732 2024-02-19 07:51:53.000000 subprocess-mock-0.4.4/tests/test_functions.py
--rw-rw-rw-   0 root         (0) root         (0)     1805 2024-02-19 07:51:53.000000 subprocess-mock-0.4.4/tests/test_main.py
--rw-rw-rw-   0 root         (0) root         (0)    15942 2024-02-19 07:51:53.000000 subprocess-mock-0.4.4/tests/test_streams.py
--rw-rw-rw-   0 root         (0) root         (0)     9007 2024-02-19 07:51:53.000000 subprocess-mock-0.4.4/tests/test_workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 10:41:53.634490 subprocess_mock-0.4.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2024-05-20 10:41:44.000000 subprocess_mock-0.4.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4114 2024-05-20 10:41:53.634490 subprocess_mock-0.4.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1444 2024-05-20 10:41:44.000000 subprocess_mock-0.4.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2024-05-20 10:41:44.000000 subprocess_mock-0.4.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 10:41:53.634490 subprocess_mock-0.4.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 10:41:53.627490 subprocess_mock-0.4.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 10:41:53.631490 subprocess_mock-0.4.5/src/subprocess_mock/
+-rw-rw-rw-   0 root         (0) root         (0)      900 2024-05-20 10:41:44.000000 subprocess_mock-0.4.5/src/subprocess_mock/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      984 2024-05-20 10:41:44.000000 subprocess_mock-0.4.5/src/subprocess_mock/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13464 2024-05-20 10:41:44.000000 subprocess_mock-0.4.5/src/subprocess_mock/child.py
+-rw-rw-rw-   0 root         (0) root         (0)     3511 2024-05-20 10:41:44.000000 subprocess_mock-0.4.5/src/subprocess_mock/commandline.py
+-rw-rw-rw-   0 root         (0) root         (0)      939 2024-05-20 10:41:44.000000 subprocess_mock-0.4.5/src/subprocess_mock/commons.py
+-rw-rw-rw-   0 root         (0) root         (0)     2986 2024-05-20 10:41:44.000000 subprocess_mock-0.4.5/src/subprocess_mock/functions.py
+-rw-rw-rw-   0 root         (0) root         (0)    35890 2024-05-20 10:41:44.000000 subprocess_mock-0.4.5/src/subprocess_mock/parent.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 10:41:44.000000 subprocess_mock-0.4.5/src/subprocess_mock/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    17951 2024-05-20 10:41:44.000000 subprocess_mock-0.4.5/src/subprocess_mock/streams.py
+-rw-rw-rw-   0 root         (0) root         (0)    12534 2024-05-20 10:41:44.000000 subprocess_mock-0.4.5/src/subprocess_mock/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 10:41:53.634490 subprocess_mock-0.4.5/src/subprocess_mock.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4114 2024-05-20 10:41:53.000000 subprocess_mock-0.4.5/src/subprocess_mock.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      632 2024-05-20 10:41:53.000000 subprocess_mock-0.4.5/src/subprocess_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 10:41:53.000000 subprocess_mock-0.4.5/src/subprocess_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-20 10:41:53.000000 subprocess_mock-0.4.5/src/subprocess_mock.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 10:41:53.633490 subprocess_mock-0.4.5/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1879 2024-05-20 10:41:44.000000 subprocess_mock-0.4.5/tests/test_commandline.py
+-rw-rw-rw-   0 root         (0) root         (0)     1732 2024-05-20 10:41:44.000000 subprocess_mock-0.4.5/tests/test_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1804 2024-05-20 10:41:44.000000 subprocess_mock-0.4.5/tests/test_main.py
+-rw-rw-rw-   0 root         (0) root         (0)    15666 2024-05-20 10:41:44.000000 subprocess_mock-0.4.5/tests/test_streams.py
+-rw-rw-rw-   0 root         (0) root         (0)     8909 2024-05-20 10:41:44.000000 subprocess_mock-0.4.5/tests/test_workflow.py
```

### Comparing `subprocess-mock-0.4.4/LICENSE` & `subprocess_mock-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `subprocess-mock-0.4.4/PKG-INFO` & `subprocess_mock-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subprocess-mock
-Version: 0.4.4
+Version: 0.4.5
 Summary: Subprocess Mock
 Author-email: Rainer Schwarzbach <rainer@blackstream.de>
 License: MIT License
         
         Copyright (c) 2024 Rainer Schwarzbach
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `subprocess-mock-0.4.4/README.md` & `subprocess_mock-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `subprocess-mock-0.4.4/pyproject.toml` & `subprocess_mock-0.4.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `subprocess-mock-0.4.4/src/subprocess_mock/__init__.py` & `subprocess_mock-0.4.5/src/subprocess_mock/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 subprocess-mock is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the LICENSE file for more details.
 
 """
 
-
 from .workflow import Orchestrator  # noqa: F401
 from .child import (  # noqa: F401
     Filter,
     SetReturncode,
     Sleep,
     WriteOutput,
     WriteError,
@@ -38,11 +37,11 @@
     getstatusoutput,
     getoutput,
     check_output,
     run,
 )
 
 
-__version__ = "0.4.4"
+__version__ = "0.4.5"
 
 
 # vim: fileencoding=utf-8 ts=4 sts=4 sw=4 autoindent expandtab syntax=python:
```

### Comparing `subprocess-mock-0.4.4/src/subprocess_mock/__main__.py` & `subprocess_mock-0.4.5/src/subprocess_mock/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 subprocess-mock is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the LICENSE file for more details.
 
 """
 
-
 import sys
 
 from subprocess_mock import commandline
 
 
 #
 # Functions
```

### Comparing `subprocess-mock-0.4.4/src/subprocess_mock/child.py` & `subprocess_mock-0.4.5/src/subprocess_mock/child.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 subprocess-mock is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the LICENSE file for more details.
 
 """
 
-
 import io
 import logging
 import sys
 import time
 
 from typing import Any, Callable, Iterator, Optional, Tuple, Type, Union
 
@@ -44,17 +43,15 @@
         if selector.readable:
             wrapper: Type[streams.ConnectionWrapper] = streams.ConnectionReader
             logging.debug("[child] … using read wrapper %r", wrapper)
         elif selector.writable:
             wrapper = streams.ConnectionWriter
             logging.debug("[child] … using write wrapper %r", wrapper)
         else:
-            raise ValueError(
-                f"object ({selector!r}) must be read- or writable"
-            )
+            raise ValueError(f"object ({selector!r}) must be read- or writable")
         #
         return wrapper(selector), None
     #
     if isinstance(selector, io.BufferedIOBase):
         logging.debug("[child] … using bytes stream %r", selector)
         return selector, None
     #
@@ -65,23 +62,19 @@
             selector.encoding,
         )
         return selector, selector.encoding
     #
     if isinstance(selector, int) and selector > 0:
         # pylint: disable=consider-using-with, unspecified-encoding
         stream = io.open(selector, mode=mode)
-        logging.debug(
-            "[child] … using file descriptor %s as %r", selector, stream
-        )
+        logging.debug("[child] … using file descriptor %s as %r", selector, stream)
         return stream, None
     #
     if selector != commons.NO_PIPE:
-        raise TypeError(
-            f"Unsupported object ({selector!r} of type {type(selector)})"
-        )
+        raise TypeError(f"Unsupported object ({selector!r} of type {type(selector)})")
     #
     try:
         stream = standard_stream.buffer
     except AttributeError:
         # assume a text stream
         logging.debug(
             "[child] … using standard stream (text) %r with encoding %r",
@@ -308,17 +301,15 @@
         self.__program: Program = Program(*steps)
         logging.debug("[child] initialized with program: %r", self.__program)
         self.__redirected = {
             commons.KW_STDIN: stdin != commons.NO_PIPE,
             commons.KW_STDERR: stderr != commons.NO_PIPE,
             commons.KW_STDOUT: stdout != commons.NO_PIPE,
         }
-        self.__stdin = get_stream_and_encoding(
-            stdin, sys.stdin, "stdin", mode="rb"
-        )[0]
+        self.__stdin = get_stream_and_encoding(stdin, sys.stdin, "stdin", mode="rb")[0]
         self.__stderr, self.__stderr_encoding = get_stream_and_encoding(
             stderr, sys.stderr, "stderr"
         )
         self.__stdout, self.__stdout_encoding = get_stream_and_encoding(
             stdout, sys.stdout, "stdout"
         )
         self.__returncode = commons.RETURNCODE_OK
@@ -334,24 +325,20 @@
         """Set returncode, proxy method for steps"""
         logging.debug("[child] setting returncode: %r", returncode)
         self.__returncode = returncode
 
     def write_stderr(self, message: Union[bytes, str]):
         """Write message to stderr, proxy method for steps"""
         logging.debug("[child] writing to stderr: %r", message)
-        write_to_stream(
-            self.__stderr, message, encoding=self.__stderr_encoding
-        )
+        write_to_stream(self.__stderr, message, encoding=self.__stderr_encoding)
 
     def write_stdout(self, message: Union[bytes, str]):
         """Write message to stdout, proxy method for steps"""
         logging.debug("[child] writing to stdout: %r", message)
-        write_to_stream(
-            self.__stdout, message, encoding=self.__stdout_encoding
-        )
+        write_to_stream(self.__stdout, message, encoding=self.__stdout_encoding)
 
     def run(self) -> int:
         """Read once and blocking from stdin if any step requires it.
         Otherwise, try a non-blocking read.
         Run the steps one after another.
         Return the returncode.
         """
```

### Comparing `subprocess-mock-0.4.4/src/subprocess_mock/commandline.py` & `subprocess_mock-0.4.5/src/subprocess_mock/commandline.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 subprocess-mock is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the LICENSE file for more details.
 
 """
 
-
 import argparse
 import logging
 
 from subprocess_mock import __version__
 
 
 #
@@ -42,28 +41,24 @@
 #
 
 
 class Program:
     """Command line program"""
 
     name: str = "subprocess_mock"
-    description: str = (
-        "Mock objects for the standard library’s subprocess module"
-    )
+    description: str = "Mock objects for the standard library’s subprocess module"
 
     def __init__(self, *args: str) -> None:
         """Parse command line arguments and initialize the logger
 
         :param args: a list of command line arguments
         """
         self.__arguments = self._parse_args(*args)
         if self.arguments.loglevel < logging.DEBUG:
-            message_format = (
-                "%(levelname)-8s | (%(funcName)s:%(lineno)s) %(message)s"
-            )
+            message_format = "%(levelname)-8s | (%(funcName)s:%(lineno)s) %(message)s"
         else:
             message_format = "%(levelname)-8s | %(message)s"
         #
         logging.basicConfig(
             format=message_format,
             level=self.arguments.loglevel,
         )
```

### Comparing `subprocess-mock-0.4.4/src/subprocess_mock/commons.py` & `subprocess_mock-0.4.5/src/subprocess_mock/commons.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 subprocess-mock is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the LICENSE file for more details.
 
 """
 
-
 import subprocess
 
 
 # Magic numbers
 PIPE = subprocess.PIPE
 STDOUT = subprocess.STDOUT
 DEVNULL = subprocess.DEVNULL
```

### Comparing `subprocess-mock-0.4.4/src/subprocess_mock/functions.py` & `subprocess_mock-0.4.5/src/subprocess_mock/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,17 +60,15 @@
 
 def check_output(*popenargs, timeout=None, **kwargs):
     r"""Run command with arguments and return its output.
 
     See the check_output() method of the StoringRunner class below
     for details.
     """
-    return workflow.Orchestrator().check_output(
-        *popenargs, timeout=timeout, **kwargs
-    )
+    return workflow.Orchestrator().check_output(*popenargs, timeout=timeout, **kwargs)
 
 
 # pylint: disable=redefined-builtin
 def run(
     *popenargs,
     input=None,
     timeout=None,
```

### Comparing `subprocess-mock-0.4.4/src/subprocess_mock/parent.py` & `subprocess_mock-0.4.5/src/subprocess_mock/parent.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,17 +199,15 @@
             bufsize = -1  # Restore default
         #
         if not isinstance(bufsize, int):
             raise TypeError("bufsize must be an integer")
         #
         if _MSWINDOWS:
             if preexec_fn is not None:
-                raise ValueError(
-                    "preexec_fn is not supported on Windows platforms"
-                )
+                raise ValueError("preexec_fn is not supported on Windows platforms")
             #
             any_stdio_set = (
                 stdin is not None or stdout is not None or stderr is not None
             )
             if close_fds is _PLATFORM_DEFAULT_CLOSE_FDS:
                 if any_stdio_set:
                     close_fds = False
@@ -228,22 +226,18 @@
                 close_fds = True
             #
             if pass_fds and not close_fds:
                 warnings.warn("pass_fds overriding close_fds.", RuntimeWarning)
                 close_fds = True
             #
             if startupinfo is not None:
-                raise ValueError(
-                    "startupinfo is only supported on Windows platforms"
-                )
+                raise ValueError("startupinfo is only supported on Windows platforms")
             #
             if creationflags != 0:
-                raise ValueError(
-                    "creationflags is only supported on Windows platforms"
-                )
+                raise ValueError("creationflags is only supported on Windows platforms")
             #
         #
         self.args = args
         self.stdin: Union[IO, streams.ConnectionWrapper, None] = None
         self.stdout: Union[IO, streams.ConnectionWrapper, None] = None
         self.stderr: Union[IO, streams.ConnectionWrapper, None] = None
         self.pid: Optional[int] = None
@@ -298,17 +292,15 @@
                         self.stdin = streams.TextConnectionWriter(
                             p2cwrite,
                             bufsize,
                             encoding=encoding__,
                             errors=errors__,
                         )
                     else:
-                        self.stdin = streams.ConnectionWriter(
-                            p2cwrite, bufsize
-                        )
+                        self.stdin = streams.ConnectionWriter(p2cwrite, bufsize)
                     #
                 else:
                     self.stdin = io.open(p2cwrite, "wb", bufsize)
                 #
             #
             if c2pread != commons.NO_PIPE:
                 if isinstance(c2pread, streams.Connection):
@@ -316,17 +308,15 @@
                         self.stdout = streams.TextConnectionReader(
                             c2pread,
                             bufsize,
                             encoding=encoding__,
                             errors=errors__,
                         )
                     else:
-                        self.stdout = streams.ConnectionReader(
-                            c2pread, bufsize
-                        )
+                        self.stdout = streams.ConnectionReader(c2pread, bufsize)
                     #
                 else:
                     self.stdout = io.open(c2pread, "rb", bufsize)
                 #
             #
             if errread != commons.NO_PIPE:
                 if isinstance(errread, streams.Connection):
@@ -335,17 +325,15 @@
                         self.stderr = streams.TextConnectionReader(
                             errread,
                             bufsize,
                             encoding=encoding__,
                             errors=errors__,
                         )
                     else:
-                        self.stderr = streams.ConnectionReader(
-                            errread, bufsize
-                        )
+                        self.stderr = streams.ConnectionReader(errread, bufsize)
                     #
                 else:
                     self.stderr = io.open(errread, "rb", bufsize)
                 #
             #
             # pylint: enable=consider-using-with
             self._execute_child(
@@ -424,17 +412,15 @@
                 self.stdin.close()
             #
         finally:
             # Wait for the process to terminate, to avoid zombies.
             self.wait()
         #
 
-    def __del__(
-        self, _maxsize: int = sys.maxsize, _warn=warnings.warn
-    ) -> None:
+    def __del__(self, _maxsize: int = sys.maxsize, _warn=warnings.warn) -> None:
         """Delete the instance"""
         if not self._child_created:
             # We didn't get to successfully create a child process.
             return
         #
         if self.returncode is None:
             # Not reading subprocess exit status creates a zombi process which
@@ -697,18 +683,16 @@
             # Prevent a double close of these fds from __init__ on error.
             self._closed_child_pipe_fds = True
 
             # Wait for exec to fail or succeed; possibly raising an
             # exception (limited in size)
             errpipe_data = bytearray()
             while not errpipe_read.poll():
-                logging.debug(
-                    "[parent] … waiting for process %s startup", self.pid
-                )
-                time.sleep(0.5)
+                logging.debug("[parent] … waiting for process %s startup", self.pid)
+                time.sleep(0.05)
             #
             try:
                 errpipe_data.extend(errpipe_read.recv_bytes())
             except EOFError:
                 pass
             #
         finally:
@@ -735,17 +719,15 @@
                 exception_name, err_msg_bin = bytes(errpipe_data).split(b":")
                 # The encoding here should match the encoding
                 # written in by the subprocess implementations
                 # like _posixsubprocess
                 err_msg = err_msg_bin.decode()
             except ValueError:
                 exception_name = b"SubprocessError"
-                err_msg = (
-                    f"Bad exception data from child: {bytes(errpipe_data)!r}"
-                )
+                err_msg = f"Bad exception data from child: {bytes(errpipe_data)!r}"
             #
             child_exception_type = getattr(
                 builtins,
                 exception_name.decode("ascii"),
                 SubprocessError,
             )
             raise child_exception_type(err_msg)
@@ -785,17 +767,15 @@
             returncode = -rc_part
         else:
             # Should never happen
             raise SubprocessError("Unknown child exit status!")
         #
         return returncode
 
-    def _internal_poll_mock(
-        self, _deadstate: Optional[int] = None
-    ) -> Optional[int]:
+    def _internal_poll_mock(self, _deadstate: Optional[int] = None) -> Optional[int]:
         """Check if child process has terminated.
         Sets and returns returncode attribute.
         """
         if self.mocked_child_process.exitcode is None:
             return None
         #
         if self._orchestrator_callback is not None:
@@ -847,17 +827,15 @@
                 #
             finally:
                 self._waitpid_lock.release()
             #
         #
         return self.returncode
 
-    def wait(
-        self, timeout=None, endtime: Optional[float] = None
-    ) -> Optional[int]:
+    def wait(self, timeout=None, endtime: Optional[float] = None) -> Optional[int]:
         """Wait for child process to terminate.  Returns returncode
         attribute."""
         if self.returncode is not None:
             return self.returncode
 
         if endtime is not None:
             warnings.warn(
@@ -959,32 +937,30 @@
             except BrokenPipeError:
                 pass
             finally:
                 self.stdin.close()
             #
         #
         while True:
-            time.sleep(0.1)
+            time.sleep(0.05)
             for fileobj in (self.stdout, self.stderr):
                 if not fileobj:
                     continue
                 #
                 if self._pipe_broken.get(fileobj, True):
                     continue
                 #
                 try:
                     data = fileobj.read()
                 except BrokenPipeError:
                     logging.warning("[parent] Pipe broken: %r", fileobj)
                     self._pipe_broken[fileobj] = True
                 else:
                     if data:
-                        logging.debug(
-                            "[parent] Got data from %r: %r", fileobj, data
-                        )
+                        logging.debug("[parent] Got data from %r: %r", fileobj, data)
                         self._fileobj2output[fileobj].append(data)
                     #
                 #
             #
             if all(probe for probe in self._pipe_broken.values()):
                 break
             #
```

### Comparing `subprocess-mock-0.4.4/src/subprocess_mock/streams.py` & `subprocess_mock-0.4.5/src/subprocess_mock/streams.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 subprocess-mock is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the LICENSE file for more details.
 
 """
 
-
 import io
 import sys
 
 from multiprocessing import Lock
 from typing import List, Optional, Union
 
 # pylint: disable=ungrouped-imports
@@ -145,17 +144,15 @@
         """Write data to the stream."""
         self._check_writable()
         return 0
 
     def flush(self) -> None:
         """Flush the stream."""
         if not self.writable:
-            raise ValueError(
-                "This stream is not writable and cannot be flushed."
-            )
+            raise ValueError("This stream is not writable and cannot be flushed.")
         #
 
 
 class ConnectionReader(ConnectionWrapper):
     """ConnectionReader(connection[, buffer_size])
 
     A wrapper for read access to a multiprocessing.connection.Connection
@@ -250,17 +247,15 @@
         if n < 1:
             raise ValueError("n must be at least 1")
         #
         self._read_buf.extend(self.raw[:n])
         del self.raw[:n]
         return n
 
-    def _read_unlocked(
-        self, n: Optional[int] = None, blocking: bool = False
-    ) -> bytes:
+    def _read_unlocked(self, n: Optional[int] = None, blocking: bool = False) -> bytes:
         """Read data from the internal buffer"""
         nodata_val = b""
         if blocking:
             self._update_raw_unlocked()
         else:
             self._update_raw_unlocked_noblock()
         #
@@ -336,17 +331,15 @@
         self._check_readable()
         if size < 0:
             raise ValueError("number of bytes to read must be positive")
         if size == 0:
             return b""
         with self._read_lock:
             self._peek_unlocked(1)
-            return self._read_unlocked(
-                min(size, len(self._read_buf) - self._read_pos)
-            )
+            return self._read_unlocked(min(size, len(self._read_buf) - self._read_pos))
         #
 
     def tell(self):
         """Tell the current position in the stream"""
         return self._total_read_bytes
 
 
@@ -489,17 +482,15 @@
         without advancing the position.
 
         The argument indicates a desired minimal number of bytes.
         We never return more than self.buffer_size.
         """
         self._check_readable()
         with self._read_lock:
-            return self._peek_unlocked(size).decode(
-                self._encoding, self._errors
-            )
+            return self._peek_unlocked(size).decode(self._encoding, self._errors)
         #
 
 
 class TextConnectionWriter(ConnectionWriter):
     """TextConnectionWriter(connection[, buffer_size])
 
     A wrapper for text mode write access
@@ -539,45 +530,39 @@
             if self.line_buffered:
                 splitted = data.splitlines(keepends=True)
                 if self._text_buffer:
                     last_buffered_line = self._text_buffer.pop()
                     if last_buffered_line.endswith("\n"):
                         first_new_line = last_buffered_line
                     else:
-                        first_new_line = (
-                            f"{last_buffered_line}{splitted.pop(0)}"
-                        )
+                        first_new_line = f"{last_buffered_line}{splitted.pop(0)}"
                     #
                     splitted.insert(0, first_new_line)
                     splitted = self._text_buffer + splitted
                     self._text_buffer.clear()
                 #
                 if not splitted[-1].endswith("\n"):
                     self._text_buffer.append(splitted.pop())
                 #
-                binary_data = "".join(splitted).encode(
-                    self._encoding, self._errors
-                )
+                binary_data = "".join(splitted).encode(self._encoding, self._errors)
             else:
                 binary_data = data.encode(self._encoding, self._errors)
             #
         #
         with self._write_lock:
             written_bytes = self._write_unlocked(binary_data)
         #
         return written_bytes
 
     def flush(self) -> None:
         """Flush the internal buffer"""
         with self._tb_lock:
             with self._write_lock:
                 self.raw.extend(
-                    "".join(self._text_buffer).encode(
-                        self._encoding, self._errors
-                    )
+                    "".join(self._text_buffer).encode(self._encoding, self._errors)
                 )
             #
             self._text_buffer.clear()
         #
         super().flush()
```

### Comparing `subprocess-mock-0.4.4/src/subprocess_mock/workflow.py` & `subprocess_mock-0.4.5/src/subprocess_mock/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 subprocess-mock is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the LICENSE file for more details.
 
 """
 
-
 import heapq
 import logging
 import shlex
 import subprocess
 
 from typing import Any, Dict, List, Tuple, Union
 
@@ -56,17 +55,15 @@
             Tuple[child.Program, subprocess.CompletedProcess, Dict[str, Any]]
         ] = []
         self.__all_programs: List[Tuple[Tuple[str, ...], child.Program]] = []
 
     @property
     def all_results(
         self,
-    ) -> List[
-        Tuple[child.Program, subprocess.CompletedProcess, Dict[str, Any]]
-    ]:
+    ) -> List[Tuple[child.Program, subprocess.CompletedProcess, Dict[str, Any]]]:
         """Property: the collected results list"""
         return list(self.__all_results)
 
     def add_program(
         self,
         *args: str,
         program: child.Program = EMPTY_PROGRAM,
@@ -153,20 +150,16 @@
 
         The arguments are the same as for the
         subprocess_mock.parent.Popen constructor.
         Example:
 
         retcode = call(["ls", "-l"])
         """
-        program: child.Program = self.get_matching_program(
-            *popenargs, **kwargs
-        )
-        with parent.Popen(
-            *popenargs, child_steps=program.steps, **kwargs
-        ) as popen_obj:
+        program: child.Program = self.get_matching_program(*popenargs, **kwargs)
+        with parent.Popen(*popenargs, child_steps=program.steps, **kwargs) as popen_obj:
             try:
                 retcode = popen_obj.wait(timeout=timeout) or 0
             except Exception as exc:
                 popen_obj.kill()
                 popen_obj.wait()
                 raise exc
             #
@@ -192,17 +185,15 @@
             if cmd is None:
                 cmd = popenargs[0]
             #
             raise subprocess.CalledProcessError(retcode, cmd)
         #
         return 0
 
-    def check_output(
-        self, *popenargs, timeout=None, **kwargs
-    ) -> Union[bytes, str]:
+    def check_output(self, *popenargs, timeout=None, **kwargs) -> Union[bytes, str]:
         """Run command with arguments and return its output.
 
         If the exit code was non-zero it raises a CalledProcessError.  The
         CalledProcessError object will have the return code in the returncode
         attribute and output in the output attribute.
 
         The arguments are the same as for the Popen constructor.
@@ -229,25 +220,21 @@
         ...              input=b"when in the course of fooman events\n")
         b'when in the course of barman events\n'
 
         If universal_newlines=True is passed, the "input" argument must be a
         string and the return value will be a string rather than bytes.
         """
         if commons.KW_STDOUT in kwargs:
-            raise ValueError(
-                "stdout argument not allowed, it will be overridden."
-            )
+            raise ValueError("stdout argument not allowed, it will be overridden.")
         #
         if "input" in kwargs and kwargs["input"] is None:
             # Explicitly passing input=None was previously equivalent
             # to passing an empty string.
             # That is maintained here for backwards compatibility.
-            kwargs["input"] = (
-                "" if kwargs.get("universal_newlines", False) else b""
-            )
+            kwargs["input"] = "" if kwargs.get("universal_newlines", False) else b""
         #
         return self.run(
             *popenargs,
             stdout=commons.PIPE,
             timeout=timeout,
             check=True,
             **kwargs,
@@ -333,24 +320,20 @@
 
         If universal_newlines=True is passed, the "input" argument
         must be a string and stdout/stderr in the returned object
         will be strings rather than bytes.
         """
         if input is not None:
             if commons.KW_STDIN in kwargs:
-                raise ValueError(
-                    "stdin and input arguments may not both be used."
-                )
+                raise ValueError("stdin and input arguments may not both be used.")
             #
             kwargs[commons.KW_STDIN] = commons.PIPE
         #
         program: child.Program = self.get_matching_program(*popenargs)
-        with parent.Popen(
-            *popenargs, child_steps=program.steps, **kwargs
-        ) as popen_obj:
+        with parent.Popen(*popenargs, child_steps=program.steps, **kwargs) as popen_obj:
             try:
                 stdout, stderr = popen_obj.communicate(input, timeout=timeout)
             except subprocess.TimeoutExpired as timeout_expired:
                 popen_obj.kill()
                 stdout, stderr = popen_obj.communicate()
                 raise subprocess.TimeoutExpired(
                     popen_obj.args, timeout, output=stdout, stderr=stderr
```

### Comparing `subprocess-mock-0.4.4/src/subprocess_mock.egg-info/PKG-INFO` & `subprocess_mock-0.4.5/src/subprocess_mock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subprocess-mock
-Version: 0.4.4
+Version: 0.4.5
 Summary: Subprocess Mock
 Author-email: Rainer Schwarzbach <rainer@blackstream.de>
 License: MIT License
         
         Copyright (c) 2024 Rainer Schwarzbach
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `subprocess-mock-0.4.4/src/subprocess_mock.egg-info/SOURCES.txt` & `subprocess_mock-0.4.5/src/subprocess_mock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `subprocess-mock-0.4.4/tests/test_commandline.py` & `subprocess_mock-0.4.5/tests/test_commandline.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 subprocess-mock is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the LICENSE file for more details.
 
 """
 
-
 import io
 import sys
 
 from unittest import TestCase
 
 from unittest.mock import patch
```

### Comparing `subprocess-mock-0.4.4/tests/test_functions.py` & `subprocess_mock-0.4.5/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `subprocess-mock-0.4.4/tests/test_main.py` & `subprocess_mock-0.4.5/tests/test_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 subprocess-mock is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the LICENSE file for more details.
 
 """
 
-
 import io
 import sys
 
 from unittest import TestCase
 
 from unittest.mock import patch
```

### Comparing `subprocess-mock-0.4.4/tests/test_streams.py` & `subprocess_mock-0.4.5/tests/test_streams.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,33 +53,25 @@
         """.buffer_size attribute as initialized"""
         with self.subTest("default"):
             wrapper = streams.ConnectionWrapper(self.read_conn)
             self.assertEqual(wrapper.buffer_size, io.DEFAULT_BUFFER_SIZE)
         #
         bufsize = 23
         with self.subTest("as initialized", bufsize=bufsize):
-            wrapper = streams.ConnectionWrapper(
-                self.read_conn, buffer_size=bufsize
-            )
+            wrapper = streams.ConnectionWrapper(self.read_conn, buffer_size=bufsize)
             self.assertEqual(wrapper.buffer_size, bufsize)
         #
         bufsize = 1
         with self.subTest("changed to 0", bufsize=bufsize):
-            wrapper = streams.ConnectionWrapper(
-                self.read_conn, buffer_size=bufsize
-            )
+            wrapper = streams.ConnectionWrapper(self.read_conn, buffer_size=bufsize)
             self.assertEqual(wrapper.buffer_size, 0)
         #
         bufsize = -25
-        with self.subTest(
-            "negative value changed to system default", bufsize=bufsize
-        ):
-            wrapper = streams.ConnectionWrapper(
-                self.read_conn, buffer_size=bufsize
-            )
+        with self.subTest("negative value changed to system default", bufsize=bufsize):
+            wrapper = streams.ConnectionWrapper(self.read_conn, buffer_size=bufsize)
             self.assertEqual(wrapper.buffer_size, io.DEFAULT_BUFFER_SIZE)
         #
 
     def test_property_connection(self) -> None:
         """.connection property is the connection as initialized"""
         wrapper = streams.ConnectionWrapper(self.read_conn)
         self.assertIs(wrapper.connection, self.read_conn)
@@ -166,17 +158,15 @@
             total_bytes += number_of_bytes
             self.assertEqual(read_data, written_data[:number_of_bytes])
         #
         with self.subTest("tell() result", expected=total_bytes):
             self.assertEqual(wrapper.tell(), total_bytes)
         #
         size = -7
-        with self.subTest(
-            "negative values smaller than -1 not accepted", size=size
-        ):
+        with self.subTest("negative values smaller than -1 not accepted", size=size):
             self.assertRaisesRegex(
                 ValueError,
                 "^invalid number of bytes to read",
                 wrapper.read,
                 size,
             )
         #
@@ -193,17 +183,15 @@
             total_bytes += old_number_of_bytes
             self.assertEqual(read_data, written_data[:old_number_of_bytes])
         #
         with self.subTest("read1 another part"):
             new_number_of_bytes = 2
             read_data = wrapper.read1(new_number_of_bytes)
             total_bytes += new_number_of_bytes
-            self.assertEqual(
-                read_data, written_data[old_number_of_bytes:total_bytes]
-            )
+            self.assertEqual(read_data, written_data[old_number_of_bytes:total_bytes])
         #
         with self.subTest("read1 0 bytes"):
             read_data = wrapper.read1(0)
             self.assertEqual(read_data, b"")
         #
         with self.subTest("tell() result", expected=total_bytes):
             self.assertEqual(wrapper.tell(), total_bytes)
@@ -249,25 +237,21 @@
         #
         with self.subTest("read a part"):
             written_data = b"longer message"
             number_of_bytes = 4
             self.write_conn.send_bytes(written_data)
             read_data = wrapper.read(number_of_bytes)
             total_bytes += number_of_bytes
-            self.assertEqual(
-                read_data, written_data[:number_of_bytes].decode()
-            )
+            self.assertEqual(read_data, written_data[:number_of_bytes].decode())
         #
         with self.subTest("tell() result", expected=total_bytes):
             self.assertEqual(wrapper.tell(), total_bytes)
         #
         size = -7
-        with self.subTest(
-            "negative values smaller than -1 not accepted", size=size
-        ):
+        with self.subTest("negative values smaller than -1 not accepted", size=size):
             self.assertRaisesRegex(
                 ValueError,
                 "^invalid number of bytes to read",
                 wrapper.read,
                 size,
             )
         #
@@ -278,17 +262,15 @@
         total_bytes = 0
         with self.subTest("read1 a part"):
             written_data = b"longer message"
             old_number_of_bytes = 4
             self.write_conn.send_bytes(written_data)
             read_data = wrapper.read1(old_number_of_bytes)
             total_bytes += old_number_of_bytes
-            self.assertEqual(
-                read_data, written_data[:old_number_of_bytes].decode()
-            )
+            self.assertEqual(read_data, written_data[:old_number_of_bytes].decode())
         #
         with self.subTest("read1 another part"):
             new_number_of_bytes = 2
             read_data = wrapper.read1(new_number_of_bytes)
             total_bytes += new_number_of_bytes
             self.assertEqual(
                 read_data,
@@ -316,17 +298,15 @@
         """.peek() and .tell() methods"""
         wrapper = streams.TextConnectionReader(self.read_conn)
         with self.subTest("read all"):
             written_data = b"testdata"
             number_of_bytes = 4
             self.write_conn.send_bytes(written_data)
             poke_data = wrapper.peek(number_of_bytes)
-            self.assertEqual(
-                poke_data, written_data[:number_of_bytes].decode()
-            )
+            self.assertEqual(poke_data, written_data[:number_of_bytes].decode())
         #
         with self.subTest("tell() result", expected=0):
             self.assertEqual(wrapper.tell(), 0)
         #
 
 
 class ConnectionWriterBase(BaseConnectionWrapper):
```

### Comparing `subprocess-mock-0.4.4/tests/test_workflow.py` & `subprocess_mock-0.4.5/tests/test_workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,17 +123,15 @@
             with self.subTest("call arguments"):
                 self.assertEqual(result.args, echo_command)
             #
             with self.subTest(commons.KW_RETURNCODE):
                 self.assertEqual(result.returncode, commons.RETURNCODE_OK)
             #
             expected_stdout = mock_output.encode()
-            with self.subTest(
-                commons.KW_STDOUT, expected_stdout=expected_stdout
-            ):
+            with self.subTest(commons.KW_STDOUT, expected_stdout=expected_stdout):
                 self.assertEqual(result.stdout, expected_stdout)
             #
             with self.subTest(commons.KW_STDERR):
                 self.assertIsNone(result.stderr)
             #
             with self.subTest("mock call result was registered"):
                 last_result = orchestrator.get_last_result()
@@ -143,17 +141,15 @@
 
     def test_set_returncode(self) -> None:
         """.run() method – Set returncode"""
         command = ["false"]
         orchestrator = workflow.Orchestrator()
         orchestrator.add_program(
             *command,
-            program=child.Program(
-                child.SetReturncode(commons.RETURNCODE_ERROR)
-            ),
+            program=child.Program(child.SetReturncode(commons.RETURNCODE_ERROR)),
         )
         with patch(SUBPROCESS_RUN, new=orchestrator.run):
             with self.subTest(
                 "Exception is raised with nonzero returncode and check=True"
             ):
                 self.assertRaises(
                     subprocess.CalledProcessError,
@@ -164,17 +160,15 @@
             #
             logging.warning("Results store: %r", orchestrator.all_results)
             last_result = orchestrator.get_last_result()
             with self.subTest("Result was registered"):
                 self.assertEqual(last_result[1].args, command)
             #
             with self.subTest("Returncode was recorded"):
-                self.assertEqual(
-                    last_result[1].returncode, commons.RETURNCODE_ERROR
-                )
+                self.assertEqual(last_result[1].returncode, commons.RETURNCODE_ERROR)
             #
         #
         #
 
     def test_run_stdout_only(self) -> None:
         """.run() method – Output to stdout only"""
         orchestrator = workflow.Orchestrator()
```

