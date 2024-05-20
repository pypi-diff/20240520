# Comparing `tmp/salientsdk-0.1.6.tar.gz` & `tmp/salientsdk-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salientsdk-0.1.6.tar", max compression
+gzip compressed data, was "salientsdk-0.2.1.tar", max compression
```

## Comparing `salientsdk-0.1.6.tar` & `salientsdk-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,22 @@
--rw-r--r--   0        0        0     3611 2024-05-03 12:49:01.789628 salientsdk-0.1.6/docs/index.md
--rw-r--r--   0        0        0     7707 2024-05-03 12:49:01.793628 salientsdk-0.1.6/examples/downscale.ipynb
--rw-r--r--   0        0        0     7990 2024-05-03 12:49:01.793628 salientsdk-0.1.6/examples/hindcast_summary.ipynb
--rw-r--r--   0        0        0    32274 2024-05-03 12:49:01.793628 salientsdk-0.1.6/examples/ski.ipynb
--rw-r--r--   0        0        0     3006 2024-05-03 12:49:23.045599 salientsdk-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       27 2024-05-03 12:49:01.793628 salientsdk-0.1.6/salientsdk/.gitignore
--rw-r--r--   0        0        0     2022 2024-05-03 12:49:01.793628 salientsdk-0.1.6/salientsdk/__init__.py
--rw-r--r--   0        0        0    11106 2024-05-03 12:49:01.793628 salientsdk-0.1.6/salientsdk/__main__.py
--rw-r--r--   0        0        0      335 2024-05-03 12:49:01.793628 salientsdk-0.1.6/salientsdk/cli.py
--rw-r--r--   0        0        0     7531 2024-05-03 12:49:01.793628 salientsdk-0.1.6/salientsdk/constants.py
--rw-r--r--   0        0        0     7493 2024-05-03 12:49:01.793628 salientsdk-0.1.6/salientsdk/data_timeseries_api.py
--rw-r--r--   0        0        0     4619 2024-05-03 12:49:01.793628 salientsdk-0.1.6/salientsdk/downscale_api.py
--rw-r--r--   0        0        0     6431 2024-05-03 12:49:01.793628 salientsdk-0.1.6/salientsdk/forecast_timeseries_api.py
--rw-r--r--   0        0        0    12001 2024-05-03 12:49:01.793628 salientsdk-0.1.6/salientsdk/hindcast_summary_api.py
--rw-r--r--   0        0        0     6548 2024-05-03 12:49:01.793628 salientsdk-0.1.6/salientsdk/location.py
--rw-r--r--   0        0        0    11778 2024-05-03 12:49:01.797628 salientsdk-0.1.6/salientsdk/login_api.py
--rw-r--r--   0        0        0    13515 2024-05-03 12:49:01.797628 salientsdk-0.1.6/salientsdk/snow.py
--rw-r--r--   0        0        0     6214 2024-05-03 12:49:01.797628 salientsdk-0.1.6/salientsdk/upload_file_api.py
--rw-r--r--   0        0        0     4714 1970-01-01 00:00:00.000000 salientsdk-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      781 2024-05-20 12:18:08.253095 salientsdk-0.2.1/data/power_curves.csv
+-rw-r--r--   0        0        0     5089 2024-05-20 12:18:08.253095 salientsdk-0.2.1/docs/index.md
+-rw-r--r--   0        0        0     7707 2024-05-20 12:18:08.253095 salientsdk-0.2.1/examples/downscale.ipynb
+-rw-r--r--   0        0        0     7990 2024-05-20 12:18:08.253095 salientsdk-0.2.1/examples/hindcast_summary.ipynb
+-rw-r--r--   0        0        0    32286 2024-05-20 12:18:08.253095 salientsdk-0.2.1/examples/ski.ipynb
+-rw-r--r--   0        0        0    16487 2024-05-20 12:18:08.253095 salientsdk-0.2.1/examples/wind.ipynb
+-rw-r--r--   0        0        0     3106 2024-05-20 12:18:23.405014 salientsdk-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       27 2024-05-20 12:18:08.253095 salientsdk-0.2.1/salientsdk/.gitignore
+-rw-r--r--   0        0        0     2196 2024-05-20 12:18:08.253095 salientsdk-0.2.1/salientsdk/__init__.py
+-rw-r--r--   0        0        0    11106 2024-05-20 12:18:08.253095 salientsdk-0.2.1/salientsdk/__main__.py
+-rw-r--r--   0        0        0      324 2024-05-20 12:18:08.253095 salientsdk-0.2.1/salientsdk/cli.py
+-rw-r--r--   0        0        0     7515 2024-05-20 12:18:08.253095 salientsdk-0.2.1/salientsdk/constants.py
+-rw-r--r--   0        0        0     7880 2024-05-20 12:18:08.253095 salientsdk-0.2.1/salientsdk/data_timeseries_api.py
+-rw-r--r--   0        0        0     4589 2024-05-20 12:18:08.253095 salientsdk-0.2.1/salientsdk/downscale_api.py
+-rw-r--r--   0        0        0     6568 2024-05-20 12:18:08.257095 salientsdk-0.2.1/salientsdk/forecast_timeseries_api.py
+-rw-r--r--   0        0        0    12009 2024-05-20 12:18:08.257095 salientsdk-0.2.1/salientsdk/hindcast_summary_api.py
+-rw-r--r--   0        0        0    13567 2024-05-20 12:18:08.257095 salientsdk-0.2.1/salientsdk/hydro.py
+-rw-r--r--   0        0        0     6516 2024-05-20 12:18:08.257095 salientsdk-0.2.1/salientsdk/location.py
+-rw-r--r--   0        0        0    11616 2024-05-20 12:18:08.257095 salientsdk-0.2.1/salientsdk/login_api.py
+-rw-r--r--   0        0        0     6957 2024-05-20 12:18:08.257095 salientsdk-0.2.1/salientsdk/upload_file_api.py
+-rw-r--r--   0        0        0    11044 2024-05-20 12:18:08.257095 salientsdk-0.2.1/salientsdk/wind.py
+-rw-r--r--   0        0        0     6345 1970-01-01 00:00:00.000000 salientsdk-0.2.1/PKG-INFO
```

### Comparing `salientsdk-0.1.6/examples/downscale.ipynb` & `salientsdk-0.2.1/examples/downscale.ipynb`

 * *Files identical despite different names*

### Comparing `salientsdk-0.1.6/examples/hindcast_summary.ipynb` & `salientsdk-0.2.1/examples/hindcast_summary.ipynb`

 * *Files identical despite different names*

### Comparing `salientsdk-0.1.6/examples/ski.ipynb` & `salientsdk-0.2.1/examples/ski.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997834429824561%*

 * *Differences: {"'cells'": "{1: {'outputs': {0: {'data': {'text/plain': ['<requests.sessions.Session at "*

 * *            '0x7fdfce177bd0>\']}}}}, 10: {\'source\': {insert: [(1, \'    fcst["swe"] = '*

 * *            'sk.hydro.calc_swe(fcst, "time")\\n\'), (4, \'    hist["swe"] = '*

 * *            'sk.hydro.calc_swe(hist, "time")\\n\')], delete: [4, 1]}}}'}*

