# Comparing `tmp/yt_aspect-0.2.0.tar.gz` & `tmp/yt_aspect-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt_aspect-0.2.0.tar", last modified: Fri Nov 17 17:59:05 2023, max compression
+gzip compressed data, was "yt_aspect-0.2.1.tar", last modified: Mon May 20 18:56:46 2024, max compression
```

## Comparing `yt_aspect-0.2.0.tar` & `yt_aspect-0.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 17:59:05.567075 yt_aspect-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-11-17 17:58:51.000000 yt_aspect-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2023-11-17 17:59:05.567075 yt_aspect-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2023-11-17 17:58:51.000000 yt_aspect-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2023-11-17 17:58:51.000000 yt_aspect-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-17 17:59:05.567075 yt_aspect-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 17:59:05.563075 yt_aspect-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2023-11-17 17:58:51.000000 yt_aspect-0.2.0/tests/test_outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2023-11-17 17:58:51.000000 yt_aspect-0.2.0/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2023-11-17 17:58:51.000000 yt_aspect-0.2.0/tests/test_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 17:59:05.563075 yt_aspect-0.2.0/yt_aspect/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-17 17:58:51.000000 yt_aspect-0.2.0/yt_aspect/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 17:59:05.563075 yt_aspect-0.2.0/yt_aspect/_pvtu_test_data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-17 17:58:51.000000 yt_aspect-0.2.0/yt_aspect/_pvtu_test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2023-11-17 17:58:52.000000 yt_aspect-0.2.0/yt_aspect/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2023-11-17 17:58:52.000000 yt_aspect-0.2.0/yt_aspect/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    19104 2023-11-17 17:58:52.000000 yt_aspect-0.2.0/yt_aspect/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2023-11-17 17:58:52.000000 yt_aspect-0.2.0/yt_aspect/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     6164 2023-11-17 17:58:52.000000 yt_aspect-0.2.0/yt_aspect/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2023-11-17 17:58:52.000000 yt_aspect-0.2.0/yt_aspect/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 17:59:05.563075 yt_aspect-0.2.0/yt_aspect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2023-11-17 17:59:05.000000 yt_aspect-0.2.0/yt_aspect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      485 2023-11-17 17:59:05.000000 yt_aspect-0.2.0/yt_aspect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-17 17:59:05.000000 yt_aspect-0.2.0/yt_aspect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-11-17 17:59:05.000000 yt_aspect-0.2.0/yt_aspect.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2023-11-17 17:59:05.000000 yt_aspect-0.2.0/yt_aspect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-17 17:59:05.000000 yt_aspect-0.2.0/yt_aspect.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:56:46.871342 yt_aspect-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-20 18:56:37.000000 yt_aspect-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-20 18:56:46.871342 yt_aspect-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-20 18:56:37.000000 yt_aspect-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-20 18:56:37.000000 yt_aspect-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 18:56:46.871342 yt_aspect-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:56:46.867342 yt_aspect-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-05-20 18:56:37.000000 yt_aspect-0.2.1/tests/test_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-20 18:56:37.000000 yt_aspect-0.2.1/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-20 18:56:37.000000 yt_aspect-0.2.1/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:56:46.867342 yt_aspect-0.2.1/yt_aspect/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 18:56:37.000000 yt_aspect-0.2.1/yt_aspect/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:56:46.871342 yt_aspect-0.2.1/yt_aspect/_pvtu_test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 18:56:37.000000 yt_aspect-0.2.1/yt_aspect/_pvtu_test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-20 18:56:37.000000 yt_aspect-0.2.1/yt_aspect/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-20 18:56:37.000000 yt_aspect-0.2.1/yt_aspect/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19110 2024-05-20 18:56:37.000000 yt_aspect-0.2.1/yt_aspect/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-20 18:56:37.000000 yt_aspect-0.2.1/yt_aspect/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-05-20 18:56:37.000000 yt_aspect-0.2.1/yt_aspect/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-20 18:56:37.000000 yt_aspect-0.2.1/yt_aspect/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:56:46.871342 yt_aspect-0.2.1/yt_aspect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-20 18:56:46.000000 yt_aspect-0.2.1/yt_aspect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-20 18:56:46.000000 yt_aspect-0.2.1/yt_aspect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 18:56:46.000000 yt_aspect-0.2.1/yt_aspect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-20 18:56:46.000000 yt_aspect-0.2.1/yt_aspect.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-20 18:56:46.000000 yt_aspect-0.2.1/yt_aspect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 18:56:46.000000 yt_aspect-0.2.1/yt_aspect.egg-info/top_level.txt
```

### Comparing `yt_aspect-0.2.0/LICENSE` & `yt_aspect-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yt_aspect-0.2.0/PKG-INFO` & `yt_aspect-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt_aspect
-Version: 0.2.0
+Version: 0.2.1
 Summary: A yt plugin for loading ASPECT output
 Author-email: Chris Havlin <chris.havlin@gmail.com>
 Project-URL: Homepage, https://github.com/data-exp-lab/yt_aspect
 Project-URL: Bug Tracker, https://github.com/data-exp-lab/yt_aspect/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `yt_aspect-0.2.0/README.md` & `yt_aspect-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `yt_aspect-0.2.0/pyproject.toml` & `yt_aspect-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yt_aspect"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Chris Havlin", email="chris.havlin@gmail.com" },
 ]
 description="A yt plugin for loading ASPECT output"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `yt_aspect-0.2.0/tests/test_outputs.py` & `yt_aspect-0.2.1/tests/test_outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
         ("ASPECT", "shell_2D", 2),
         ("PVTU", "cleaned_aspect", 3),
     ),
 )
 def test_3d_aspect_load(
     pvtu_test_data, dataset_type, dataset_name, expected_dims, tmp_path
 ):
-
     fi = get_file_path_from_data_info(dataset_type, pvtu_test_data, dataset_name)
 
     if os.path.isfile(fi) is False:
         pytest.skip(f"Could not locate {fi}")
 
     ds = yt.load(fi)
     assert ds.dataset_type == dataset_type.lower()
@@ -59,15 +58,14 @@
 def _get_slice_frb(ds):
     slc = yt.SlicePlot(ds, "z", ("connect0", "Temperature2"))
     slc._setup_plots()
     return slc.frb[("connect0", "Temperature2")]
 
 
 def test_element_validation(pvtu_test_data):
-
     # this sample ds does not include null elements... so not a great test.
     fi = get_file_path_from_data_info("PVTU", pvtu_test_data, "two2_with_invalid_els")
     ds_1 = yt.load(fi, detect_null_elements=True)
     frb_1 = _get_slice_frb(ds_1)
     n_finite_no_null = np.isfinite(frb_1).sum()
 
     ds_0 = yt.load(fi, detect_null_elements=False)
```

