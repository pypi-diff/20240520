# Comparing `tmp/jobqueues-0.9.3.tar.gz` & `tmp/jobqueues-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobqueues-0.9.3.tar", last modified: Fri May 10 08:43:43 2024, max compression
+gzip compressed data, was "jobqueues-0.9.4.tar", last modified: Mon May 20 12:15:53 2024, max compression
```

## Comparing `jobqueues-0.9.3.tar` & `jobqueues-0.9.4.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:43:43.813156 jobqueues-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-10 08:42:48.000000 jobqueues-0.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-10 08:43:43.813156 jobqueues-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-10 08:42:48.000000 jobqueues-0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:43:43.813156 jobqueues-0.9.3/jobqueues/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-10 08:43:43.813156 jobqueues-0.9.3/jobqueues/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:43:43.813156 jobqueues-0.9.3/jobqueues/celeryfiles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/celeryfiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/celeryfiles/celery.py
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/celeryfiles/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/celeryqueue.py
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/config_lsf.yml
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/config_slurm.yml
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/home.py
--rw-r--r--   0 runner    (1001) docker     (127)    14057 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/localqueue.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/logging.ini
--rw-r--r--   0 runner    (1001) docker     (127)    14566 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/lsfqueue.py
--rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/pbsqueue.py
--rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/playqueue.py
--rw-r--r--   0 runner    (1001) docker     (127)    12161 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/sgequeue.py
--rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/simqueue.py
--rw-r--r--   0 runner    (1001) docker     (127)    26717 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/slurmqueue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:43:43.813156 jobqueues-0.9.3/jobqueues/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/templates/SGE_job.sh.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/templates/SLURM_job.sh.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-10 08:42:48.000000 jobqueues-0.9.3/jobqueues/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:43:43.813156 jobqueues-0.9.3/jobqueues.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-10 08:43:43.000000 jobqueues-0.9.3/jobqueues.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-10 08:43:43.000000 jobqueues-0.9.3/jobqueues.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:43:43.000000 jobqueues-0.9.3/jobqueues.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:43:35.000000 jobqueues-0.9.3/jobqueues.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-10 08:43:43.000000 jobqueues-0.9.3/jobqueues.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 08:43:43.000000 jobqueues-0.9.3/jobqueues.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-10 08:42:48.000000 jobqueues-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-10 08:43:43.813156 jobqueues-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-10 08:42:48.000000 jobqueues-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:15:53.408791 jobqueues-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-20 12:14:53.000000 jobqueues-0.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-20 12:15:53.408791 jobqueues-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-20 12:14:53.000000 jobqueues-0.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:15:53.408791 jobqueues-0.9.4/jobqueues/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-20 12:14:53.000000 jobqueues-0.9.4/jobqueues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-20 12:15:53.408791 jobqueues-0.9.4/jobqueues/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:15:53.408791 jobqueues-0.9.4/jobqueues/celeryfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 12:14:53.000000 jobqueues-0.9.4/jobqueues/celeryfiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-20 12:14:53.000000 jobqueues-0.9.4/jobqueues/celeryfiles/celery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-05-20 12:14:53.000000 jobqueues-0.9.4/jobqueues/celeryfiles/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-05-20 12:14:53.000000 jobqueues-0.9.4/jobqueues/celeryqueue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-20 12:14:53.000000 jobqueues-0.9.4/jobqueues/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-20 12:14:53.000000 jobqueues-0.9.4/jobqueues/config_lsf.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-20 12:14:53.000000 jobqueues-0.9.4/jobqueues/config_slurm.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-20 12:14:53.000000 jobqueues-0.9.4/jobqueues/home.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14057 2024-05-20 12:14:53.000000 jobqueues-0.9.4/jobqueues/localqueue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-20 12:14:53.000000 jobqueues-0.9.4/jobqueues/logging.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    14566 2024-05-20 12:14:53.000000 jobqueues-0.9.4/jobqueues/lsfqueue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-05-20 12:14:53.000000 jobqueues-0.9.4/jobqueues/pbsqueue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-05-20 12:14:53.000000 jobqueues-0.9.4/jobqueues/playqueue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12161 2024-05-20 12:14:53.000000 jobqueues-0.9.4/jobqueues/sgequeue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-05-20 12:14:53.000000 jobqueues-0.9.4/jobqueues/simqueue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20764 2024-05-20 12:14:53.000000 jobqueues-0.9.4/jobqueues/slurmqueue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:15:53.408791 jobqueues-0.9.4/jobqueues/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-20 12:14:53.000000 jobqueues-0.9.4/jobqueues/templates/SGE_job.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-20 12:14:53.000000 jobqueues-0.9.4/jobqueues/templates/SLURM_job.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-20 12:14:53.000000 jobqueues-0.9.4/jobqueues/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:15:53.408791 jobqueues-0.9.4/jobqueues.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-20 12:15:53.000000 jobqueues-0.9.4/jobqueues.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-20 12:15:53.000000 jobqueues-0.9.4/jobqueues.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 12:15:53.000000 jobqueues-0.9.4/jobqueues.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 12:15:45.000000 jobqueues-0.9.4/jobqueues.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-20 12:15:53.000000 jobqueues-0.9.4/jobqueues.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 12:15:53.000000 jobqueues-0.9.4/jobqueues.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-20 12:14:53.000000 jobqueues-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-20 12:15:53.408791 jobqueues-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-20 12:14:53.000000 jobqueues-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:15:53.408791 jobqueues-0.9.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-05-20 12:14:53.000000 jobqueues-0.9.4/tests/test_slurmqueue.py
```

### Comparing `jobqueues-0.9.3/PKG-INFO` & `jobqueues-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobqueues
-Version: 0.9.3
+Version: 0.9.4
 Summary: Wrappers for various queueing systems in python
 Author-email: Acellera <info@acellera.com>
 Project-URL: Homepage, https://github.com/Acellera/jobqueues
 Project-URL: Bug Tracker, https://github.com/Acellera/jobqueues/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
