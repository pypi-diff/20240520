# Comparing `tmp/brother_printer_fwupd-0.6.0.tar.gz` & `tmp/brother_printer_fwupd-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brother_printer_fwupd-0.6.0.tar", max compression
+gzip compressed data, was "brother_printer_fwupd-0.7.0.tar", max compression
```

## Comparing `brother_printer_fwupd-0.6.0.tar` & `brother_printer_fwupd-0.7.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35150 2019-05-05 22:45:01.929067 brother_printer_fwupd-0.6.0/LICENSE
--rw-r--r--   0        0        0     2543 2024-03-06 23:48:26.559435 brother_printer_fwupd-0.6.0/README.md
--rw-r--r--   0        0        0       75 2022-06-04 19:12:12.377682 brother_printer_fwupd-0.6.0/brother_printer_fwupd/__init__.py
--rwxr-xr-x   0        0        0     7982 2024-03-06 23:59:53.718039 brother_printer_fwupd-0.6.0/brother_printer_fwupd/__main__.py
--rw-r--r--   0        0        0     7358 2024-03-06 23:59:53.712039 brother_printer_fwupd-0.6.0/brother_printer_fwupd/autodiscover_printer.py
--rw-r--r--   0        0        0     6320 2024-03-06 23:59:53.681039 brother_printer_fwupd-0.6.0/brother_printer_fwupd/firmware_downloader.py
--rw-r--r--   0        0        0      746 2024-03-07 00:03:14.655049 brother_printer_fwupd-0.6.0/brother_printer_fwupd/firmware_uploader.py
--rw-r--r--   0        0        0     1755 2024-03-07 00:03:14.702048 brother_printer_fwupd-0.6.0/brother_printer_fwupd/models.py
--rw-r--r--   0        0        0     3049 2024-03-06 23:58:05.584576 brother_printer_fwupd-0.6.0/brother_printer_fwupd/snmp_info.py
--rw-r--r--   0        0        0     7313 2024-03-06 23:59:53.710039 brother_printer_fwupd-0.6.0/brother_printer_fwupd/utils.py
--rw-r--r--   0        0        0     1013 2024-03-07 00:04:59.973533 brother_printer_fwupd-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3588 1970-01-01 00:00:00.000000 brother_printer_fwupd-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    35150 2019-05-05 22:45:01.929067 brother_printer_fwupd-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2646 2024-05-20 20:35:50.754575 brother_printer_fwupd-0.7.0/README.md
+-rw-r--r--   0        0        0       75 2022-06-04 19:12:12.377682 brother_printer_fwupd-0.7.0/brother_printer_fwupd/__init__.py
+-rwxr-xr-x   0        0        0     8250 2024-05-20 20:36:02.381530 brother_printer_fwupd-0.7.0/brother_printer_fwupd/__main__.py
+-rw-r--r--   0        0        0     7380 2024-05-20 20:36:02.381530 brother_printer_fwupd-0.7.0/brother_printer_fwupd/autodiscover_printer.py
+-rw-r--r--   0        0        0     7071 2024-05-20 20:36:02.381530 brother_printer_fwupd-0.7.0/brother_printer_fwupd/firmware_downloader.py
+-rw-r--r--   0        0        0      849 2024-05-20 20:36:02.381530 brother_printer_fwupd-0.7.0/brother_printer_fwupd/firmware_uploader.py
+-rw-r--r--   0        0        0     1821 2024-05-20 20:36:02.381530 brother_printer_fwupd-0.7.0/brother_printer_fwupd/models.py
+-rw-r--r--   0        0        0     3049 2024-05-20 20:33:32.554098 brother_printer_fwupd-0.7.0/brother_printer_fwupd/snmp_info.py
+-rw-r--r--   0        0        0     7578 2024-05-20 20:36:02.381530 brother_printer_fwupd-0.7.0/brother_printer_fwupd/utils.py
+-rw-r--r--   0        0        0     1071 2024-05-20 20:36:23.124451 brother_printer_fwupd-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3846 1970-01-01 00:00:00.000000 brother_printer_fwupd-0.7.0/PKG-INFO
```

### Comparing `brother_printer_fwupd-0.6.0/LICENSE` & `brother_printer_fwupd-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `brother_printer_fwupd-0.6.0/README.md` & `brother_printer_fwupd-0.7.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -46,27 +46,33 @@
 - HL-5370DW
 - MFC-9142CDN
 - MFC-9332CDW
 - MFC-L3750CDW
 
 ## Usage
 
-### A: Install package using pip:
+### A: Run package using `pipx`:
+
+```shell
+pipx run brother-printer-fwupd
+```
+
+### B: Install package using `pip`:
 
 ```shell
 pip install --user --upgrade brother-printer-fwupd
 ```
 
 *If this does not work, try `pip install --user --upgrade brother_printer_fwupd`.*
 
-### B: Development installation:
+### C: Development installation:
 
 1. Clone the repo
 2. Install system dependencies: `libxslt-dev`, `libxml2-dev`
-3. `poetry install`
+3. `poetry install --extras autodiscover`
 4. `poetry run brother_printer_fwupd`
 
 Use at your own risk!™
 
 Contributions welcome.
 
 ## License
```

