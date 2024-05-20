# Comparing `tmp/wled-0.8.0.tar.gz` & `tmp/wled-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wled-0.8.0.tar", max compression
+gzip compressed data, was "wled-0.9.0.tar", max compression
```

## Comparing `wled-0.8.0.tar` & `wled-0.9.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1077 2021-07-23 10:25:08.731161 wled-0.8.0/LICENSE.md
--rw-r--r--   0        0        0     5922 2021-07-23 10:25:08.731161 wled-0.8.0/README.md
--rw-r--r--   0        0        0     3020 2021-07-23 10:25:23.827172 wled-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      689 2021-07-23 10:25:08.731161 wled-0.8.0/src/wled/__init__.py
--rw-r--r--   0        0        0      462 2021-07-23 10:25:08.731161 wled-0.8.0/src/wled/exceptions.py
--rw-r--r--   0        0        0    17814 2021-07-23 10:25:08.731161 wled-0.8.0/src/wled/models.py
--rw-r--r--   0        0        0        0 2021-07-23 10:25:08.731161 wled-0.8.0/src/wled/py.typed
--rw-r--r--   0        0        0    21184 2021-07-23 10:25:08.731161 wled-0.8.0/src/wled/wled.py
--rw-r--r--   0        0        0     6858 2021-07-23 10:25:24.480490 wled-0.8.0/setup.py
--rw-r--r--   0        0        0     7103 2021-07-23 10:25:24.481232 wled-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2021-11-13 12:55:58.158731 wled-0.9.0/LICENSE.md
+-rw-r--r--   0        0        0     5922 2021-11-13 12:55:58.158731 wled-0.9.0/README.md
+-rw-r--r--   0        0        0     3066 2021-11-13 12:56:14.310733 wled-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      689 2021-11-13 12:55:58.158731 wled-0.9.0/src/wled/__init__.py
+-rw-r--r--   0        0        0      462 2021-11-13 12:55:58.162731 wled-0.9.0/src/wled/exceptions.py
+-rw-r--r--   0        0        0    18804 2021-11-13 12:55:58.162731 wled-0.9.0/src/wled/models.py
+-rw-r--r--   0        0        0        0 2021-11-13 12:55:58.162731 wled-0.9.0/src/wled/py.typed
+-rw-r--r--   0        0        0    21135 2021-11-13 12:55:58.162731 wled-0.9.0/src/wled/wled.py
+-rw-r--r--   0        0        0     6858 2021-11-13 12:56:14.899465 wled-0.9.0/setup.py
+-rw-r--r--   0        0        0     7154 2021-11-13 12:56:14.900036 wled-0.9.0/PKG-INFO
```

### Comparing `wled-0.8.0/LICENSE.md` & `wled-0.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `wled-0.8.0/README.md` & `wled-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `wled-0.8.0/pyproject.toml` & `wled-0.9.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wled"
-version = "0.8.0"
+version = "0.9.0"
 description = "Asynchronous Python client for WLED."
 authors = ["Franck Nijhof <opensource@frenck.dev>"]
 maintainers = ["Franck Nijhof <opensource@frenck.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/frenck/python-wled"
 repository = "https://github.com/frenck/python-wled"
@@ -13,14 +13,15 @@
 classifiers = [
   "Development Status :: 4 - Beta",
   "Framework :: AsyncIO",
   "Intended Audience :: Developers",
   "Natural Language :: English",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3",
   "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 packages = [
     { include = "wled", from = "src" },
 ]
 
@@ -28,38 +29,38 @@
 python = "^3.8"
 aiohttp = ">=3.0.0"
 yarl = ">=1.6.0"
 backoff = ">=1.9.0"
 
 [tool.poetry.dev-dependencies]
 aresponses = "^2.1.4"
-black = "^21.7b0"
-blacken-docs = "^1.10.0"
-coverage = {version = "^5.5", extras = ["toml"]}
-flake8 = "^3.8.4"
+black = "^21.10b0"
+blacken-docs = "^1.11.0"
+coverage = {version = "^6.1", extras = ["toml"]}
+flake8 = "^4.0.1"
 flake8-docstrings = "^1.5.0"
-isort = "^5.9.2"
+isort = "^5.10.1"
 mypy = "^0.910"
-pre-commit = "^2.11.1"
+pre-commit = "^2.15.0"
 pre-commit-hooks = "^4.0.1"
-pylint = "^2.9.5"
-pytest = "^6.2.2"
-pytest-asyncio = "^0.15.1"
-pytest-cov = "^2.11.1"
-yamllint = "^1.26.0"
-pyupgrade = "^2.21.2"
-flake8-simplify = "^0.14.0"
+pylint = "^2.11.1"
+pytest = "^6.2.5"
+pytest-asyncio = "^0.16.0"
+pytest-cov = "^3.0.0"
+yamllint = "^1.26.3"
+pyupgrade = "^2.29.0"
+flake8-simplify = "^0.14.2"
 vulture = "^2.3"
 flake8-bandit = "^2.1.2"
-flake8-bugbear = "^21.3.2"
+flake8-bugbear = "^21.9.2"
 flake8-builtins = "^1.5.3"
-flake8-comprehensions = "^3.3.1"
-flake8-eradicate = "^1.1.0"
-flake8-markdown = "^0.2.0"
-darglint = "^1.7.0"
+flake8-comprehensions = "^3.7.0"
+flake8-eradicate = "^1.2.0"
+flake8-markdown = "^0.3.0"
+darglint = "^1.8.1"
 safety = "^1.10.3"
 codespell = "^2.1.0"
 bandit = "^1.7.0"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/frenck/python-wled/issues"
 Changelog = "https://github.com/frenck/python-wled/releases"
```

### Comparing `wled-0.8.0/src/wled/__init__.py` & `wled-0.9.0/src/wled/__init__.py`

 * *Files identical despite different names*

### Comparing `wled-0.8.0/src/wled/models.py` & `wled-0.9.0/src/wled/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -252,22 +252,62 @@
             channel=wifi.get("channel", 0),
             rssi=wifi.get("rssi", 0),
             signal=wifi.get("signal", 0),
         )
 
 
 @dataclass
