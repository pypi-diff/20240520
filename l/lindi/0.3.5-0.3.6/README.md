# Comparing `tmp/lindi-0.3.5.tar.gz` & `tmp/lindi-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lindi-0.3.5.tar", max compression
+gzip compressed data, was "lindi-0.3.6.tar", max compression
```

## Comparing `lindi-0.3.5.tar` & `lindi-0.3.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1512 2024-03-13 15:25:45.816228 lindi-0.3.5/LICENSE
--rw-r--r--   0        0        0     5609 2024-05-09 21:23:47.131899 lindi-0.3.5/README.md
--rw-r--r--   0        0        0     1314 2024-05-09 21:23:47.131899 lindi-0.3.5/lindi/File/File.py
--rw-r--r--   0        0        0        0 2024-05-09 21:23:47.131899 lindi-0.3.5/lindi/File/__init__.py
--rw-r--r--   0        0        0    31601 2024-05-16 21:59:28.615995 lindi-0.3.5/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py
--rw-r--r--   0        0        0      613 2024-05-16 21:59:28.615995 lindi-0.3.5/lindi/LindiH5ZarrStore/LindiH5ZarrStoreOpts.py
--rw-r--r--   0        0        0      169 2024-05-09 21:23:47.135899 lindi-0.3.5/lindi/LindiH5ZarrStore/__init__.py
--rw-r--r--   0        0        0     5310 2024-05-16 21:59:28.615995 lindi-0.3.5/lindi/LindiH5ZarrStore/_util.py
--rw-r--r--   0        0        0     2242 2024-04-19 19:44:06.440621 lindi-0.3.5/lindi/LindiH5pyFile/LindiH5pyAttributes.py
--rw-r--r--   0        0        0    11982 2024-05-09 21:23:47.135899 lindi-0.3.5/lindi/LindiH5pyFile/LindiH5pyDataset.py
--rw-r--r--   0        0        0    26328 2024-05-16 21:59:28.619995 lindi-0.3.5/lindi/LindiH5pyFile/LindiH5pyFile.py
--rw-r--r--   0        0        0     6051 2024-04-19 19:44:06.440621 lindi-0.3.5/lindi/LindiH5pyFile/LindiH5pyGroup.py
--rw-r--r--   0        0        0      255 2024-03-21 11:16:09.352672 lindi-0.3.5/lindi/LindiH5pyFile/LindiH5pyLink.py
--rw-r--r--   0        0        0      478 2024-04-04 18:56:02.146012 lindi-0.3.5/lindi/LindiH5pyFile/LindiH5pyReference.py
--rw-r--r--   0        0        0    11404 2024-05-16 21:59:25.631995 lindi-0.3.5/lindi/LindiH5pyFile/LindiReferenceFileSystemStore.py
--rw-r--r--   0        0        0      327 2024-03-21 11:16:09.352672 lindi-0.3.5/lindi/LindiH5pyFile/__init__.py
--rw-r--r--   0        0        0      528 2024-04-19 19:44:06.440621 lindi-0.3.5/lindi/LindiH5pyFile/writers/LindiH5pyAttributesWriter.py
--rw-r--r--   0        0        0     1941 2024-05-09 01:58:05.679967 lindi-0.3.5/lindi/LindiH5pyFile/writers/LindiH5pyDatasetWriter.py
--rw-r--r--   0        0        0     6651 2024-04-24 16:16:12.091927 lindi-0.3.5/lindi/LindiH5pyFile/writers/LindiH5pyGroupWriter.py
--rw-r--r--   0        0        0        0 2024-04-04 18:56:02.146012 lindi-0.3.5/lindi/LindiH5pyFile/writers/__init__.py
--rw-r--r--   0        0        0    16420 2024-05-16 21:59:25.631995 lindi-0.3.5/lindi/LindiRemfile/LindiRemfile.py
--rw-r--r--   0        0        0        0 2024-05-09 21:23:47.135899 lindi-0.3.5/lindi/LindiRemfile/__init__.py
--rw-r--r--   0        0        0     8772 2024-05-09 21:23:47.135899 lindi-0.3.5/lindi/LindiStagingStore/LindiStagingStore.py
--rw-r--r--   0        0        0     3506 2024-05-09 21:23:47.135899 lindi-0.3.5/lindi/LindiStagingStore/StagingArea.py
--rw-r--r--   0        0        0       76 2024-04-19 19:44:06.440621 lindi-0.3.5/lindi/LindiStagingStore/__init__.py
--rw-r--r--   0        0        0     2299 2024-05-16 21:59:25.631995 lindi-0.3.5/lindi/LocalCache/LocalCache.py
--rw-r--r--   0        0        0        0 2024-05-09 21:23:47.135899 lindi-0.3.5/lindi/LocalCache/__init__.py
--rw-r--r--   0        0        0      388 2024-05-09 21:23:47.135899 lindi-0.3.5/lindi/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 18:56:02.146012 lindi-0.3.5/lindi/conversion/__init__.py
--rw-r--r--   0        0        0      167 2024-04-04 18:56:02.146012 lindi-0.3.5/lindi/conversion/_util.py
--rw-r--r--   0        0        0     5907 2024-04-24 16:16:12.091927 lindi-0.3.5/lindi/conversion/attr_conversion.py
--rw-r--r--   0        0        0    10819 2024-04-24 16:16:12.091927 lindi-0.3.5/lindi/conversion/create_zarr_dataset_from_h5_data.py
--rw-r--r--   0        0        0     1079 2024-04-15 13:56:49.245944 lindi-0.3.5/lindi/conversion/decode_references.py
--rw-r--r--   0        0        0     2887 2024-04-15 13:02:34.168232 lindi-0.3.5/lindi/conversion/h5_filters_to_codecs.py
--rw-r--r--   0        0        0     2041 2024-04-24 16:16:12.091927 lindi-0.3.5/lindi/conversion/h5_ref_to_zarr_attr.py
--rw-r--r--   0        0        0      936 2024-04-18 21:52:00.325839 lindi-0.3.5/lindi/conversion/nan_inf_ninf.py
--rw-r--r--   0        0        0      503 2024-04-15 12:44:19.013722 lindi-0.3.5/lindi/conversion/reformat_json.py
--rw-r--r--   0        0        0      746 2024-05-16 21:59:47.239995 lindi-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     6307 1970-01-01 00:00:00.000000 lindi-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1512 2024-03-13 15:25:45.816228 lindi-0.3.6/LICENSE
+-rw-r--r--   0        0        0     5609 2024-05-09 21:23:47.131899 lindi-0.3.6/README.md
+-rw-r--r--   0        0        0     1314 2024-05-09 21:23:47.131899 lindi-0.3.6/lindi/File/File.py
+-rw-r--r--   0        0        0        0 2024-05-09 21:23:47.131899 lindi-0.3.6/lindi/File/__init__.py
+-rw-r--r--   0        0        0    32249 2024-05-20 14:59:02.651924 lindi-0.3.6/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py
+-rw-r--r--   0        0        0      613 2024-05-16 21:59:28.615995 lindi-0.3.6/lindi/LindiH5ZarrStore/LindiH5ZarrStoreOpts.py
+-rw-r--r--   0        0        0      169 2024-05-09 21:23:47.135899 lindi-0.3.6/lindi/LindiH5ZarrStore/__init__.py
+-rw-r--r--   0        0        0     5310 2024-05-16 21:59:28.615995 lindi-0.3.6/lindi/LindiH5ZarrStore/_util.py
+-rw-r--r--   0        0        0     2242 2024-04-19 19:44:06.440621 lindi-0.3.6/lindi/LindiH5pyFile/LindiH5pyAttributes.py
+-rw-r--r--   0        0        0    11982 2024-05-09 21:23:47.135899 lindi-0.3.6/lindi/LindiH5pyFile/LindiH5pyDataset.py
+-rw-r--r--   0        0        0    26328 2024-05-16 21:59:28.619995 lindi-0.3.6/lindi/LindiH5pyFile/LindiH5pyFile.py
+-rw-r--r--   0        0        0     6051 2024-04-19 19:44:06.440621 lindi-0.3.6/lindi/LindiH5pyFile/LindiH5pyGroup.py
+-rw-r--r--   0        0        0      255 2024-03-21 11:16:09.352672 lindi-0.3.6/lindi/LindiH5pyFile/LindiH5pyLink.py
+-rw-r--r--   0        0        0      478 2024-04-04 18:56:02.146012 lindi-0.3.6/lindi/LindiH5pyFile/LindiH5pyReference.py
+-rw-r--r--   0        0        0    11404 2024-05-20 14:58:59.695925 lindi-0.3.6/lindi/LindiH5pyFile/LindiReferenceFileSystemStore.py
+-rw-r--r--   0        0        0      327 2024-03-21 11:16:09.352672 lindi-0.3.6/lindi/LindiH5pyFile/__init__.py
+-rw-r--r--   0        0        0      528 2024-04-19 19:44:06.440621 lindi-0.3.6/lindi/LindiH5pyFile/writers/LindiH5pyAttributesWriter.py
+-rw-r--r--   0        0        0     1941 2024-05-09 01:58:05.679967 lindi-0.3.6/lindi/LindiH5pyFile/writers/LindiH5pyDatasetWriter.py
+-rw-r--r--   0        0        0     6651 2024-04-24 16:16:12.091927 lindi-0.3.6/lindi/LindiH5pyFile/writers/LindiH5pyGroupWriter.py
+-rw-r--r--   0        0        0        0 2024-04-04 18:56:02.146012 lindi-0.3.6/lindi/LindiH5pyFile/writers/__init__.py
+-rw-r--r--   0        0        0    16420 2024-05-20 14:58:59.695925 lindi-0.3.6/lindi/LindiRemfile/LindiRemfile.py
+-rw-r--r--   0        0        0        0 2024-05-09 21:23:47.135899 lindi-0.3.6/lindi/LindiRemfile/__init__.py
+-rw-r--r--   0        0        0     8772 2024-05-09 21:23:47.135899 lindi-0.3.6/lindi/LindiStagingStore/LindiStagingStore.py
+-rw-r--r--   0        0        0     3506 2024-05-09 21:23:47.135899 lindi-0.3.6/lindi/LindiStagingStore/StagingArea.py
+-rw-r--r--   0        0        0       76 2024-04-19 19:44:06.440621 lindi-0.3.6/lindi/LindiStagingStore/__init__.py
+-rw-r--r--   0        0        0     2299 2024-05-20 14:58:59.695925 lindi-0.3.6/lindi/LocalCache/LocalCache.py
+-rw-r--r--   0        0        0        0 2024-05-09 21:23:47.135899 lindi-0.3.6/lindi/LocalCache/__init__.py
+-rw-r--r--   0        0        0      388 2024-05-09 21:23:47.135899 lindi-0.3.6/lindi/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 18:56:02.146012 lindi-0.3.6/lindi/conversion/__init__.py
+-rw-r--r--   0        0        0      167 2024-04-04 18:56:02.146012 lindi-0.3.6/lindi/conversion/_util.py
+-rw-r--r--   0        0        0     5907 2024-04-24 16:16:12.091927 lindi-0.3.6/lindi/conversion/attr_conversion.py
+-rw-r--r--   0        0        0    10819 2024-04-24 16:16:12.091927 lindi-0.3.6/lindi/conversion/create_zarr_dataset_from_h5_data.py
+-rw-r--r--   0        0        0     1079 2024-04-15 13:56:49.245944 lindi-0.3.6/lindi/conversion/decode_references.py
+-rw-r--r--   0        0        0     2887 2024-04-15 13:02:34.168232 lindi-0.3.6/lindi/conversion/h5_filters_to_codecs.py
+-rw-r--r--   0        0        0     2041 2024-04-24 16:16:12.091927 lindi-0.3.6/lindi/conversion/h5_ref_to_zarr_attr.py
+-rw-r--r--   0        0        0      936 2024-04-18 21:52:00.325839 lindi-0.3.6/lindi/conversion/nan_inf_ninf.py
+-rw-r--r--   0        0        0      503 2024-04-15 12:44:19.013722 lindi-0.3.6/lindi/conversion/reformat_json.py
+-rw-r--r--   0        0        0      746 2024-05-20 15:04:24.419922 lindi-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     6307 1970-01-01 00:00:00.000000 lindi-0.3.6/PKG-INFO
```

### Comparing `lindi-0.3.5/LICENSE` & `lindi-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lindi-0.3.5/README.md` & `lindi-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `lindi-0.3.5/lindi/File/File.py` & `lindi-0.3.6/lindi/File/File.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.5/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py` & `lindi-0.3.6/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,15 +226,15 @@
         h5_item = self._h5f.get('/' + parent_key, None)
         if h5_item is None:
             raise KeyError(parent_key)
         if not isinstance(h5_item, h5py.Group) and not isinstance(h5_item, h5py.Dataset):
             raise Exception(f"Item {parent_key} is not a group or dataset. It is {type(h5_item)}")  # pragma: no cover
 
         # Check whether this is a soft link
-        if isinstance(h5_item, h5py.Group) and parent_key != '':
+        if isinstance(h5_item, (h5py.Group, h5py.Dataset)) and parent_key != '':
             link = self._h5f.get('/' + parent_key, getlink=True)
             if isinstance(link, h5py.ExternalLink):
                 raise Exception(f"External links not supported: {parent_key}")
             elif isinstance(link, h5py.SoftLink):
                 # if it's a soft link, we return a special attribute and ignore
                 # the rest of the attributes because they should be stored in
                 # the target of the soft link
@@ -264,15 +264,16 @@
         return zattrs_content
 
     def _get_zgroup_bytes(self, parent_key: str):
         """Get the .zgroup JSON text for a group"""
         if self._h5f is None:
             raise Exception("Store is closed")
         h5_item = self._h5f.get('/' + parent_key, None)
-        if not isinstance(h5_item, h5py.Group):
+        link = self._h5f.get('/' + parent_key, getlink=True) if parent_key != '' else None
+        if not isinstance(link, h5py.SoftLink) and not isinstance(h5_item, h5py.Group):
             # Important to raise a KeyError here because that's what zarr expects
             raise KeyError(f"Item {parent_key} is not a group")
         # We create a dummy zarr group and then get the .zgroup JSON text
         # from it.
         memory_store = MemoryStore()
         zarr.group(store=memory_store)
         return reformat_json(memory_store.get(".zgroup"))
@@ -604,30 +605,40 @@
                     return
                 for k in item.keys():
                     subitem = item[k]
                     if isinstance(subitem, h5py.Group):
                         # recursively process subgroups
                         _process_group(_join(key, k), subitem)
                     elif isinstance(subitem, h5py.Dataset):
-                        _process_dataset(_join(key, k))
+                        _process_dataset(_join(key, k), subitem)
 
-        def _process_dataset(key):
-            # Add the .zattrs and .zarray files for the dataset=
+        def _process_dataset(key, item: h5py.Dataset):
+            # Add the .zattrs and .zarray files for the dataset
             zattrs_bytes = self[f"{key}/.zattrs"]
             assert zattrs_bytes is not None
             if zattrs_bytes != b"{}":  # don't include empty zattrs
                 _add_ref(f"{key}/.zattrs", zattrs_bytes)
-            zattrs_dict = json.loads(zattrs_bytes.decode("utf-8"))
-            external_array_link = zattrs_dict.get(
-                "_EXTERNAL_ARRAY_LINK", None
-            )
+
+            # check if this is a soft link
+            link = item.file.get('/' + key, getlink=True) if key != '' else None
+            if isinstance(link, h5py.SoftLink):
+                # if it's a soft link, we create a zgroup and don't include
+                # the .zarray or array chunks because those should be in the
+                # target of the soft link
+                _add_ref(_join(key, ".zgroup"), self.get(_join(key, ".zgroup")))
+                return
+
             zarray_bytes = self.get(f"{key}/.zarray")
             assert zarray_bytes is not None
             _add_ref(f"{key}/.zarray", zarray_bytes)
 
+            zattrs_dict = json.loads(zattrs_bytes.decode("utf-8"))
+            external_array_link = zattrs_dict.get(
+                "_EXTERNAL_ARRAY_LINK", None
+            )
             if external_array_link is None:
                 # Only add chunk references for datasets without an external array link
                 self._add_chunk_info_to_refs(key, _add_ref, _add_ref_chunk)
 
         # Process the groups recursively starting with the root group
         _process_group("", self._h5f)
```