```diff
@@ -13,15 +13,15 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<requests.sessions.Session at 0x7f9fb3fe3810>"
+                            "<requests.sessions.Session at 0x7fdfce177bd0>"
                         ]
                     },
                     "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -416,18 +416,18 @@
                         "    swe      (time, location) float64 104kB 0.0 2.444 0.0 ... 0.0 248.8 425.3\n",
                         "    swe_avg  (location) float64 736B 6.142 125.1 4.767 ... 5.589 120.3 270.9\n"
                     ]
                 }
             ],
             "source": [
                 "if \"swe\" not in fcst:\n",
-                "    fcst[\"swe\"] = sk.calc_swe(fcst, \"time\")\n",
+                "    fcst[\"swe\"] = sk.hydro.calc_swe(fcst, \"time\")\n",
                 "\n",
                 "if \"swe\" not in hist:\n",
-                "    hist[\"swe\"] = sk.calc_swe(hist, \"time\")\n",
+                "    hist[\"swe\"] = sk.hydro.calc_swe(hist, \"time\")\n",
                 "\n",
                 "fcst[\"swe_avg\"] = fcst[\"swe\"].mean([\"ensemble\", \"time\"])\n",
                 "hist[\"swe_avg\"] = hist[\"swe\"].mean([\"time\"])\n",
                 "\n",
                 "print(\"Forecast -----\")\n",
                 "print(fcst.data_vars)\n",
                 "print(\"Historical ---\")\n",
```

