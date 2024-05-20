# Comparing `tmp/zut-0.9.0-py3-none-any.whl.zip` & `tmp/zut-0.9.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,18 @@
-Zip file size: 49858 bytes, number of entries: 15
--rw-rw-rw-  2.0 fat    87531 b- defN 24-Mar-22 22:19 zut/__init__.py
--rw-rw-rw-  2.0 fat      427 b- defN 24-Mar-22 22:41 zut/_version.py
+Zip file size: 54123 bytes, number of entries: 16
+-rw-rw-rw-  2.0 fat    88849 b- defN 24-May-20 08:57 zut/__init__.py
+-rw-rw-rw-  2.0 fat      427 b- defN 24-May-20 15:24 zut/_version.py
 -rw-rw-rw-  2.0 fat    24764 b- defN 24-Mar-21 02:07 zut/excel.py
 -rw-rw-rw-  2.0 fat    12859 b- defN 24-Mar-21 10:49 zut/files.py
--rw-rw-rw-  2.0 fat     2576 b- defN 24-Mar-21 02:07 zut/db/__init__.py
--rw-rw-rw-  2.0 fat    26431 b- defN 24-Mar-22 07:28 zut/db/base.py
--rw-rw-rw-  2.0 fat     8802 b- defN 24-Mar-21 09:36 zut/db/mssql.py
--rw-rw-rw-  2.0 fat    19191 b- defN 24-Mar-22 07:52 zut/db/pg.py
+-rw-rw-rw-  2.0 fat     2984 b- defN 24-May-20 14:22 zut/db/__init__.py
+-rw-rw-rw-  2.0 fat    27603 b- defN 24-May-20 14:04 zut/db/base.py
+-rw-rw-rw-  2.0 fat    11635 b- defN 24-May-20 14:18 zut/db/mssql.py
+-rw-rw-rw-  2.0 fat     8390 b- defN 24-May-20 15:01 zut/db/mysql.py
+-rw-rw-rw-  2.0 fat    19153 b- defN 24-May-20 13:13 zut/db/pg.py
 -rw-rw-rw-  2.0 fat     3808 b- defN 24-Mar-21 09:36 zut/db/pg2.py
 -rw-rw-rw-  2.0 fat     1641 b- defN 24-Jan-24 18:06 zut/db/sql-utils/pg.sql
--rw-rw-rw-  2.0 fat     1103 b- defN 24-Mar-22 22:41 zut-0.9.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     3758 b- defN 24-Mar-22 22:41 zut-0.9.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-22 22:41 zut-0.9.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 24-Mar-22 22:41 zut-0.9.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1092 b- defN 24-Mar-22 22:41 zut-0.9.0.dist-info/RECORD
-15 files, 194079 bytes uncompressed, 48112 bytes compressed:  75.2%
+-rw-rw-rw-  2.0 fat     1103 b- defN 24-May-20 15:24 zut-0.9.1.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     3872 b- defN 24-May-20 15:24 zut-0.9.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-20 15:24 zut-0.9.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 24-May-20 15:24 zut-0.9.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1165 b- defN 24-May-20 15:24 zut-0.9.1.dist-info/RECORD
+16 files, 208349 bytes uncompressed, 52271 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -15,32 +15,35 @@
 
 Filename: zut/db/base.py
 Comment: 
 
 Filename: zut/db/mssql.py
 Comment: 
 
+Filename: zut/db/mysql.py
+Comment: 
+
 Filename: zut/db/pg.py
 Comment: 
 
 Filename: zut/db/pg2.py
 Comment: 
 
 Filename: zut/db/sql-utils/pg.sql
 Comment: 
 
-Filename: zut-0.9.0.dist-info/LICENSE.txt
+Filename: zut-0.9.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: zut-0.9.0.dist-info/METADATA
+Filename: zut-0.9.1.dist-info/METADATA
 Comment: 
 
-Filename: zut-0.9.0.dist-info/WHEEL
+Filename: zut-0.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: zut-0.9.0.dist-info/top_level.txt
+Filename: zut-0.9.1.dist-info/top_level.txt
 Comment: 
 
-Filename: zut-0.9.0.dist-info/RECORD
+Filename: zut-0.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zut/__init__.py

