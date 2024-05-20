# Comparing `tmp/fn5-1.2.2rc2.tar.gz` & `tmp/fn5-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fn5-1.2.2rc2.tar", last modified: Fri Mar  8 13:48:35 2024, max compression
+gzip compressed data, was "fn5-2.0.0.tar", last modified: Mon May 20 14:54:24 2024, max compression
```

## Comparing `fn5-1.2.2rc2.tar` & `fn5-2.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-03-08 13:48:35.265632 fn5-1.2.2rc2/
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     5730 2023-06-28 14:48:41.000000 fn5-1.2.2rc2/LICENSE
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)     3149 2024-03-08 13:48:35.265632 fn5-1.2.2rc2/PKG-INFO
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     5732 2023-06-28 14:48:41.000000 fn5-1.2.2rc2/README.md
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-03-08 13:48:35.265632 fn5-1.2.2rc2/fn5.egg-info/
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)     3149 2024-03-08 13:48:35.000000 fn5-1.2.2rc2/fn5.egg-info/PKG-INFO
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      326 2024-03-08 13:48:35.000000 fn5-1.2.2rc2/fn5.egg-info/SOURCES.txt
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)        1 2024-03-08 13:48:35.000000 fn5-1.2.2rc2/fn5.egg-info/dependency_links.txt
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)        1 2024-03-08 13:21:49.000000 fn5-1.2.2rc2/fn5.egg-info/not-zip-safe
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)        4 2024-03-08 13:48:35.000000 fn5-1.2.2rc2/fn5.egg-info/top_level.txt
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      115 2024-02-27 16:49:26.000000 fn5-1.2.2rc2/pyproject.toml
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       38 2024-03-08 13:48:35.265632 fn5-1.2.2rc2/setup.cfg
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     1925 2024-03-08 13:47:45.000000 fn5-1.2.2rc2/setup.py
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-03-08 13:48:35.265632 fn5-1.2.2rc2/src/
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    21758 2024-02-28 12:17:42.000000 fn5-1.2.2rc2/src/comparisons.cpp
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     5800 2024-02-26 12:49:41.000000 fn5-1.2.2rc2/src/fn5_python.cpp
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-03-08 13:48:35.265632 fn5-1.2.2rc2/src/include/
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     5357 2024-02-23 13:03:54.000000 fn5-1.2.2rc2/src/include/comparisons.hpp
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     5364 2024-02-28 13:12:19.000000 fn5-1.2.2rc2/src/include/sample.hpp
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     8961 2024-02-28 12:24:03.000000 fn5-1.2.2rc2/src/sample.cpp
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-03-08 13:48:35.265632 fn5-1.2.2rc2/test/
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     1887 2024-02-26 13:34:11.000000 fn5-1.2.2rc2/test/test_outputs.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     1019 2024-02-26 15:24:01.000000 fn5-1.2.2rc2/test/test_py_bindings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:54:24.538692 fn5-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-05-20 14:53:36.000000 fn5-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-20 14:54:24.538692 fn5-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-05-20 14:53:36.000000 fn5-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:54:24.538692 fn5-2.0.0/fn5.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-20 14:54:24.000000 fn5-2.0.0/fn5.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-20 14:54:24.000000 fn5-2.0.0/fn5.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:54:24.000000 fn5-2.0.0/fn5.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:53:59.000000 fn5-2.0.0/fn5.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-20 14:54:24.000000 fn5-2.0.0/fn5.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-20 14:53:36.000000 fn5-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 14:54:24.538692 fn5-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-20 14:53:36.000000 fn5-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:54:24.538692 fn5-2.0.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    21409 2024-05-20 14:53:36.000000 fn5-2.0.0/src/comparisons.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-05-20 14:53:36.000000 fn5-2.0.0/src/fn5_python.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:54:24.538692 fn5-2.0.0/src/include/
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-05-20 14:53:36.000000 fn5-2.0.0/src/include/comparisons.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-05-20 14:53:36.000000 fn5-2.0.0/src/include/sample.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14308 2024-05-20 14:53:36.000000 fn5-2.0.0/src/sample.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:54:24.538692 fn5-2.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-20 14:53:36.000000 fn5-2.0.0/test/test_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-20 14:53:36.000000 fn5-2.0.0/test/test_py_bindings.py
```

### Comparing `fn5-1.2.2rc2/LICENSE` & `fn5-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fn5-1.2.2rc2/PKG-INFO` & `fn5-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fn5
-Version: 1.2.2rc2
+Version: 2.0.0
 Summary: Fast, scalable SNP distance calculation from disk.
 Home-page: https://github.com/oxfordmmm/FN5
 Author: Jeremy Westhead
 Author-email: jeremy.westhead@ndm.ox.ac.uk
 License: University of Oxford, see LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `fn5-1.2.2rc2/README.md` & `fn5-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `fn5-1.2.2rc2/fn5.egg-info/PKG-INFO` & `fn5-2.0.0/fn5.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fn5