### Comparing `brother_printer_fwupd-0.6.0/brother_printer_fwupd/__main__.py` & `brother_printer_fwupd-0.7.0/brother_printer_fwupd/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,55 +2,65 @@
 """
 Script to update the firmware of some Brother printers (e. g. MFC).
 """
 
 import argparse
 import logging
 import sys
-import typing
 import webbrowser
 from pathlib import Path
+from typing import TYPE_CHECKING, Optional
 
 import termcolor
 
 from . import ISSUE_URL
-from .autodiscover_printer import PrinterDiscoverer
+
+try:
+    from .autodiscover_printer import PrinterDiscoverer
+except ImportError:
+    PrinterDiscoverer = None
+
 from .firmware_downloader import download_fw, get_download_url
 from .firmware_uploader import upload_fw
 from .models import FWInfo, SNMPPrinterInfo
 from .snmp_info import get_snmp_info
 from .utils import (
     CONSOLE_LOG_HANDLER,
     LOGGER,
     GitHubIssueReporter,
     get_running_os,
     gooey_if_exists,
 )
 
-if typing.TYPE_CHECKING:
+if TYPE_CHECKING:
     from .models import IPAddress
 
 
 RUNNING_OS = get_running_os()
 
 
 @gooey_if_exists
 def parse_args():
     """Parse command line args."""
     parser = argparse.ArgumentParser(
         prog=__file__,
         description=__doc__.strip().splitlines()[0],
     )
+    if PrinterDiscoverer:
+        blurb = "default: autodiscover via mdns"
+    else:
+        blurb = "required, because zeroconf is not available"
     parser.add_argument(
         "-p",
         "--printer",
+        required=not PrinterDiscoverer,
         dest="printer",
         metavar="host",
         default=None,
-        help="IP Address or hostname of the printer (default: autodiscover via mdns).",
+        help=f"IP Address or hostname of the printer ({blurb})).",
     )
     parser.add_argument(
         "--model",
         dest="model",
         type=str,
         help="Skip SNMP scanning by directly specifying the printer model.",
     )