```diff
@@ -1,38 +1,38 @@
 """
 Reusable Python utilities (top-level API).
 """
 from __future__ import annotations
 
 import atexit
-from contextlib import nullcontext
 import csv
 import ctypes
 import inspect
 import json
 import locale
 import logging
 import logging.config
 import os
 import re
 import socket
-from subprocess import CompletedProcess, SubprocessError
 import sys
 import unicodedata
 from argparse import ArgumentParser, RawTextHelpFormatter, _SubParsersAction
 from configparser import _UNSET, ConfigParser, RawConfigParser
+from contextlib import nullcontext
 from datetime import date, datetime, time, timedelta, timezone, tzinfo
 from decimal import Decimal
 from enum import Enum, Flag
 from http.client import HTTPResponse
 from importlib import import_module
 from importlib.util import find_spec
 from io import BufferedIOBase, IOBase, StringIO, TextIOBase, TextIOWrapper
 from ipaddress import AddressValueError, IPv4Address, IPv6Address, ip_address
 from pathlib import Path
+from subprocess import CompletedProcess, SubprocessError
 from textwrap import dedent
 from threading import Thread
 from traceback import format_exception
 from types import FunctionType, ModuleType, TracebackType
 from typing import (TYPE_CHECKING, Any, Callable, Iterable, MutableMapping,
                     TypeVar, overload)
 from urllib.error import HTTPError, URLError
@@ -63,22 +63,20 @@
 
     # Used to parse timezones from strings through ZoneInfo on Windows (Windows does not maintain a database of timezones)
 except ImportError:
     tzdata = None
 
 try:
     import tzlocal
-
     # Used to parse timezones from strings on Windows (Windows does not maintain a database of timezones and `tzdata` only is not enough)
 except ImportError:
     tzlocal = None
 
 try:
     import pytz
-
     # Used to parse timezones on Python < 3.9 (no ZoneInfo available)
 except ImportError:
     pytz = None
 
 try:
     import colorlog
 except ImportError:
@@ -542,15 +540,15 @@
     Dump a list of dicts or iterables to CSV.
     """
     with out_table(out, tablefmt='csv', headers=headers, encoding=encoding, csv_decimal_separator=csv_decimal_separator, csv_delimiter=csv_delimiter, csv_quotechar=csv_quotechar, csv_nullval=csv_nullval, **params) as t:
         for row in data:
             t.append(row)
 
 
-def get_dicts_from_csv(file: os.PathLike|IOBase, *, headers: list[str|Header] = None, encoding: str = 'utf-8', noheaders: bool = False, csv_delimiter: str = None, csv_quotechar: str = None, csv_nullval: str = None):
+def iter_dicts_from_csv(file: os.PathLike|IOBase, *, headers: list[str|Header] = None, encoding: str = 'utf-8', noheaders: bool = False, csv_delimiter: str = None, csv_quotechar: str = None, csv_nullval: str = None):
     """
     Iterate over CSV as dicts.
     """    
     from zut import files
 
     if noheaders and not headers:
         raise ValueError("Headers must be given has an argument if CSV file does not contain headers.")
@@ -586,19 +584,19 @@
 
                 yield data
 
         if isinstance(file, IOBase):
             file.seek(0)
 
 
-def list_dicts_from_csv(file: os.PathLike|IOBase, *, headers: list[str|Header] = None, encoding: str = 'utf-8', noheaders: bool = False, csv_delimiter: str = None, csv_quotechar: str = None, csv_nullval: str = None):
+def get_dicts_from_csv(file: os.PathLike|IOBase, *, headers: list[str|Header] = None, encoding: str = 'utf-8', noheaders: bool = False, csv_delimiter: str = None, csv_quotechar: str = None, csv_nullval: str = None):
     """
     Load CSV as a dict list.
     """
-    return [row for row in get_dicts_from_csv(file, headers=headers, encoding=encoding, noheaders=noheaders, csv_delimiter=csv_delimiter, csv_quotechar=csv_quotechar, csv_nullval=csv_nullval)]
+    return [row for row in iter_dicts_from_csv(file, headers=headers, encoding=encoding, noheaders=noheaders, csv_delimiter=csv_delimiter, csv_quotechar=csv_quotechar, csv_nullval=csv_nullval)]
 
 
 def get_csv_headers(file: os.PathLike|IOBase, *, encoding: str = 'utf-8', csv_delimiter: str = None, csv_quotechar: str = None) -> list[Header]:
     from zut import files
 
     with nullcontext(file) if isinstance(file, IOBase) else files.open(file, 'r', newline='', encoding=encoding) as fp:
         _, csv_delimiter, csv_quotechar, _ = _get_csv_params(None, csv_delimiter, csv_quotechar, None, context=fp)
@@ -760,20 +758,27 @@
             return super().default(o)
 
 #endregion
 
 
 #region Locale
 
-def register_locale(value: str = ''):
+def register_locale(value: str = '', *, use_excel_csv: bool = True):
+    """
+    Register locale (default locale if argument `value` is None).
+
+    - `use_excel_csv`: if True, use Excel-compatible version of CSV (which is localized) in OutTable by default.
+    """
     lang, encoding = locale.getlocale(locale.LC_NUMERIC)
     if lang:
         logger.warning("Locale already set: lang=%s, encoding=%s", lang, encoding)
 
     locale.setlocale(locale.LC_ALL, value)
+    if use_excel_csv:
+        OutTable.DEFAULT_CSV_FMT = 'csv-excel'
 
 
 def is_locale_registered(warn = False):
     lang, encoding = locale.getlocale(locale.LC_NUMERIC)
     if lang and warn:
         logger.warning("Locale already set: lang=%s, encoding=%s", lang, encoding)
     return lang is not None
@@ -1426,21 +1431,15 @@
             self.db = None
         
         super().__init__(out, title=title, append=append, encoding=encoding, atexit=atexit)
 
         if self.db:
             self.out_name = self.db.get_url(hide_password=True)
 
-        self.headers: list[Header] = None  # for CSV, not None <=> export started
-        if headers:
-            self.headers = []
-            for header in headers:            
-                if not isinstance(header, Header):
-                    header = Header(str(header), dict_key=header)
-                self.headers.append(header)
+        self.headers: list[Header] = headers  # for CSV, not None <=> export started
 
         if self.db:
             if tablefmt and tablefmt != 'csv':
                 raise ValueError(f"Tablefmt \"{tablefmt}\" cannot be used for a database output")
             if csv_decimal_separator and csv_decimal_separator != '.':
                 raise ValueError(f"CSV decimal separator \"{csv_decimal_separator}\" cannot be used for a database output")
             self.tablefmt = 'csv'
@@ -1481,14 +1480,22 @@
         self._delayed_rows: list[Iterable] = []
         self._reordering: list[int] = None
         self._reordering_default: list|None = None
 
 
     def __enter__(self):
         super().__enter__()
+        
+        if self.headers: # ensure all headers are of type Header
+            actual_headers = []
+            for header in self.headers:            
+                if not isinstance(header, Header):
+                    header = Header(str(header), dict_key=header)
+                actual_headers.append(header)
+            self.headers = actual_headers
             
         if not self.out:
             pass
         elif self.tablefmt.startswith('csv') and self.headers is not None:
             self._export_started = True
             self._export_headers()
         
@@ -2044,15 +2051,22 @@
         _kernel32 = ctypes.windll.kernel32
         _kernel32.SetConsoleMode(_kernel32.GetStdHandle(-11), 7)
         del _kernel32
 
 #endregion
 
 
-#region Subprocesses
+#region Errors
+
+class MessageError(ValueError):
+    """
+    An error that should result to only an error message being printed on the console, without a stack trace.
+    """
+    pass
+
 
 def check_completed_subprocess(cp: CompletedProcess, logger: logging.Logger = None, *, label: str = None, level: int|str = None, accept_returncode: int|list[int]|bool = False, accept_stdout: bool = False, accept_stderr: bool = False, maxlen: int = 200):
     """
     Improve message in case of subprocess error, to ease debugging.
     """
     if not label:
         label = cp.args[0]
@@ -2070,16 +2084,18 @@
             return returncode != accept_returncode
         elif isinstance(accept_returncode, (list,tuple)):
             return returncode not in accept_returncode
         else:
             return returncode != 0
     
 
-    def extract_stream(content: str|bytes, name: str, color: str):
-        if not isinstance(content, str):
+    def extract_stream(content: str|bytes|None, name: str, color: str):
+        if content is None:
+            return None
+        elif not isinstance(content, str):
             try:
                 content = content.decode('utf-8')
             except UnicodeDecodeError:
                 content = content.decode('cp1252')
         
         data = content.strip()
         if maxlen and len(data) > maxlen:
@@ -2225,23 +2241,48 @@
 def get_description_text(docstring: str):
     if docstring is None:
         return None
     
     return dedent(docstring)
 
 
+def get_exit_code(return_value: Any) -> int:
+    if not isinstance(return_value, int):
+        return_value = 0 if return_value is None or return_value is True else 1
+    return return_value
+
+
+def exec_command(handle: Callable, args: dict):
+    if not handle:
+        logger.error("No command given")
+        return 1
+
+    try:
+        r = handle(**args)
+        r = get_exit_code(r)
+    except MessageError as err:
+        logger.error(str(err))
+        r = 1
+    except BaseException as err: # including KeyboardInterrupt
+        message = str(err)
+        logger.exception(f"Exiting on {type(err).__name__}{f': {message}' if message else ''}")
+        r = 1
+
+    sys.exit(r)
+
+
 #endregion
 
 
 #region Config
 
 _configs: dict[Path,ExtendedConfigParser] = {}
 
-def get_config(prog_module: ModuleType|str|Path, *, if_none: Literal['warn'] = None):
-    prog_root = _get_module_root(prog_module)
+def get_config(prog: ModuleType|str|Path, *, if_none: Literal['warn'] = None):
+    prog_root = _get_module_root(prog)
     config = _configs.get(prog_root)
 
     if config:
         return config
     
     else:
         config = ExtendedConfigParser()
@@ -2255,16 +2296,16 @@
         else:
             if if_none == 'warn':
                 logger.warning("No config file found")
 
         return config
 
 
-def get_config_paths(prog_module: ModuleType|str|Path, name: str = None, *, if_exist: bool = False):
-    prog_root = _get_module_root(prog_module)
+def get_config_paths(prog: ModuleType|str|Path, name: str = None, *, if_exist: bool = False):
+    prog_root = _get_module_root(prog)
     prog_name = prog_root.name.replace('_', '-')
 
     if name is None:
         name = '' # will point on config directories
     elif name.startswith('.'):
         name = f"{prog_name}{name}"
     
@@ -2513,15 +2554,15 @@
 
 
 #region Files
 
 def configure_smb_credentials(user: str = None, password: str = None):
     global _smb_credentials_configured
     
-    from zut.files import smbclient, _smb_credentials_configured
+    from zut.files import _smb_credentials_configured, smbclient
 
     if user or password:
         if not smbclient:
             raise ValueError(f"Package `smbprotocol` is required to specify smb credentials")
         smbclient.ClientConfig(username=user, password=password)
         _smb_credentials_configured = True
```

## zut/_version.py

```diff
@@ -8,9 +8,9 @@
     VERSION_TUPLE = object
 
 version: str
 __version__: str
 __version_tuple__: VERSION_TUPLE
 version_tuple: VERSION_TUPLE
 
-__version__ = version = '0.9.0'
-__version_tuple__ = version_tuple = (0, 9, 0)
+__version__ = version = '0.9.1'
+__version_tuple__ = version_tuple = (0, 9, 1)
```

