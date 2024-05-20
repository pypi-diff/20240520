# Comparing `tmp/simply_nwb-0.6.2.tar.gz` & `tmp/simply_nwb-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simply_nwb-0.6.2.tar", last modified: Wed Jan 24 02:28:47 2024, max compression
+gzip compressed data, was "simply_nwb-0.7.0.tar", last modified: Mon May 20 21:53:43 2024, max compression
```

## Comparing `simply_nwb-0.6.2.tar` & `simply_nwb-0.7.0.tar`

### file list

```diff
@@ -1,33 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-01-24 02:28:47.888861 simply_nwb-0.6.2/
--rw-rw-rw-   0        0        0    35819 2023-05-12 18:05:03.000000 simply_nwb-0.6.2/LICENSE
--rw-rw-rw-   0        0        0      566 2024-01-24 02:28:47.887860 simply_nwb-0.6.2/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-05-12 18:23:04.000000 simply_nwb-0.6.2/README.rst
--rw-rw-rw-   0        0        0       42 2024-01-24 02:28:47.889861 simply_nwb-0.6.2/setup.cfg
--rw-rw-rw-   0        0        0      695 2024-01-24 02:28:42.000000 simply_nwb-0.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-24 02:28:47.843860 simply_nwb-0.6.2/simply_nwb/
--rw-rw-rw-   0        0        0       87 2023-06-04 02:15:34.000000 simply_nwb-0.6.2/simply_nwb/__init__.py
--rw-rw-rw-   0        0        0    28040 2024-01-18 03:03:50.000000 simply_nwb-0.6.2/simply_nwb/simple_nwb.py
-drwxrwxrwx   0        0        0        0 2024-01-24 02:28:47.857864 simply_nwb-0.6.2/simply_nwb/transferring/
--rw-rw-rw-   0        0        0      514 2023-06-04 02:15:34.000000 simply_nwb-0.6.2/simply_nwb/transferring/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-24 02:28:47.861862 simply_nwb-0.6.2/simply_nwb/transferring/filesync/
--rw-rw-rw-   0        0        0       38 2023-06-04 02:15:34.000000 simply_nwb-0.6.2/simply_nwb/transferring/filesync/__init__.py
--rw-rw-rw-   0        0        0     7226 2023-07-16 05:48:20.000000 simply_nwb-0.6.2/simply_nwb/transferring/filesync/oneway.py
--rw-rw-rw-   0        0        0     7208 2023-09-10 07:06:39.000000 simply_nwb-0.6.2/simply_nwb/transferring/nwb_transfer.py
-drwxrwxrwx   0        0        0        0 2024-01-24 02:28:47.885863 simply_nwb-0.6.2/simply_nwb/transforms/
--rw-rw-rw-   0        0        0      179 2023-06-04 02:15:34.000000 simply_nwb-0.6.2/simply_nwb/transforms/__init__.py
--rw-rw-rw-   0        0        0     3011 2023-07-16 05:48:20.000000 simply_nwb-0.6.2/simply_nwb/transforms/blackrock.py
--rw-rw-rw-   0        0        0     1060 2023-07-16 05:48:20.000000 simply_nwb-0.6.2/simply_nwb/transforms/csv.py
--rw-rw-rw-   0        0        0     2555 2023-07-16 05:48:20.000000 simply_nwb-0.6.2/simply_nwb/transforms/labjack.py
--rw-rw-rw-   0        0        0     2146 2023-07-16 05:48:20.000000 simply_nwb-0.6.2/simply_nwb/transforms/mp4.py
--rw-rw-rw-   0        0        0    22553 2024-01-24 02:26:23.000000 simply_nwb-0.6.2/simply_nwb/transforms/neuropixels.py
--rw-rw-rw-   0        0        0     3935 2023-07-16 05:48:20.000000 simply_nwb-0.6.2/simply_nwb/transforms/p_erg.py
--rw-rw-rw-   0        0        0      639 2023-07-16 05:48:20.000000 simply_nwb-0.6.2/simply_nwb/transforms/plaintext.py
--rw-rw-rw-   0        0        0     4644 2023-07-16 05:48:20.000000 simply_nwb-0.6.2/simply_nwb/transforms/tif.py
--rw-rw-rw-   0        0        0      472 2023-07-16 05:48:20.000000 simply_nwb-0.6.2/simply_nwb/transforms/yaml.py
--rw-rw-rw-   0        0        0    12433 2024-01-18 04:05:26.000000 simply_nwb-0.6.2/simply_nwb/util.py
-drwxrwxrwx   0        0        0        0 2024-01-24 02:28:47.853863 simply_nwb-0.6.2/simply_nwb.egg-info/
--rw-rw-rw-   0        0        0      566 2024-01-24 02:28:47.000000 simply_nwb-0.6.2/simply_nwb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      749 2024-01-24 02:28:47.000000 simply_nwb-0.6.2/simply_nwb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-24 02:28:47.000000 simply_nwb-0.6.2/simply_nwb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      117 2024-01-24 02:28:47.000000 simply_nwb-0.6.2/simply_nwb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-01-24 02:28:47.000000 simply_nwb-0.6.2/simply_nwb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 21:53:43.238034 simply_nwb-0.7.0/
+-rw-rw-rw-   0        0        0    35819 2023-05-12 18:05:03.000000 simply_nwb-0.7.0/LICENSE
+-rw-rw-rw-   0        0        0      566 2024-05-20 21:53:43.237034 simply_nwb-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-05-12 18:23:04.000000 simply_nwb-0.7.0/README.rst
+-rw-rw-rw-   0        0        0       42 2024-05-20 21:53:43.238034 simply_nwb-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0      695 2024-05-20 21:50:28.000000 simply_nwb-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 21:53:43.194033 simply_nwb-0.7.0/simply_nwb/
+-rw-rw-rw-   0        0        0       87 2023-06-04 02:15:34.000000 simply_nwb-0.7.0/simply_nwb/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 21:53:43.204034 simply_nwb-0.7.0/simply_nwb/pipeline/
+-rw-rw-rw-   0        0        0     3885 2024-05-20 21:51:27.000000 simply_nwb-0.7.0/simply_nwb/pipeline/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 21:53:43.207034 simply_nwb-0.7.0/simply_nwb/pipeline/enrichments/
+-rw-rw-rw-   0        0        0     2871 2024-05-18 18:39:29.000000 simply_nwb-0.7.0/simply_nwb/pipeline/enrichments/__init__.py
+-rw-rw-rw-   0        0        0      982 2024-05-18 18:39:29.000000 simply_nwb-0.7.0/simply_nwb/pipeline/enrichments/example.py
+drwxrwxrwx   0        0        0        0 2024-05-20 21:53:43.212034 simply_nwb-0.7.0/simply_nwb/pipeline/enrichments/saccades/
+-rw-rw-rw-   0        0        0      100 2024-05-18 18:39:29.000000 simply_nwb-0.7.0/simply_nwb/pipeline/enrichments/saccades/__init__.py
+-rw-rw-rw-   0        0        0     6398 2024-05-20 21:45:29.000000 simply_nwb-0.7.0/simply_nwb/pipeline/enrichments/saccades/predicted.py
+-rw-rw-rw-   0        0        0    15072 2024-05-20 21:53:16.000000 simply_nwb-0.7.0/simply_nwb/pipeline/enrichments/saccades/putative.py
+drwxrwxrwx   0        0        0        0 2024-05-20 21:53:43.213034 simply_nwb-0.7.0/simply_nwb/pipeline/util/
+-rw-rw-rw-   0        0        0     2431 2024-05-18 18:39:29.000000 simply_nwb-0.7.0/simply_nwb/pipeline/util/__init__.py
+-rw-rw-rw-   0        0        0     3021 2024-05-18 18:39:29.000000 simply_nwb-0.7.0/simply_nwb/pipeline/value_mapping.py
+-rw-rw-rw-   0        0        0    14262 2024-05-10 20:55:30.000000 simply_nwb-0.7.0/simply_nwb/simple_nwb.py
+drwxrwxrwx   0        0        0        0 2024-05-20 21:53:43.216034 simply_nwb-0.7.0/simply_nwb/transferring/
+-rw-rw-rw-   0        0        0      514 2023-06-04 02:15:34.000000 simply_nwb-0.7.0/simply_nwb/transferring/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 21:53:43.219035 simply_nwb-0.7.0/simply_nwb/transferring/filesync/
+-rw-rw-rw-   0        0        0       38 2023-06-04 02:15:34.000000 simply_nwb-0.7.0/simply_nwb/transferring/filesync/__init__.py
+-rw-rw-rw-   0        0        0     7226 2023-07-16 05:48:20.000000 simply_nwb-0.7.0/simply_nwb/transferring/filesync/oneway.py
+-rw-rw-rw-   0        0        0     7208 2023-09-10 07:06:39.000000 simply_nwb-0.7.0/simply_nwb/transferring/nwb_transfer.py
+drwxrwxrwx   0        0        0        0 2024-05-20 21:53:43.236034 simply_nwb-0.7.0/simply_nwb/transforms/
+-rw-rw-rw-   0        0        0      207 2024-05-10 20:55:30.000000 simply_nwb-0.7.0/simply_nwb/transforms/__init__.py
+-rw-rw-rw-   0        0        0     5431 2024-05-10 20:55:30.000000 simply_nwb-0.7.0/simply_nwb/transforms/blackrock.py
+-rw-rw-rw-   0        0        0     1060 2023-07-16 05:48:20.000000 simply_nwb-0.7.0/simply_nwb/transforms/csv.py
+-rw-rw-rw-   0        0        0     2449 2024-05-14 19:47:58.000000 simply_nwb-0.7.0/simply_nwb/transforms/eyetracking.py
+-rw-rw-rw-   0        0        0     7595 2024-05-10 20:55:30.000000 simply_nwb-0.7.0/simply_nwb/transforms/labjack.py
+-rw-rw-rw-   0        0        0     4316 2024-05-10 20:55:30.000000 simply_nwb-0.7.0/simply_nwb/transforms/mp4.py
+-rw-rw-rw-   0        0        0    22593 2024-01-24 02:30:37.000000 simply_nwb-0.7.0/simply_nwb/transforms/neuropixels.py
+-rw-rw-rw-   0        0        0     8257 2024-05-10 20:55:30.000000 simply_nwb-0.7.0/simply_nwb/transforms/p_erg.py
+-rw-rw-rw-   0        0        0      639 2023-07-16 05:48:20.000000 simply_nwb-0.7.0/simply_nwb/transforms/plaintext.py
+-rw-rw-rw-   0        0        0     6902 2024-05-10 20:55:30.000000 simply_nwb-0.7.0/simply_nwb/transforms/tif.py
+-rw-rw-rw-   0        0        0      472 2023-07-16 05:48:20.000000 simply_nwb-0.7.0/simply_nwb/transforms/yaml.py
+-rw-rw-rw-   0        0        0    13361 2024-05-14 23:12:33.000000 simply_nwb-0.7.0/simply_nwb/util.py
+drwxrwxrwx   0        0        0        0 2024-05-20 21:53:43.201033 simply_nwb-0.7.0/simply_nwb.egg-info/
+-rw-rw-rw-   0        0        0      566 2024-05-20 21:53:43.000000 simply_nwb-0.7.0/simply_nwb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1139 2024-05-20 21:53:43.000000 simply_nwb-0.7.0/simply_nwb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 21:53:43.000000 simply_nwb-0.7.0/simply_nwb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      151 2024-05-20 21:53:43.000000 simply_nwb-0.7.0/simply_nwb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-20 21:53:43.000000 simply_nwb-0.7.0/simply_nwb.egg-info/top_level.txt
```

### Comparing `simply_nwb-0.6.2/LICENSE` & `simply_nwb-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.6.2/PKG-INFO` & `simply_nwb-0.7.0/simply_nwb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: simply_nwb
-Version: 0.6.2
+Name: simply-nwb
+Version: 0.7.0
 Summary: Common NWB use cases and simplified interface for common usage
 Author: Spencer Hanson
 Keywords: neuroscience,nwb,tools,science
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 ###########
```

### Comparing `simply_nwb-0.6.2/setup.py` & `simply_nwb-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.6.2"
+VERSION = "0.7.0"
 
 
 def parse_requirements(requirement_file):
     with open(requirement_file) as fi:
         return fi.readlines()