@@ -67,15 +77,15 @@
         help="Skip SNMP scanning by directly specifying the printer spec.",
     )
     parser.add_argument(
         "--fw",
         "--fw-versions",
         dest="fw_versions",
         nargs="*",
-        default=list[FWInfo](),
+        default=[],  # In Python 3.10+: list[FWInfo]
         type=FWInfo.from_str,
         help="Skip SNMP scanning by directly specifying the firmware parts to update.",
     )
     parser.add_argument(
         "-c",
         "--community",
         dest="community",
@@ -162,16 +172,16 @@
     issue_reporter.set_context_data("--fw-dir", str(args.fw_dir))
     issue_reporter.set_context_data("--os", args.os)
     issue_reporter.set_context_data("--download-only", args.download_only)
     issue_reporter.set_context_data("--debug", args.debug)
 
     CONSOLE_LOG_HANDLER.setLevel(logging.DEBUG if args.debug else logging.INFO)
 
-    printer_ip: typing.Optional["IPAddress"] = args.printer
-    upload_port: int | None = None
+    printer_ip: Optional["IPAddress"] = args.printer
+    upload_port: Optional[int] = None
     use_snmp = (
         not args.model or not args.serial or not args.spec or not args.fw_versions
     )
     printer_ip_required = use_snmp or not args.download_only
 
     if not printer_ip and printer_ip_required:
         LOGGER.info("Discovering printer via MDNS.")
@@ -220,15 +230,15 @@
     LOGGER.success(
         "%s %s with following firmware version(s): %s",
         "Detected" if use_snmp else "Using",
         printer_info.model,
         versions_str,
     )
     LOGGER.info("Querying firmware download URL from Brother update API.")
-    download_url: str | None = None
+    download_url: Optional[str] = None
 
     for fw_part in printer_info.fw_versions:
         LOGGER.info("Try to get information for firmware part %s", fw_part)
 
         latest_version, download_url = get_download_url(
             printer_info=printer_info,
             firmid=str(fw_part.firmid),
```

### Comparing `brother_printer_fwupd-0.6.0/brother_printer_fwupd/autodiscover_printer.py` & `brother_printer_fwupd-0.7.0/brother_printer_fwupd/autodiscover_printer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Auto detect printer using zeroconf."""
 
 # pylint: disable=C0103
 # pylint: disable=R1723
 
 import ipaddress
 import typing
+from typing import List, Optional
 
 import termcolor
 import zeroconf
 
 from .models import MDNSPrinterInfo
 from .utils import LOGGER, clear_screen
 
@@ -17,19 +18,19 @@
 termcolor.ATTRIBUTES["italic"] = 3  # type: ignore
 
 
 class PrinterDiscoverer(zeroconf.ServiceListener):
     """Discoverer of printers."""
 
     def __init__(self) -> None:
-        self._printers: list[MDNSPrinterInfo] = list[MDNSPrinterInfo]()
+        self._printers: List[MDNSPrinterInfo] = []
         self._zc = zeroconf.Zeroconf()
         self._mode = "CLI"
         self._invalid_answer = False
-        self._browser: zeroconf.ServiceBrowser | None = None
+        self._browser: Optional[zeroconf.ServiceBrowser] = None
 
     def remove_service(self, zc: zeroconf.Zeroconf, type_: str, name: str):
         LOGGER.debug(f"Service {name} removed")
         self._remove_printer_infos_by_name(name)
 
         if self._mode == "CLI":
             self._update_screen()
@@ -181,18 +182,18 @@
                 "No printers found yet.", "yellow", attrs=["italic"], end=" "
             )
             termcolor.cprint(
                 "Run with --printer=<ip> to skip autodiscovery. [Enter: Cancel]",
                 attrs=["italic"],
             )
 
-    def run_cli(self) -> MDNSPrinterInfo | None:
+    def run_cli(self) -> Optional[MDNSPrinterInfo]:
         """Run as interactive terminal application."""
         self._mode = "CLI"
-        choice: int | None = None
+        choice: Optional[int] = None
         self._run()
         self._update_screen()
 
         try:
             while True:
                 inpt = input().strip()
```

### Comparing `brother_printer_fwupd-0.6.0/brother_printer_fwupd/firmware_downloader.py` & `brother_printer_fwupd-0.7.0/brother_printer_fwupd/firmware_downloader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Logic to download the correct firmware from the official Brother server."""
 
 import typing
 from copy import copy
 from pathlib import Path
+from typing import List, Optional, Tuple
 
 import requests
 from bs4 import BeautifulSoup, Tag
 
 from . import ISSUE_URL
 from .utils import LOGGER, sluggify
 
@@ -45,15 +46,15 @@
 )
 
 
 def get_download_url(
     printer_info: "SNMPPrinterInfo",
     reported_os: str,
     firmid: str = "MAIN",
-) -> tuple[str | None, str | None]:
+) -> Tuple[Optional[str], Optional[str]]:
     """
     Get the firmware download URL for the target printer.
 
     :return: Tuple of download latest version and URL.
     """
 
     api_request_data = copy(API_REQUEST_DATA_TEMPLATE)
@@ -71,21 +72,20 @@
         firm_info.append(Tag(name="ID", parser="xml"))
         firm_info.append(Tag(name="VERSION", parser="xml"))
         firm_info.ID.string = fw_info.firmid
         firm_info.VERSION.string = fw_info.firmver
 
         api_request_data.REQUESTINFO.FIRMUPDATEINFO.MODELINFO.FIRMINFO.append(firm_info)
 
-    errors: list[ValueError] = []
+    errors: List[ValueError] = []
 