## zut/db/__init__.py

```diff
@@ -4,14 +4,15 @@
 from __future__ import annotations
 
 import re
 from urllib.parse import urlparse
 
 from .base import DbAdapter, _get_connection_from_wrapper
 from .mssql import MssqlAdapter
+from .mysql import MysqlAdapter
 from .pg import PgAdapter
 from .pg2 import Pg2Adapter
 
 
 def get_db_adapter(origin) -> DbAdapter:
     if isinstance(origin, str):
         if origin.startswith('db:'):
@@ -22,16 +23,18 @@
         if r.scheme in ['postgresql', 'postgres', 'pg']:
             if PgAdapter.is_available():
                 adapter = PgAdapter
             elif Pg2Adapter.is_available():
                 adapter = Pg2Adapter
             else:
                 raise ValueError(f"PgAdapter and Pg2Adapter not available (psycopg missing)")
-        elif r.scheme in ['mssql']:
+        elif r.scheme in ['mssql', 'mssqls']:
             adapter = MssqlAdapter
+        elif r.scheme in ['mysql', 'mariadb']:
+            adapter = MysqlAdapter
         elif r.scheme:
             raise ValueError(f"unsupported db engine: {r.scheme}")
         else:
             raise ValueError(f"invalid db: no scheme in {origin}")
         
         if not adapter.is_available():
             raise ValueError(f"cannot use db {r.scheme} ({adapter.__name__} not available)")
@@ -41,14 +44,16 @@
     elif isinstance(origin, dict) and 'ENGINE' in origin: # Django
         engine = origin['ENGINE']
         if engine in ["django.db.backends.postgresql", "django.contrib.gis.db.backends.postgis"]:
             if PgAdapter.is_available():
                 return PgAdapter(origin), None, None
             else:
                 return Pg2Adapter(origin), None, None
+        elif engine in ["django.db.backends.mysql", "django.contrib.gis.db.backends.mysql"]:
+            return MysqlAdapter(origin), None, None
         elif engine in ["mssql"]:
             return MssqlAdapter(origin), None, None
         else:
             raise ValueError(f"invalid db: unsupported django db engine: {engine}")
         
     elif isinstance(origin, DbAdapter):
         return origin, None, None
@@ -58,17 +63,19 @@
         
         type_fullname: str = type(origin).__module__ + '.' + type(origin).__qualname__
 
         if type_fullname == 'psycopg2.extension.connection':
             return Pg2Adapter(origin), None, None
         elif type_fullname == 'psycopg.Connection':
             return PgAdapter(origin), None, None
+        elif type_fullname == 'MySQLdb.connections.Connection':
+            return MysqlAdapter(origin), None, None
         elif type_fullname == 'pyodbc.Connection':
             return MssqlAdapter(origin), None, None
 
         raise ValueError(f"invalid db: unsupported origin type: {type(origin)}")
 
 
 __all__ = (
-    'DbAdapter', 'MssqlAdapter', 'PgAdapter', 'Pg2Adapter',
+    'DbAdapter', 'MssqlAdapter', 'MysqlAdapter', 'PgAdapter', 'Pg2Adapter',
     'get_db_adapter',
 )
```

## zut/db/base.py

