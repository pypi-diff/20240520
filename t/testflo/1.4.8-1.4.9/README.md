# Comparing `tmp/testflo-1.4.8.tar.gz` & `tmp/testflo-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflo-1.4.8.tar", last modified: Mon Feb 14 17:22:43 2022, max compression
+gzip compressed data, was "testflo-1.4.9.tar", last modified: Mon Jul 25 18:09:09 2022, max compression
```

## Comparing `testflo-1.4.8.tar` & `testflo-1.4.9.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2022-02-14 17:22:43.796443 testflo-1.4.8/
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2175 2021-12-12 22:38:56.000000 testflo-1.4.8/DESIGN.txt
--rw-r--r--   0 swryan    (1000) swryan    (1000)      554 2021-12-12 22:38:56.000000 testflo-1.4.8/LICENSE.txt
--rw-r--r--   0 swryan    (1000) swryan    (1000)       82 2021-12-12 22:38:56.000000 testflo-1.4.8/MANIFEST.in
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5010 2022-02-14 17:22:43.796443 testflo-1.4.8/PKG-INFO
--rw-r--r--   0 swryan    (1000) swryan    (1000)     7073 2021-12-12 22:38:56.000000 testflo-1.4.8/README.md
--rw-r--r--   0 swryan    (1000) swryan    (1000)       79 2022-02-14 17:22:43.796443 testflo-1.4.8/setup.cfg
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4885 2021-12-12 22:38:56.000000 testflo-1.4.8/setup.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2022-02-14 17:22:43.796443 testflo-1.4.8/testflo/
--rw-r--r--   0 swryan    (1000) swryan    (1000)       22 2022-02-14 17:21:28.000000 testflo-1.4.8/testflo/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      798 2021-12-12 22:38:56.000000 testflo-1.4.8/testflo/benchmark.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2576 2021-12-12 22:38:56.000000 testflo-1.4.8/testflo/cover.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      238 2021-12-12 22:38:56.000000 testflo-1.4.8/testflo/devnull.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     8478 2021-12-12 22:38:56.000000 testflo-1.4.8/testflo/discover.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1263 2021-12-12 22:38:56.000000 testflo-1.4.8/testflo/filters.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      886 2021-12-12 22:38:56.000000 testflo-1.4.8/testflo/isolatedrun.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     7373 2022-02-14 16:59:21.000000 testflo-1.4.8/testflo/main.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2036 2021-12-12 22:38:56.000000 testflo-1.4.8/testflo/mpirun.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      268 2021-12-12 22:38:56.000000 testflo-1.4.8/testflo/options.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2452 2021-12-12 22:38:56.000000 testflo-1.4.8/testflo/printer.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1459 2021-12-12 22:38:56.000000 testflo-1.4.8/testflo/qman.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4433 2021-12-12 22:38:56.000000 testflo-1.4.8/testflo/runner.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2274 2021-12-12 22:38:56.000000 testflo-1.4.8/testflo/summary.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    13803 2021-12-12 22:38:56.000000 testflo-1.4.8/testflo/test.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    16641 2021-12-12 22:38:56.000000 testflo-1.4.8/testflo/util.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2022-02-14 17:22:43.796443 testflo-1.4.8/testflo.egg-info/
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5010 2022-02-14 17:22:43.000000 testflo-1.4.8/testflo.egg-info/PKG-INFO
--rw-r--r--   0 swryan    (1000) swryan    (1000)      547 2022-02-14 17:22:43.000000 testflo-1.4.8/testflo.egg-info/SOURCES.txt
--rw-r--r--   0 swryan    (1000) swryan    (1000)        1 2022-02-14 17:22:43.000000 testflo-1.4.8/testflo.egg-info/dependency_links.txt
--rw-r--r--   0 swryan    (1000) swryan    (1000)       71 2022-02-14 17:22:43.000000 testflo-1.4.8/testflo.egg-info/entry_points.txt
--rw-r--r--   0 swryan    (1000) swryan    (1000)       13 2022-02-14 17:22:43.000000 testflo-1.4.8/testflo.egg-info/requires.txt
--rw-r--r--   0 swryan    (1000) swryan    (1000)        8 2022-02-14 17:22:43.000000 testflo-1.4.8/testflo.egg-info/top_level.txt
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2022-07-25 18:09:09.121010 testflo-1.4.9/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2175 2021-12-12 22:38:56.000000 testflo-1.4.9/DESIGN.txt
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      554 2021-12-12 22:38:56.000000 testflo-1.4.9/LICENSE.txt
+-rw-r--r--   0 swryan    (1000) swryan    (1000)       82 2021-12-12 22:38:56.000000 testflo-1.4.9/MANIFEST.in
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4469 2022-07-25 18:09:09.121010 testflo-1.4.9/PKG-INFO
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     7073 2021-12-12 22:38:56.000000 testflo-1.4.9/README.md
+-rw-r--r--   0 swryan    (1000) swryan    (1000)       79 2022-07-25 18:09:09.121010 testflo-1.4.9/setup.cfg
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4885 2022-07-25 16:54:24.000000 testflo-1.4.9/setup.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2022-07-25 18:09:09.121010 testflo-1.4.9/testflo/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)       22 2022-07-25 18:08:14.000000 testflo-1.4.9/testflo/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      798 2021-12-12 22:38:56.000000 testflo-1.4.9/testflo/benchmark.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2576 2022-07-25 16:54:24.000000 testflo-1.4.9/testflo/cover.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      238 2021-12-12 22:38:56.000000 testflo-1.4.9/testflo/devnull.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     8478 2021-12-12 22:38:56.000000 testflo-1.4.9/testflo/discover.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1263 2022-07-21 18:19:19.000000 testflo-1.4.9/testflo/duration.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1263 2021-12-12 22:38:56.000000 testflo-1.4.9/testflo/filters.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      886 2022-07-25 16:54:24.000000 testflo-1.4.9/testflo/isolatedrun.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     7690 2022-07-25 16:54:24.000000 testflo-1.4.9/testflo/main.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2036 2022-07-25 16:54:24.000000 testflo-1.4.9/testflo/mpirun.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      268 2021-12-12 22:38:56.000000 testflo-1.4.9/testflo/options.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2452 2021-12-12 22:38:56.000000 testflo-1.4.9/testflo/printer.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1459 2021-12-12 22:38:56.000000 testflo-1.4.9/testflo/qman.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4433 2021-12-12 22:38:56.000000 testflo-1.4.9/testflo/runner.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2274 2021-12-12 22:38:56.000000 testflo-1.4.9/testflo/summary.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    13803 2022-07-21 18:16:33.000000 testflo-1.4.9/testflo/test.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    18072 2022-07-21 18:19:19.000000 testflo-1.4.9/testflo/util.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2022-07-25 18:09:09.121010 testflo-1.4.9/testflo.egg-info/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4469 2022-07-25 18:09:09.000000 testflo-1.4.9/testflo.egg-info/PKG-INFO
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      567 2022-07-25 18:09:09.000000 testflo-1.4.9/testflo.egg-info/SOURCES.txt
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        1 2022-07-25 18:09:09.000000 testflo-1.4.9/testflo.egg-info/dependency_links.txt
+-rw-r--r--   0 swryan    (1000) swryan    (1000)       46 2022-07-25 18:09:09.000000 testflo-1.4.9/testflo.egg-info/entry_points.txt
+-rw-r--r--   0 swryan    (1000) swryan    (1000)       13 2022-07-25 18:09:09.000000 testflo-1.4.9/testflo.egg-info/requires.txt
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        8 2022-07-25 18:09:09.000000 testflo-1.4.9/testflo.egg-info/top_level.txt
```

### Comparing `testflo-1.4.8/DESIGN.txt` & `testflo-1.4.9/DESIGN.txt`

 * *Files identical despite different names*

### Comparing `testflo-1.4.8/LICENSE.txt` & `testflo-1.4.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `testflo-1.4.8/PKG-INFO` & `testflo-1.4.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,81 +1,79 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: testflo
-Version: 1.4.8
+Version: 1.4.9
 Summary: A simple flow-based testing framework
-Home-page: UNKNOWN
-Author: UNKNOWN
-Author-email: UNKNOWN
 License: Apache 2.0
-Description: 
-                usage: testflo [options]
-        
-                positional arguments:
-                  test                  A test method, test case, module, or directory to run.
-        
-                optional arguments:
-                  -h, --help            show this help message and exit
-                  -c FILE, --config FILE
-                                        Path of config file where preferences are specified.
-                  -t FILE, --testfile FILE
-                                        Path to a file containing one testspec per line.
-                  --maxtime TIME_LIMIT  Specifies a time limit in seconds for tests to be
-                                        saved to the quicktests.in file.
-                  -n NUM_PROCS, --numprocs NUM_PROCS
-                                        Number of processes to run. By default, this will use
-                                        the number of CPUs available. To force serial
-                                        execution, specify a value of 1.
-                  -o FILE, --outfile FILE
-                                        Name of test report file. Default is
-                                        testflo_report.out.
-                  -v, --verbose         Include testspec and elapsed time in screen output.
-                                        Also shows all stderr output, even if test doesn't
-                                        fail
-                  --compact             Limit output to a single character for each test.
-                  --dryrun              Don't actually run tests, but print which tests would
-                                        have been run.
-                  --pre_announce        Announce the name of each test before it runs. This
-                                        can help track down a hanging test. This automatically
-                                        sets -n 1.
-                  -f, --fail            Save failed tests to failtests.in file.
-                  --full_path           Display full test specs instead of shortened names.
-                  -i, --isolated        Run each test in a separate subprocess.
-                  --nompi               Force all tests to run without MPI. This can be useful
-                                        for debugging.
-                  -x, --stop            Stop after the first test failure, or as soon as
-                                        possible when running concurrent tests.
-                  -s, --nocapture       Standard output (stdout) will not be captured and will
-                                        be written to the screen immediately.
-                  --coverage            Perform coverage analysis and display results on
-                                        stdout
-                  --coverage-html       Perform coverage analysis and display results in
-                                        browser
-                  --coverpkg PKG        Add the given package to the coverage list. You can
-                                        use this option multiple times to cover multiple
-                                        packages.
-                  --cover-omit FILE     Add a file name pattern to remove it from coverage.
-                  -b, --benchmark       Specifies that benchmarks are to be run rather than
-                                        tests, so only files starting with "benchmark\_" will
-                                        be executed.
-                  -d FILE, --datafile FILE
-                                        Name of benchmark data file. Default is
-                                        benchmark_data.csv.
-                  --noreport            Don't create a test results file.
-                  -m GLOB, --match GLOB, --testmatch GLOB
-                                        Pattern to use for test discovery. Multiple patterns
-                                        are allowed.
-                  --timeout TIMEOUT     Timeout in seconds. Test will be terminated if it
-                                        takes longer than timeout. Only works for tests
-                                        running in a subprocess (MPI and isolated).
-              
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
+License-File: LICENSE.txt
+
+
+        usage: testflo [options]
+
+        positional arguments:
+          test                  A test method, test case, module, or directory to run.
+
+        optional arguments:
+          -h, --help            show this help message and exit
+          -c FILE, --config FILE
+                                Path of config file where preferences are specified.
+          -t FILE, --testfile FILE
+                                Path to a file containing one testspec per line.
+          --maxtime TIME_LIMIT  Specifies a time limit in seconds for tests to be
+                                saved to the quicktests.in file.
+          -n NUM_PROCS, --numprocs NUM_PROCS
+                                Number of processes to run. By default, this will use
+                                the number of CPUs available. To force serial
+                                execution, specify a value of 1.
+          -o FILE, --outfile FILE
+                                Name of test report file. Default is
+                                testflo_report.out.
+          -v, --verbose         Include testspec and elapsed time in screen output.
+                                Also shows all stderr output, even if test doesn't
+                                fail
+          --compact             Limit output to a single character for each test.
+          --dryrun              Don't actually run tests, but print which tests would
+                                have been run.
+          --pre_announce        Announce the name of each test before it runs. This
+                                can help track down a hanging test. This automatically
+                                sets -n 1.
+          -f, --fail            Save failed tests to failtests.in file.
+          --full_path           Display full test specs instead of shortened names.
+          -i, --isolated        Run each test in a separate subprocess.
+          --nompi               Force all tests to run without MPI. This can be useful
+                                for debugging.
+          -x, --stop            Stop after the first test failure, or as soon as
+                                possible when running concurrent tests.
+          -s, --nocapture       Standard output (stdout) will not be captured and will
+                                be written to the screen immediately.
+          --coverage            Perform coverage analysis and display results on
+                                stdout
+          --coverage-html       Perform coverage analysis and display results in
+                                browser
+          --coverpkg PKG        Add the given package to the coverage list. You can
+                                use this option multiple times to cover multiple
+                                packages.
+          --cover-omit FILE     Add a file name pattern to remove it from coverage.
+          -b, --benchmark       Specifies that benchmarks are to be run rather than
+                                tests, so only files starting with "benchmark\_" will
+                                be executed.
+          -d FILE, --datafile FILE
+                                Name of benchmark data file. Default is
+                                benchmark_data.csv.
+          --noreport            Don't create a test results file.
+          -m GLOB, --match GLOB, --testmatch GLOB
+                                Pattern to use for test discovery. Multiple patterns
+                                are allowed.
+          --timeout TIMEOUT     Timeout in seconds. Test will be terminated if it
+                                takes longer than timeout. Only works for tests
+                                running in a subprocess (MPI and isolated).
+
```