-    for modification_callback in (copy, apply_mfc_l3750cdw_hack):
-        api_request_data = modification_callback(api_request_data)
+    for modification_callback in (copy, apply_driver_ews, apply_api_misspelling):
+        api_request_data_str = str(modification_callback(api_request_data))
 
         # curl -X POST -d @hl3040cn-update.xml -H "Content-Type:text/xml"
-        api_request_data_str = str(api_request_data)
         LOGGER.debug(
             "Sending POST request to %s with following content:\n%s",
             FW_UPDATE_URL,
             api_request_data_str,
         )
         resp = requests.post(
             FW_UPDATE_URL,
@@ -95,21 +95,21 @@
         resp.raise_for_status()
         LOGGER.debug("Response:\n%s", resp.text)
 
         try:
             return parse_response(response=resp.text, firmid=firmid)
         except ValueError as err:
             errors.append(err)
-            LOGGER.error(err)
+            LOGGER.warning(err)
             continue
 
     raise ExceptionGroup("Giving up fetching firmware.", errors)
 
 
-def parse_response(response: str, firmid: str) -> tuple[str | None, str | None]:
+def parse_response(response: str, firmid: str) -> Tuple[Optional[str], Optional[str]]:
     """
     Parse the API response and return a tuple of the latest version and the download URL.
     """
     resp_xml = BeautifulSoup(response, "xml")
 
     def select_one(name: str) -> str:
         tags = resp_xml.select(name)
@@ -145,37 +145,56 @@
     else:
         raise ValueError(
             f"Unknown value of 'versioncheck' in response for firmid={firmid}: '{resp_xml}'."
         )
 
     latest_version = select_one("LATESTVERSION")
     LOGGER.info(
-        "Firmware update for %s to version %s required.", firmid, latest_version
+        "Update for firmware part '%s' available (version '%s')", firmid, latest_version
     )
 
     firmid_val = select_one("FIRMID")
     if firmid_val != firmid:
         LOGGER.warning(
             "Request for firmid=%s was answered with firmid=%s. Be careful!",
             firmid,
             firmid_val,
         )
 
     return latest_version, select_one("PATH")
 
 
-def apply_mfc_l3750cdw_hack(data: BeautifulSoup) -> BeautifulSoup:
+def apply_driver_ews(data: BeautifulSoup) -> BeautifulSoup:
     """
-    Modify the request data in the way it is required for MFC-L3750CDW.
+    Modify the request data in the way it is required for MFC-L3750CDW, HL-L2360DW and others.
+
+    1. Remove `<SERIALNO>` / `<SELIALNO>`
+    2. Add "EWS" to `<DRIVER>`
+    See https://github.com/sedrubal/brother_printer_fwupd/issues/19#issuecomment-2079813638
+    """
+    LOGGER.info(
+        "Trying again without <SERIALNO> in API request but with <DRIVER>EWS</DRIVER>..."
+    )
+    data = copy(data)
+    data.REQUESTINFO.FIRMUPDATEINFO.MODELINFO.DRIVER.string = "EWS"
+    data.REQUESTINFO.FIRMUPDATEINFO.MODELINFO.SERIALNO.replace_with(
+        Tag(name="SELIALNO", parser="xml")
+    )
+    return data
+
+
+def apply_api_misspelling(data: BeautifulSoup) -> BeautifulSoup:
+    """
+    Another modification which works for MFC-L3750CDW, HL-L2360DW and others.
 
     1. Replace `<SERIALNO>` with typo `<SELIALNO>`
     2. Add "EWS" to `<DRIVER>`
     See https://github.com/sedrubal/brother_printer_fwupd/issues/19
     """
-    LOGGER.info("Retry with MFC-L3750CDW hack...")
+    LOGGER.info("Trying again with misspelling in API request...")
     data = copy(data)
     data.REQUESTINFO.FIRMUPDATEINFO.MODELINFO.DRIVER.string = "EWS"
     data.REQUESTINFO.FIRMUPDATEINFO.MODELINFO.SERIALNO.replace_with(
         Tag(name="SELIALNO", parser="xml")
     )
     return data
 
@@ -201,7 +220,8 @@
     with out_file.open("wb") as out:
         for chunk in resp.iter_content(chunk_size):
             size_written += out.write(chunk)
             progress = size_written / total_size * 100
             print(f"\r{progress: 5.1f} %", end="", flush=True)
 
     print()
+    return out_file
```

### Comparing `brother_printer_fwupd-0.6.0/brother_printer_fwupd/firmware_uploader.py` & `brother_printer_fwupd-0.7.0/brother_printer_fwupd/firmware_uploader.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 """Upload firmware to the brinter."""
 
 import socket
 from pathlib import Path
+from typing import Optional
 
 from .models import IPAddress
 
 PORT_SERVICE_NAME = "pdl-datastream"
 
 
 def upload_fw(
     target: IPAddress,
-    port: int | None,
+    port: Optional[int],
     fw_file_path: Path = Path("firmware.djf"),
 ):
     """
     Upload the firmware to the printer via PDL Datastream / JetDirect.
 
     Equals:
     ```
     cat LZ5413_P.djf | nc lp.local 9100
     ```
     """
-    port = port if port else socket.getservbyname(PORT_SERVICE_NAME)
+    if port is None:
+        try:
+            port = socket.getservbyname(PORT_SERVICE_NAME)
+        except OSError:
+            port = 9100
     addr_info = socket.getaddrinfo(str(target), port, 0, 0, socket.SOL_TCP)[0]
     with socket.socket(addr_info[0], addr_info[1], 0) as sock:
         sock.connect(addr_info[4])
 
         with fw_file_path.open("rb") as fw_file:
             sock.sendfile(fw_file)
```

### Comparing `brother_printer_fwupd-0.6.0/brother_printer_fwupd/snmp_info.py` & `brother_printer_fwupd-0.7.0/brother_printer_fwupd/snmp_info.py`

 * *Files identical despite different names*

### Comparing `brother_printer_fwupd-0.6.0/brother_printer_fwupd/utils.py` & `brother_printer_fwupd-0.7.0/brother_printer_fwupd/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,24 +7,30 @@
 import os
 import shlex
 import string
 import sys
 import traceback
 import typing
 from pathlib import Path
+from typing import Dict, List, Literal, Optional, Union
 from urllib.parse import urlencode
 
 import termcolor
 
 try:
     from gooey import Gooey
 except ImportError:
     Gooey = None
 
 
+ExceptionGroup = getattr(
+    __builtins__, "ExceptionGroup", None
+)  # will be None until Python 3.11
+
+
 def gooey_if_exists(func):
     """Make the app graphical, if gooey is installed."""
 
     if Gooey:
         return Gooey(func)
     else:
         return func
@@ -38,28 +44,30 @@
         handler_cb: typing.Callable[[str], None],
     ):
         self.logger = logger
         self.issue_url = issue_url
         self.handler_cb = handler_cb
         self._handler = logging.StreamHandler(stream=io.StringIO())
         self._handler.setLevel(logging.DEBUG)