```

### Comparing `jobqueues-0.9.3/jobqueues/celeryfiles/tasks.py` & `jobqueues-0.9.4/jobqueues/celeryfiles/tasks.py`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.3/jobqueues/celeryqueue.py` & `jobqueues-0.9.4/jobqueues/celeryqueue.py`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.3/jobqueues/config.py` & `jobqueues-0.9.4/jobqueues/config.py`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.3/jobqueues/home.py` & `jobqueues-0.9.4/jobqueues/home.py`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.3/jobqueues/localqueue.py` & `jobqueues-0.9.4/jobqueues/localqueue.py`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.3/jobqueues/lsfqueue.py` & `jobqueues-0.9.4/jobqueues/lsfqueue.py`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.3/jobqueues/pbsqueue.py` & `jobqueues-0.9.4/jobqueues/pbsqueue.py`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.3/jobqueues/playqueue.py` & `jobqueues-0.9.4/jobqueues/playqueue.py`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.3/jobqueues/sgequeue.py` & `jobqueues-0.9.4/jobqueues/sgequeue.py`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.3/jobqueues/simqueue.py` & `jobqueues-0.9.4/jobqueues/simqueue.py`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.3/jobqueues/slurmqueue.py` & `jobqueues-0.9.4/jobqueues/slurmqueue.py`

 * *Files 20% similar despite different names*

```diff
@@ -324,17 +324,19 @@
                 return None
             raise FileNotFoundError(
                 "Could not find required executable [{}]".format(binary)
             )
         ret = os.path.abspath(ret)
         return ret
 
-    def _createJobScript(self, fname, workdir, runsh):
+    def _createJobScript(self, fname, workdir, runsh, nvidia_mps=False):
         from jobqueues.config import template_env
 
+        runsh = ensurelist(runsh)
+
         workdir = os.path.abspath(workdir)
         sentinel = os.path.normpath(os.path.join(workdir, self._sentinel))
 
         # Move completed trajectories
         odir = None
         if self.datadir is not None:
             simname = os.path.basename(os.path.normpath(workdir))