```diff
@@ -6,15 +6,15 @@
 from contextlib import nullcontext
 from datetime import datetime, time, tzinfo
 from io import IOBase, StringIO, TextIOWrapper
 from pathlib import Path
 from typing import Any, Generic, Sequence, TypeVar
 from urllib.parse import ParseResult, quote, urlparse
 
-from .. import (Literal, build_url, hide_url_password, is_aware, make_aware,
+from .. import (Literal, OutTable, build_url, hide_url_password, is_aware, make_aware,
                 out_table, skip_utf8_bom)
 
 try:
     from tabulate import tabulate
 except ImportError:
     tabulate = None
 
@@ -48,15 +48,15 @@
     EXPECTED_CONNECTION_TYPES: list[str]
 
     @classmethod
     def is_available(cls):
         raise NotImplementedError()
     
 
-    def __init__(self, origin: T_Connection|str|dict|ParseResult, autocommit: bool = True, tz: tzinfo = None):
+    def __init__(self, origin: T_Connection|str|dict|ParseResult, password_required: bool = False, autocommit: bool = True, tz: tzinfo = None):
         """
         Create a new adapter.
         - `origin`: an existing connection object, or the URL or django alias (e.g. 'default') for the new connection to create by the adapter.
         - `autocommit`: whether or not to auto-commit transactions (applies only for connections created by the adapter)
         """
         if not self.is_available():
             raise ValueError(f"Cannot use {type(self).__name__} (not available)")
@@ -150,108 +150,245 @@
             fulltype = type(origin).__module__ + '.' + type(origin).__qualname__
             if fulltype not in self.EXPECTED_CONNECTION_TYPES:
                 raise ValueError(f"invalid connection type for {type(self).__name__}: {fulltype}")
             self._connection = origin
             self._connection_url: str = None
             self._must_close_connection = False
         
-        self.autocommit: bool = autocommit
+        self.password_required = password_required
+        self.autocommit = autocommit
         self.tz = tz
+    
+
+    def get_url(self, *, hide_password = False):
+        if self._connection_url:
+            url = self._connection_url
+        else:
+            url = self._get_url_from_connection()
+
+        if hide_password:
+            url = hide_url_password(url)
 
+        if self.table:
+            url += f"/"
+            if self.schema:
+                url += quote(self.schema)
+                url += '.'
+            url += quote(self.table)
+
+        return url
+
+
+    def _get_url_from_connection(self):
+        raise NotImplementedError()
+
+
+    #region Connection
 
     def __enter__(self):
         return self
 
 
     def __exit__(self, exc_type = None, exc_val = None, exc_tb = None):
         self.close()
 
 
     def close(self):
         if self._connection and self._must_close_connection:
             if logger.isEnabledFor(logging.DEBUG):
-                logger.debug(f"close %s (%s) connection to %s", type(self).__name__, type(self._connection).__module__ + '.' + type(self._connection).__qualname__, hide_url_password(self._connection_url))
+                logger.debug(f"Close %s (%s) connection to %s", type(self).__name__, type(self._connection).__module__ + '.' + type(self._connection).__qualname__, hide_url_password(self._connection_url))
             self._connection.close()
 
 
     @property
     def connection(self):
         if not self._connection:                
+            if self.password_required:
+                password = urlparse(self._connection_url).password
+                if not password:
+                    raise ValueError("Cannot create %s connection to %s: password not provided" % (type(self).__name__, hide_url_password(self._connection_url)))
             if logger.isEnabledFor(logging.DEBUG):
-                logger.debug(f"create %s connection to %s", type(self).__name__, hide_url_password(self._connection_url))
+                logger.debug(f"Create %s connection to %s", type(self).__name__, hide_url_password(self._connection_url))
             self._connection = self._create_connection()
         return self._connection
 
 
+    def _create_connection(self) -> T_Connection:
+        raise NotImplementedError()
+
+
     def cursor(self) -> T_Cursor:
         return self.connection.cursor()
 
+    #endregion
+    
 
-    def _create_connection(self) -> T_Connection:
-        raise NotImplementedError()
+    #region Queries
 
+    def to_positional_params(self, query: str, params: dict) -> tuple[str, Sequence[Any]]:
+        from sqlparams import \
+            SQLParams  # not at the top because the enduser might not need this feature
 
-    def get_url(self, *, hide_password = False):
-        if self._connection_url:
-            url = self._connection_url
-        else:
-            url = self._get_url_from_connection()
+        if not hasattr(self.__class__, '_params_formatter'):
+            self.__class__._params_formatter = SQLParams('named', 'qmark')
+        query, params = self.__class__._params_formatter.format(query, params)
 
-        if hide_password:
-            url = hide_url_password(url)
+        return query, params
+    
+    
+    def get_paginated_query(self, query: str, *, limit: int|None, offset: int|None) -> str:
+        paginated_query, _ = self.get_paginated_and_total_query(query, limit=limit, offset=offset)
+        return paginated_query
+    
 
-        if self.table:
-            url += f"/"
-            if self.schema:
-                url += quote(self.schema)
-                url += '.'
-            url += quote(self.table)
+    def get_paginated_and_total_query(self, query: str, *, limit: int|None, offset: int|None) -> tuple[str,str]:        
+        if limit is not None:
+            if isinstance(limit, str) and re.match(r"^[0-9]+$", limit):
+                limit = int(limit)
+            elif not isinstance(limit, int):
+                raise TypeError(f"Invalid type for limit: {type(limit).__name__} (expected int)")
+            
+        if offset is not None:
+            if isinstance(offset, str) and re.match(r"^[0-9]+$", offset):
+                offset = int(offset)
+            elif not isinstance(offset, int):
+                raise TypeError(f"Invalid type for offset: {type(limit).__name__} (expected int)")
+        
+        beforepart, selectpart, orderpart = self._parse_select_query(query)
 
-        return url
+        paginated_query = beforepart
+        total_query = beforepart
+        
+        paginated_query += self._paginate_parsed_query(selectpart, orderpart, limit=limit, offset=offset)
+        total_query += f"SELECT COUNT(*) FROM ({selectpart}) s"
 
+        return paginated_query, total_query
+    
 
-    def _get_url_from_connection(self):
-        raise NotImplementedError()
+    def _parse_select_query(self, query: str):
+        import sqlparse  # not at the top because the enduser might not need this feature
+
+        # Parse SQL to remove token before the SELECT keyword
+        # example: WITH (CTE) tokens
+        statements = sqlparse.parse(query)
+        if len(statements) != 1:
+            raise ValueError(f"query contains {len(statements)} statements")
+
+        # Get first DML keyword
+        dml_keyword = None
+        dml_keyword_index = None
+        order_by_index = None
+        for i, token in enumerate(statements[0].tokens):
+            if token.ttype == sqlparse.tokens.DML:
+                if dml_keyword is None:
+                    dml_keyword = str(token).upper()
+                    dml_keyword_index = i
+            elif token.ttype == sqlparse.tokens.Keyword:
+                if order_by_index is None:
+                    keyword = str(token).upper()
+                    if keyword == "ORDER BY":
+                        order_by_index = i
+
+        # Check if the DML keyword is SELECT
+        if not dml_keyword:
+            raise ValueError(f"no SELECT found (query does not contain DML keyword)")
+        if dml_keyword != 'SELECT':
+            raise ValueError(f"first DML keyword is {dml_keyword}, expected SELECT")
+
+        # Get part before SELECT (example: WITH)
+        if dml_keyword_index > 0:
+            tokens = statements[0].tokens[:dml_keyword_index]
+            beforepart = ''.join(str(token) for token in tokens)
+        else:
+            beforepart = ''
+    
+        # Determine actual SELECT query
+        if order_by_index is not None:
+            tokens = statements[0].tokens[dml_keyword_index:order_by_index]
+            selectpart = ''.join(str(token) for token in tokens)
+            tokens = statements[0].tokens[order_by_index:]
+            orderpart = ''.join(str(token) for token in tokens)
+        else:
+            tokens = statements[0].tokens[dml_keyword_index:]
+            selectpart = ''.join(str(token) for token in tokens)
+            orderpart = ''
+
+        return beforepart, selectpart, orderpart
     
 
-    #region Execution
+    def _paginate_parsed_query(self, selectpart: str, orderpart: str, *, limit: int|None, offset: int|None) -> str:
+        result = f"{selectpart} {orderpart}"
+        if limit is not None:
+            result += f" LIMIT {limit}"
+        if offset is not None:
+            result += f" OFFSET {offset}"
+        return result
+    
 
-    def _log_cursor_messages(self, cursor: T_Cursor):
+    def get_select_table_query(self, table: str|tuple = None, *, schema_only = False) -> T_Composed:
         """
-        Log cursor messages produced after execution of a query, if this cannot be done through a connection handler.
+        Build a query on the given table.
+
+        If `schema_only` is given, no row will be returned (this is used to get information on the table).
+        Otherwise, all rows will be returned.
+
+        The return type of this function depends on the database engine.
+        It is passed directly to the cursor's execute function for this engine.
         """
-        pass
+        raise NotImplementedError()
+
+
+    def _get_composable_param(self, value) -> T_Composable:
+        if value is None:
+            return "null"
+        elif value == '__now__':
+            return "CURRENT_DATETIME()"
+        else:
+            return self.escape_literal(value)
+                
 
-    def execute_query(self, query: str, params: list|tuple|dict = None, *, cursor: T_Cursor = None, results: bool|Literal['warning']|TextIOWrapper|str|Path = False, tz: tzinfo = None, offset: int = None, limit: int = None, query_id: str = None):
+    def escape_identifier(self, value) -> T_Composable:
+        raise NotImplementedError()
+                
+
+    def escape_literal(self, value) -> T_Composable:
+        raise NotImplementedError()
+    
+    #endregion
+    
+
+    #region Execution
+
+    def execute_query(self, query: str, params: list|tuple|dict = None, *, cursor: T_Cursor = None, results: bool|Literal['warning']|TextIOWrapper|OutTable|str|Path = False, tz: tzinfo = None, limit: int = None, offset: int = None, query_id: str = None):
         """
         - `results`:
             - If True, return results as a dict list.
             - If False, ignore results.
             - If `warning`, produce a warning log if there is results.
             - If a stream or a str/path, write results as CSV to the given stream and return tuple (columns, row_count)
         - `tz`: naive datetimes in results are made aware in the given timezone.
         """
-        if offset is not None or limit is not None:
-            query = self.get_paginated_query(query, offset=offset, limit=limit)
+        if limit is not None or offset is not None:
+            query = self.get_paginated_query(query, limit=limit, offset=offset)
                 
         # Example of positional param: cursor.execute("INSERT INTO foo VALUES (%s)", ["bar"])
         # Example of named param: cursor.execute("INSERT INTO foo VALUES (%(foo)s)", {"foo": "bar"})
         if params is None:
             params = []
         elif isinstance(params, dict) and self.ONLY_POSITIONAL_PARAMS:
             query, params = self.to_positional_params(query, params)
 
         with nullcontext(cursor) if cursor else self.cursor() as _cursor:            
             # Execute query
             _cursor.execute(query, params)
-            self._log_cursor_messages(_cursor)
+            self._log_execute_messages(_cursor)
 
             # Log number of affected rows for non-select queries
             if not _cursor.description and _cursor.rowcount >= 0:
-                logger.debug(f"affected rows: {_cursor.rowcount:,}")
+                logger.debug(f"Affected rows: {_cursor.rowcount:,}")
 
             def format_row(row):
                 if tz or self.tz:
                     for i, value in enumerate(row):
                         if isinstance(value, (datetime,time)):
                             if not is_aware(value):
                                 row[i] = make_aware(value, tz or self.tz)
@@ -275,55 +412,66 @@
                             text_rows = fp.getvalue()
 
                         if row_count > 10:
                             text_rows += "\n…"
                         logger.warning("query%s returned %d row%s:\n%s", f" {query_id}" if query_id else "", row_count, "s" if row_count > 1 else "", text_rows)
                 return None
             
-            elif isinstance(results, (IOBase,str,Path)):
+            elif isinstance(results, (OutTable,IOBase,str,Path)):
                 # Write results as CSV to the given stream
                 columns = self.get_cursor_column_names(_cursor)
+
+                if isinstance(results, OutTable):
+                    o = results
+                    o.headers = columns
+                else:
+                    o = out_table(results, headers=columns, title=False, tablefmt='csv')
                 
-                with out_table(results, headers=columns, title=False, tablefmt='csv') as o:
-                    row_count = 0
+                with o:
                     for row in _cursor:
                         o.append(format_row(row))
-                        row_count += 1
                     
                     o.file.seek(0)
-                    return columns, row_count
+                    return columns, o.row_count
 
             elif results:
                 # Return results as a dict list
                 columns = self.get_cursor_column_names(_cursor)
                 return [{columns[i]: value for i, value in enumerate(format_row(row))} for row in _cursor]
             
             else:
                 return None
 
 
-    def execute_file(self, path: str|Path, params: list|tuple|dict = None, *, cursor: T_Cursor = None, results: bool|TextIOWrapper|str|Path = False, tz: tzinfo = None, offset: int = None, limit: int = None, encoding: str = 'utf-8') -> None:
+    def _log_execute_messages(self, cursor: T_Cursor):
+        """
+        Log messages produced during execution of a query, if this cannot be done through a connection handler.
+        """
+        pass
+
+
+    def execute_file(self, path: str|Path, params: list|tuple|dict = None, *, cursor: T_Cursor = None, results: bool|TextIOWrapper|str|Path = False, tz: tzinfo = None, limit: int = None, offset: int = None, encoding: str = 'utf-8') -> None:
         with open(path, 'r', encoding=encoding) as fp:
             skip_utf8_bom(fp)
             query = fp.read()
             
-        self.execute_query(query, params, cursor=cursor, results=results, tz=tz, offset=offset, limit=limit)
+        self.execute_query(query, params, cursor=cursor, results=results, tz=tz, limit=limit, offset=offset)
     
 
     def execute_procedure(self, name: str|tuple, *args) -> T_Cursor:
         return NotImplementedError()
     
     #endregion
 
 
-    #region Particular types of results
+    #region Results
 
-    def get_scalar(self, query: str, params: list|tuple|dict = None, *, offset: int = None, limit: int = None):
+    def get_scalar(self, query: str, params: list|tuple|dict = None, *, limit: int = None, offset: int = None):
         with self.cursor() as cursor:
-            self.execute_query(query, params, cursor=cursor, offset=offset, limit=limit)
+            self.execute_query(query, params, cursor=cursor, limit=limit, offset=offset)
 
             iterator = iter(cursor)
             try:
                 row = next(iterator)
             except StopIteration:
                 raise NotFoundError()
 
@@ -332,28 +480,28 @@
                 raise SeveralFoundError()
             except StopIteration:
                 pass
 
             return row[0]
     
 
-    def list_scalars(self, query: str, params: list|tuple|dict = None, *, offset: int = None, limit: int = None):
+    def get_scalars(self, query: str, params: list|tuple|dict = None, *, limit: int = None, offset: int = None):
         results = []
 
         with self.cursor() as cursor:
-            self.execute_query(query, params, cursor=cursor, offset=offset, limit=limit)
+            self.execute_query(query, params, cursor=cursor, limit=limit, offset=offset)
             for row in cursor:
                 results.append(row[0])
 
         return results
 
 
-    def get_dict(self, query: str, params: list|tuple|dict = None):
+    def get_dict(self, query: str, params: list|tuple|dict = None, *, limit: int = None, offset: int = None):
         with self.cursor() as cursor:
-            self.execute_query(query, params, cursor=cursor)
+            self.execute_query(query, params, limit=limit, offset=offset, cursor=cursor)
 
             iterator = iter(cursor)
             try:
                 row = next(iterator)
             except StopIteration:
                 raise NotFoundError()
 
@@ -363,178 +511,42 @@
             except StopIteration:
                 pass
 
             columns = self.get_cursor_column_names(cursor)
             return {columns[i]: value for i, value in enumerate(row)}
     
 
-    def get_result(self, query: str, params: list|tuple|dict = None, *, offset: int = None, limit: int = None):
+    def get_result(self, query: str, params: list|tuple|dict = None, *, limit: int = None, offset: int = None):
         cursor = self.cursor()
-        self.execute_query(query, params, offset=offset, limit=limit, cursor=cursor)
+        self.execute_query(query, params, limit=limit, offset=offset, cursor=cursor)
         return CursorResult(self, cursor)
     
 
-    def get_dicts(self, query: str, params: list|tuple|dict = None, *, offset: int = None, limit: int = None):        
+    def iter_dicts(self, query: str, params: list|tuple|dict = None, *, limit: int = None, offset: int = None):        
         with self.cursor() as cursor:
-            self.execute_query(query, params, offset=offset, limit=limit, cursor=cursor)
+            self.execute_query(query, params, limit=limit, offset=offset, cursor=cursor)
             columns = self.get_cursor_column_names(cursor)
             for row in cursor:
                 yield {columns[i]: value for i, value in enumerate(row)}
+                
     
-    
-    def list_dicts(self, query: str, params: list|tuple|dict = None, *, offset: int = None, limit: int = None):        
-        return [row for row in self.get_dicts(query, params, offset=offset, limit=limit)]
+    def get_dicts(self, query: str, params: list|tuple|dict = None, *, limit: int = None, offset: int = None):        
+        return [row for row in self.iter_dicts(query, params, limit=limit, offset=offset)]
     
 
-    def list_paginated_dicts(self, query: str, params: list|dict = None, *, offset: int, limit: int):        
-        paginated_query, total_query = self.get_paginated_and_total_query(query, offset=offset, limit=limit)
+    def get_dicts_and_total(self, query: str, params: list|dict = None, *, limit: int, offset: int):
+        paginated_query, total_query = self.get_paginated_and_total_query(query, limit=limit, offset=offset)
 
-        rows = self.list_dicts(paginated_query, params)
+        rows = self.get_dicts(paginated_query, params)
         total = self.get_scalar(total_query, params)
         return {"rows": rows, "total": total}
 
     #endregion
 
 
-    #region Queries
-
-    def to_positional_params(self, query: str, params: dict) -> tuple[str, Sequence[Any]]:
-        from sqlparams import \
-            SQLParams  # not at the top because the enduser might not need this feature
-
-        if not hasattr(self.__class__, '_params_formatter'):
-            self.__class__._params_formatter = SQLParams('named', 'qmark')
-        query, params = self.__class__._params_formatter.format(query, params)
-
-        return query, params
-    
-    
-    def get_paginated_query(self, query: str, *, offset: int|None, limit: int|None) -> str:
-        paginated_query, _ = self.get_paginated_and_total_query(query, offset=offset, limit=limit)
-        return paginated_query
-    
-
-    def get_paginated_and_total_query(self, query: str, *, offset: int|None, limit: int|None) -> tuple[str,str]:
-        if offset is not None:
-            if isinstance(offset, str) and re.match(r"^[0-9]+$", offset):
-                offset = int(offset)
-            elif not isinstance(offset, int):
-                raise TypeError(f"invalid type for offset: {type(limit).__name__} (expected int)")
-        else:
-            offset = 0
-        
-        if limit is not None:
-            if isinstance(limit, str) and re.match(r"^[0-9]+$", limit):
-                limit = int(limit)
-            elif not isinstance(limit, int):
-                raise TypeError(f"invalid type for limit: {type(limit).__name__} (expected int)")
-        
-        beforepart, selectpart, orderpart = self._parse_select_query(query)
-
-        paginated_query = beforepart
-        total_query = beforepart
-        
-        paginated_query += self._paginate_parsed_query(selectpart, orderpart, offset=offset, limit=limit)
-        total_query += f"SELECT COUNT(*) FROM ({selectpart}) s"
-
-        return paginated_query, total_query
-    
-
-    def _parse_select_query(self, query: str):
-        import sqlparse  # not at the top because the enduser might not need this feature
-
-        # Parse SQL to remove token before the SELECT keyword
-        # example: WITH (CTE) tokens
-        statements = sqlparse.parse(query)
-        if len(statements) != 1:
-            raise ValueError(f"query contains {len(statements)} statements")
-
-        # Get first DML keyword
-        dml_keyword = None
-        dml_keyword_index = None
-        order_by_index = None
-        for i, token in enumerate(statements[0].tokens):
-            if token.ttype == sqlparse.tokens.DML:
-                if dml_keyword is None:
-                    dml_keyword = str(token).upper()
-                    dml_keyword_index = i
-            elif token.ttype == sqlparse.tokens.Keyword:
-                if order_by_index is None:
-                    keyword = str(token).upper()
-                    if keyword == "ORDER BY":
-                        order_by_index = i
-
-        # Check if the DML keyword is SELECT
-        if not dml_keyword:
-            raise ValueError(f"no SELECT found (query does not contain DML keyword)")
-        if dml_keyword != 'SELECT':
-            raise ValueError(f"first DML keyword is {dml_keyword}, expected SELECT")
-
-        # Get part before SELECT (example: WITH)
-        if dml_keyword_index > 0:
-            tokens = statements[0].tokens[:dml_keyword_index]
-            beforepart = ''.join(str(token) for token in tokens)
-        else:
-            beforepart = ''
-    
-        # Determine actual SELECT query
-        if order_by_index is not None:
-            tokens = statements[0].tokens[dml_keyword_index:order_by_index]
-            selectpart = ''.join(str(token) for token in tokens)
-            tokens = statements[0].tokens[order_by_index:]
-            orderpart = ''.join(str(token) for token in tokens)
-        else:
-            tokens = statements[0].tokens[dml_keyword_index:]
-            selectpart = ''.join(str(token) for token in tokens)
-            orderpart = ''
-
-        return beforepart, selectpart, orderpart
-    
-
-    def _paginate_parsed_query(self, selectpart: str, orderpart: str, *, offset: int, limit: int|None) -> str:
-        result = f"{selectpart} {orderpart}"
-        if offset > 0:
-            result += f" OFFSET {offset}"
-        if limit is not None:
-            result += f" LIMIT {limit}"
-        return result
-    
-
-    def get_select_table_query(self, table: str|tuple = None, *, schema_only = False) -> T_Composed:
-        """
-        Build a query on the given table.
-
-        If `schema_only` is given, no row will be returned (this is used to get information on the table).
-        Otherwise, all rows will be returned.
-
-        The return type of this function depends on the database engine.
-        It is passed directly to the cursor's execute function for this engine.
-        """
-        raise NotImplementedError()
-
-
-    def _get_composable_param(self, value) -> T_Composable:
-        if value is None:
-            return "null"
-        elif value == '__now__':
-            return "CURRENT_DATETIME()"
-        else:
-            return self._escape_literal(value)
-                
-
-    def _escape_identifier(self, value) -> T_Composable:
-        raise NotImplementedError()
-                
-
-    def _escape_literal(self, value) -> T_Composable:
-        raise NotImplementedError()
-    
-    #endregion
-    
-
     #region Tables and columns
 
     def split_name(self, name: str|tuple = None) -> tuple[str,str]:
         if name is None:
             if not self.table:
                 raise ValueError("No table given")
             return self.schema, self.table
@@ -592,23 +604,42 @@
         query = self.get_select_table_query(table, schema_only=True)
         with self.cursor() as cursor:
             self.execute_query(query, cursor=cursor)
             return self.get_cursor_columns(cursor)
         
 
     def _update_column_info(self, info: ColumnInfo, cursor: T_Cursor, index: int):
-        info.name = cursor.description[index]
+        info.name = cursor.description[index][0]
     
 
     def drop_table(self, table: str|tuple = None):
-        raise NotImplementedError()
+        schema, table = self.split_name(table)
+        
+        query = "DROP TABLE "
+            
+        if schema:    
+            query += f"{self.escape_identifier(schema)}."
+        query += f"{self.escape_identifier(table)}"
+
+        self.execute_query(query)
 
 
     def truncate_table(self, table: str|tuple = None, *, cascade: bool = False):
-        raise NotImplementedError()
+        schema, table = self.split_name(table)
+        
+        query = "TRUNCATE TABLE "
+            
+        if schema:    
+            query += f"{self.escape_identifier(schema)}."
+        query += f"{self.escape_identifier(table)}"
+
+        if cascade:
+            query += " CASCADE"
+
+        self.execute_query(query)
 
 
     def load_from_csv(self, file: os.PathLike|IOBase, table: str|tuple = None, *, columns: list[str] = None, encoding: str = 'utf-8', merge: Literal['truncate', 'truncate-cascade', 'upsert'] = None, noheaders: bool = False, csv_delimiter: str = None, csv_quotechar: str = None, csv_nullval: str = None) -> int:
         raise NotImplementedError()
    
 
     # endregion
@@ -626,14 +657,15 @@
 
 
 class ColumnInfo:
     def __init__(self, db: DbAdapter, cursor: T_Cursor, index: int):
         self.name = None
         self.python_type: type = None
         self.sql_type: str = None
+        self.sql_typecode: int = None
         self.nullable: bool = None
         db._update_column_info(self, cursor, index)
 
     def __str__(self):
         return self.name
     
     def __repr__(self):
```