### Comparing `yt_aspect-0.2.0/tests/test_utilities.py` & `yt_aspect-0.2.1/tests/test_utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,14 @@
         _ = yt_is("~", Version("1.0.0"))
 
 
 @pytest.mark.parametrize(
     "n_elements,nodes_per_element,n_invalid", [(5, 3, 2), (5, 8, 2), (5, 8, 0)]
 )
 def test_valid_element_mask(n_elements, nodes_per_element, n_invalid):
-
     one_element = np.arange(nodes_per_element)
     test_conn = np.repeat(one_element[:, np.newaxis], n_elements, axis=1).transpose()
 
     if n_invalid > 0:
         test_conn[-n_invalid:, :] = 1
 
     valid_elements, n_actual = _valid_element_mask(test_conn)
```

### Comparing `yt_aspect-0.2.0/yt_aspect/_utilities.py` & `yt_aspect-0.2.1/yt_aspect/_utilities.py`

 * *Files identical despite different names*

### Comparing `yt_aspect-0.2.0/yt_aspect/data_structures.py` & `yt_aspect-0.2.1/yt_aspect/data_structures.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,14 @@
 
         super()._setup_coordinate_handler(axis_order)
 
         self.coordinates._x_pairs = (("x", "y"), ("y", "x"), ("z", "x"))
         self.coordinates._y_pairs = (("x", "z"), ("y", "z"), ("z", "y"))
 
     def _parse_parameter_file(self):
-
         # store the top level pvtu info
         with open(self.parameter_filename) as pvtu_fi:
             self.parameters["pXML"] = xmltodict.parse(pvtu_fi.read())
 
         pieces = self.parameters["pXML"]["VTKFile"]["PUnstructuredGrid"]["Piece"]
         if not isinstance(pieces, list):
             pieces = [pieces]
@@ -295,15 +294,15 @@
         conns = []  # connectivity (node --> index of coordinate arrays)
         alloffs = []  # element offsets
         x, y, z = [], [], []  # node coordinates
         n_p_cells = []  # nodes per cell of each piece
         pieceoff = 0  # connectivity index offset between pieces
 
         # do some piece sanitization and documentation
-        if type(xmlPieces) != list:
+        if not isinstance(xmlPieces, list):
             # handles the case where we have a single piece in this vtu file
             xmlPieces = [xmlPieces]
         self._add_piece_to_field_map(src_file, xmlPieces)
 
         # loop over pieces of this vtu, decode and add to containers
         for piece_id in range(0, len(xmlPieces)):
             coords, conn, offsets, cell_types = decode_piece(xmlPieces[piece_id])