### Comparing `salientsdk-0.1.6/pyproject.toml` & `salientsdk-0.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 [tool.poetry]
 name = "salientsdk"
-version = "0.1.6"
+version = "0.2.1"
 description = "Salient Predictions Software Development Kit"
 authors = ["Salient Predictions <help@salientpredictions.com>"]
 license = "LicenseRef-Custom"
 readme = "docs/index.md"
 keywords = ["weather","climate","forecasting","sdk","salient","s2s"]
 homepage = "https://salientpredictions.com"
 # Native doc at https://salient-predictions.github.io/salientsdk/
 # Redirect to sdk via CNAME at https://domains.google.com/registrar/salientpredictions.com/dns
 # Configure custom domain at https://github.com/Salient-Predictions/salientsdk/settings/pages
-documentation = "https://sdk.salientpredictions.com"
+documentation = "https://salient-predictions.github.io/salientsdk"
 repository = "https://github.com/Salient-Predictions/salientsdk"
-include = ["examples/*.ipynb"]
+include = ["examples/*.ipynb","data/*.csv"]
 
 [tool.poetry.urls]
 "License" = "https://sdk.salientpredictions.com/LICENSE/"
 
 
 [tool.poetry.dependencies]
 # use "poetry add <packagename>" to edit this list
+dask = "^2024.4.2"
+google = "^3.0.0"
+google-cloud-secret-manager = "^2.19.0"
 h5netcdf = "^1.3.0"
 netCDF4 = "^1.6.5"
+numpy = "^1.26.4"
 pandas = "^2.2.1"
 python = "^3.11"
 requests = "^2.31.0"
+scipy = "^1.13.0"
 toml = "^0.10.2"
 xarray = "^2024.2.0"
-numpy = "^1.26.4"
-dask = "^2024.4.2"
 
 [tool.poetry.group.dev.dependencies]
 # use "poetry add --dev <packagename>" to edit this list
-google = "^3.0.0"
-google-cloud-secret-manager = "^2.19.0"
 markdown-include = "^0.8.1"
 mkdocs = "^1.5.3"
 mkdocs-material = "^9.5.15"
 mkdocs-jupyter = "^0.24.6"
 mkdocs-glightbox = "^0.3.7"
+mkdocs-static-i18n = "^1.2.3"
 mkdocstrings = "^0.24.1"
 mkdocstrings-python = "^1.9.0"
 nbmake = "^1.5.3"
 pydoc-markdown = "^4.8.2"
 pytest = "^8.1.1"
 pytest-cov = "^5.0.0"
 ruff = "^0.3.4"
@@ -81,20 +83,19 @@
 
 # These are the ruff settings that are explicitly supplied to pre-commit for enforcement
 [tool.ruff]
 # Should match black
 line-length = 99
 # Assume Python 3.9
 target-version = "py39"
-
 # Currently enforce:
 # C90=mccabe-complexity
 # E722=do not use base except
 # Eventually add: F=pyflakes, E=pycodestyle, I=isort, W=pycodestyle warnings, N=pep8-naming, D=pydocstyle
-select = ["C90", "E722","D"]
+select = ["C90", "E722", "E9", "D", "F401", "W", "F7"]
 ignore = []
 
 [tool.ruff.mccabe]
 max-complexity = 25
 
 [tool.ruff.pydocstyle]
 convention = "google"
```

### Comparing `salientsdk-0.1.6/salientsdk/__init__.py` & `salientsdk-0.2.1/salientsdk/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #!/usr/bin/env python
 # Copyright Salient Predictions 2024
 
 """Salient Predictions Software Development Kit."""
 
