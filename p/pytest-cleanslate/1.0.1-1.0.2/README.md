# Comparing `tmp/pytest_cleanslate-1.0.1.tar.gz` & `tmp/pytest_cleanslate-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_cleanslate-1.0.1.tar", last modified: Wed May 15 17:38:00 2024, max compression
+gzip compressed data, was "pytest_cleanslate-1.0.2.tar", last modified: Mon May 20 01:29:40 2024, max compression
```

## Comparing `pytest_cleanslate-1.0.1.tar` & `pytest_cleanslate-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:38:00.880888 pytest_cleanslate-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-15 17:37:53.000000 pytest_cleanslate-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-15 17:38:00.880888 pytest_cleanslate-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-15 17:37:53.000000 pytest_cleanslate-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-15 17:37:53.000000 pytest_cleanslate-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 17:38:00.880888 pytest_cleanslate-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:38:00.876888 pytest_cleanslate-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:38:00.876888 pytest_cleanslate-1.0.1/src/pytest_cleanslate/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-15 17:37:53.000000 pytest_cleanslate-1.0.1/src/pytest_cleanslate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-15 17:37:53.000000 pytest_cleanslate-1.0.1/src/pytest_cleanslate/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-15 17:37:53.000000 pytest_cleanslate-1.0.1/src/pytest_cleanslate/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:38:00.880888 pytest_cleanslate-1.0.1/src/pytest_cleanslate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-15 17:38:00.000000 pytest_cleanslate-1.0.1/src/pytest_cleanslate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-15 17:38:00.000000 pytest_cleanslate-1.0.1/src/pytest_cleanslate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 17:38:00.000000 pytest_cleanslate-1.0.1/src/pytest_cleanslate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-15 17:38:00.000000 pytest_cleanslate-1.0.1/src/pytest_cleanslate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-15 17:38:00.000000 pytest_cleanslate-1.0.1/src/pytest_cleanslate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 17:38:00.000000 pytest_cleanslate-1.0.1/src/pytest_cleanslate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:38:00.880888 pytest_cleanslate-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-05-15 17:37:53.000000 pytest_cleanslate-1.0.1/tests/test_cleanslate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:29:40.614946 pytest_cleanslate-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-20 01:29:30.000000 pytest_cleanslate-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-05-20 01:29:40.614946 pytest_cleanslate-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-20 01:29:30.000000 pytest_cleanslate-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-20 01:29:30.000000 pytest_cleanslate-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 01:29:40.614946 pytest_cleanslate-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:29:40.610946 pytest_cleanslate-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:29:40.614946 pytest_cleanslate-1.0.2/src/pytest_cleanslate/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-20 01:29:30.000000 pytest_cleanslate-1.0.2/src/pytest_cleanslate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-20 01:29:30.000000 pytest_cleanslate-1.0.2/src/pytest_cleanslate/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-05-20 01:29:30.000000 pytest_cleanslate-1.0.2/src/pytest_cleanslate/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:29:40.614946 pytest_cleanslate-1.0.2/src/pytest_cleanslate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-05-20 01:29:40.000000 pytest_cleanslate-1.0.2/src/pytest_cleanslate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-20 01:29:40.000000 pytest_cleanslate-1.0.2/src/pytest_cleanslate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 01:29:40.000000 pytest_cleanslate-1.0.2/src/pytest_cleanslate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-20 01:29:40.000000 pytest_cleanslate-1.0.2/src/pytest_cleanslate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-20 01:29:40.000000 pytest_cleanslate-1.0.2/src/pytest_cleanslate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-20 01:29:40.000000 pytest_cleanslate-1.0.2/src/pytest_cleanslate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:29:40.614946 pytest_cleanslate-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6279 2024-05-20 01:29:30.000000 pytest_cleanslate-1.0.2/tests/test_cleanslate.py
```

### Comparing `pytest_cleanslate-1.0.1/LICENSE` & `pytest_cleanslate-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_cleanslate-1.0.1/PKG-INFO` & `pytest_cleanslate-1.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pytest-cleanslate
-Version: 1.0.1
+Version: 1.0.2
 Summary: Collects and executes pytest tests separately
 Author-email: Juan Altmayer Pizzorno <juan@altmayer.com>
-Project-URL: Repository, https://github.com/jaltmayerpizzorno/pytest_cleanslate
+Project-URL: Repository, https://github.com/plasma-umass/pytest_cleanslate
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
@@ -15,25 +15,41 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pytest
 Requires-Dist: py
 Requires-Dist: pytest-forked
 