@@ -470,15 +469,14 @@
 
 
 class ASPECTUnstructuredMesh(PVTUMesh):
     _type_name = "aspect_unstructured_mesh"
 
 
 class ASPECTUnstructuredIndex(PVTUIndex):
-
     _mesh_class = ASPECTUnstructuredMesh
 
     def __init__(self, ds, dataset_type="aspect"):
         super().__init__(ds, dataset_type)
 
 
 class ASPECTDataset(PVTUDataset):
```

### Comparing `yt_aspect-0.2.0/yt_aspect/fields.py` & `yt_aspect-0.2.1/yt_aspect/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 
 class PVTUFieldInfo(FieldInfoContainer):
     pass
 
 
 class ASPECTFieldInfo(PVTUFieldInfo):
-
     known_other_fields = (
         ("T", ("K", [], None)),
         ("p", ("Pa", [], None)),
         ("viscosity", ("Pa*s", [], None)),
         ("velocity_x", ("m/s", [], None)),
         ("velocity_y", ("m/s", [], None)),
         ("velocity_z", ("m/s", [], None)),
@@ -35,15 +34,14 @@
         # Identical form to above
         # ( "name", ("units", ["fields", "to", "alias"], # "display_name")),
     )
 
     log_fields = ["viscosity", "strain_rate"]
 
     def __init__(self, ds, field_list):
-
         # add the stress tensors to the known fields
         for xx in ["xx", "xy", "xz", "yy", "yz", "zz"]:
             self.known_other_fields += (("shear_stress_" + xx, ("Pa", [], None)),)
             self.known_other_fields += (("stress_" + xx, ("Pa", [], None)),)
 
         super().__init__(ds, field_list)
         for name in self:
```

### Comparing `yt_aspect-0.2.0/yt_aspect/io.py` & `yt_aspect-0.2.1/yt_aspect/io.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,28 +51,27 @@
                 # rather than (n_elements, n_verts). These apply to all fields,
                 # so pull them out here:
                 mask = selector.fill_mesh_cell_mask(mesh)  # global mask
                 if mask is not None:
                     # each mesh piece will pull the connectivity, mask values
                     # for the indices corresponding to each vtu file
                     for vtu_id, vtu_fi in enumerate(mesh.filenames):
-
                         # the element mask for this piece
                         element_offset_start = el_counts[0:vtu_id].sum()
                         element_offset_end = element_offset_start + el_counts[vtu_id]
                         vtu_mask = mask[element_offset_start:element_offset_end]
 
                         # load this vtu's part of the mesh
                         vtu_file = os.path.join(self.ds.data_dir, vtu_fi)
                         f2id = self.ds.parameters["field_to_piece_index"][vtu_file]
                         with open(vtu_file) as data:
                             xml = xmltodict.parse(data.read())
                             xmlPieces = xml["VTKFile"]["UnstructuredGrid"]["Piece"]
 
-                        if type(xmlPieces) != list:
+                        if not isinstance(xmlPieces, list):
                             xmlPieces = [xmlPieces]
 
                         for field in fields:
                             ftype, fname = field
 
                             # check if we are dealing with a velocity component
                             vdim = -1
```

### Comparing `yt_aspect-0.2.0/yt_aspect/util.py` & `yt_aspect-0.2.1/yt_aspect/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     second = base64.decodebytes(blob[split_location:])
     if use_zlib:
         second = zlib.decompress(second)
     return np.frombuffer(first, dtype="<f4"), np.frombuffer(second, dtype=dtype)
 
 
 def _recursive_key_check(dict_inst: dict, nested_key_list: list) -> bool:
-
     key_len = len(nested_key_list)
     if key_len == 0:
         raise ValueError("nested_key_list must have at least 1 element")
 
     c_key = nested_key_list[0]  # the current key
     if key_len == 1:
         # at the final level
```

### Comparing `yt_aspect-0.2.0/yt_aspect.egg-info/PKG-INFO` & `yt_aspect-0.2.1/yt_aspect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: yt-aspect
-Version: 0.2.0
+Name: yt_aspect
+Version: 0.2.1
 Summary: A yt plugin for loading ASPECT output
 Author-email: Chris Havlin <chris.havlin@gmail.com>
 Project-URL: Homepage, https://github.com/data-exp-lab/yt_aspect
 Project-URL: Bug Tracker, https://github.com/data-exp-lab/yt_aspect/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