-import os
 from importlib.metadata import PackageNotFoundError, version
 from pathlib import Path
 
 import toml
 
+from . import hydro  # noqa: F401 - users access .hydro functions via submodule
+from . import wind  # noqa: F401 - users access .wind functions via submodule
 from .constants import (
     get_file_destination,
     get_model_version,
     set_file_destination,
     set_model_version,
 )
 from .data_timeseries_api import data_timeseries, load_multihistory
@@ -23,16 +24,20 @@
 from .login_api import (
     get_current_session,
     get_verify_ssl,
     login,
     set_current_session,
     set_verify_ssl,
 )
-from .snow import calc_swe
-from .upload_file_api import upload_bounding_box, upload_file, upload_location_file
+from .upload_file_api import (
+    merge_location_data,
+    upload_bounding_box,
+    upload_file,
+    upload_location_file,
+)
 
 
 def _get_version(pkgname):
     pyproject_path = Path(__file__).resolve().parent.parent / "pyproject.toml"
     if pyproject_path.exists():
         pyproject_content = toml.load(pyproject_path)
         return pyproject_content["tool"]["poetry"]["version"]
@@ -45,26 +50,26 @@
             return "unknown"  # Development fallback
 
 
 __version__ = _get_version("salientsdk")
 __author__ = "Salient Predictions"
 __all__ = [
     "login",
-    "calc_swe",
     "data_timeseries",
     "downscale",
     "forecast_timeseries",
     "get_current_session",
     "set_file_destination",
     "get_model_version",
     "get_verify_ssl",
     "hindcast_summary",
     "transpose_hindcast_summary",
     "load_multihistory",
     "Location",
+    "merge_location_data",
     "set_current_session",
     "get_file_destination",
     "set_model_version",
     "set_verify_ssl",
     "upload_file",
     "upload_bounding_box",
     "upload_location_file",
```

### Comparing `salientsdk-0.1.6/salientsdk/__main__.py` & `salientsdk-0.2.1/salientsdk/__main__.py`

 * *Files identical despite different names*

### Comparing `salientsdk-0.1.6/salientsdk/constants.py` & `salientsdk-0.2.1/salientsdk/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 import datetime
 import hashlib
 import itertools
 import os
 import urllib
 
 import pandas as pd
-import requests
 
 # This is the base URL for the Salient API:
 URL = "https://api.salientpredictions.com/"
 
 API_VERSION = "v2"
 
 MODEL_VERSION = "v8"
```

### Comparing `salientsdk-0.1.6/salientsdk/data_timeseries_api.py` & `salientsdk-0.2.1/salientsdk/data_timeseries_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,25 +16,39 @@
 python -m salientsdk data_timeseries -lat 42 -lon -73 -fld all -var temp,precip -u username -p password
 # test with an apikey
 python -m salientsdk data_timeseries -lat 42 -lon -73 -fld anom --start 2020-01-01 --end 2020-12-31 --force --apikey testkey
 ```
 
 """
 
-import os
 
 import numpy as np
 import pandas as pd
 import requests
 import xarray as xr
 
 from .constants import _build_urls, _expand_comma
 from .location import Location
 from .login_api import download_queries
 
+HOURLY_VARIABLES = [
+    "cc",
+    "precip",
+    "sm",
+    "snow",
+    "st",
+    "temp",
+    "tsi",
+    "wdir",
+    "wdir100",
+    "wgst",
+    "wspd",
+    "wspd100",
+]
+
 
 def data_timeseries(
     # API inputs -------
     loc: Location,
     variable: str | list[str] = "temp",
     field: str = "anom",
     debias: bool = False,
@@ -106,21 +120,27 @@
         "stdv",
         "trend",
         "vals",
         "all",
     ], f"Invalid field {field}"
     assert format in ["nc", "csv"], f"Invalid format {format}"
     assert frequency in [
+        "hourly",
         "daily",
         "weekly",
         "monthly",
         "3-monthly",
     ], f"Invalid frequency {frequency}"
 
-    variable = _expand_comma(variable)
+    if field != "vals" and frequency == "hourly":
+        raise ValueError("Only field `vals` is available for hourly frequency")
+
+    variable = _expand_comma(
+        variable, HOURLY_VARIABLES if frequency == "hourly" else None, "variable"
+    )
 
     endpoint = "data_timeseries"
     args = loc.asdict(
         start=start,
         end=end,
         debias=debias,
         field=field,
```

### Comparing `salientsdk-0.1.6/salientsdk/downscale_api.py` & `salientsdk-0.2.1/salientsdk/downscale_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,19 +7,17 @@
 ```
 cd ~/salientsdk
 python -m salientsdk downscale -lat 42 -lon -73 --date 2020-01-01 -u username -p password --force
 ```
 
 """
 
-import os
 from datetime import datetime
 
 import requests
-import xarray as xr
 
 from .constants import _build_urls
 from .location import Location
 from .login_api import download_queries
 
 REFERENCE_CLIMS = ["30_yr", "10_yr", "5_yr"]
```

### Comparing `salientsdk-0.1.6/salientsdk/forecast_timeseries_api.py` & `salientsdk-0.2.1/salientsdk/forecast_timeseries_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,22 +14,19 @@
 python -m salientsdk forecast_timeseries -lat 42 -lon -73 --timescale seasonal -u username -p password
 # this will get multiple variables in separate files:
 python -m salientsdk forecast_timeseries -lat 42 -lon -73 -var temp,precip --timescale seasonal
 ```
 
 """
 
-import os
 from datetime import datetime
 
 import pandas as pd
 import requests
-import xarray as xr
 
-from . import login_api
 from .constants import _build_urls, _expand_comma
 from .location import Location
 from .login_api import download_queries
 
 FORECAST_VARIABLES = ["temp", "precip", "wspd", "tsi", "cdd", "hdd"]
 
 
@@ -85,15 +82,18 @@
         variable (str): The variable to query, defaults to `temp`
             To request multiple variables, separate them with a comma `temp,precip` or use a `list`.
             This will download one file per variable
             See the
             [Data Fields](https://salientpredictions.notion.site/Variables-d88463032846402e80c9c0972412fe60)
             documentation for a full list of available historical variables.
         version (str): The model version of the Salient `blend` forecast.
+            To request multiple versions, provide a list or comma-separated string.
+            `-default` calls `get_default_version()`.
         destination (str): The destination directory for downloaded files.
+            `-default` uses `get_file_destination()`
         force (bool): If False (default), don't download the data if it already exists
         session (requests.Session): The session object to use for the request
         apikey (str | None): The API key to use for the request.
             In most cases, this is not needed if a `session` is provided.
         verify (bool): If True (default), verify the SSL certificate.
             Defaults to use the value returned by `get_verify_ssl()`
         verbose (bool): If True (default False) print status messages
```

### Comparing `salientsdk-0.1.6/salientsdk/hindcast_summary_api.py` & `salientsdk-0.2.1/salientsdk/hindcast_summary_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,24 +17,19 @@
 # to request variables AND multiple seasons:
 python -m salientsdk hindcast_summary -lat 42 -lon -73 --variable temp,precip --season DJF,MAM
 
 ```
 
 """
 
-import hashlib
-import os
-from datetime import datetime
 
 import numpy as np
 import pandas as pd
 import requests
-import xarray as xr
 
-from . import login_api
 from .constants import _build_url, _build_urls, _expand_comma
 from .location import Location
 from .login_api import download_queries
 
 REFERENCE_VALUES = ["-auto", "ai", "clim", "gfs", "ecmwf", "blend", "norm_5yr", "norm_10yr"]
 METRIC_VALUES = ["rps", "mae", "crps", "rps_skill_score", "mae_skill_score", "crps_skill_score"]
 SEASON_VALUES = ["all", "DJF", "MAM", "JJA", "SON"]
@@ -88,15 +83,17 @@
             To request multiple variables, separate them with a comma `temp,precip` or use a list.
             This will download one file per variable
             See the
             [Data Fields](https://salientpredictions.notion.site/Variables-d88463032846402e80c9c0972412fe60)
             documentation for a full list of available historical variables.
         version (str | list[str]): The model version of the Salient `blend` forecast.
             To compare multiple versions, provide a list or comma-separated string.
+            `-default` calls `get_default_version()`.
         destination (str): The destination directory for downloaded files.
+            `-default` uses `get_file_destination()`
         force (bool): If False (default), don't download the data if it already exists
         session (requests.Session): The `Session` object to use for the request.
             Defaults to use get_current_session(), typically set during `login()`.
         apikey (str | None): The API key to use for the request.
             In most cases, this is not needed if a `session` is provided.
         verify (bool): Verify the SSL certificate.
             Defaults to use get_verify_ssl(), typically set during `login()`.
```

### Comparing `salientsdk-0.1.6/salientsdk/location.py` & `salientsdk-0.2.1/salientsdk/location.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 # Copyright Salient Predictions 2024
 
 """Define the Location class."""
 
 # Usage example:
 # python location.py --lat 42 --lon -73
 
-import argparse
-import datetime
 import os
 import urllib
 
 from . import constants, login_api
 
 
 class Location:
```

### Comparing `salientsdk-0.1.6/salientsdk/login_api.py` & `salientsdk-0.2.1/salientsdk/login_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,30 +10,22 @@
 # or, to use api keys:
 python -m salientsdk login --apikey testkey
 
 ```
 
 """
 
-import argparse
 import os
 from concurrent.futures import ThreadPoolExecutor
 
 import requests
+from google.cloud import secretmanager
 
 from .constants import _build_url
 
-try:
-    from google.cloud import secretmanager
-except ImportError as ie:
-    # secretmanager is a convenience for internal Salient users.
-    # Not needed for customer use.
-    pass
-
-
 VERIFY_SSL = True
 
 CURRENT_SESSION = None
 
 
 def _get_api_key(apikey: str | None = None) -> str | None:
     """Regularize API key values."""
```

### Comparing `salientsdk-0.1.6/salientsdk/snow.py` & `salientsdk-0.2.1/salientsdk/hydro.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-"""Snow accumulation model."""
+#!/usr/bin/env python
+# Copyright Salient Predictions 2024
+
+"""Hydro functions."""
 
 import numpy as np
 import pandas as pd
 import xarray as xr
 
 
 def calc_swe(met: xr.Dataset, timedim: str = "forecast_day") -> xr.DataArray:
```

### Comparing `salientsdk-0.1.6/salientsdk/upload_file_api.py` & `salientsdk-0.2.1/salientsdk/upload_file_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 """
 
 import json
 import os
 
 import pandas as pd
 import requests
+import xarray as xr
 
 from .constants import _build_url, get_file_destination
-from .login_api import download_query, get_current_session, get_verify_ssl
+from .login_api import download_query, get_current_session
 
 
 def upload_file(file: str, verbose: bool = True, session: requests.Session | None = None) -> None:
     """Uploads a geography file to the Salient API.
 
     An interface to to the Salient
     [upload_file](https://api.salientpredictions.com/v2/documentation/api/#/General/upload_file)
@@ -154,14 +155,35 @@
     loc_table.to_csv(geofile, index=False)
 
     upload_file(file=geofile, verbose=verbose, session=session)
 
     return geofile
 
 
+def merge_location_data(ds: xr.Dataset, loc_file: str):
+    """Merge additional data columns from a location_file into a dataset.
+
+    Will add any additional columns in `loc_file` to `ds`.
+
+    Args:
+        ds (xr.Dataset): A `Dataset` with a vector `location` coordinate
+        loc_file (str): Path to a CSV file containing location data.
+
+    Returns:
+        xr.Dataset: A new `Dataset` with the additional columns from `loc_file`
+            along the `location` coordinate.
+    """
+    geo = pd.read_csv(loc_file)
+    geo = geo.drop(columns=["lat", "lon"])
+    geo = geo.rename(columns={"name": "location"}).set_index("location")
+    geo = xr.Dataset.from_dataframe(geo)
+
+    return xr.merge([geo, ds], combine_attrs="override")
+
+
 def user_files(
     destination: str = "-default",
     session: requests.Session | None = None,
     verify: bool | None = None,
     verbose: bool = False,
 ) -> str:
     """List the files uploaded by the user.
```

### Comparing `salientsdk-0.1.6/PKG-INFO` & `salientsdk-0.2.1/docs/index.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,19 @@
-Metadata-Version: 2.1
-Name: salientsdk
-Version: 0.1.6
-Summary: Salient Predictions Software Development Kit
-Home-page: https://salientpredictions.com
-License: LicenseRef-Custom
-Keywords: weather,climate,forecasting,sdk,salient,s2s
-Author: Salient Predictions
-Author-email: help@salientpredictions.com
-Requires-Python: >=3.11,<4.0
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: dask (>=2024.4.2,<2025.0.0)
-Requires-Dist: h5netcdf (>=1.3.0,<2.0.0)
-Requires-Dist: netCDF4 (>=1.6.5,<2.0.0)
-Requires-Dist: numpy (>=1.26.4,<2.0.0)
-Requires-Dist: pandas (>=2.2.1,<3.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: toml (>=0.10.2,<0.11.0)
-Requires-Dist: xarray (>=2024.2.0,<2025.0.0)
-Project-URL: Documentation, https://sdk.salientpredictions.com
-Project-URL: License, https://sdk.salientpredictions.com/LICENSE/
-Project-URL: Repository, https://github.com/Salient-Predictions/salientsdk
-Description-Content-Type: text/markdown
+# Salient Predictions SDK
 
-
-# Intended Use
+## Intended Use
 
 The Salient SDK is a python convenience wrapper around Salient Predictions' customer-facing  
-[web API](https://api.salientpredictions.com/v2/documentation/api/).  It also contains utility functions for manipulating and analyzing the data delivered from the API.
+[web API](https://api.salientpredictions.com/v2/documentation/api/). It also contains utility functions for manipulating and analyzing the data delivered from the API.
 
-# Setting up the SDK
+## Setting up the SDK
 
-## Prerequisites 
+### Prerequisites
 
-The Salient SDK requires Python 3.11 to use.   If you have Python installed, you can check your version with:
+The Salient SDK requires Python 3.11 to use. If you have Python installed, you can check your version with:
 
 ```bash
 python3 --version
 ```
 
 To get version 3.11:
 
@@ -55,92 +29,112 @@
 ```bash
 # macOS:
 /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
 brew update
 brew install python@3.11
 ```
 
-## Installing the SDK
+### Installing the SDK
 
 The easiest way to get the Salient SDK is to install it like any other package:
 
 ```bash
 pip install salientsdk --upgrade
 # to verify version with
 pip show salientsdk
 ```
 
-# Usage
+## Usage
 
-## Command Line
+### Command Line
 
 The Salient SDK contains a full command line interface that can access each of the primary
-API functions without even opening python.  You can get help for all options or specific commands:
+API functions without even opening python. You can get help for all options or specific commands:
 
 ```bash
-python3 -m salientsdk --help
-python3 -m salientsdk forecast_timeseries --help
+# Show help for all available commands:
+salientsdk --help
+# Show help for one specific command:
+salientsdk forecast_timeseries --help
+# Get the version number:
+salientsdk version
 ```
 
-To verify that you are set up to execute the sdk, ask for its version number:
+To verify that you can access Salient's API, use the limited universal credentials `testusr` and `testpwd` to log in. If you see errors or warnings relating to `VERIFY SSL` you may need to adjust your firewall settings.
 
 ```bash
-python3 -m salientsdk version
+salientsdk login -u testusr -p testpwd
+# If successful, the command should return a Session object:
+<requests.sessions.Session object at 0x12cf45590>
 ```
 
-To verify that you can access Salient's API, use the limited universal credentials `testusr` and `testpwd` to log in:
+To verify that you can download data from Salient, try the `testusr/testpwd` credentials to download historical data with the `data_timeseries` function. This will download a NetCDF file to your current directory and display its contents.
 
 ```bash
-python3 -m salientsdk login -u testusr -p testpwd
+salientsdk data_timeseries -lat 42 -lon -73 -fld all --start 2020-01-01 --end 2020-12-31 -u testusr -p testpwd
 ```
 
-To verify that you can download data from Salient, try the `testusr/testpwd` credentials to download historical data with the `data_timeseries` function.  This will download a NetCDF file to your current directory and display its contents.
+To test that your specific Salient-issued credentials are functioning properly, try them with the `forecast_timeseries` function. Replace `username` and `password` in the example below with your credentials. Note that you may need to change the location (North America) and timescale (seasonal) if your license does not include them.
 
 ```bash
-python3 -m salientsdk data_timeseries -lat 42 -lon -73 -fld all --start 2020-01-01 --end 2020-12-31 -u testusr -p testpwd
+salientsdk forecast_timeseries -lat 42 -lon -73 --variable precip --timescale seasonal --date 2020-01-01 -u username -p "password"
 ```
 
-To test that your specific Salient-issued credentials are functioning properly, try them with the `forecast_timeseries` function.  Replace `username` and `password` in the example below with your credentials.  Note that you may need to change the location (North America) and timescale (seasonal) if your license does not include them.
+### Example Notebooks
+
+The package ships with examples that show `salientsdk` in action. You can list the file locations and copy them to a working directory for use. Let's work with the `hindcast_summary` notebook example:
 
-```bash
-python3 -m salientsdk forecast_timeseries -lat 42 -lon -73 --variable precip --timescale seasonal --date 2020-01-01 -u username -p password
+```
+mkdir salient_env && cd salient_env
+# show all of the available examples:
+salientsdk examples
+# Copy the "hindcast_summary" example to the current directory:
+salientsdk examples | grep "hindcast_summary" | xargs -I {} cp {} .
 ```
 
+`salientsdk` uses a dependency manager called `poetry` that can set up a virtual environment with all the dependencies you need to run the examples:
 
+```
+pip install poetry
+poetry init --no-interaction
+poetry add jupyter salientsdk
+poetry run ipython kernel install --user --name="salient_env"
+poetry run jupyter notebook
+```
+
+Once the notebook launches in your browser:
 
-## Via Python
+- Select "hindcast_summary.ipynb" from the file list
+- Kernel > Change Kernel > salient_env > Select
+- Add your username/password credentials to the "login" step in the first cell:<br>
+  `sk.login(<username>, <password>, verbose=False)`
+- The notebook assumes you are licenced for regions `north-america` and `europe`, and variables `temp` and `precip`. If you are not, change cell 2 to generate a request consistent with your licensing:<br>
+  `loc=sk.Location(region=["<region1>", "<region2>"]),`<br>
+  `variable=["<var1>", <var2>"],`
+- Run > Run All Cells
+- This will generate files in the `hindcast_summary_example` directory:<br>
+  `hindcast_summary_<hash>.csv` the source validation files from the API.<br>
+  `hindcast_summary_transposed.csv` a combined version of the results
+
+### Via Python
 
 In a python 3.11 script, this example code will login and request a historical ERA5 data timeseries.
 
 ```python
 import salientsdk as sk
 import xarray as xr
 import netcdf4
 
 session = sk.login("testusr","testpwd")
 history = sk.data_timeseries(loc = Location(lat=42, lon=-73), field="all", variable="temp", session=session)
 print(xr.open_file(history))
 ```
 
-Note that this example uses the limited credentials `testusr` and `testpwd`.  To access the full capabilities of your license, use your Salient-provided credentials.
+Note that this example uses the limited credentials `testusr` and `testpwd`. To access the full capabilities of your license, use your Salient-provided credentials.
 
 See all available functions in the [API Reference](api.md).
 
-# Examples
-
-
-The [examples](https://github.com/Salient-Predictions/salientsdk/tree/main/examples) directory contains `ipynb` notebooks to help you get started with common operations. 
-
-These examples are also included within the package. You can list their file locations with:
-
-```
-python3 -m salientsdk examples
-```
-
-
-# License
+## License
 
 This SDK is licensed for use by Salient customers [details](https://salient-predictions.github.io/salientsdk/LICENSE/).
 
-
 Copyright 2024 [Salient Predictions](https://www.salientpredictions.com/)
-
```