```

### Comparing `simply_nwb-0.6.2/simply_nwb/transferring/__init__.py` & `simply_nwb-0.7.0/simply_nwb/transferring/__init__.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.6.2/simply_nwb/transferring/filesync/oneway.py` & `simply_nwb-0.7.0/simply_nwb/transferring/filesync/oneway.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.6.2/simply_nwb/transferring/nwb_transfer.py` & `simply_nwb-0.7.0/simply_nwb/transferring/nwb_transfer.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.6.2/simply_nwb/transforms/csv.py` & `simply_nwb-0.7.0/simply_nwb/transforms/csv.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.6.2/simply_nwb/transforms/neuropixels.py` & `simply_nwb-0.7.0/simply_nwb/transforms/neuropixels.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,16 @@
     :param recording_path: path to the recording str
     :param probe_depth: depth of the probe
     :param site_positions: Channel positions on the neuropixels probe
     :param probe_name: Name of the probe, defaults to the recording path
     :param spikes_filename: Spikes filename, defaults to spike_secs.npy
     :param aligned: bool if the spike times are aligned along the sampling rate, if not will be converted
     :param df: Return data as a dataframe
-    :param
+
+    :return: Dict or Dataframe of the unit data
     """
 
     if site_positions is None:
         site_positions = OPTION234_POSITIONS
 
     if probe_name is None:
         probe_name = recording_path
@@ -307,15 +308,15 @@
                             insertion_angle: float = 0) -> dict:
     """
     Load unit data from Phy
     Requires that phy has been run to generate cluster_info.tsv
     searches the folder for the chanmap the KS used, or searches one folder up for it
 
     :param recording_path: Path to the recording data