### Comparing `lindi-0.3.5/lindi/LindiH5ZarrStore/LindiH5ZarrStoreOpts.py` & `lindi-0.3.6/lindi/LindiH5ZarrStore/LindiH5ZarrStoreOpts.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.5/lindi/LindiH5ZarrStore/_util.py` & `lindi-0.3.6/lindi/LindiH5ZarrStore/_util.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.5/lindi/LindiH5pyFile/LindiH5pyAttributes.py` & `lindi-0.3.6/lindi/LindiH5pyFile/LindiH5pyAttributes.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.5/lindi/LindiH5pyFile/LindiH5pyDataset.py` & `lindi-0.3.6/lindi/LindiH5pyFile/LindiH5pyDataset.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.5/lindi/LindiH5pyFile/LindiH5pyFile.py` & `lindi-0.3.6/lindi/LindiH5pyFile/LindiH5pyFile.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.5/lindi/LindiH5pyFile/LindiH5pyGroup.py` & `lindi-0.3.6/lindi/LindiH5pyFile/LindiH5pyGroup.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.5/lindi/LindiH5pyFile/LindiReferenceFileSystemStore.py` & `lindi-0.3.6/lindi/LindiH5pyFile/LindiReferenceFileSystemStore.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.5/lindi/LindiH5pyFile/writers/LindiH5pyAttributesWriter.py` & `lindi-0.3.6/lindi/LindiH5pyFile/writers/LindiH5pyAttributesWriter.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.5/lindi/LindiH5pyFile/writers/LindiH5pyDatasetWriter.py` & `lindi-0.3.6/lindi/LindiH5pyFile/writers/LindiH5pyDatasetWriter.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.5/lindi/LindiH5pyFile/writers/LindiH5pyGroupWriter.py` & `lindi-0.3.6/lindi/LindiH5pyFile/writers/LindiH5pyGroupWriter.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.5/lindi/LindiRemfile/LindiRemfile.py` & `lindi-0.3.6/lindi/LindiRemfile/LindiRemfile.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.5/lindi/LindiStagingStore/LindiStagingStore.py` & `lindi-0.3.6/lindi/LindiStagingStore/LindiStagingStore.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.5/lindi/LindiStagingStore/StagingArea.py` & `lindi-0.3.6/lindi/LindiStagingStore/StagingArea.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.5/lindi/LocalCache/LocalCache.py` & `lindi-0.3.6/lindi/LocalCache/LocalCache.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.5/lindi/conversion/attr_conversion.py` & `lindi-0.3.6/lindi/conversion/attr_conversion.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.5/lindi/conversion/create_zarr_dataset_from_h5_data.py` & `lindi-0.3.6/lindi/conversion/create_zarr_dataset_from_h5_data.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.5/lindi/conversion/decode_references.py` & `lindi-0.3.6/lindi/conversion/decode_references.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.5/lindi/conversion/h5_filters_to_codecs.py` & `lindi-0.3.6/lindi/conversion/h5_filters_to_codecs.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.5/lindi/conversion/h5_ref_to_zarr_attr.py` & `lindi-0.3.6/lindi/conversion/h5_ref_to_zarr_attr.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.5/lindi/conversion/nan_inf_ninf.py` & `lindi-0.3.6/lindi/conversion/nan_inf_ninf.py`

 * *Files identical despite different names*

### Comparing `lindi-0.3.5/pyproject.toml` & `lindi-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lindi"
-version = "0.3.5"
+version = "0.3.6"
 description = ""
 authors = [
     "Jeremy Magland <jmagland@flatironinstitute.org>",
     "Ryan Ly <rly@lbl.gov>",
     "Oliver Ruebel <oruebel@lbl.gov>"
 ]
 readme = "README.md"
```

### Comparing `lindi-0.3.5/PKG-INFO` & `lindi-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lindi
-Version: 0.3.5
+Version: 0.3.6
 Summary: 
 Author: Jeremy Magland
 Author-email: jmagland@flatironinstitute.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