## zut/db/mssql.py

```diff
@@ -1,31 +1,32 @@
 from __future__ import annotations
 
 import logging
+import os
 import re
 from contextlib import nullcontext
 from datetime import tzinfo
-from io import TextIOWrapper
+from io import IOBase, TextIOWrapper
 from pathlib import Path
 from urllib.parse import unquote, urlparse
 
-from .. import build_url, skip_utf8_bom
+from .. import OutTable, Literal, build_url, skip_utf8_bom, _get_csv_params
 from .base import ColumnInfo, DbAdapter
 
 logger = logging.getLogger(__name__)
 notice_logger = logging.getLogger("mssql")
 
 try:
     from pyodbc import Connection, Cursor, connect, drivers
 
     class MssqlAdapter(DbAdapter[Connection, Cursor, str, str]):
         """
         Database adapter for Microsoft SQL Server (using `pyodbc` driver).
         """
-        URL_SCHEME = 'mssql'
+        URL_SCHEME = 'mssql' # or mssqls (if encrypted)
         DEFAULT_SCHEMA = 'dbo'
         ONLY_POSITIONAL_PARAMS = True
         EXPECTED_CONNECTION_TYPES = ['pyodbc.Connection']
 
         @classmethod
         def is_available(cls):
             return True
@@ -72,15 +73,15 @@
             return build_url(scheme=self.URL_SCHEME, username=user, hostname=host, port=port, path='/'+dbname)
         
 
         # -------------------------------------------------------------------------
         # Execution
         #
         
-        def execute_file(self, path: str|Path, params: list|tuple|dict = None, *, cursor: Cursor = None, results: bool|TextIOWrapper|str|Path = False, tz: tzinfo = None, offset: int = None, limit: int = None, encoding: str = 'utf-8') -> None:
+        def execute_file(self, path: str|Path, params: list|tuple|dict = None, *, cursor: Cursor = None, results: bool|TextIOWrapper|OutTable|str|Path = False, tz: tzinfo = None, limit: int = None, offset: int = None, encoding: str = 'utf-8') -> None:
             import sqlparse  # not at the top because the enduser might not need this feature
 
             # Read file
             with open(path, 'r', encoding=encoding) as fp:
                 skip_utf8_bom(fp)
                 file_content = fp.read()
 
@@ -96,58 +97,58 @@
                         title = re.sub(r"\s+", " ", query).strip()[0:100] + "…"
                         logger.debug("Execute query %d/%d: %s ...", query_num, query_count, title)
 
                     # Execute query
                     query_id = f'{query_num}/{query_count}' if query_count > 1 else None
                     if query_num < query_count:
                         # Not last query: should not have results
-                        self.execute_query(query, params, cursor=_cursor, results='warning', tz=tz, query_id=query_id, offset=offset, limit=limit)
+                        self.execute_query(query, params, cursor=_cursor, results='warning', tz=tz, query_id=query_id, limit=limit, offset=offset)
 
                     else:
                         # Last query
-                        return self.execute_query(query, params, cursor=_cursor, results=results, tz=tz, query_id=query_id, offset=offset, limit=limit)
+                        return self.execute_query(query, params, cursor=_cursor, results=results, tz=tz, query_id=query_id, limit=limit, offset=offset)
 
 
         # -------------------------------------------------------------------------
         # Queries
         #
             
-        def _paginate_parsed_query(self, selectpart: str, orderpart: str, *, offset: int, limit: int|None) -> str:
+        def _paginate_parsed_query(self, selectpart: str, orderpart: str, *, limit: int|None, offset: int|None) -> str:
             if orderpart:
-                result = f"{selectpart} {orderpart} OFFSET {offset} ROWS"
+                result = f"{selectpart} {orderpart} OFFSET {offset or 0} ROWS"
                 if limit is not None:
                     result += f" FETCH NEXT {limit} ROWS ONLY"
                 return result
             elif limit is not None:
-                if offset > 0:
+                if offset is not None:
                     raise ValueError("an ORDER BY clause is required for OFFSET")
                 return f"SELECT TOP {limit} * FROM ({selectpart}) s"
             else:
                 return selectpart
 
 
         def get_select_table_query(self, table: str|tuple = None, *, schema_only = False) -> str:
             schema, table = self.split_name(table)
             
-            query = f'SELECT * FROM {self._escape_identifier(schema)}.{self._escape_identifier(table)}'
+            query = f'SELECT * FROM {self.escape_identifier(schema)}.{self.escape_identifier(table)}'
             if schema_only:
                 query += ' WHERE 1 = 0'
 
             return query
             
 
-        def _escape_identifier(self, value: str) -> str:
+        def escape_identifier(self, value: str) -> str:
             return f"[{value.replace(']', ']]')}]"
         
 
-        def _escape_literal(self, value: str) -> str:
+        def escape_literal(self, value: str) -> str:
             return f"'" + value.replace("'", "''") + "'"
 
 
-        def _log_cursor_messages(self, cursor: Cursor):
+        def _log_execute_messages(self, cursor: Cursor):
             if cursor.messages:
                 for msg_type, msg_text in cursor.messages:
                     m = re.match(r"^\[Microsoft\]\[ODBC Driver \d+ for SQL Server\]\[SQL Server\](.+)$", msg_text)
                     if m:
                         msg_text = m[1]
                     
                     if msg_type in {"[01000] (0)", "[01000] (50000)"}: # PRINT or RAISERROR
@@ -167,43 +168,100 @@
 
         def table_exists(self, table: str|tuple = None) -> bool:        
             schema, table = self.split_name(table)
 
             query = "SELECT CASE WHEN EXISTS(SELECT 1 FROM information_schema.tables WHERE table_schema = ? AND table_name = ?) THEN 1 ELSE 0 END"
             params = [schema, table]
 
-            return self.get_scalar(query, params)
-
-            
-        def drop_table(self, table: str|tuple = None):
-            schema, table = self.split_name(table)
-            query = "DROP TABLE %s.%s" % (schema, table)
-            self.execute_query(query)
+            return self.get_scalar(query, params) == 1
 
             
         def truncate_table(self, table: str|tuple = None, *, cascade: bool = False):
             if cascade:
-                raise ValueError("Cascade truncate not supported by mssql.")
-            schema, table = self.split_name(table)
-            query = "TRUNCATE TABLE %s.%s" % (schema, table)
-            self.execute_query(query)
+                raise ValueError("Cascade truncate is not supported by mssql.")
+            super().truncate_table(table)
             
 
         def _update_column_info(self, info: ColumnInfo, cursor: Cursor, index: int):
             info.name, info.python_type, display_size, internal_size, precision, scale, info.nullable = cursor.description[index]
 
+        #endregion
+
+
+        def load_from_csv(self, file: os.PathLike, table: str|tuple = None, *, columns: list[str] = None, encoding: str = 'utf-8', merge: Literal['truncate', 'truncate-cascade', 'upsert'] = None, noheaders: bool = False, csv_delimiter: str = None, csv_quotechar: str = None, csv_nullval: str = None) -> int:
+            if isinstance(file, IOBase):
+                # TODO: use named pipes?
+                raise NotImplementedError("Cannot use IOBase file with mssql.")
+            if columns or not noheaders:
+                # TODO: compare CSV headers with columns (check consistency) + use named pipes?
+                raise NotImplementedError("Arguments 'columns' or 'noheaders' cannot be used yet.")
+
+            sche, tab = self.split_name(table)
+            tmp_tab: str = None
+            key_columns: list[str] = []
+            nonkey_target_columns: list[str] = []
+
+            _, csv_delimiter, csv_quotechar, csv_nullval = _get_csv_params(None, csv_delimiter, csv_quotechar, csv_nullval, context=file)
+            if csv_nullval != '':
+                raise ValueError(f"Invalid csv nullval for mssql: \"{csv_nullval}\"")
+
+            try:
+                if merge in ['truncate', 'truncate-cascade']:                
+                    self.truncate_table((sche, tab), cascade=merge == 'truncate-cascade')
+
+                elif merge == 'upsert':
+                    raise NotImplementedError("Cannot use 'upsert' yet") #TODO
+
+                # Prepare actual copy operation
+                sql = f"BULK INSERT "
+                    
+                if tmp_tab:
+                    sql += f"{self.escape_identifier(tmp_tab)}"
+                else:    
+                    if sche:    
+                        sql +=f"{self.escape_identifier(sche)}."
+                    sql += f"{self.escape_identifier(tab)}"
+
+                sql += f" FROM {self.escape_literal(os.path.abspath(file))}"
+                sql += f' WITH ('
+                sql += f' CODEPAGE = {self.escape_literal('utf-8' if encoding == 'utf-8-sig' else encoding)}'
+                sql += f', FIELDTERMINATOR = {self.escape_literal(csv_delimiter)}'
+                sql += f', FIELDQUOTE = {self.escape_literal(csv_quotechar)}'
+                if csv_nullval == '':
+                    sql += f', KEEPNULLS'
+                sql += ")"
+
+                if tmp_tab:
+                    logger.debug("Actual copy from %s to %s", file, tmp_tab)
+                
+                #TODO: skip_utf8_bom(fp)
+                with self.cursor() as cursor:
+                    self.execute_query(sql)
+                    result_count = cursor.rowcount
+                
+                # Upsert from tmp table if necessary
+                if tmp_tab:
+                    pass #TODO
+
+                return result_count
+
+            finally:
+                if tmp_tab:
+                    self.execute_query(f"DROP TABLE IF EXISTS {self.escape_identifier(tmp_tab)}")
+
+
 
 except ImportError:  
 
     class MssqlAdapter(DbAdapter):
         """
         Database adapter for Microsoft SQL Server (using `pyodbc` driver).
         """
                 
-        URL_SCHEME = 'mssql'
+        URL_SCHEME = 'mssql' # or mssqls (if encrypted)
         DEFAULT_SCHEMA = 'dbo'
         ONLY_POSITIONAL_PARAMS = True
         EXPECTED_CONNECTION_TYPES = ['pyodbc.Connection']
 
         @classmethod
         def is_available(cls):
             return False
```