-    :param chanmap: Channel map, if not provided will attempt to find a file matching '*hanMap.mat'
+    :param chanmap: Channel map, if not provided will attempt to find a file matching '\*hanMap.mat'
     :param insertion_angle: insertion angle
     :param insertion_depth: insertion depth
 
     :return: dict of unit data
     """
 
     cluster_info = pd.read_csv(os.path.join(recording_path, 'cluster_info.tsv'), '\t')
```

### Comparing `simply_nwb-0.6.2/simply_nwb/transforms/plaintext.py` & `simply_nwb-0.7.0/simply_nwb/transforms/plaintext.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.6.2/simply_nwb/transforms/tif.py` & `simply_nwb-0.7.0/simply_nwb/transforms/tif.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,74 @@
 import os
+import warnings
+from typing import Any
+
 from PIL import Image
 import numpy as np
 import glob
 
+from hdmf.backends.hdf5 import H5DataIO
+from pynwb import NWBFile
+from pynwb.image import ImageSeries
+
+
+class _TIFMixin(object):
+    @staticmethod
+    def tif_add_as_processing_imageseries(
+            nwbfile: NWBFile,
+            name: str,
+            processing_module_name: str,
+            numpy_data: Any,
+            sampling_rate: float,
+            description: str,
+            starting_time: float = 0.0,
+            chunking: bool = True,
+            compression: bool = True
+    ) -> NWBFile:
+        """
+
+        Add a numpy array as a processing module with image data, meant to work in conjunction with the tif reader utility
+
+        :param nwbfile: NWBFile to add the tif data to
+        :param name: Name of the movie
+        :param numpy_data: data, can be np.memmap
+        :param processing_module_name: Name of the processing module to append or create to add the images to
+        :param sampling_rate: frames per second
+        :param description: description of the movie
+        :param starting_time: Starting time of this movie, relative to experiment start. Defaults to 0.0
+        :param chunking: Optional chunking for large files, defaults to True
+        :param compression: Optional compression for large files, defaults to True
+        :return: NWBFile
+        """
+        if len(numpy_data.shape) < 3:
+            raise ValueError("Invalid data shape! numpy_data must be at least 3 dimensional. If you only have 1 image, add an axis using myimgarr[None, :] to go from (a, b) to (1, a, b)")
+
+        images = ImageSeries(
+            name=name,
+            data=H5DataIO(
+                data=numpy_data,
+                compression=compression,
+                chunks=chunking
+            ),
+            description=description,
+            unit="n.a.",
+            rate=sampling_rate,
+            format="raw",
+            starting_time=starting_time
+        )
+
+        from simply_nwb import SimpleNWB
+        SimpleNWB.add_to_processing_module(
+            nwbfile,
+            module_name=processing_module_name,
+            module_description=description,
+            data=images
+        )
+        return nwbfile
+
 
 class ImageLoadError(Exception):
     pass
 
 
 def tif_read_image(filename: str, show_error: bool = True) -> np.ndarray:
     """