-        self._context = dict[str, str | bool | list[str]]()
+
+        # In Python 3.10+: dict[str, str | bool | list[str]]()
+        self._context: Dict[str, str | bool | List[str]] = {}
 
     def __enter__(self):
         self._handler.stream.seek(0)
         self._handler.stream.truncate()
         self.logger.addHandler(self._handler)
 
         return self
 
     def __exit__(self, exc_class, exc, tb):
         if not exc_class or exc_class in (SystemExit, KeyboardInterrupt):
             return
 
-        if isinstance(exc, ExceptionGroup):
+        if ExceptionGroup and isinstance(exc, ExceptionGroup):
             LOGGER.error("%s  Errors:", exc.message)
             for err in exc.exceptions:
                 LOGGER.error("  - %s", err)
         else:
             LOGGER.error(exc)
         self.logger.removeHandler(self._handler)
         self._handler.stream.seek(0)
@@ -124,30 +132,32 @@
 """.strip(),
                 }
             )
         )
         self.handler_cb(report_url)
         sys.exit(1)
 
-    def set_context_data(self, key: str, value: str | bool | list[str]):
+    def set_context_data(self, key: str, value: Union[str, bool, List[str]]):
         self._context[key] = value
 
 
 def get_running_os() -> (
-    typing.Literal["WINDOWS"] | typing.Literal["MAC"] | typing.Literal["LINUX"]
+    Union[typing.Literal["WINDOWS"], typing.Literal["MAC"], typing.Literal["LINUX"]]
 ):
     if sys.platform.startswith("win") or sys.platform.startswith("cygwin"):
         return "WINDOWS"
     elif sys.platform.startswith("darwin"):
         return "MAC"
     else:
         return "LINUX"
 
 
-def add_logging_level(level_name: str, level_num: int, method_name: str | None = None):
+def add_logging_level(
+    level_name: str, level_num: int, method_name: Optional[str] = None
+):
     """
     Comprehensively adds a new logging level to the `logging` module and the
     currently configured logging class.
 
     `level_name` becomes an attribute of the `logging` module with the value
     `level_num`. `method_name` becomes a convenience method for both `logging`
     itself and the class returned by `logging.getLoggerClass()` (usually just
```

### Comparing `brother_printer_fwupd-0.6.0/pyproject.toml` & `brother_printer_fwupd-0.7.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "brother_printer_fwupd"
-version = "0.6.0"
+version = "0.7.0"
 description = "Script to update the firmware of some Brother printers (e. g. MFC)."
 authors = ["sedrubal <dev@sedrubal.de>"]
 repository = "https://github.com/sedrubal/brother_printer_fwupd.git"
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.9"
 pysnmp = "^4.4.12"
 pyasn1 = "^0.5.1"
 requests = "^2.31.0"
 BeautifulSoup4 = "^4.12.0"
 Gooey = { version = "^1.0.8", optional = true }
 lxml = "^4.9.0"
-zeroconf = "^0.28.8"
+zeroconf = { version = "^0.28.8", optional = true }
 termcolor = "^1.1.0"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.8.0"
 ruff = "^0.1.15"
 isort = "^5.13.0"
 pre-commit = "^3.6.0"
@@ -31,13 +31,14 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.extras]
 graphical = ["Gooey"]