### Comparing `testflo-1.4.8/README.md` & `testflo-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `testflo-1.4.8/setup.py` & `testflo-1.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `testflo-1.4.8/testflo/benchmark.py` & `testflo-1.4.9/testflo/benchmark.py`

 * *Files identical despite different names*

### Comparing `testflo-1.4.8/testflo/cover.py` & `testflo-1.4.9/testflo/cover.py`

 * *Files identical despite different names*

### Comparing `testflo-1.4.8/testflo/discover.py` & `testflo-1.4.9/testflo/discover.py`

 * *Files identical despite different names*

### Comparing `testflo-1.4.8/testflo/filters.py` & `testflo-1.4.9/testflo/filters.py`

 * *Files identical despite different names*

### Comparing `testflo-1.4.8/testflo/isolatedrun.py` & `testflo-1.4.9/testflo/isolatedrun.py`

 * *Files identical despite different names*

### Comparing `testflo-1.4.8/testflo/main.py` & `testflo-1.4.9/testflo/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,18 +33,19 @@
 from fnmatch import fnmatch, fnmatchcase
 
 import testflo
 from testflo.runner import ConcurrentTestRunner
 from testflo.printer import ResultPrinter
 from testflo.benchmark import BenchmarkWriter
 from testflo.summary import ResultSummary
