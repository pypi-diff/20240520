# Comparing `tmp/migmose-0.0.0.tar.gz` & `tmp/migmose-0.1.0.tar.gz`

## Comparing `migmose-0.0.0.tar` & `migmose-0.1.0.tar`

### file list

```diff
@@ -1,44 +1,45 @@
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 migmose-0.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 migmose-0.0.0/README.md
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 migmose-0.0.0/domain-specific-terms.txt
--rw-r--r--   0        0        0   381008 2020-02-02 00:00:00.000000 migmose-0.0.0/migmose-logo.jpeg
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 migmose-0.0.0/requirements.txt
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 migmose-0.0.0/tox.ini
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 migmose-0.0.0/.github/dependabot.yml
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 migmose-0.0.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 migmose-0.0.0/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 migmose-0.0.0/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 migmose-0.0.0/.github/workflows/dev_test.yml
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 migmose-0.0.0/.github/workflows/formatting.yml
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 migmose-0.0.0/.github/workflows/no_byte_order_mark.yml
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 migmose-0.0.0/.github/workflows/packaging_test.yml
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 migmose-0.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 migmose-0.0.0/.github/workflows/pythonlint.yml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 migmose-0.0.0/.github/workflows/unittests.yml
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 migmose-0.0.0/dev_requirements/requirements-coverage.in
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 migmose-0.0.0/dev_requirements/requirements-coverage.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 migmose-0.0.0/dev_requirements/requirements-formatting.in
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 migmose-0.0.0/dev_requirements/requirements-formatting.txt
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 migmose-0.0.0/dev_requirements/requirements-linting.in
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 migmose-0.0.0/dev_requirements/requirements-linting.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 migmose-0.0.0/dev_requirements/requirements-packaging.in
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 migmose-0.0.0/dev_requirements/requirements-packaging.txt
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 migmose-0.0.0/dev_requirements/requirements-spell_check.in
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 migmose-0.0.0/dev_requirements/requirements-spell_check.txt
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 migmose-0.0.0/dev_requirements/requirements-tests.in
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 migmose-0.0.0/dev_requirements/requirements-tests.txt
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 migmose-0.0.0/dev_requirements/requirements-type_check.in
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 migmose-0.0.0/dev_requirements/requirements-type_check.txt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 migmose-0.0.0/src/_migmose_version.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 migmose-0.0.0/src/migmose/__init__.py
--rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 migmose-0.0.0/src/migmose/__main__.py
--rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 migmose-0.0.0/src/migmose/parsing.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 migmose-0.0.0/src/migmose/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 migmose-0.0.0/src/migmose/mig/__init__.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 migmose-0.0.0/src/migmose/mig/nachrichtenstrukturtabelle.py
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 migmose-0.0.0/src/migmose/mig/nachrichtenstrukturzeile.py
--rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 migmose-0.0.0/src/migmose/mig/nestednachrichtenstruktur.py
--rw-r--r--   0        0        0     6403 2020-02-02 00:00:00.000000 migmose-0.0.0/src/migmose/mig/reducednestednachrichtenstruktur.py
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 migmose-0.0.0/.gitignore
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 migmose-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 migmose-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 migmose-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     4271 2020-02-02 00:00:00.000000 migmose-0.1.0/README.md
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 migmose-0.1.0/domain-specific-terms.txt
+-rw-r--r--   0        0        0   381008 2020-02-02 00:00:00.000000 migmose-0.1.0/migmose-logo.jpeg
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 migmose-0.1.0/requirements.txt
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 migmose-0.1.0/tox.ini
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 migmose-0.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 migmose-0.1.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 migmose-0.1.0/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 migmose-0.1.0/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 migmose-0.1.0/.github/workflows/dev_test.yml
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 migmose-0.1.0/.github/workflows/formatting.yml
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 migmose-0.1.0/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 migmose-0.1.0/.github/workflows/packaging_test.yml
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 migmose-0.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 migmose-0.1.0/.github/workflows/pythonlint.yml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 migmose-0.1.0/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 migmose-0.1.0/dev_requirements/requirements-coverage.in
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 migmose-0.1.0/dev_requirements/requirements-coverage.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 migmose-0.1.0/dev_requirements/requirements-formatting.in
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 migmose-0.1.0/dev_requirements/requirements-formatting.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 migmose-0.1.0/dev_requirements/requirements-linting.in
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 migmose-0.1.0/dev_requirements/requirements-linting.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 migmose-0.1.0/dev_requirements/requirements-packaging.in
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 migmose-0.1.0/dev_requirements/requirements-packaging.txt
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 migmose-0.1.0/dev_requirements/requirements-spell_check.in
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 migmose-0.1.0/dev_requirements/requirements-spell_check.txt
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 migmose-0.1.0/dev_requirements/requirements-tests.in
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 migmose-0.1.0/dev_requirements/requirements-tests.txt
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 migmose-0.1.0/dev_requirements/requirements-type_check.in
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 migmose-0.1.0/dev_requirements/requirements-type_check.txt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 migmose-0.1.0/src/_migmose_version.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 migmose-0.1.0/src/migmose/__init__.py
+-rw-r--r--   0        0        0     5137 2020-02-02 00:00:00.000000 migmose-0.1.0/src/migmose/__main__.py
+-rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 migmose-0.1.0/src/migmose/parsing.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 migmose-0.1.0/src/migmose/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 migmose-0.1.0/src/migmose/mig/__init__.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 migmose-0.1.0/src/migmose/mig/nachrichtenstrukturtabelle.py
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 migmose-0.1.0/src/migmose/mig/nachrichtenstrukturzeile.py
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 migmose-0.1.0/src/migmose/mig/nestednachrichtenstruktur.py
+-rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 migmose-0.1.0/src/migmose/mig/reducednestednachrichtenstruktur.py
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 migmose-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 migmose-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 migmose-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 migmose-0.1.0/PKG-INFO
```