+autodiscover = ["zeroconf"]
 
 [tool.poetry.scripts]
 brother_printer_fwupd = 'brother_printer_fwupd.__main__:main'
 
 [tool.ruff]
 line-length = 100
```

### Comparing `brother_printer_fwupd-0.6.0/PKG-INFO` & `brother_printer_fwupd-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: brother_printer_fwupd
-Version: 0.6.0
+Version: 0.7.0
 Summary: Script to update the firmware of some Brother printers (e. g. MFC).
 Home-page: https://github.com/sedrubal/brother_printer_fwupd.git
 License: GPL-3.0-or-later
 Author: sedrubal
 Author-email: dev@sedrubal.de
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: autodiscover
 Provides-Extra: graphical
 Requires-Dist: BeautifulSoup4 (>=4.12.0,<5.0.0)
 Requires-Dist: Gooey (>=1.0.8,<2.0.0) ; extra == "graphical"
 Requires-Dist: lxml (>=4.9.0,<5.0.0)
 Requires-Dist: pyasn1 (>=0.5.1,<0.6.0)
 Requires-Dist: pysnmp (>=4.4.12,<5.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: termcolor (>=1.1.0,<2.0.0)
-Requires-Dist: zeroconf (>=0.28.8,<0.29.0)
+Requires-Dist: zeroconf (>=0.28.8,<0.29.0) ; extra == "autodiscover"
 Project-URL: Repository, https://github.com/sedrubal/brother_printer_fwupd.git
 Description-Content-Type: text/markdown
 
 # Brother Printer Firmware Update Tool
 
 Script to update the firmware of some Brother printers (e.g. MFC).
 
@@ -71,27 +74,33 @@
 - HL-5370DW
 - MFC-9142CDN
 - MFC-9332CDW
 - MFC-L3750CDW
 
 ## Usage
 
-### A: Install package using pip:
+### A: Run package using `pipx`:
+
+```shell
+pipx run brother-printer-fwupd
+```
+
+### B: Install package using `pip`:
 
 ```shell
 pip install --user --upgrade brother-printer-fwupd
 ```
 
 *If this does not work, try `pip install --user --upgrade brother_printer_fwupd`.*
 
-### B: Development installation:
+### C: Development installation:
 
 1. Clone the repo
 2. Install system dependencies: `libxslt-dev`, `libxml2-dev`
-3. `poetry install`
+3. `poetry install --extras autodiscover`
 4. `poetry run brother_printer_fwupd`
 
 Use at your own risk!™
 
 Contributions welcome.
 
 ## License
```