+from testflo.duration import DurationSummary
 from testflo.discover import TestDiscoverer
 from testflo.filters import TimeFilter, FailFilter
 
-from testflo.util import read_config_file, read_test_file
+from testflo.util import read_config_file, read_test_file, _get_parser
 from testflo.cover import setup_coverage, finalize_coverage
 from testflo.options import get_options
 from testflo.qman import get_server_queue
 
 options = get_options()
 
 
@@ -111,14 +112,15 @@
     rcfile = os.path.join(homedir, '.testflo')
     if not os.path.isfile(rcfile):
         with open(rcfile, 'w') as f:
             f.write("""[testflo]
 skip_dirs=site-packages,
     dist-packages,
     build,
+    _build,
     contrib
 """)
     read_config_file(rcfile, options)
     if options.cfg:
         read_config_file(options.cfg, options)
 
     if nprocs is None and options.num_procs is None:
@@ -135,16 +137,17 @@
     if options.testfile:
         tests += list(read_test_file(options.testfile))
 
     if not tests:
         tests = [os.getcwd()]
 
     def dir_exclude(d):
+        base = os.path.basename(d)
         for skip in options.skip_dirs:
-            if fnmatch(os.path.basename(d), skip):
+            if fnmatch(base, skip):
                 return True
         return False
 
     # set this so code will know when it's running under testflo
     os.environ['TESTFLO_RUNNING'] = '1'
 
     setup_coverage(options)