-class Info:
+class Filesystem:
+    """Object holding Filesystem information from WLED.
+
+    Args:
+        data: The data from the WLED device API.
+
+    Returns:
+        A Filesystem object.
+    """
+
+    total: int
+    used: int
+    free: int
+    percentage: int
+
+    @staticmethod
+    def from_dict(data: dict[str, Any]) -> Filesystem | None:
+        """Return Filesystem object form WLED API response.
+
+        Args:
+            data: The response from the WLED API.
+
+        Returns:
+            An Filesystem object.
+        """
+        if "fs" not in data:
+            return None
+        filesystem = data.get("fs", {})
+        total = filesystem.get("t", 1)
+        used = filesystem.get("u", 1)
+        return Filesystem(
+            total=total,
+            used=used,
+            free=(total - used),
+            percentage=round((used / total) * 100),
+        )
+
+
+@dataclass
+class Info:  # pylint: disable=too-many-instance-attributes
     """Object holding information from WLED."""
 
     architecture: str
     arduino_core_version: str
     brand: str
     build_type: str
     effect_count: int
+    filesystem: Filesystem | None
     free_heap: int
     leds: Leds
     live_ip: str
     live_mode: str
     live: bool
     mac_address: str
     name: str
@@ -286,24 +326,24 @@
 
         Args:
             data: The data from the WLED device API.
 
         Returns:
             A info object.
         """
-        websocket = data.get("ws")
-        if websocket == -1:
+        if (websocket := data.get("ws")) == -1:
             websocket = None
 
         return Info(
             architecture=data.get("arch", "Unknown"),
             arduino_core_version=data.get("core", "Unknown").replace("_", "."),
             brand=data.get("brand", "WLED"),
             build_type=data.get("btype", "Unknown"),
             effect_count=data.get("fxcount", 0),
+            filesystem=Filesystem.from_dict(data),
             free_heap=data.get("freeheap", 0),
             leds=Leds.from_dict(data),
             live_ip=data.get("lip", "Unknown"),
             live_mode=data.get("lm", "Unknown"),
             live=data.get("live", False),
             mac_address=data.get("mac", ""),
             name=data.get("name", "WLED Light"),
```

### Comparing `wled-0.8.0/src/wled/wled.py` & `wled-0.9.0/src/wled/wled.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Asynchronous Python client for WLED."""
 from __future__ import annotations
 
 import asyncio
 import json
 import socket
+from collections.abc import Callable
 from dataclasses import dataclass
-from typing import Any, Callable
+from typing import Any
 
 import aiohttp
 import async_timeout
 import backoff  # type: ignore
 from packaging import version
 from yarl import URL
 