```

### Comparing `simply_nwb-0.6.2/simply_nwb/util.py` & `simply_nwb-0.7.0/simply_nwb/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,29 +89,39 @@
     isn't corrupted
 
     :param nwb_obj: pynwb.file.NWBFile object
     :param filename: path of a local file, doesn't need to exist
     :param verify: Verify that *most* fields wrote correctly and the file didn't corrupt
     :return: None
     """
-
     io = NWBHDF5IO(filename, mode="w")
-    io.write(nwb_obj)
-    io.close()
-
-    if verify:
-        from pynwb import NWBHDF5IO as nwbio  # Want to load file to check that it didn't corrupt
-        try:
-            test_nwb = nwbio(filename).read()
-            # Also note that your data can just 'be missing' because NWB decided not to write it 'for some reason'
-        except Exception as e:
-            warnings.warn(f"File is corrupted! NWB lets you write data that it won't read correctly, check your input data!")
-            raise e
-
-        compare_nwbfiles(nwb_obj, test_nwb, "InMemoryNWB", "WrittenFileNWB")
+    try:
+        src = nwb_obj.container_source
+        if src == filename or src is None:  # Overwriting same NWB or writing a new one
+            io.write(nwb_obj)
+        else:
+            src_io = nwb_obj.read_io
+            nwb_obj.set_modified()
+            io.export(nwbfile=nwb_obj, src_io=src_io)
+
+        if verify:
+            # Want to load file to check that it didn't corrupt
+            tio = NWBHDF5IO(filename)
+            try:
+                test_nwb = tio.read()
+                # Also note that your data can just 'be missing' because NWB decided not to write it 'for some reason'
+            except Exception as e:
+                warnings.warn(f"File is corrupted! NWB lets you write data that it won't read correctly, check your input data!")
+                raise e
+            finally:
+                tio.close()
+
+            compare_nwbfiles(nwb_obj, test_nwb, "InMemoryNWB", "WrittenFileNWB")
+    finally:
+        io.close()
 
 
 def warn_on_name_format(name_value: str, context_str: str = "") -> bool:
     """
     Send a warning if the name format isn't in 'snake_case'
 
     :param name_value: value to check
@@ -343,8 +353,24 @@
         age=age_str_from_birthday(birthday_str),
         strain=strain,
         sex=sex,
         description=desc
     )
 
 
+def date_to_mouse_age(date_str: Optional[str]) -> Optional[str]:
+    """
+    Convert a date into an ISO-8601 period time value
+
+    :param date_str: string of the date, should be pendulum parsable
+    :return: string like 'P90D'
+    """
+    if date_str is None:
+        return None
+
+    if date_str.lower() != "unknown":
+        mouse_age = "P" + str(pendulum.parse(date_str, strict=False).diff(
+            pendulum.now()).in_days()) + "D"  # How many days since birthday
+    else:
+        mouse_age = None
 
+    return mouse_age
```

### Comparing `simply_nwb-0.6.2/simply_nwb.egg-info/PKG-INFO` & `simply_nwb-0.7.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: simply-nwb
-Version: 0.6.2
+Name: simply_nwb
+Version: 0.7.0
 Summary: Common NWB use cases and simplified interface for common usage
 Author: Spencer Hanson
 Keywords: neuroscience,nwb,tools,science
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 ###########
```