-# pytest-CleanSlate: work around test state pollution
+# pytest-cleanslate: work around test state pollution
 by [Juan Altmayer Pizzorno](https://jaltmayerpizzorno.github.io) and [Emery Berger](https://emeryberger.com)
 at UMass Amherst's [PLASMA lab](https://plasma-umass.org/).
 
 [![license](https://img.shields.io/github/license/plasma-umass/pytest-cleanslate?color=blue)](LICENSE)
 [![pypi](https://img.shields.io/pypi/v/pytest-cleanslate?color=blue)](https://pypi.org/project/pytest-cleanslate/)
-[![Downloads](https://static.pepy.tech/badge/pytest-cleanslate)](https://pepy.tech/project/pytest-cleanslate)
 ![pyversions](https://img.shields.io/pypi/pyversions/pytest-cleanslate?logo=python&logoColor=FBE072)
 ![tests](https://github.com/plasma-umass/pytest-cleanslate/workflows/tests/badge.svg)
+[![Downloads](https://static.pepy.tech/badge/pytest-cleanslate)](https://pepy.tech/project/pytest-cleanslate)
 
 ## About
 pytest-cleanslate is a small plugin for the [pytest](https://github.com/pytest-dev/pytest)
 test framework which, as the name implies, helps give each test module a "clean slate" to execute.
 Plugins such as [pytest-forked](https://github.com/pytest-dev/pytest-forked) and
 [pytest-isolate](https://github.com/gilfree/pytest-isolate) allow you to execute tests
 in separate processes, working around in-memory test "state pollution" resulting from
 their execution, but do not protect against pollution caused by top-level code in test
 modules. This is what pytest-CleanSlate remedies.
+
+## How to use
+After `pip install pytest-cleanslate`, simply add `--cleanslate` to your `pytest` invocation.
+
+## Interaction with other plugins
+This plugin implies the use of `pytest-forked`, i.e., it is as though you installed that
+plugin and passed in `--forked` to execute all tests in separate processes.
+
+This plugin subverts somewhat `pytest`'s mode of operation in that it postpones collecting
+test items within test modules (i.e., within Python test files) until the test execution phase.
+While we have attempted to stay as compatible with other plugins as possible, it is likely
+to not work in some combinations (such as, for example, [pytest-xdist](https://github.com/pytest-dev/pytest-xdist)).
+Feel free to [open an issue](https://github.com/plasma-umass/pytest-cleanslate/issues) if you come across a case where it doesn't work.
+
+## Requirements
+Python 3.8+, Linux or MacOS.
```

### Comparing `pytest_cleanslate-1.0.1/pyproject.toml` & `pytest_cleanslate-1.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pytest-cleanslate"
-version = "1.0.1"
+version = "1.0.2"
 description = "Collects and executes pytest tests separately"
 readme = "README.md"
 requires-python = ">= 3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
@@ -20,11 +20,17 @@
 dependencies = [
     "pytest",
     "py",
     "pytest-forked",
 ]
 
 [project.urls]
-"Repository" = "https://github.com/jaltmayerpizzorno/pytest_cleanslate"
+"Repository" = "https://github.com/plasma-umass/pytest_cleanslate"
 
 [project.entry-points.pytest11]
 pytest_cleanslate = "pytest_cleanslate.plugin"
+
+[tool.pytest.ini_options]
+required_plugins = [
+    'pytest-cleanslate',    # must be installed to test
+    'pytest-asyncio',       # required by tests
+]
```

### Comparing `pytest_cleanslate-1.0.1/src/pytest_cleanslate.egg-info/PKG-INFO` & `pytest_cleanslate-1.0.2/src/pytest_cleanslate.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pytest-cleanslate
-Version: 1.0.1
+Version: 1.0.2
 Summary: Collects and executes pytest tests separately
 Author-email: Juan Altmayer Pizzorno <juan@altmayer.com>
-Project-URL: Repository, https://github.com/jaltmayerpizzorno/pytest_cleanslate
+Project-URL: Repository, https://github.com/plasma-umass/pytest_cleanslate
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
@@ -15,25 +15,41 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pytest
 Requires-Dist: py
 Requires-Dist: pytest-forked
 
-# pytest-CleanSlate: work around test state pollution
+# pytest-cleanslate: work around test state pollution
 by [Juan Altmayer Pizzorno](https://jaltmayerpizzorno.github.io) and [Emery Berger](https://emeryberger.com)
 at UMass Amherst's [PLASMA lab](https://plasma-umass.org/).
 
 [![license](https://img.shields.io/github/license/plasma-umass/pytest-cleanslate?color=blue)](LICENSE)
 [![pypi](https://img.shields.io/pypi/v/pytest-cleanslate?color=blue)](https://pypi.org/project/pytest-cleanslate/)
-[![Downloads](https://static.pepy.tech/badge/pytest-cleanslate)](https://pepy.tech/project/pytest-cleanslate)
 ![pyversions](https://img.shields.io/pypi/pyversions/pytest-cleanslate?logo=python&logoColor=FBE072)
 ![tests](https://github.com/plasma-umass/pytest-cleanslate/workflows/tests/badge.svg)
+[![Downloads](https://static.pepy.tech/badge/pytest-cleanslate)](https://pepy.tech/project/pytest-cleanslate)
 
 ## About
 pytest-cleanslate is a small plugin for the [pytest](https://github.com/pytest-dev/pytest)
 test framework which, as the name implies, helps give each test module a "clean slate" to execute.
 Plugins such as [pytest-forked](https://github.com/pytest-dev/pytest-forked) and
 [pytest-isolate](https://github.com/gilfree/pytest-isolate) allow you to execute tests
 in separate processes, working around in-memory test "state pollution" resulting from
 their execution, but do not protect against pollution caused by top-level code in test
 modules. This is what pytest-CleanSlate remedies.
+
+## How to use
+After `pip install pytest-cleanslate`, simply add `--cleanslate` to your `pytest` invocation.
+
+## Interaction with other plugins
+This plugin implies the use of `pytest-forked`, i.e., it is as though you installed that
+plugin and passed in `--forked` to execute all tests in separate processes.
+
+This plugin subverts somewhat `pytest`'s mode of operation in that it postpones collecting
+test items within test modules (i.e., within Python test files) until the test execution phase.
+While we have attempted to stay as compatible with other plugins as possible, it is likely
+to not work in some combinations (such as, for example, [pytest-xdist](https://github.com/pytest-dev/pytest-xdist)).
+Feel free to [open an issue](https://github.com/plasma-umass/pytest-cleanslate/issues) if you come across a case where it doesn't work.
+
+## Requirements
+Python 3.8+, Linux or MacOS.
```

### Comparing `pytest_cleanslate-1.0.1/tests/test_cleanslate.py` & `pytest_cleanslate-1.0.2/tests/test_cleanslate.py`

 * *Files 23% similar despite different names*

```diff
@@ -44,58 +44,55 @@
 
 {'test_foo()' if fail_collect else ''}
 """)
 
     return failing, polluter
 
 
-@pytest.mark.parametrize("fail_collect", [True, False])
-@pytest.mark.parametrize("fail_kind", list(FAILURES.keys() - {'kill'}))
-def test_check_suite_fails(tmp_path, monkeypatch, fail_collect, fail_kind):
+@pytest.fixture
+def tests_dir(tmp_path, monkeypatch):
     monkeypatch.chdir(tmp_path)
     tests_dir = Path('tests')
     tests_dir.mkdir()
+    yield tests_dir
+
+
+@pytest.mark.parametrize("fail_collect", [True, False])
+@pytest.mark.parametrize("fail_kind", list(FAILURES.keys() - {'kill'}))
+def test_check_suite_fails(tests_dir, fail_collect, fail_kind):
     make_polluted_suite(tests_dir, fail_collect, fail_kind)
 
     p = subprocess.run([sys.executable, '-m', 'pytest', tests_dir], check=False)
     if fail_collect or fail_kind in ('exit', 'interrupt'):
         assert p.returncode == pytest.ExitCode.INTERRUPTED
     else:
         assert p.returncode == pytest.ExitCode.TESTS_FAILED
 
 
+@pytest.mark.parametrize("plugin", ['asyncio', 'no:asyncio'])
 @pytest.mark.parametrize("fail_collect", [True, False])
 @pytest.mark.parametrize("fail_kind", list(FAILURES.keys()))
-def test_isolate_polluted(tmp_path, monkeypatch, fail_collect, fail_kind):
-    monkeypatch.chdir(tmp_path)
-    tests_dir = Path('tests')
-    tests_dir.mkdir()
+def test_isolate_polluted(tests_dir, fail_collect, fail_kind, plugin):
     make_polluted_suite(tests_dir, fail_collect, fail_kind)
 
-    p = subprocess.run([sys.executable, '-m', 'pytest', '--cleanslate', tests_dir], check=False)
+    p = subprocess.run([sys.executable, '-m', 'pytest', '-p', plugin, '--cleanslate', tests_dir], check=False)
     assert p.returncode == pytest.ExitCode.OK
 
 
 @pytest.mark.parametrize("fail_kind", list(FAILURES.keys()))
-def test_pytest_discover_tests(tmp_path, fail_kind, monkeypatch):
-    monkeypatch.chdir(tmp_path)
-    tests_dir = Path('tests')
-    tests_dir.mkdir()
+def test_pytest_discover_tests(tests_dir, fail_kind):
     make_polluted_suite(tests_dir, fail_collect=False, fail_kind=fail_kind)
 
     p = subprocess.run([sys.executable, '-m', 'pytest', '--cleanslate'], check=False) # no tests_dir here
     assert p.returncode == pytest.ExitCode.OK
 
 
 @pytest.mark.parametrize("fail_collect", [True, False])
 @pytest.mark.parametrize("fail_kind", list(FAILURES.keys()))
-def test_unconditionally_failing_test(tmp_path, monkeypatch, fail_collect, fail_kind):
-    monkeypatch.chdir(tmp_path)
-    tests_dir = Path('tests')
-    tests_dir.mkdir()
+def test_unconditionally_failing_test(tests_dir, fail_collect, fail_kind):
     make_polluted_suite(tests_dir, fail_collect, fail_kind)
 
     # _unconditionally_ failing test
     failing = seq2p(tests_dir, 2)
     failing.write_text(f"""\
 import sys
 import os
@@ -110,28 +107,108 @@
 {'test_foo()' if fail_collect else ''}
 """)
 
     p = subprocess.run([sys.executable, '-m', 'pytest', '--cleanslate', tests_dir], check=False)
     assert p.returncode == pytest.ExitCode.TESTS_FAILED
 
 
-def test_isolate_module_yields_collector(tmp_path, monkeypatch):
+def test_isolate_module_yields_collector(tests_dir):
     # A pytest.Collector.collect()'s return value may include not only pytest.Item,
     # but also pytest.Collector.
     #
     # Here we test for this by including a class within the test module:
     # when the module is being collected, pytest.Module.collect() will include
     # a pytest.Class collector to actually collect items from within the class.
 
-    monkeypatch.chdir(tmp_path)
-    tests_dir = Path('tests')
-    tests_dir.mkdir()
-
     test = seq2p(tests_dir, 1)
     test.write_text("""\
 class TestClass:
     def test_foo(self):
         assert True
 """)
 
     p = subprocess.run([sys.executable, '-m', 'pytest', '--cleanslate', tests_dir], check=False)
     assert p.returncode == pytest.ExitCode.OK
+
+
+# If asyncio is missing/disabled, the test may show as skipped; we detect it here
+# with the 'fail=True' version of the test.
+@pytest.mark.parametrize("fail", [False, True])
+def test_asyncio(tests_dir, fail):
+    test = seq2p(tests_dir, 1)
+    test.write_text(f"""\
+import pytest
+import asyncio
+
+async def foo(s):
+    return s
+
+@pytest.mark.asyncio
+async def test_asyncio():
+    assert "bar" {'!=' if fail else '=='} await foo("bar")
+""")
+
+    p = subprocess.run([sys.executable, '-m', 'pytest', '--cleanslate', tests_dir], check=False)
+    if fail:
+        assert p.returncode == pytest.ExitCode.TESTS_FAILED
+    else:
+        assert p.returncode == pytest.ExitCode.OK
+
+
+@pytest.mark.parametrize("tf", ['test_one', 'test_two'])
+def test_mark(tests_dir, tf):
+    # the built-in "mark" plugin implements '-k' and '-m'
+
+    test = seq2p(tests_dir, 1)
+    test.write_text("""\
+def test_one():
+    assert True
+
+def test_two():
+    assert False
+""")
+
+    p = subprocess.run([sys.executable, '-m', 'pytest', '--cleanslate', '-k', tf, tests_dir], check=False)
+    if tf == 'test_two':
+        assert p.returncode == pytest.ExitCode.TESTS_FAILED
+    else:
+        assert p.returncode == pytest.ExitCode.OK
+
+
+def test_exitfirst(tests_dir):
+    test = seq2p(tests_dir, 1)
+    test.write_text("""\
+from pathlib import Path
+
+def test_one():
+    assert False
+
+def test_two():
+    Path('litmus.txt').touch()
+""")
+
+    p = subprocess.run([sys.executable, '-m', 'pytest', '--cleanslate', '--exitfirst', '-s', tests_dir], check=False,
+                       capture_output=True)
+    assert p.returncode == pytest.ExitCode.TESTS_FAILED
+    assert not Path('litmus.txt').exists()
+    assert 'CRASHED' not in str(p.stdout, 'utf-8')
+
+
+def test_shouldstop(tests_dir):
+    test = seq2p(tests_dir, 1)
+    test.write_text("""\
+import pytest
+from pathlib import Path
+
+def test_one():
+    assert False
+
+def test_two():
+    Path('litmus.txt').touch()
+""")
+
+    # --stepwise sets session.shouldstop upon a test failure.
+    p = subprocess.run([sys.executable, '-m', 'pytest', '--cleanslate', '--stepwise', '-s', tests_dir], check=False,
+                       capture_output=True)
+    assert p.returncode == pytest.ExitCode.INTERRUPTED
+    assert not Path('litmus.txt').exists()
+    assert 'CRASHED' not in str(p.stdout, 'utf-8')
```