## zut/db/pg.py

```diff
@@ -131,18 +131,18 @@
         schema, name = self.split_name(name)
         
         query = "CALL "
         params = []
             
         if schema:    
             query +="{}."
-            params += [self._escape_identifier(schema)]
+            params += [self.escape_identifier(schema)]
 
         query += "{}"
-        params += [self._escape_identifier(name)]
+        params += [self.escape_identifier(name)]
 
         query += "(" + ", ".join(['{}'] * len(args)) + ")"
         params += [self._get_composable_param(arg) for arg in args]
 
         with self.cursor() as cursor:
             with self.register_notice_handler(if_exists=None, logprefix=f"pg:{schema + '.' if schema and schema != self.DEFAULT_SCHEMA else ''}{name}"):
                 cursor.execute(self._sql.SQL(query).format(*params))
@@ -161,18 +161,18 @@
         schema, table = self.split_name(table)
 
         query = "SELECT * FROM "
         params = []
             
         if schema:    
             query +="{}."
-            params += [self._escape_identifier(schema)]
+            params += [self.escape_identifier(schema)]
 
         query += "{}"
-        params += [self._escape_identifier(table)]
+        params += [self.escape_identifier(table)]
         
         if schema_only:
             query += ' WHERE false'
 
         return self._sql.SQL(query).format(*params)
 
 
@@ -180,22 +180,22 @@
         if value is None:
             return self._sql.SQL("null")
         elif value == '__now__':
             return self._sql.SQL("NOW()")
         elif isinstance(value, self._sql.Composable):
             return value
         else:
-            return self._escape_literal(value)
+            return self.escape_literal(value)
         
 
-    def _escape_identifier(self, value):
+    def escape_identifier(self, value):
         return self._sql.Identifier(value)
     
 
-    def _escape_literal(self, value):
+    def escape_literal(self, value):
         return self._sql.Literal(value)
     
     #endregion
     
 
     #region Schemas, tables and columns  
 
@@ -236,48 +236,46 @@
         schema, table = self.split_name(table)
         
         query = "DROP TABLE "
         params = []
             
         if schema:    
             query +="{}."
-            params += [self._escape_identifier(schema)]
+            params += [self.escape_identifier(schema)]
 
         query += "{}"
-        params += [self._escape_identifier(table)]
+        params += [self.escape_identifier(table)]
 
         self.execute_query(self._sql.SQL(query).format(*params))
         
 
     def truncate_table(self, table: str|tuple = None, *, cascade: bool = False):
         schema, table = self.split_name(table)
         
-        query = "TRUNCATE "
+        query = "TRUNCATE TABLE "
         params = []
             
         if schema:    
             query +="{}."
-            params += [self._escape_identifier(schema)]
+            params += [self.escape_identifier(schema)]
 
         query += "{}"
-        params += [self._escape_identifier(table)]
+        params += [self.escape_identifier(table)]
 
         if cascade:
             query += " CASCADE"
 
         self.execute_query(self._sql.SQL(query).format(*params))
 
 
     def _update_column_info(self, info: ColumnInfo, cursor, index: int):
-        info.name, type_oid, display_size, internal_size, precision, scale, always_none = cursor.description[index]
-        type_info = OID_CATALOG.get(type_oid)
+        info.name, info.sql_typecode, _display_size, _internal_size, _precision, _scale, _nullok_alwaysnone = cursor.description[index]
+        type_info = OID_CATALOG.get(info.sql_typecode)
         if type_info:
             info.sql_type, info.python_type = type_info
-        else:
-            info.sql_type = type_oid
     
     #endregion
 
 
     #region Copy
 
     def load_from_csv(self, file: os.PathLike|IOBase, table: str|tuple = None, *, columns: list[str] = None, encoding: str = 'utf-8', merge: Literal['truncate', 'truncate-cascade', 'upsert'] = None, noheaders: bool = False, csv_delimiter: str = None, csv_quotechar: str = None, csv_nullval: str = None) -> int:
@@ -362,41 +360,41 @@
                     logger.debug("Create temp table %s", tmp_tab)
                     self.execute_query(self._sql.SQL(sql).format(*params), cursor=cursor)
 
             # Prepare actual copy operation
             sql = "COPY "; params = []
                 
             if tmp_tab:
-                sql += "{}"; params += [self._escape_identifier(tmp_tab)]
+                sql += "{}"; params += [self.escape_identifier(tmp_tab)]
             else:    
                 if sche:    
-                    sql +="{}."; params += [self._escape_identifier(sche)]
-                sql += "{}"; params += [self._escape_identifier(tab)]
+                    sql +="{}."; params += [self.escape_identifier(sche)]
+                sql += "{}"; params += [self.escape_identifier(tab)]
 
             if columns:
                 sql += " ("
                 for i, colinfo in enumerate(columns):
-                    sql += (", " if i > 0 else "") + "{}"; params += [self._escape_identifier(colinfo)]
+                    sql += (", " if i > 0 else "") + "{}"; params += [self.escape_identifier(colinfo)]
                 sql += ")"
 
             sql += " FROM STDIN (FORMAT csv"
-            sql += ', ENCODING {}'; params.append('utf-8' if encoding == 'utf-8-sig' else self._escape_literal(encoding))
-            sql += ', DELIMITER {}'; params.append(self._escape_literal(csv_delimiter))
-            sql += ', QUOTE {}'; params.append(self._escape_literal(csv_quotechar))            
-            sql += ', ESCAPE {}'; params.append(self._escape_literal(csv_quotechar))
-            sql += ', NULL {}'; params.append(self._escape_literal(csv_nullval))
+            sql += ', ENCODING {}'; params.append('utf-8' if encoding == 'utf-8-sig' else self.escape_literal(encoding))
+            sql += ', DELIMITER {}'; params.append(self.escape_literal(csv_delimiter))
+            sql += ', QUOTE {}'; params.append(self.escape_literal(csv_quotechar))            
+            sql += ', ESCAPE {}'; params.append(self.escape_literal(csv_quotechar))
+            sql += ', NULL {}'; params.append(self.escape_literal(csv_nullval))
                 
             if not noheaders:
                 sql += ", HEADER match"
             sql += ")"
 
             with nullcontext(file) if isinstance(file, IOBase) else open(file, "rb") as fp:
                 skip_utf8_bom(fp)
                 if tmp_tab:
-                    logger.debug("actual copy from %s to %s", file, tmp_tab)
+                    logger.debug("Actual copy from %s to %s", file, tmp_tab)
                 result_count = self._actual_copy(self._sql.SQL(sql).format(*params), fp)
             
             # Upsert from tmp table if necessary
             if tmp_tab:
                 params = []
                 sql = "INSERT INTO {}.{} ("; params += [self._sql.Identifier(sche), self._sql.Identifier(tab)]
                 for i, colinfo in enumerate([*key_columns, *nonkey_target_columns]):
```