@@ -221,16 +222,15 @@
         Returns:
             WLED Device data.
 
         Raises:
             WLEDEmptyResponseError: The WLED device returned an empty response.
         """
         if self._device is None or full_update:
-            data = await self.request("/json")
-            if not data:
+            if not (data := await self.request("/json")):
                 raise WLEDEmptyResponseError(
                     f"WLED device at {self.host} returned an empty API"
                     " response on full update"
                 )
 
             # Try to get presets, introduced in WLED 0.11
             try:
@@ -256,42 +256,38 @@
                     self._supports_si_request = True
                 except WLEDError:
                     self._supports_si_request = False
 
             return self._device
 
         if self._supports_presets:
-            presets = await self.request("/presets.json")
-            if not presets:
+            if not (presets := await self.request("/presets.json")):
                 raise WLEDEmptyResponseError(
                     f"WLED device at {self.host} returned an empty API"
                     " response on presets update"
                 )
             self._device.update_from_dict({"presets": presets})
 
         # Handle legacy state and update in separate requests
         if not self._supports_si_request:
-            info = await self.request("/json/info")
-            if not info:
+            if not (info := await self.request("/json/info")):
                 raise WLEDEmptyResponseError(
                     f"WLED device at {self.host} returned an empty API"
                     " response on info update"
                 )
 
-            state = await self.request("/json/state")
-            if not state:
+            if not (state := await self.request("/json/state")):
                 raise WLEDEmptyResponseError(
                     f"WLED device {self.host} returned an empty API"
                     " response on state update"
                 )
             self._device.update_from_dict({"info": info, "state": state})
             return self._device
 
-        state_info = await self.request("/json/si")
-        if not state_info:
+        if not (state_info := await self.request("/json/si")):
             raise WLEDEmptyResponseError(
                 f"WLED device at {self.host} returned an empty API"
                 " response on state & info update"
             )
         self._device.update_from_dict(state_info)
 
         return self._device
```

### Comparing `wled-0.8.0/setup.py` & `wled-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.0.0', 'backoff>=1.9.0', 'yarl>=1.6.0']
 
 setup_kwargs = {
     'name': 'wled',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Asynchronous Python client for WLED.',
     'long_description': '# Python: WLED API Client\n\n[![GitHub Release][releases-shield]][releases]\n[![Python Versions][python-versions-shield]][pypi]\n![Project Stage][project-stage-shield]\n![Project Maintenance][maintenance-shield]\n[![License][license-shield]](LICENSE.md)\n\n[![Build Status][build-shield]][build]\n[![Code Coverage][codecov-shield]][codecov]\n[![Code Quality][code-quality-shield]][code-quality]\n[![Deepcode.ai][deepcode-shield]][deepcode]\n\n[![Sponsor Frenck via GitHub Sponsors][github-sponsors-shield]][github-sponsors]\n\n[![Support Frenck on Patreon][patreon-shield]][patreon]\n\nAsynchronous Python client for WLED.\n\n## About\n\nThis package allows you to control and monitor an WLED device\nprogrammatically. It is mainly created to allow third-party programs to automate\nthe behavior of WLED.\n\n## Installation\n\n```bash\npip install wled\n```\n\n## Usage\n\n```python\nimport asyncio\n\nfrom wled import WLED\n\n\nasync def main():\n    """Show example on controlling your WLED device."""\n    async with WLED("wled-frenck.local") as led:\n        device = await led.update()\n        print(device.info.version)\n\n        # Turn strip on, full brightness\n        await led.light(on=True, brightness=255)\n\n\nif __name__ == "__main__":\n    loop = asyncio.get_event_loop()\n    loop.run_until_complete(main())\n```\n\n## Changelog & Releases\n\nThis repository keeps a change log using [GitHub\'s releases][releases]\nfunctionality.\n\nReleases are based on [Semantic Versioning][semver], and use the format\nof `MAJOR.MINOR.PATCH`. In a nutshell, the version will be incremented\nbased on the following:\n\n- `MAJOR`: Incompatible or major changes.\n- `MINOR`: Backwards-compatible new features and enhancements.\n- `PATCH`: Backwards-compatible bugfixes and package updates.\n\n## Contributing\n\nThis is an active open-source project. We are always open to people who want to\nuse the code or contribute to it.\n\nWe\'ve set up a separate document for our\n[contribution guidelines](CONTRIBUTING.md).\n\nThank you for being involved! :heart_eyes:\n\n## Setting up development environment\n\nThis Python project is fully managed using the [Poetry][poetry] dependency\nmanager. But also relies on the use of NodeJS for certain checks during\ndevelopment.\n\nYou need at least:\n\n- Python 3.8+\n- [Poetry][poetry-install]\n- NodeJS 12+ (including NPM)\n\nTo install all packages, including all development requirements:\n\n```bash\nnpm install\npoetry install\n```\n\nAs this repository uses the [pre-commit][pre-commit] framework, all changes\nare linted and tested with each commit. You can run all checks and tests\nmanually, using the following command:\n\n```bash\npoetry run pre-commit run --all-files\n```\n\nTo run just the Python tests:\n\n```bash\npoetry run pytest\n```\n\n## Authors & contributors\n\nThe original setup of this repository is by [Franck Nijhof][frenck].\n\nFor a full list of all authors and contributors,\ncheck [the contributor\'s page][contributors].\n\n## License\n\nMIT License\n\nCopyright (c) 2019-2021 Franck Nijhof\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the "Software"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n\n[build-shield]: https://github.com/frenck/python-wled/actions/workflows/tests.yaml/badge.svg\n[build]: https://github.com/frenck/python-wled/actions/workflows/tests.yaml\n[code-quality-shield]: https://img.shields.io/lgtm/grade/python/g/frenck/python-wled.svg?logo=lgtm&logoWidth=18\n[code-quality]: https://lgtm.com/projects/g/frenck/python-wled/context:python\n[codecov-shield]: https://codecov.io/gh/frenck/python-wled/branch/master/graph/badge.svg\n[codecov]: https://codecov.io/gh/frenck/python-wled\n[contributors]: https://github.com/frenck/python-wled/graphs/contributors\n[deepcode-shield]: https://www.deepcode.ai/api/gh/badge?key=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJwbGF0Zm9ybTEiOiJnaCIsIm93bmVyMSI6ImZyZW5jayIsInJlcG8xIjoicHl0aG9uLWVsZ2F0byIsImluY2x1ZGVMaW50IjpmYWxzZSwiYXV0aG9ySWQiOjI4MDU1LCJpYXQiOjE2MTUxODgzODh9.hJsD6PTw8K8bnTmHUzroQi7XkXRi46bdt-oMqx2zXj0\n[deepcode]: https://www.deepcode.ai/app/gh/frenck/python-wled/_/dashboard?utm_content=gh%2Ffrenck%2Fpython-wled\n[frenck]: https://github.com/frenck\n[github-sponsors-shield]: https://frenck.dev/wp-content/uploads/2019/12/github_sponsor.png\n[github-sponsors]: https://github.com/sponsors/frenck\n[license-shield]: https://img.shields.io/github/license/frenck/python-wled.svg\n[maintenance-shield]: https://img.shields.io/maintenance/yes/2021.svg\n[patreon-shield]: https://frenck.dev/wp-content/uploads/2019/12/patreon.png\n[patreon]: https://www.patreon.com/frenck\n[poetry-install]: https://python-poetry.org/docs/#installation\n[poetry]: https://python-poetry.org\n[pre-commit]: https://pre-commit.com/\n[project-stage-shield]: https://img.shields.io/badge/project%20stage-experimental-yellow.svg\n[pypi]: https://pypi.org/project/wled/\n[python-versions-shield]: https://img.shields.io/pypi/pyversions/wled\n[releases-shield]: https://img.shields.io/github/release/frenck/python-wled.svg\n[releases]: https://github.com/frenck/python-wled/releases\n[semver]: http://semver.org/spec/v2.0.0.html\n',
     'author': 'Franck Nijhof',
     'author_email': 'opensource@frenck.dev',
     'maintainer': 'Franck Nijhof',
     'maintainer_email': 'opensource@frenck.dev',
     'url': 'https://github.com/frenck/python-wled',
```

### Comparing `wled-0.8.0/PKG-INFO` & `wled-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wled
-Version: 0.8.0
+Version: 0.9.0
 Summary: Asynchronous Python client for WLED.
 Home-page: https://github.com/frenck/python-wled
 License: MIT
 Keywords: wled,api,async,client
 Author: Franck Nijhof
 Author-email: opensource@frenck.dev
 Maintainer: Franck Nijhof
@@ -12,14 +12,15 @@
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aiohttp (>=3.0.0)
 Requires-Dist: backoff (>=1.9.0)
 Requires-Dist: yarl (>=1.6.0)
 Project-URL: Bug Tracker, https://github.com/frenck/python-wled/issues
```