@@ -388,43 +390,73 @@
             trajext=self.trajext,
             nodes=self.nodes,
             ntasks=self.ntasks,
             ntasks_per_node=self.ntasks_per_node,
             ntasks_per_core=self.ntasks_per_core,
             cpus_per_task=self.cpus_per_task,
             constraint=self.constraint,
+            run_as_daemon=len(runsh) > 1,
+            nvidia_mps=nvidia_mps,
         )
         with open(fname, "w") as f:
             f.write(job_str)
         os.chmod(fname, 0o700)
 
     def retrieve(self):
         # Nothing to do
         pass
 
     def _autoJobName(self, path):
+        path = ensurelist(path)
         return (
-            os.path.basename(os.path.abspath(path))
+            "_".join([os.path.basename(os.path.abspath(x)) for x in path])
             + "_"
             + "".join([random.choice(string.digits) for _ in range(5)])
         )
 
-    def submit(self, dirs, commands=None, _dryrun=False):
+    def submit(self, dirs, commands=None, _dryrun=False, nvidia_mps=False):
         """Submits all directories
 
         Parameters
         ----------
         dirs : list
             A list of executable directories.
+        nvidia_mps : bool
+            Whether to use Nvidia's Multi-Process Service (MPS) to share GPU resources among all jobs in `dirs`.
         """
         dirs = self._submitinit(dirs)
 
         if self.partition is None:
             raise ValueError("The partition needs to be defined.")
 
+        if nvidia_mps:
+            logger.info(f"Queueing single job with directories {dirs}")
+            if self.jobname is None:
+                self.jobname = self._autoJobName(dirs)
+
+            runscripts = []
+            for d in dirs:
+                runscripts.append(self._getRunScript(d))
+                self._cleanSentinel(d)
+
+            jobscript = os.path.abspath(os.path.join(dirs[0], self.jobscript))
+            self._createJobScript(jobscript, dirs[0], runscripts, nvidia_mps=True)
+            try:
+                if _dryrun:
+                    logger.info(f"Dry run. Here it would call submit on {jobscript}")
+                else:
+                    ret = check_output([self._qsubmit, jobscript])
+                    logger.debug(ret.decode("ascii"))
+            except CalledProcessError as e:
+                logger.error(e.output)
+                raise
+            except Exception:
+                raise
+            return
+
         # if all folders exist, submit
         for i, d in enumerate(dirs):
             logger.info("Queueing " + d)
 
             if self.jobname is None:
                 self.jobname = self._autoJobName(d)
 
@@ -594,206 +626,7 @@
     @property
     def memory(self):
         return self.__dict__["memory"]
 
     @memory.setter
     def memory(self, value):
         self.memory = value