## Comparing `zut-0.9.0.dist-info/LICENSE.txt` & `zut-0.9.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `zut-0.9.0.dist-info/METADATA` & `zut-0.9.1.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zut
-Version: 0.9.0
+Version: 0.9.1
 Summary: Reusable Python utilities.
 Author-email: Sébastien Hocquet <dev@ipamo.net>
 Project-URL: Homepage, https://github.com/ipamo/zut
 Project-URL: Bug Tracker, https://github.com/ipamo/zut/issues
 Keywords: reusable,util,utils,common,commons,base,flexout,csv,excel,tabulate,smb,samba,share,out_table,out_file,db,DbAdapter
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -24,14 +24,17 @@
 Provides-Extra: excel
 Requires-Dist: openpyxl ; extra == 'excel'
 Requires-Dist: defusedxml ; extra == 'excel'
 Provides-Extra: mssql
 Requires-Dist: pyodbc ; extra == 'mssql'
 Requires-Dist: sqlparse ; extra == 'mssql'
 Requires-Dist: sqlparams ; extra == 'mssql'
+Provides-Extra: mysql
+Requires-Dist: mysqlclient ; extra == 'mysql'
+Requires-Dist: sqlparse ; extra == 'mysql'
 Provides-Extra: pg
 Requires-Dist: psycopg ; extra == 'pg'
 Requires-Dist: sqlparse ; extra == 'pg'
 Provides-Extra: smb
 Requires-Dist: smbprotocol ; extra == 'smb'
 Provides-Extra: systemd
 Requires-Dist: systemd-python ; (sys_platform == "linux") and extra == 'systemd'
```