-Version: 1.2.2rc2
+Version: 2.0.0
 Summary: Fast, scalable SNP distance calculation from disk.
 Home-page: https://github.com/oxfordmmm/FN5
 Author: Jeremy Westhead
 Author-email: jeremy.westhead@ndm.ox.ac.uk
 License: University of Oxford, see LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `fn5-1.2.2rc2/setup.py` & `fn5-2.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # Based on example https://github.com/pybind/python_example
 from pybind11.setup_helpers import Pybind11Extension
 from setuptools import setup
 from pathlib import Path
 import os
 
-__version__ = "v1.2.2rc2"
+__version__ = "v2.0.0"
 
 try:
     this_directory = Path(__file__).parent
     long_description = (this_directory / "PYTHON_README.md").read_text()
 except FileNotFoundError:
     # Issues around packaging other readme means we can just skip on install
     long_description = "Fast, scalable SNP distance calculation from disk."
 
-# There's some odd behaviour going on here where pip won't install if this has the headers in it, but they're required to be distributed with the rest of the files
-# So we have to run `python -m build` first including the headers, then again without before running `twine`
+# There's some odd behaviour going on here where pip won't install if this has the headers in it, 
+#   but they're required to be distributed with the rest of the files
+# So we have to run `python -m build` first including the headers, 
+#   then again without before running `twine`
 # So control with an env variable for automation
 if os.environ.get("FN5_FIRST_PASS", None):
     files = sorted(["src/sample.cpp", "src/comparisons.cpp", "src/fn5_python.cpp", "src/include/sample.hpp", "src/include/comparisons.hpp"])
 else:
     files = sorted(["src/sample.cpp", "src/comparisons.cpp", "src/fn5_python.cpp"])
 
 ext_modules = [
```

### Comparing `fn5-1.2.2rc2/src/comparisons.cpp` & `fn5-2.0.0/src/comparisons.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -13,32 +13,48 @@
 
 string ref_genome_path = "NC_000962.3.fasta";
 
 string exclude_mask_path = "tb-exclude.txt";
 
 bool debug = false;
 