-
-
-class _TestSlurmQueue(unittest.TestCase):
-    def test_config(self):
-        from jobqueues.home import home
-        import os
-
-        configfile = os.path.join(home(), "config_slurm.yml")
-        with open(configfile, "r") as f:
-            reference = yaml.load(f, Loader=yaml.FullLoader)
-
-        for appkey in reference:
-            sq = SlurmQueue(
-                _configapp=appkey, _configfile=configfile, _findExecutables=False
-            )
-            for key in reference[appkey]:
-                assert (
-                    sq.__getattribute__(key) == reference[appkey][key]
-                ), f'Config setup of SlurmQueue failed on app "{appkey}" and key "{key}""'
-
-    def test_submit_command(self):
-        import tempfile
-
-        with tempfile.TemporaryDirectory() as tmpdir:
-            sl = SlurmQueue(_findExecutables=False)
-            sl.partition = "jobqueues_test"
-            sl.ngpu = 2
-            sl.gpumemory = 2000
-            sl.exclude = ["node1", "node4"]
-            sl.nodelist = ["node2"]
-            sl.envvars = "TEST=3"
-            sl.useworkdir = False
-            try:
-                sl.submit([tmpdir], commands=["sleep 5"])
-            except Exception as e:
-                print(e)
-                pass
-
-            with open(os.path.join(tmpdir, "job.sh"), "r") as f:
-                joblines = f.readlines()
-
-            reflines = [
-                "#!/bin/bash\n",
-                "#\n",
-                "#SBATCH --job-name=tmpwnq0uoqw_28851\n",
-                "#SBATCH --partition=jobqueues_test\n",
-                "#SBATCH --cpus-per-task=1\n",
-                "#SBATCH --mem=1000\n",
-                "#SBATCH --priority=None\n",
-                "#SBATCH -D /tmp/\n",
-                "#SBATCH --gres=gpu:2,gpu_mem:2000\n",
-                "#SBATCH --export=TEST=3\n",
-                "#SBATCH --nodelist=node2\n",
-                "#SBATCH --exclude=node1,node4\n",
-                "\n",
-                "\n",
-                "\n",
-                "sleep 5\n",
-                "\n",
-            ]
-            skiplines = [2]
-
-            assert len(joblines) == len(reflines)
-            for i, (l1, l2) in enumerate(zip(reflines, joblines)):
-                if i in skiplines:
-                    continue
-                assert (
-                    l1 == l2
-                ), f"Difference found in line {i} of job file: {l1} vs {l2}"
-
-    def test_submit_folder(self):
-        import tempfile
-
-        with tempfile.TemporaryDirectory() as tmpdir:
-            with open(os.path.join(tmpdir, "run.sh"), "w") as f:
-                f.write("sleep 5")
-            os.chmod(os.path.join(tmpdir, "run.sh"), 0o700)
-
-            sl = SlurmQueue(_findExecutables=False)
-            sl.partition = "jobqueues_test"
-            sl.ngpu = 2
-            sl.gpumemory = 2000
-            sl.exclude = ["node1", "node4"]
-            sl.nodelist = ["node2"]
-            sl.envvars = "TEST=3"
-            try:
-                sl.submit(tmpdir)
-            except Exception as e:
-                print(e)
-                pass
-
-            with open(os.path.join(tmpdir, "job.sh"), "r") as f:
-                joblines = f.readlines()
-
-            donefile = os.path.join("tmpdir", "jobqueues.done")
-            runfile = os.path.join("tmpdir", "run.sh")
-            reflines = [
-                "#!/bin/bash\n",
-                "#\n",
-                "#SBATCH --job-name=tmp8dj2zuya_44185\n",
-                "#SBATCH --partition=jobqueues_test\n",
-                "#SBATCH --cpus-per-task=1\n",
-                "#SBATCH --mem=1000\n",
-                "#SBATCH --priority=None\n",
-                "#SBATCH -D tmpdir\n",
-                "#SBATCH --gres=gpu:2,gpu_mem:2000\n",
-                "#SBATCH --output=slurm.%N.%j.out\n",
-                "#SBATCH --error=slurm.%N.%j.err\n",
-                "#SBATCH --export=TEST=3\n",
-                "#SBATCH --nodelist=node2\n",
-                "#SBATCH --exclude=node1,node4\n",
-                "\n",
-                f'trap "touch {donefile}" EXIT SIGTERM\n',
-                "\n",
-                "cd tmpdir\n",
-                "\n",
-                f"{runfile}\n",
-                "\n",
-            ]
-            skiplines = [2]
-
-            assert len(joblines) == len(reflines)
-            for i, (l1, l2) in enumerate(zip(reflines, joblines)):
-                l1 = l1.replace(tmpdir, "tmpdir")
-                l2 = l2.replace(tmpdir, "tmpdir")
-                if i in skiplines:
-                    continue
-                assert (
-                    l1 == l2
-                ), f"Difference found in line {i} of job file: {l1} vs {l2}"
-
-    def test_submit_multi_folder(self):
-        import tempfile
-
-        with tempfile.TemporaryDirectory() as tmpdir:
-            sl = SlurmQueue(_findExecutables=False)
-            sl.partition = "jobqueues_test"
-            sl.ngpu = 2
-            sl.gpumemory = 2000
-            sl.exclude = ["node1", "node4"]
-            sl.nodelist = ["node2"]
-            sl.envvars = "TEST=3"
-
-            for i in range(2):
-                subdir = os.path.join(tmpdir, str(i))
-                os.makedirs(subdir, exist_ok=True)
-                with open(os.path.join(subdir, "run.sh"), "w") as f:
-                    f.write("sleep 5")
-                os.chmod(os.path.join(subdir, "run.sh"), 0o700)
-
-                try:
-                    sl.submit(subdir)
-                except Exception as e:
-                    print(e)
-                    pass
-
-                with open(os.path.join(subdir, "job.sh"), "r") as f:
-                    joblines = f.readlines()
-
-                donefile = os.path.join("tmpdir", "jobqueues.done")
-                runfile = os.path.join("tmpdir", "run.sh")
-                reflines = [
-                    "#!/bin/bash\n",
-                    "#\n",
-                    "#SBATCH --job-name=tmp8dj2zuya_44185\n",
-                    "#SBATCH --partition=jobqueues_test\n",
-                    "#SBATCH --cpus-per-task=1\n",
-                    "#SBATCH --mem=1000\n",
-                    "#SBATCH --priority=None\n",
-                    "#SBATCH -D tmpdir\n",
-                    "#SBATCH --gres=gpu:2,gpu_mem:2000\n",
-                    "#SBATCH --output=slurm.%N.%j.out\n",
-                    "#SBATCH --error=slurm.%N.%j.err\n",
-                    "#SBATCH --export=TEST=3\n",
-                    "#SBATCH --nodelist=node2\n",
-                    "#SBATCH --exclude=node1,node4\n",
-                    "\n",
-                    f'trap "touch {donefile}" EXIT SIGTERM\n',
-                    "\n",
-                    "cd tmpdir\n",
-                    "\n",
-                    f"{runfile}\n",
-                    "\n",
-                ]
-                skiplines = [2]
-
-                assert len(joblines) == len(reflines)
-                for i, (l1, l2) in enumerate(zip(reflines, joblines)):
-                    l1 = l1.replace(subdir, "tmpdir")
-                    l2 = l2.replace(subdir, "tmpdir")
-                    if i in skiplines:
-                        continue
-                    assert (
-                        l1 == l2
-                    ), f"Difference found in line {i} of job file: {l1} vs {l2}"
-
-
-if __name__ == "__main__":
-    unittest.main(verbosity=2)
```

### Comparing `jobqueues-0.9.3/jobqueues/templates/SGE_job.sh.j2` & `jobqueues-0.9.4/jobqueues/templates/SGE_job.sh.j2`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.3/jobqueues/util.py` & `jobqueues-0.9.4/jobqueues/util.py`

 * *Files identical despite different names*