### Comparing `migmose-0.0.0/.pre-commit-config.yaml` & `migmose-0.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `migmose-0.0.0/README.md` & `migmose-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 ![migmose-logo](migmose-logo.jpeg)
 
 # MIG_mose
 
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
+![Python Versions (officially) supported](https://img.shields.io/pypi/pyversions/migmose.svg)
+![Pypi status badge](https://img.shields.io/pypi/v/migmose)
 ![Unittests status badge](https://github.com/Hochfrequenz/migmose/workflows/Unittests/badge.svg)
 ![Coverage status badge](https://github.com/Hochfrequenz/migmose/workflows/Coverage/badge.svg)
 ![Linting status badge](https://github.com/Hochfrequenz/migmose/workflows/Linting/badge.svg)
 ![Black status badge](https://github.com/Hochfrequenz/migmose/workflows/Formatting/badge.svg)
 
 MIG_mose generates machine-readable files from MIG documents ([edi-energy](https://www.edi-energy.de/index.php?id=38)).
 MIG_mose is the sister of [kohlrahbi](https://github.com/Hochfrequenz/kohlrahbi).
@@ -15,18 +18,18 @@
 - .docx files a processed by the [python-docx](https://python-docx.readthedocs.io/en/latest/) library.
 - EdiFact formats are used as in [maus.edifact](https://github.com/Hochfrequenz/mig_ahb_utility_stack/blob/main/src/maus/edifact.py).
 
 This is at the moment a MWE (Minimum Working Example) and will be extended in the future.
 See below for an overview of its features.
 
 ## Installation
-MIG_mose is a Python based tool.
-Therefore you have to make sure, that Python is running on your machine.
+MIG_mose is a Python-based tool.
+Therefore, you have to make sure, that Python is running on your machine.
 
-We recommend to use virtual environments to keep your system clean.
+We recommend using virtual environments to keep your system clean.
 
 Create a new virtual environment with
 ```bash
 python -m venv .venv
 ```
 
 The activation of the virtual environment depends on your used OS.
@@ -40,14 +43,15 @@
 source .venv/bin/activate
 ```
 Finally, install the package with
 
 ```bash
 pip install migmose
 ```
+
 ## Features And How To Use Them
 
 At this point, MIG_mose works as a command-line interface tool (CLI).
 There are several flags available to provide a user-friendly way to interact with MIG_mose.
 Below the available options are listed:
 
 - **Input Directory (`-i`, `--input-dir`):**
```

### Comparing `migmose-0.0.0/migmose-logo.jpeg` & `migmose-0.1.0/migmose-logo.jpeg`

 * *Files identical despite different names*

### Comparing `migmose-0.0.0/requirements.txt` & `migmose-0.1.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `migmose-0.0.0/tox.ini` & `migmose-0.1.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 [testenv:type_check]
 # the type_check environment checks the type hints using mypy
 setenv = PYTHONPATH = {toxinidir}/src
 deps =
     {[testenv:tests]deps}
     -r dev_requirements/requirements-type_check.txt
 commands =
-    mypy --show-error-codes src/migmose
+    mypy --show-error-codes src/migmose --strict
     mypy --show-error-codes unittests
     # add single files (ending with .py) or packages here
 
 [testenv:spell_check]
 # the spellcheck environment checks the code for typos
 setenv = PYTHONPATH = {toxinidir}/src
 deps =
@@ -79,15 +79,14 @@
     {[testenv:coverage]deps}
     {[testenv:spell_check]deps}
     -r dev_requirements/requirements-formatting.txt
     pip-tools
     pre-commit
 commands =
     python -m pip install --upgrade pip
-    pip-compile pyproject.toml
     pip install -r requirements.txt
     pre-commit install
 
 [testenv:test_packaging]
 skip_install = true
 deps =
     -r dev_requirements/requirements-packaging.txt
```

### Comparing `migmose-0.0.0/.github/dependabot.yml` & `migmose-0.1.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `migmose-0.0.0/.github/workflows/codeql-analysis.yml` & `migmose-0.1.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `migmose-0.0.0/.github/workflows/coverage.yml` & `migmose-0.1.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `migmose-0.0.0/.github/workflows/dependabot_automerge.yml` & `migmose-0.1.0/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `migmose-0.0.0/.github/workflows/dev_test.yml` & `migmose-0.1.0/.github/workflows/dev_test.yml`

 * *Files identical despite different names*

### Comparing `migmose-0.0.0/.github/workflows/formatting.yml` & `migmose-0.1.0/.github/workflows/formatting.yml`

 * *Files identical despite different names*

### Comparing `migmose-0.0.0/.github/workflows/packaging_test.yml` & `migmose-0.1.0/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `migmose-0.0.0/.github/workflows/python-publish.yml` & `migmose-0.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `migmose-0.0.0/.github/workflows/pythonlint.yml` & `migmose-0.1.0/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `migmose-0.0.0/.github/workflows/unittests.yml` & `migmose-0.1.0/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `migmose-0.0.0/dev_requirements/requirements-packaging.txt` & `migmose-0.1.0/dev_requirements/requirements-packaging.txt`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     # via twine
 rfc3986==2.0.0
     # via twine
 rich==13.7.1
     # via twine
 secretstorage==3.3.3
     # via keyring
-twine==5.0.0
+twine==5.1.0
     # via -r dev_requirements/requirements-packaging.in
 urllib3==2.2.1
     # via
     #   requests
     #   twine
 zipp==3.18.1
     # via importlib-metadata
```

### Comparing `migmose-0.0.0/src/migmose/__main__.py` & `migmose-0.1.0/src/migmose/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     type=click.Choice(["csv", "nested_json", "reduced_nested_json"], case_sensitive=False),
     default=["csv", "nested_json", "reduced_nested_json"],
     help="Defines the output format. Choose between csv and nested_json and reduced_nested_json. Default is csv.",
     multiple=True,
 )
 def main(
     edi_energy_mirror_path: Path,
-    output_dir,
+    output_dir: Path,
     format_version: EdifactFormatVersion | str,
     message_format: list[EdifactFormat],
     file_type: list[str],
 ) -> None:
     """
     Main function. Uses CLI input.
     """
```

### Comparing `migmose-0.0.0/src/migmose/parsing.py` & `migmose-0.1.0/src/migmose/parsing.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from datetime import datetime
 from pathlib import Path
 from typing import Generator, Union
 
 import click
 import docx
 from docx.document import Document
-from docx.oxml import CT_Tbl
+from docx.oxml import CT_Tbl  # type:ignore[attr-defined]
 from docx.table import Table, _Cell
 from loguru import logger
-from maus.edifact import EdifactFormat
+from maus.edifact import EdifactFormat, EdifactFormatVersion
 
 
 def find_file_to_format(
-    message_formats: list[EdifactFormat], edi_energy_repo: Path, format_version
+    message_formats: list[EdifactFormat], edi_energy_repo: Path, format_version: EdifactFormatVersion
 ) -> dict[EdifactFormat, Path]:
     """
     finds the file with the message type in the input directory
     """
     input_dir = edi_energy_repo / Path("edi_energy_de") / Path(format_version)
     file_dict: dict[EdifactFormat, Path] = {}
     for message_format in message_formats:
@@ -39,47 +39,48 @@
             logger.warning(f"⚠️ No file found for {message_format}.", fg="red")
     if file_dict:
         return file_dict
     logger.error("❌ No files found in the input directory.", fg="red")
     raise click.Abort()
 
 
+def _extract_date(file_path: Path) -> tuple[datetime, Path]:
+    # Regex to extract the date format YYYYMMDD from the filename as a string
+    match = re.search(r"(\d{8})\.docx$", file_path.name)
+    if match:
+        # Return the date as a datetime object for comparison and the path for use
+        return datetime.strptime(match.group(1), "%Y%m%d"), file_path
+    logger.warning(
+        f"⚠️ No timestamp in filename found in {file_path}."
+        + "in case of multiple docx files in this path, it must be a "
+        + "timestamp with format 'yyyyMMdd.docx' in filename.",
+        fg="red",
+    )
+    raise click.Abort()
+
+
 def get_latest_file(file_list: list[Path]) -> Path:
     """
     This function takes a list of docx files Path
     and returns the Path of the latest MIG docx file based on the timestamp in its name.
     The timestamp is assumed to be formatted as YYYYMMDD and located just before the ".docx" extension.
 
     Parameters:
         file_list (list of Path): A list containing file paths with timestamps.
 
     Returns:
         Path: The path of the latest file. Returns None if no valid date is found.
     """
 
-    def extract_date(file_path: Path) -> tuple[datetime, Path]:
-        # Regex to extract the date format YYYYMMDD from the filename as a string
-        match = re.search(r"(\d{8})\.docx$", file_path.name)
-        if match:
-            # Return the date as a datetime object for comparison and the path for use
-            return datetime.strptime(match.group(1), "%Y%m%d"), file_path
-        logger.warning(
-            f"⚠️ No timestamp in filename found in {file_path}."
-            + "in case of multiple docx files in this path, it must be a "
-            + "timestamp with format 'yyyyMMdd.docx' in filename.",
-            fg="red",
-        )
-        raise click.Abort()
-
     # Initialize variables to keep track of the latest file and date
     latest_file: Path
     latest_date: datetime | None = None
 
     for file_path in file_list:
-        date, path = extract_date(file_path)
+        date, path = _extract_date(file_path)
         if latest_date is None or date > latest_date:
             latest_file = path
             latest_date = date
 
     # Return the path of the file with the latest date
     return latest_file
 
@@ -95,14 +96,30 @@
         raise ValueError("Passed parent argument must be of type Document or _Cell")
 
     for child in parent_elm.iterchildren():
         if isinstance(child, CT_Tbl):
             yield Table(child, parent)
 
 
+_row_regex = re.compile(r"^(?P<left>\t\d+\t)(?P<nr>\d{0,5})(?P<right>\t.*)$")
+"""
+https://regex101.com/r/vtF07B/2
+"""
+
+
+def _zfill_nr(row_str: str) -> str:
+    match = _row_regex.match(row_str)
+    if not match:
+        return row_str
+    left = match.group("left")
+    nr = match.group("nr")
+    right = match.group("right")
+    return f"{left}{nr.zfill(5)}{right}"
+
+
 def parse_raw_nachrichtenstrukturzeile(input_path: Path) -> list[str]:
     """
     parses raw nachrichtenstrukturzeile from a table. returns list of raw lines
     """
     # pylint: disable=protected-access
     doc = docx.Document(str(input_path.absolute()))
     docx_objects = get_paragraphs_up_to_diagram(doc)
@@ -111,9 +128,9 @@
     for docx_object in docx_objects:
         for ind, line in enumerate(docx_object._cells):
             # marks the beginning of the complete nachrichtentruktur table
             if line.text == nachrichtenstruktur_header:
                 mig_tables.extend([row.text for row in docx_object._cells[ind + 1 :]])
             break
     # filter empty rows and headers
-    mig_tables = [row for row in mig_tables if row not in ("", "\n", nachrichtenstruktur_header)]
+    mig_tables = [_zfill_nr(row) for row in mig_tables if row not in ("", "\n", nachrichtenstruktur_header)]
     return mig_tables
```

### Comparing `migmose-0.0.0/src/migmose/mig/nachrichtenstrukturtabelle.py` & `migmose-0.1.0/src/migmose/mig/nachrichtenstrukturtabelle.py`

 * *Files identical despite different names*

### Comparing `migmose-0.0.0/src/migmose/mig/nachrichtenstrukturzeile.py` & `migmose-0.1.0/src/migmose/mig/nachrichtenstrukturzeile.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 """
 contains class for lines in mig tables
 """
 
 from typing import Any
 
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 
 
 class NachrichtenstrukturZeile(BaseModel):
     """
     class for lines in mig tables, e.g. (ORDCHG):
     {
         "zaehler": "0010",
-        "nr": "1",
+        "nr": "00001",
         "bezeichnung": "UNH",
         "standard_status": "M",
         "bdew_status": "M",
         "standard_maximale_wiederholungen": 1,
         "bdew_maximale_wiederholungen": 1,
         "ebene": 0,
         "inhalt": "Nachrichten-Kopfsegment"
         }
     """
 
     zaehler: str
-    nr: str | None = None
+    nr: str | None = Field(default=None, pattern=r"^\d{5}$")  #: the segment ID (can be used to match with AHBs)
     bezeichnung: str
     standard_status: str
     bdew_status: str
     standard_maximale_wiederholungen: int
     bdew_maximale_wiederholungen: int
     ebene: int
     inhalt: str
@@ -54,8 +54,10 @@
         is_line_incomplete = len(fields) != len(field_names) and not is_line_segmentgroup
 
         if is_line_segmentgroup:
             field_names = field_names[:1] + field_names[2:]
         if is_line_incomplete:
             raise ValueError(f"Expected 8 or 9 fields, got {len(fields)}, line: {raw_line}")
         field_dict: dict[str, Any] = dict(zip(field_names, fields))
+        if "nr" in field_dict and len(field_dict["nr"]) < 5:
+            field_dict["nr"] = field_dict["nr"].zfill(5)
         return cls(**field_dict)
```

### Comparing `migmose-0.0.0/src/migmose/mig/nestednachrichtenstruktur.py` & `migmose-0.1.0/src/migmose/mig/nestednachrichtenstruktur.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,55 +5,55 @@
 import json
 from pathlib import Path
 from types import NoneType
 from typing import Any, Optional, Tuple
 
 from loguru import logger
 from maus.edifact import EdifactFormat
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 
 from migmose.mig.nachrichtenstrukturtabelle import NachrichtenstrukturTabelle
 from migmose.mig.nachrichtenstrukturzeile import NachrichtenstrukturZeile
 
 
 class NestedNachrichtenstruktur(BaseModel):
     """
     class for structured segmentgroups in mig tables. Builds table recursively. Inherits from NachrichtenstrukturZeile
     e.g.(ORDCHG):
     {
     "segmente": [
         {
         "zaehler": "0160",
-        "nr": "7",
+        "nr": "00007",
         "bezeichnung": "NAD",
         "standard_status": "M",
         "bdew_status": "M",
         "standard_maximale_wiederholungen": 1,
         "bdew_maximale_wiederholungen": 1,
         "ebene": 1,
         "inhalt": "MP-ID Absender"
         }
         ],
     "segmentgruppen": [
     {
         "segmente": [
         {
             "zaehler": "0260",
-            "nr": "8",
+            "nr": "00008",
             "bezeichnung": "CTA",
             "standard_status": "M",
             "bdew_status": "M",
             "standard_maximale_wiederholungen": 1,
             "bdew_maximale_wiederholungen": 1,
             "ebene": 2,
             "inhalt": "Ansprechpartner"
             },
             {
             "zaehler": "0270",
-            "nr": "9",
+            "nr": "00009",
             "bezeichnung": "COM",
             "standard_status": "C",
             "bdew_status": "R",
             "standard_maximale_wiederholungen": 5,
             "bdew_maximale_wiederholungen": 5,
             "ebene": 3,
             "inhalt": "Kommunikationsverbindung"
@@ -62,16 +62,16 @@
         "segmentgruppen": []
         }
         ]
     }
     """
 
     header_linie: Optional[NachrichtenstrukturZeile] = None
-    segmente: list[Optional[NachrichtenstrukturZeile]] = []
-    segmentgruppen: list[Optional["NestedNachrichtenstruktur"]] = []
+    segmente: list[Optional[NachrichtenstrukturZeile]] = Field(default_factory=list)
+    segmentgruppen: list[Optional["NestedNachrichtenstruktur"]] = Field(default_factory=list)
 
     @classmethod
     def create_nested_nachrichtenstruktur(
         cls, table: NachrichtenstrukturTabelle, header_line: Optional[NachrichtenstrukturZeile] = None, index: int = 0
     ) -> Tuple["NestedNachrichtenstruktur", int]:
         """init nested Nachrichtenstruktur"""
         collected_segments: list[Optional[NachrichtenstrukturZeile]] = []
```

### Comparing `migmose-0.0.0/src/migmose/mig/reducednestednachrichtenstruktur.py` & `migmose-0.1.0/src/migmose/mig/reducednestednachrichtenstruktur.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,134 +1,144 @@
 """
 contains class for trees consisting of segments of mig tables
 """
 
 import json
 from pathlib import Path
-from typing import Any, Optional
+from typing import Any, Optional, TypeAlias
 
 from loguru import logger
 from maus.edifact import EdifactFormat
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 
 from migmose.mig.nachrichtenstrukturzeile import NachrichtenstrukturZeile
 from migmose.mig.nestednachrichtenstruktur import NestedNachrichtenstruktur
 
+_SegmentDict: TypeAlias = (
+    dict[
+        tuple[str, str],
+        tuple[
+            list[Optional[NachrichtenstrukturZeile]],
+            Optional[NachrichtenstrukturZeile],
+            set[tuple[str, str]],
+        ],
+    ]
+    | None
+)
+
+
+# Helper function to create a unique identifier for each segment
+def _get_identifier(segment: Optional[NachrichtenstrukturZeile]) -> tuple[str, str]:
+    if segment is None:
+        return "0", "root"
+    return segment.zaehler, segment.bezeichnung
+
+
+# Function to process segments and remove duplicates within the same list.
+def _process_segments(
+    segments: list[Optional[NachrichtenstrukturZeile]],
+) -> list[Optional[NachrichtenstrukturZeile]]:
+    seen = set()
+    unique_segments: list[Optional[NachrichtenstrukturZeile]] = []
+    for segment in segments:
+        if segment is not None:
+            identifier = _get_identifier(segment)
+            if identifier not in seen:
+                seen.add(identifier)
+                unique_segments.append(segment)
+    return unique_segments
+
+
+# Recursive function to traverse and clean segment groups
+def _process_segmentgruppen(
+    segmentgruppen_identifiers: set[tuple[str, str]],
+    segment_dict: _SegmentDict,
+    depth: int = 0,
+) -> list[Optional["ReducedNestedNachrichtenstruktur"]]:
+    """
+    Recursively clean segment groups to ensure nested nachrichtenstruktur consisting only of a unique subset.
+    """
+    result: list[Optional[ReducedNestedNachrichtenstruktur]] = []
+
+    for sg in sorted(segmentgruppen_identifiers):
+        if sg is not None:
+            # not sure about those type hints... they please mypy but I'm not the dev of this code
+            segmente: list[Optional[NachrichtenstrukturZeile]]
+            header_line: Optional[NachrichtenstrukturZeile]
+            segmentgroups: set[tuple[str, str]]
+            segmente, header_line, segmentgroups = segment_dict[sg]  # type:ignore[index]
+            if segmente is not None:
+                segmente = sorted(segmente, key=lambda x: x.zaehler)
+            _new_sg = ReducedNestedNachrichtenstruktur(header_linie=header_line, segmente=segmente)
+            _new_sg.segmentgruppen = _process_segmentgruppen(segmentgroups, segment_dict, depth + 1)
+            result.append(_new_sg)
+            logger.info("Added {} with {} segments at depth {}.", sg, len(segmente), depth)
+    return result
+
+
+def _build_segment_dict(
+    segment_groups: list[Optional[NestedNachrichtenstruktur]],
+    segment_dict: _SegmentDict = None,
+) -> dict[
+    tuple[str, str],
+    tuple[list[Optional[NachrichtenstrukturZeile]], Optional[NachrichtenstrukturZeile], set[tuple[str, str]]],
+]:
+    """Build a dictionary of segments and segment groups to find unique set."""
+    if segment_dict is None:
+        segment_dict = {}
+    for _sg in segment_groups:
+        if _sg is not None:
+            name = _get_identifier(_sg.header_linie)
+
+            # Check if the current segments are already known and complete by unknown segments
+            if name in segment_dict:
+                # make sure every possible segment is included
+                segment_dict[name] = (
+                    _process_segments(_sg.segmente + segment_dict[name][0]),
+                    segment_dict[name][1],
+                    segment_dict[name][2],
+                )
+            else:
+                segment_dict[name] = (_process_segments(_sg.segmente), _sg.header_linie, set())
+
+            # Iterate recursively through nested segmentgroups
+            for segmentgruppe in _sg.segmentgruppen:
+                if segmentgruppe is not None:
+                    sg_name = _get_identifier(segmentgruppe.header_linie)
+                    segment_dict[name][2].add(sg_name)
+                    segment_dict = _build_segment_dict([segmentgruppe], segment_dict)
+
+    return segment_dict
+
 
 class ReducedNestedNachrichtenstruktur(BaseModel):
     """will contain the tree structure of nachrichtenstruktur tables"""
 
     header_linie: Optional[NachrichtenstrukturZeile] = None
-    segmente: list[Optional[NachrichtenstrukturZeile]] = []
-    segmentgruppen: list[Optional["ReducedNestedNachrichtenstruktur"]] = []
+    segmente: list[Optional[NachrichtenstrukturZeile]] = Field(default_factory=list)
+    segmentgruppen: list[Optional["ReducedNestedNachrichtenstruktur"]] = Field(default_factory=list)
 
     @classmethod
     def create_reduced_nested_nachrichtenstruktur(
         cls, nachrichten_struktur: NestedNachrichtenstruktur
     ) -> "ReducedNestedNachrichtenstruktur":
         """init nested Nachrichtenstruktur"""
 
-        # Helper function to create a unique identifier for each segment
-        def get_identifier(segment: Optional[NachrichtenstrukturZeile]) -> tuple[str, str]:
-            if segment is None:
-                return ("0", "root")
-            return (segment.zaehler, segment.bezeichnung)
-
-        # Function to process segments and remove duplicates within the same list.
-        def process_segments(
-            segments: list[Optional[NachrichtenstrukturZeile]],
-        ) -> list[Optional[NachrichtenstrukturZeile]]:
-            seen = set()
-            unique_segments: list[Optional[NachrichtenstrukturZeile]] = []
-            for segment in segments:
-                if segment is not None:
-                    identifier = get_identifier(segment)
-                    if identifier not in seen:
-                        seen.add(identifier)
-                        unique_segments.append(segment)
-            return unique_segments
-
-        # Recursive function to traverse and clean segment groups
-        def process_segmentgruppen(
-            segmentgruppen_identifiers: set[tuple[str, str]],
-            segment_dict: dict,
-            depth: int = 0,
-        ) -> list[Optional[ReducedNestedNachrichtenstruktur]]:
-            """
-            Recursively clean segment groups to ensure nested nachrichtenstruktur consisting only of a unique subset.
-            """
-            result: list[Optional[ReducedNestedNachrichtenstruktur]] = []
-
-            for sg in sorted(segmentgruppen_identifiers):
-                if sg is not None:
-                    segmente, header_line, segmentgroups = segment_dict[sg]
-                    if segmente is not None:
-                        segmente = sorted(segmente, key=lambda x: x.zaehler)
-                    _new_sg = ReducedNestedNachrichtenstruktur(header_linie=header_line, segmente=segmente)
-                    _new_sg.segmentgruppen = process_segmentgruppen(segmentgroups, segment_dict, depth + 1)
-                    result.append(_new_sg)
-                    logger.info("Added {} with {} segments at depth {}.", sg, len(segmente), depth)
-            return result
-
-        def build_segment_dict(
-            segment_groups: list[Optional[NestedNachrichtenstruktur]],
-            segment_dict: (
-                dict[
-                    tuple[str, str],
-                    tuple[
-                        list[Optional[NachrichtenstrukturZeile]],
-                        Optional[NachrichtenstrukturZeile],
-                        set[tuple[str, str]],
-                    ],
-                ]
-                | None
-            ) = None,
-        ) -> dict[
-            tuple[str, str],
-            tuple[list[Optional[NachrichtenstrukturZeile]], Optional[NachrichtenstrukturZeile], set[tuple[str, str]]],
-        ]:
-            """Build a dictionary of segments and segment groups to find unique set."""
-            if segment_dict is None:
-                segment_dict = {}
-            for _sg in segment_groups:
-                if _sg is not None:
-                    name = get_identifier(_sg.header_linie)
-
-                    # Check if the current segments are already known and complete by unknown segments
-                    if name in segment_dict:
-                        # make sure every possible segment is included
-                        segment_dict[name] = (
-                            process_segments(_sg.segmente + segment_dict[name][0]),
-                            segment_dict[name][1],
-                            segment_dict[name][2],
-                        )
-                    else:
-                        segment_dict[name] = (process_segments(_sg.segmente), _sg.header_linie, set())
-
-                    # Iterate recursively through nested segmentgroups
-                    for segmentgruppe in _sg.segmentgruppen:
-                        if segmentgruppe is not None:
-                            sg_name = get_identifier(segmentgruppe.header_linie)
-                            segment_dict[name][2].add(sg_name)
-                            segment_dict = build_segment_dict([segmentgruppe], segment_dict)
-
-            return segment_dict
-
         data = ReducedNestedNachrichtenstruktur()
         # Start processing the top-level segments
         if nachrichten_struktur.segmente is not None:
-            data.segmente = process_segments(nachrichten_struktur.segmente)
+            data.segmente = _process_segments(nachrichten_struktur.segmente)
 
         # Process segment groups recursively
         if nachrichten_struktur.segmentgruppen is not None:
-            segment_dict = build_segment_dict(nachrichten_struktur.segmentgruppen)
+            segment_dict = _build_segment_dict(nachrichten_struktur.segmentgruppen)
             segmentgruppen_identifiers = set(
-                get_identifier(sg.header_linie) for sg in nachrichten_struktur.segmentgruppen if sg is not None
+                _get_identifier(sg.header_linie) for sg in nachrichten_struktur.segmentgruppen if sg is not None
             )
-            data.segmentgruppen = process_segmentgruppen(segmentgruppen_identifiers, segment_dict)
+            data.segmentgruppen = _process_segmentgruppen(segmentgruppen_identifiers, segment_dict)
 
         return data
 
     def to_json(self, message_type: EdifactFormat, output_dir: Path) -> dict[str, Any]:
         """
         writes the reduced NestedNachrichtenstruktur as json
         """
```

### Comparing `migmose-0.0.0/.gitignore` & `migmose-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `migmose-0.0.0/pyproject.toml` & `migmose-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `migmose-0.0.0/PKG-INFO` & `migmose-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.3
 Name: migmose
-Version: 0.0.0
+Version: 0.1.0
 Summary: Tool to generate machine readable files from MIG documents
 Project-URL: Changelog, https://github.com/Hochfrequenz/migmose/releases
 Project-URL: Homepage, https://github.com/Hochfrequenz/migmose
 Author-email: Kevin Krechan <kevin.krechan@hochfrequenz.de>
 License: MIT
+License-File: LICENSE
 Keywords: automation,bdew,edi@energy,mig
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -24,14 +25,17 @@
 Requires-Dist: python-docx
 Description-Content-Type: text/markdown
 
 ![migmose-logo](migmose-logo.jpeg)
 
 # MIG_mose
 
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
+![Python Versions (officially) supported](https://img.shields.io/pypi/pyversions/migmose.svg)
+![Pypi status badge](https://img.shields.io/pypi/v/migmose)
 ![Unittests status badge](https://github.com/Hochfrequenz/migmose/workflows/Unittests/badge.svg)
 ![Coverage status badge](https://github.com/Hochfrequenz/migmose/workflows/Coverage/badge.svg)
 ![Linting status badge](https://github.com/Hochfrequenz/migmose/workflows/Linting/badge.svg)
 ![Black status badge](https://github.com/Hochfrequenz/migmose/workflows/Formatting/badge.svg)
 
 MIG_mose generates machine-readable files from MIG documents ([edi-energy](https://www.edi-energy.de/index.php?id=38)).
 MIG_mose is the sister of [kohlrahbi](https://github.com/Hochfrequenz/kohlrahbi).
@@ -41,18 +45,18 @@
 - .docx files a processed by the [python-docx](https://python-docx.readthedocs.io/en/latest/) library.
 - EdiFact formats are used as in [maus.edifact](https://github.com/Hochfrequenz/mig_ahb_utility_stack/blob/main/src/maus/edifact.py).
 
 This is at the moment a MWE (Minimum Working Example) and will be extended in the future.
 See below for an overview of its features.
 
 ## Installation
-MIG_mose is a Python based tool.
-Therefore you have to make sure, that Python is running on your machine.
+MIG_mose is a Python-based tool.
+Therefore, you have to make sure, that Python is running on your machine.
 
-We recommend to use virtual environments to keep your system clean.
+We recommend using virtual environments to keep your system clean.
 
 Create a new virtual environment with
 ```bash
 python -m venv .venv
 ```
 
 The activation of the virtual environment depends on your used OS.
@@ -66,14 +70,15 @@
 source .venv/bin/activate
 ```
 Finally, install the package with
 
 ```bash
 pip install migmose
 ```
+
 ## Features And How To Use Them
 
 At this point, MIG_mose works as a command-line interface tool (CLI).
 There are several flags available to provide a user-friendly way to interact with MIG_mose.
 Below the available options are listed:
 
 - **Input Directory (`-i`, `--input-dir`):**
```