-vector<Sample*> load_saves(){
+unordered_set<string> find_saves(){
     unordered_set<string> saves;
     for (const auto &entry : fs::directory_iterator(save_dir)){
         string p = entry.path();
         //Check for .gitkeep or nothing (we want to ignore this)
         if(p == save_dir+"/.gitkeep" || p == save_dir){
             continue;
         }
         
-        //Remove `.A` etc
-        p.pop_back();
-        p.pop_back();
+        if(p.at(p.size()-2) == '.'){
+            // 1 character file extension so likely old `.A` format
+            // Remove file extension in such cases to match old loading format
+            p.pop_back();
+            p.pop_back();
+        }
+        else {
+            // Not a 1 character file extension so check if `.fn5`
+            string ext = p.substr(p.find_last_of(".")+1);
+            if(ext != "fn5" && ext != "FN5"){
+                //  Not valid file extension for new saves so skip
+                continue;
+            }
+        }
 
         //Only add if the path found is not empty
         if(p.find_first_not_of(' ') != string::npos){
             saves.insert(p);
         }
     }
+    return saves;
+}
+
+vector<Sample*> load_saves(){
+    unordered_set<string> saves = find_saves();
 
     vector<Sample*> samples;
     for(const string &elem: saves){
         Sample *s = readSample(elem);
         samples.push_back(s);
     }
 
@@ -55,31 +71,15 @@
         for(unsigned int i=0;i<samples.size();i++){
             acc->push_back(samples.at(i));
         }
     mutex_lock.unlock();
 }
 
 vector<Sample*> load_saves_multithreaded(){
-    unordered_set<string> saves;
-    for (const auto &entry : fs::directory_iterator(save_dir)){
-        string p = entry.path();
-        //Check for .gitkeep or nothing (we want to ignore this)
-        if(p == save_dir+"/.gitkeep" || p == save_dir){
-            continue;
-        }
-        
-        //Remove `.A` etc
-        p.pop_back();
-        p.pop_back();
-
-        //Only add if the path found is not empty
-        if(p.find_first_not_of(' ') != string::npos){
-            saves.insert(p);
-        }
-    }
+    unordered_set<string> saves = find_saves();
 
     vector<Sample*> acc;
     vector<string> filenames;
     for(const string &elem: saves){
         filenames.push_back(elem);
     }
 
@@ -227,31 +227,15 @@
 
 void add_sample(string path, string reference, unordered_set<int> mask, int cutoff){
     //Parse a new sample
     //Compare it to every saved sample, then save it too
     Sample *s = new Sample(path, reference, mask);
 
     //Find all saves
-    unordered_set<string> saves_;
-    for (const auto &entry : fs::directory_iterator(save_dir)){
-        string p = entry.path();    
-        //Check for .gitkeep or nothing (we want to ignore this)
-        if(p == save_dir+"/.gitkeep" || p == save_dir){
-            continue;
-        }
-        
-        //Remove `.A` etc
-        p.pop_back();
-        p.pop_back();
-
-        //Only add if the path found is not empty
-        if(p.find_first_not_of(' ') != string::npos){
-            saves_.insert(p);
-        }
-    }
+    unordered_set<string> saves_ = find_saves();
     //Load them and perform comparisons
     vector<string> saves;
     for(const string &elem: saves_){
         saves.push_back(elem);
     }
 
     //Do comparisons with multithreading
```

### Comparing `fn5-1.2.2rc2/src/fn5_python.cpp` & `fn5-2.0.0/src/fn5_python.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -89,23 +89,23 @@
             }
         );
     m.def("save", &save, R"pbdoc(
         Save a sample to disk.
         -----------------------
 
         Args:
-            path (str): Base path to save to. Produces 5 files of <uuid>.A, <uuid>.C, ...
+            path (str): Directory to save to. Creates 1 file of `<path>/<uuid>.fn5`
             sample (fn5.Sample): Sample to save
         )pbdoc", py::arg("path"), py::arg("sample"));
     m.def("load", &readSample, R"pbdoc(
         Load a sample from disk.
         -----------------------
 
         Args:
-            path (str): Base path to load from. i.e <some path>/<uuid> will load sample <uuid>
+            path (str): Path to load from. i.e <some path>/<uuid> or <some path>/<uuid>.fn5 will load sample <uuid>
         
         Returns:
             fn5.Sample: Loaded sample.
         )pbdoc", py::arg("path"));
     m.def("load_reference", &load_reference, R"pbdoc(
         Load the reference from FASTA.
         -----------------------
```

### Comparing `fn5-1.2.2rc2/src/include/comparisons.hpp` & `fn5-2.0.0/src/include/comparisons.hpp`

 * *Files identical despite different names*

### Comparing `fn5-1.2.2rc2/src/include/sample.hpp` & `fn5-2.0.0/src/include/sample.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -110,41 +110,41 @@
          * @param cutoff Distance to stop caring after (for speed)
          * @return int The distance between the two samples. If dist == cutoff + 1, the sample is further away and shouldn't be counted
          */
         unordered_set<int> dist_x(vector<int> this_x, vector<int> this_n, vector<int> sample_x, vector<int> sample_n, unordered_set<int> acc, unsigned int cutoff);
 };
 
 /**
-* @brief Save the contents of an unordered set to disk using binary.
+* @brief **DEPRECIATED** Save the contents of an unordered set to disk using binary.
 *
 * @param to_save Set to save
 * @param filename Output filename
 */
 void save_n(vector<int> to_save, string filename);
 
 /**
-* @brief Load an unordered set from a binary save on disk
+* @brief **DEPRECIATED** Load an unordered set from a binary save on disk
 *
 * @param filename File to load
 * @returns Unordered set of the ints stored in the file
 */
 vector<int> load_n(string filename);
 
 /**
 * @brief Save a sample to disk
 * 
-* @param filename Directory to save in. Actual saves will be [<filename>/<uuid>.A, <filename>/<uuid>.C, ...]
+* @param filename Directory to save in. Actual save will be <filename>/<uuid>.fn5
 * @param sample Sample to save
 */
 void save(string filename, Sample* sample);
 
 /**
 * @brief Load a sample from disk
 * 
-* @param filename Base filename to load from. Actual saves will be [<filename>.A, <filename>.C, ...]
+* @param filename Base filename to load from. Actual saves will be <filename>/<uuid>.fn5
 * @returns Sample loaded from disk
 */
 Sample* readSample(string filename);
 
 /**
 * @brief Load the reference from disk
 *
```

### Comparing `fn5-1.2.2rc2/test/test_outputs.py` & `fn5-2.0.0/test/test_outputs.py`

 * *Files identical despite different names*

### Comparing `fn5-1.2.2rc2/test/test_py_bindings.py` & `fn5-2.0.0/test/test_py_bindings.py`

 * *Files 25% similar despite different names*

```diff
@@ -26,8 +26,34 @@
         ]
     expected = set([(x.split(" ")[0], x.split(" ")[1], int(x.split(" ")[2])) for x in expected])
     expected_map = {}
     for a, b, dist in expected:
         expected_map[(a, b)] = dist
         expected_map[(b, a)] = dist
     
+    assert actual_map == expected_map
+
+def test_1_saves():
+    '''This should be all comparisons, using saves rather than fastas
+    '''
+    samples = [fn5.load("test/saves/sample1.fn5"), fn5.load("test/saves/sample2.fn5"), fn5.load("test/saves/sample3.fn5"), fn5.load("test/saves/sample4.fn5"),]
+
+    actual = set(fn5.compute(samples))
+    actual_map = {}
+    for a, b, dist in actual:
+        actual_map[(a, b)] = dist
+        actual_map[(b, a)] = dist
+    expected = [
+        "sample4 sample1 12",
+        "sample4 sample3 11",
+        "sample4 sample2 11",
+        "sample1 sample3 1",
+        "sample1 sample2 1",
+        "sample3 sample2 0",
+        ]
+    expected = set([(x.split(" ")[0], x.split(" ")[1], int(x.split(" ")[2])) for x in expected])
+    expected_map = {}
+    for a, b, dist in expected:
+        expected_map[(a, b)] = dist
+        expected_map[(b, a)] = dist
+    
     assert actual_map == expected_map
```