### Comparing `jobqueues-0.9.3/jobqueues.egg-info/PKG-INFO` & `jobqueues-0.9.4/jobqueues.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobqueues
-Version: 0.9.3
+Version: 0.9.4
 Summary: Wrappers for various queueing systems in python
 Author-email: Acellera <info@acellera.com>
 Project-URL: Homepage, https://github.com/Acellera/jobqueues
 Project-URL: Bug Tracker, https://github.com/Acellera/jobqueues/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
```

### Comparing `jobqueues-0.9.3/jobqueues.egg-info/SOURCES.txt` & `jobqueues-0.9.4/jobqueues.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -25,8 +25,9 @@
 jobqueues.egg-info/not-zip-safe
 jobqueues.egg-info/requires.txt
 jobqueues.egg-info/top_level.txt
 jobqueues/celeryfiles/__init__.py
 jobqueues/celeryfiles/celery.py
 jobqueues/celeryfiles/tasks.py
 jobqueues/templates/SGE_job.sh.j2
-jobqueues/templates/SLURM_job.sh.j2
+jobqueues/templates/SLURM_job.sh.j2
+tests/test_slurmqueue.py
```

### Comparing `jobqueues-0.9.3/pyproject.toml` & `jobqueues-0.9.4/pyproject.toml`

 * *Files identical despite different names*