@@ -202,25 +205,31 @@
             runner = ConcurrentTestRunner(options, queue)
 
             pipeline.append(runner.get_iter)
 
             if options.benchmark:
                 pipeline.append(BenchmarkWriter(stream=bdata).get_iter)
 
+            if options.durations:
+                pipeline.append(DurationSummary(options).get_iter)
+
             if options.compact:
                 verbose = -1
             else:
                 verbose = int(options.verbose)
 
             pipeline.extend([
                 ResultPrinter(options, verbose=verbose).get_iter,
                 ResultSummary(options).get_iter,
             ])
             if not options.noreport:
                 # print verbose results and summary to a report file
+                if options.durations:
+                    pipeline.append(DurationSummary(options, stream=report).get_iter)
+
                 pipeline.extend([
                     ResultPrinter(options, report, verbose=1).get_iter,
                     ResultSummary(options, stream=report).get_iter,
                 ])
 
         if options.maxtime > 0:
             pipeline.append(TimeFilter(options.maxtime).get_iter)
```

### Comparing `testflo-1.4.8/testflo/mpirun.py` & `testflo-1.4.9/testflo/mpirun.py`

 * *Files identical despite different names*

### Comparing `testflo-1.4.8/testflo/printer.py` & `testflo-1.4.9/testflo/printer.py`

 * *Files identical despite different names*

### Comparing `testflo-1.4.8/testflo/qman.py` & `testflo-1.4.9/testflo/qman.py`

 * *Files identical despite different names*

### Comparing `testflo-1.4.8/testflo/runner.py` & `testflo-1.4.9/testflo/runner.py`

 * *Files identical despite different names*

### Comparing `testflo-1.4.8/testflo/summary.py` & `testflo-1.4.9/testflo/summary.py`

 * *Files identical despite different names*

### Comparing `testflo-1.4.8/testflo/test.py` & `testflo-1.4.9/testflo/test.py`

 * *Files identical despite different names*

### Comparing `testflo-1.4.8/testflo/util.py` & `testflo-1.4.9/testflo/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 Misc. utility routines.
 """
 
 import os
 import sys
 import itertools
 import inspect
-import warnings
 import importlib
+import warnings
 from importlib import import_module
 
 from configparser import ConfigParser
 
 from fnmatch import fnmatch
 from os.path import join, dirname, basename, isfile,  abspath, split, splitext
 
-from argparse import ArgumentParser
+from argparse import ArgumentParser, _AppendAction
 
 from testflo.cover import start_coverage, stop_coverage
 
 _store = {}
 
 
 def _get_parser():
@@ -91,14 +91,22 @@
                         help='Specifies that benchmarks are to be run rather '
                              'than tests, so only files starting with "benchmark_" '
                              'will be executed.')
     parser.add_argument('-d', '--datafile', action='store', dest='benchmarkfile',
                         metavar='FILE', default='benchmark_data.csv',
                         help='Name of benchmark data file.  Default is benchmark_data.csv.')
 
+    parser.add_argument('--durations', action='store', type=int, dest='durations', default=0,
+                        metavar='NUM',
+                        help="Display 'NUM' tests with longest durations.")
+
+    parser.add_argument('--durations-min', action='store', type=float, dest='durations_min',
+                        default=0.005, metavar='MIN_TIME',
+                        help='Specify the minimum duration test to include in the durations list.')
+
     parser.add_argument('--noreport', action='store_true', dest='noreport',
                         help="Don't create a test results file.")
 
     parser.add_argument('--show_skipped', action='store_true', dest='show_skipped',
                         help="Display a list of any skipped tests in the summary.")
 
     parser.add_argument('--disallow_skipped', action='store_true', dest='disallow_skipped',
@@ -112,17 +120,22 @@
                         metavar='GLOB',
                         help='Pattern to use for test discovery. Multiple patterns are allowed.',
                         default=[])
 
     parser.add_argument('--exclude', action='append', dest='excludes', metavar='GLOB', default=[],
                         help="Pattern to exclude test functions. Multiple patterns are allowed.")
 
-    parser.add_argument('--timeout', action='store', dest='timeout', type=float,
-                        help='Timeout in seconds. Test will be terminated if it takes longer than timeout. Only'
-                             ' works for tests running in a subprocess (MPI and isolated).')
+    parser.add_argument('--skip_dir', action='append', dest='skip_dirs', metavar='GLOB', default=[],
+                        help="Pattern to skip directories. Multiple patterns are allowed. Patterns "
+                        "are applied only to local dir names, not full paths.")
+
+    parser.add_argument('--timeout', action='store', dest='timeout', type=float, metavar='TIME_LIMIT',
+                        help="Timeout in seconds. A test will be terminated if it takes longer than "
+                             "'TIME_LIMIT'. Only works for tests running in a subprocess "
+                             "(MPI or isolated).")
 
     return parser
 
 
 def _options2args():
     """Gets the testflo args that should be used in subprocesses."""
 
@@ -389,27 +402,51 @@
                 line = line[:idx]
 
             line = line.strip()
             if line:
                 yield line
 
 
+_parser_types = None
+
+
+def _get_parser_action_map():
+    global _parser_types
+
+    if _parser_types is None:
+        _parser_types = {}
+        p = _get_parser()
+        for action in p._actions:
+            _parser_types[action.dest] = action
+
+    return _parser_types
+
+
 def read_config_file(cfgfile, options):
     config = ConfigParser()
-    config.readfp(open(cfgfile))
+    config.read_file(open(cfgfile), source=cfgfile)
 
-    if config.has_option('testflo', 'skip_dirs'):
-        skips = config.get('testflo', 'skip_dirs')
-        options.skip_dirs = [s.strip() for s in skips.split(',') if s.strip()]
+    if 'testflo' in config:
+        parser_map = _get_parser_action_map()
 
-    if config.has_option('testflo', 'num_procs'):
-        options.num_procs = int(config.get('testflo', 'num_procs'))
+        for name, optstr in config['testflo'].items():
+            if name not in parser_map:
+                warnings.warn("Unknown option '{}' in testflo config file '{}'.".format(name,
+                                                                                        cfgfile))
+                continue
+
+            action = parser_map[name]
+            typ = action.type
+            if typ is None:
+                typ = lambda x: x
 
-    if config.has_option('testflo', 'noreport'):
-        options.noreport = bool(config.get('testflo', 'noreport'))
+            if isinstance(action, _AppendAction):
+                setattr(options, name, [typ(s.strip()) for s in optstr.split(',') if s.strip()])
+            else:
+                setattr(options, name, typ(optstr))
 
 
 def get_memory_usage():
     """return memory usage for the current process"""
     k = 1024.
     try:
         # prefer psutil, it works on all platforms including Windows
```

### Comparing `testflo-1.4.8/testflo.egg-info/PKG-INFO` & `testflo-1.4.9/testflo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,81 +1,79 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: testflo
-Version: 1.4.8
+Version: 1.4.9
 Summary: A simple flow-based testing framework
-Home-page: UNKNOWN
-Author: UNKNOWN
-Author-email: UNKNOWN
 License: Apache 2.0
-Description: 
-                usage: testflo [options]
-        
-                positional arguments:
-                  test                  A test method, test case, module, or directory to run.
-        
-                optional arguments:
-                  -h, --help            show this help message and exit
-                  -c FILE, --config FILE
-                                        Path of config file where preferences are specified.
-                  -t FILE, --testfile FILE
-                                        Path to a file containing one testspec per line.
-                  --maxtime TIME_LIMIT  Specifies a time limit in seconds for tests to be
-                                        saved to the quicktests.in file.
-                  -n NUM_PROCS, --numprocs NUM_PROCS
-                                        Number of processes to run. By default, this will use
-                                        the number of CPUs available. To force serial
-                                        execution, specify a value of 1.
-                  -o FILE, --outfile FILE
-                                        Name of test report file. Default is
-                                        testflo_report.out.
-                  -v, --verbose         Include testspec and elapsed time in screen output.
-                                        Also shows all stderr output, even if test doesn't
-                                        fail
-                  --compact             Limit output to a single character for each test.
-                  --dryrun              Don't actually run tests, but print which tests would
-                                        have been run.
-                  --pre_announce        Announce the name of each test before it runs. This
-                                        can help track down a hanging test. This automatically
-                                        sets -n 1.
-                  -f, --fail            Save failed tests to failtests.in file.
-                  --full_path           Display full test specs instead of shortened names.
-                  -i, --isolated        Run each test in a separate subprocess.
-                  --nompi               Force all tests to run without MPI. This can be useful
-                                        for debugging.
-                  -x, --stop            Stop after the first test failure, or as soon as
-                                        possible when running concurrent tests.
-                  -s, --nocapture       Standard output (stdout) will not be captured and will
-                                        be written to the screen immediately.
-                  --coverage            Perform coverage analysis and display results on
-                                        stdout
-                  --coverage-html       Perform coverage analysis and display results in
-                                        browser
-                  --coverpkg PKG        Add the given package to the coverage list. You can
-                                        use this option multiple times to cover multiple
-                                        packages.
-                  --cover-omit FILE     Add a file name pattern to remove it from coverage.
-                  -b, --benchmark       Specifies that benchmarks are to be run rather than
-                                        tests, so only files starting with "benchmark\_" will
-                                        be executed.
-                  -d FILE, --datafile FILE
-                                        Name of benchmark data file. Default is
-                                        benchmark_data.csv.
-                  --noreport            Don't create a test results file.
-                  -m GLOB, --match GLOB, --testmatch GLOB
-                                        Pattern to use for test discovery. Multiple patterns
-                                        are allowed.
-                  --timeout TIMEOUT     Timeout in seconds. Test will be terminated if it
-                                        takes longer than timeout. Only works for tests
-                                        running in a subprocess (MPI and isolated).
-              
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
+License-File: LICENSE.txt
+
+
+        usage: testflo [options]
+
+        positional arguments:
+          test                  A test method, test case, module, or directory to run.
+
+        optional arguments:
+          -h, --help            show this help message and exit
+          -c FILE, --config FILE
+                                Path of config file where preferences are specified.
+          -t FILE, --testfile FILE
+                                Path to a file containing one testspec per line.
+          --maxtime TIME_LIMIT  Specifies a time limit in seconds for tests to be
+                                saved to the quicktests.in file.
+          -n NUM_PROCS, --numprocs NUM_PROCS
+                                Number of processes to run. By default, this will use
+                                the number of CPUs available. To force serial
+                                execution, specify a value of 1.
+          -o FILE, --outfile FILE
+                                Name of test report file. Default is
+                                testflo_report.out.
+          -v, --verbose         Include testspec and elapsed time in screen output.
+                                Also shows all stderr output, even if test doesn't
+                                fail
+          --compact             Limit output to a single character for each test.
+          --dryrun              Don't actually run tests, but print which tests would
+                                have been run.
+          --pre_announce        Announce the name of each test before it runs. This
+                                can help track down a hanging test. This automatically
+                                sets -n 1.
+          -f, --fail            Save failed tests to failtests.in file.
+          --full_path           Display full test specs instead of shortened names.
+          -i, --isolated        Run each test in a separate subprocess.
+          --nompi               Force all tests to run without MPI. This can be useful
+                                for debugging.
+          -x, --stop            Stop after the first test failure, or as soon as
+                                possible when running concurrent tests.
+          -s, --nocapture       Standard output (stdout) will not be captured and will
+                                be written to the screen immediately.
+          --coverage            Perform coverage analysis and display results on
+                                stdout
+          --coverage-html       Perform coverage analysis and display results in
+                                browser
+          --coverpkg PKG        Add the given package to the coverage list. You can
+                                use this option multiple times to cover multiple
+                                packages.
+          --cover-omit FILE     Add a file name pattern to remove it from coverage.
+          -b, --benchmark       Specifies that benchmarks are to be run rather than
+                                tests, so only files starting with "benchmark\_" will
+                                be executed.
+          -d FILE, --datafile FILE
+                                Name of benchmark data file. Default is
+                                benchmark_data.csv.
+          --noreport            Don't create a test results file.
+          -m GLOB, --match GLOB, --testmatch GLOB
+                                Pattern to use for test discovery. Multiple patterns
+                                are allowed.
+          --timeout TIMEOUT     Timeout in seconds. Test will be terminated if it
+                                takes longer than timeout. Only works for tests
+                                running in a subprocess (MPI and isolated).
+
```

### Comparing `testflo-1.4.8/testflo.egg-info/SOURCES.txt` & `testflo-1.4.9/testflo.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 setup.cfg
 setup.py
 testflo/__init__.py
 testflo/benchmark.py
 testflo/cover.py
 testflo/devnull.py
 testflo/discover.py
+testflo/duration.py
 testflo/filters.py
 testflo/isolatedrun.py
 testflo/main.py
 testflo/mpirun.py
 testflo/options.py
 testflo/printer.py
 testflo/qman.py
```

