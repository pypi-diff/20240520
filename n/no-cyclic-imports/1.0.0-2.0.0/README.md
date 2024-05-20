# Comparing `tmp/no_cyclic_imports-1.0.0.tar.gz` & `tmp/no_cyclic_imports-2.0.0.tar.gz`

## Comparing `no_cyclic_imports-1.0.0.tar` & `no_cyclic_imports-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,16 @@
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 no_cyclic_imports-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 no_cyclic_imports-1.0.0/.github/dependabot.yml
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 no_cyclic_imports-1.0.0/.github/workflows/pre-commit-detect-outdated.yml
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 no_cyclic_imports-1.0.0/.github/workflows/pre-commit.yml
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 no_cyclic_imports-1.0.0/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 no_cyclic_imports-1.0.0/no_cyclic_imports/__init__.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 no_cyclic_imports-1.0.0/no_cyclic_imports/__main__.py
--rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 no_cyclic_imports-1.0.0/no_cyclic_imports/_engine.py
--rw-r--r--   0        0        0     6778 2020-02-02 00:00:00.000000 no_cyclic_imports-1.0.0/no_cyclic_imports/_imports.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 no_cyclic_imports-1.0.0/no_cyclic_imports/_normalization.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 no_cyclic_imports-1.0.0/no_cyclic_imports/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 no_cyclic_imports-1.0.0/no_cyclic_imports/tests/__init__.py
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 no_cyclic_imports-1.0.0/no_cyclic_imports/tests/factories.py
--rw-r--r--   0        0        0     7546 2020-02-02 00:00:00.000000 no_cyclic_imports-1.0.0/no_cyclic_imports/tests/test_imports.py
--rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 no_cyclic_imports-1.0.0/no_cyclic_imports/tests/test_main.py
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 no_cyclic_imports-1.0.0/no_cyclic_imports/tests/test_normalization.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 no_cyclic_imports-1.0.0/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 no_cyclic_imports-1.0.0/COPYING
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 no_cyclic_imports-1.0.0/README.md
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 no_cyclic_imports-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 no_cyclic_imports-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 no_cyclic_imports-2.0.0/no_cyclic_imports/__init__.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 no_cyclic_imports-2.0.0/no_cyclic_imports/__main__.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 no_cyclic_imports-2.0.0/no_cyclic_imports/_engine.py
+-rw-r--r--   0        0        0     6788 2020-02-02 00:00:00.000000 no_cyclic_imports-2.0.0/no_cyclic_imports/_imports.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 no_cyclic_imports-2.0.0/no_cyclic_imports/_normalization.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 no_cyclic_imports-2.0.0/no_cyclic_imports/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 no_cyclic_imports-2.0.0/no_cyclic_imports/tests/__init__.py
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 no_cyclic_imports-2.0.0/no_cyclic_imports/tests/factories.py
+-rw-r--r--   0        0        0     7546 2020-02-02 00:00:00.000000 no_cyclic_imports-2.0.0/no_cyclic_imports/tests/test_imports.py
+-rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 no_cyclic_imports-2.0.0/no_cyclic_imports/tests/test_main.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 no_cyclic_imports-2.0.0/no_cyclic_imports/tests/test_normalization.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 no_cyclic_imports-2.0.0/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 no_cyclic_imports-2.0.0/COPYING
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 no_cyclic_imports-2.0.0/README.md
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 no_cyclic_imports-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 no_cyclic_imports-2.0.0/PKG-INFO
```

### Comparing `no_cyclic_imports-1.0.0/no_cyclic_imports/__main__.py` & `no_cyclic_imports-2.0.0/no_cyclic_imports/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import sys
 
 from ._engine import run
 from .version import VERSION
 
 
-def _main(argv: list[str] | None = None):
+def _inner_main(argv: list[str] | None = None):
     if argv is None:
         argv = sys.argv
 
     parser = argparse.ArgumentParser(prog="no-cyclic-imports")
     parser.add_argument("--version", action="version", version=VERSION)
     parser.add_argument(
         "--no-follow",
@@ -57,16 +57,34 @@
 
     logging.basicConfig(
         level=log_level,
         format="no-cyclic-imports: [%(levelname)s] %(message)s",
         force=True,
     )
 
-    cycles_count = run(config.paths, follow=bool(config.follow), file_=sys.stdout)
-
-    exit_code = 1 if cycles_count else 0
+    exit_code = 1
+    try:
+        cycles_count = run(config.paths, follow=bool(config.follow), file_=sys.stdout)
+    except Exception as e:  # noqa: BLE001
+        if config.debug:
+            import traceback
+
+            traceback.print_exc()
+        else:
+            logging.error(e)  # noqa: TRY400
+    else:
+        exit_code = 2 if cycles_count else 0
 
     sys.exit(exit_code)
 
 
+def _main():
+    try:
+        _inner_main()
+    except KeyboardInterrupt:
+        import signal
+
+        sys.exit(128 + signal.SIGINT)
+
+
 if __name__ == "__main__":
-    _main(sys.argv)
+    _main()
```

### Comparing `no_cyclic_imports-1.0.0/no_cyclic_imports/_engine.py` & `no_cyclic_imports-2.0.0/no_cyclic_imports/_engine.py`

 * *Files 21% similar despite different names*

```diff
@@ -62,14 +62,19 @@
 
 
 def run(abs_paths: list[str], *, follow: bool, file_: IO) -> int:
     imports = ImportGraph()
     toplevel_packages = ToplevelCollector()
 
     for abs_path in abs_paths:
+        if not os.path.exists(abs_path):
+            # This will raise FileNotFoundError the way that stdlib does:
+            open(abs_path)  # noqa: SIM115
+            raise AssertionError  # avoiding "assert" in case of "python3 -O"
+
         if os.path.isdir(abs_path):
             # Find all .py files
             _logger.info(
                 f"Scanning directory {abs_path!r} for Python files recursively...",
             )
             for root, folders, files in os.walk(abs_path):
                 folders[:] = sorted(folders)  # for alphabetical ascend
```

### Comparing `no_cyclic_imports-1.0.0/no_cyclic_imports/_imports.py` & `no_cyclic_imports-2.0.0/no_cyclic_imports/_imports.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     raise PythonSourceNotFoundError(_breadcrumbs)
 
 
 def determine_source_module_name(abs_path: str) -> str:
     abs_path_backup = abs_path
 
     if not abs_path.endswith(".py"):
-        raise ValueError(f"{abs_path} does not end in .py")  # noqa: EM102, TRY003
+        raise ValueError(f"Path {abs_path!r} does not end in '.py'.")  # noqa: EM102, TRY003
     abs_path = abs_path[: -len(".py")]
 
     parts = []
     while True:
         package_path = os.path.dirname(abs_path)
         module_name = os.path.basename(abs_path)
         init_py_path = os.path.join(package_path, "__init__.py")
```

### Comparing `no_cyclic_imports-1.0.0/no_cyclic_imports/_normalization.py` & `no_cyclic_imports-2.0.0/no_cyclic_imports/_normalization.py`

 * *Files identical despite different names*

### Comparing `no_cyclic_imports-1.0.0/no_cyclic_imports/tests/factories.py` & `no_cyclic_imports-2.0.0/no_cyclic_imports/tests/factories.py`

 * *Files identical despite different names*

### Comparing `no_cyclic_imports-1.0.0/no_cyclic_imports/tests/test_imports.py` & `no_cyclic_imports-2.0.0/no_cyclic_imports/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `no_cyclic_imports-1.0.0/no_cyclic_imports/tests/test_main.py` & `no_cyclic_imports-2.0.0/no_cyclic_imports/tests/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,30 +7,30 @@
 from tempfile import TemporaryDirectory
 from textwrap import dedent
 from unittest import TestCase
 from unittest.mock import patch
 
 from parameterized import parameterized
 
-from ..__main__ import _main
+from ..__main__ import _inner_main
 from ..version import VERSION
 from .factories import add_cyclic_import_to
 
 
 class MainTest(TestCase):
     def _invoke(self, *argv_one_plus: list[str]) -> tuple[int, str, str]:
         with (
             patch("sys.stdout", new_callable=StringIO) as stdout,
             patch(
                 "sys.stderr",
                 new_callable=StringIO,
             ) as stderr,
             self.assertRaises(SystemExit) as catcher,
         ):
-            _main(["dummy", *argv_one_plus])
+            _inner_main(["dummy", *argv_one_plus])
 
         exit_code = catcher.exception.code
 
         return exit_code, stdout.getvalue(), stderr.getvalue()
 
     def test_version(self):
         self.assertEqual(self._invoke("--version"), (0, f"{VERSION}\n", ""))
@@ -74,15 +74,15 @@
                 add_cyclic_import_to(tempdir)
             )
             exit_code, stdout, stderr = self._invoke(
                 "--no-follow",
                 *(*extra_argv, tempdir),
             )
 
-        self.assertEqual(exit_code, 1)
+        self.assertEqual(exit_code, 2)
         self.assertEqual(
             dedent(f"""\
                 {package_name} -> {package_a_name} -> {package_b_name} -> {package_name}
 
                 1 cycle(s).
             """),
             stdout,
@@ -105,15 +105,15 @@
             with patch("sys.path", [*sys.path, tempdir]):
                 exit_code, stdout, stderr = self._invoke(
                     "--verbose",
                     *(*extra_argv, a_py),
                 )
 
         if expecting_follow:
-            self.assertEqual(exit_code, 1)
+            self.assertEqual(exit_code, 2)
             self.assertEqual(
                 dedent(f"""\
                     {package_name} -> {package_a_name} -> {package_b_name} -> {package_name}
 
                     1 cycle(s).
                 """),  # noqa: E501
                 stdout,
```

### Comparing `no_cyclic_imports-1.0.0/no_cyclic_imports/tests/test_normalization.py` & `no_cyclic_imports-2.0.0/no_cyclic_imports/tests/test_normalization.py`

 * *Files identical despite different names*

### Comparing `no_cyclic_imports-1.0.0/COPYING` & `no_cyclic_imports-2.0.0/COPYING`

 * *Files identical despite different names*

### Comparing `no_cyclic_imports-1.0.0/pyproject.toml` & `no_cyclic_imports-2.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -48,14 +48,19 @@
 
 [project.urls]
 Homepage = "https://github.com/hartwork/no-cyclic-imports"
 
 [tool.hatch.version]
 path = "no_cyclic_imports/version.py"
 
+[tool.hatch.build.targets.sdist]
+only-include = [
+  "no_cyclic_imports",
+]
+
 [tool.coverage.run]
 branch = true
 source_pkgs = ["no_cyclic_imports"]
 
 [tool.coverage.report]
 skip_empty = true
```

### Comparing `no_cyclic_imports-1.0.0/PKG-INFO` & `no_cyclic_imports-2.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: no-cyclic-imports
-Version: 1.0.0
+Version: 2.0.0
 Summary: Tool to detect and report on cyclic imports in a Python codebase
 Project-URL: Homepage, https://github.com/hartwork/no-cyclic-imports
 Author-email: Sebastian Pipping <sebastian@pipping.org>
 License: AGPL-3.0-or-later
 License-File: COPYING
 Keywords: automation,lint,linter
 Classifier: Development Status :: 4 - Beta
@@ -23,14 +23,16 @@
 Requires-Dist: coverage; extra == 'tests'
 Requires-Dist: parameterized; extra == 'tests'
 Requires-Dist: pytest; extra == 'tests'
 Description-Content-Type: text/markdown
 
 # no-cyclic-imports
 
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
+[![Run the test suite](https://github.com/hartwork/no-cyclic-imports/actions/workflows/run-tests.yml/badge.svg)](https://github.com/hartwork/no-cyclic-imports/actions/workflows/run-tests.yml)
 [![PyPI - Version](https://img.shields.io/pypi/v/no-cyclic-imports.svg)](https://pypi.org/project/no-cyclic-imports)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/no-cyclic-imports.svg)](https://pypi.org/project/no-cyclic-imports)
 
 **Tool to detect and report on cyclic imports in a Python codebase**
 
 ```console
 $ no-cyclic-imports --no-follow cyclic/
```

