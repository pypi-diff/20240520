# Comparing `tmp/bonsai_prp-0.8.1.tar.gz` & `tmp/bonsai_prp-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bonsai_prp-0.8.1.tar", last modified: Thu May 16 14:43:54 2024, max compression
+gzip compressed data, was "bonsai_prp-0.8.2.tar", last modified: Mon May 20 12:04:43 2024, max compression
```

## Comparing `bonsai_prp-0.8.1.tar` & `bonsai_prp-0.8.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:43:54.521755 bonsai_prp-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-16 14:43:54.521755 bonsai_prp-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:43:54.517755 bonsai_prp-0.8.1/bonsai_prp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-16 14:43:54.000000 bonsai_prp-0.8.1/bonsai_prp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-16 14:43:54.000000 bonsai_prp-0.8.1/bonsai_prp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 14:43:54.000000 bonsai_prp-0.8.1/bonsai_prp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-16 14:43:54.000000 bonsai_prp-0.8.1/bonsai_prp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-16 14:43:54.000000 bonsai_prp-0.8.1/bonsai_prp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-16 14:43:54.000000 bonsai_prp-0.8.1/bonsai_prp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:43:54.513755 bonsai_prp-0.8.1/prp/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17803 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:43:54.517755 bonsai_prp-0.8.1/prp/models/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/models/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/models/phenotype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/models/qc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/models/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/models/species.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/models/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/models/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:43:54.517755 bonsai_prp-0.8.1/prp/parse/
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/parse/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/parse/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:43:54.517755 bonsai_prp-0.8.1/prp/parse/phenotype/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/parse/phenotype/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7084 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/parse/phenotype/amrfinder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/parse/phenotype/mykrobe.py
--rw-r--r--   0 runner    (1001) docker     (127)    14440 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/parse/phenotype/resfinder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/parse/phenotype/serotypefinder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/parse/phenotype/tbprofiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/parse/phenotype/virulencefinder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11232 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/parse/qc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/parse/species.py
--rw-r--r--   0 runner    (1001) docker     (127)     8005 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/parse/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10933 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/parse/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/prp/parse/variant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 14:43:54.521755 bonsai_prp-0.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:43:54.517755 bonsai_prp-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7892 2024-05-16 14:43:44.000000 bonsai_prp-0.8.1/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:04:43.721355 bonsai_prp-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-20 12:04:34.000000 bonsai_prp-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-20 12:04:43.721355 bonsai_prp-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-20 12:04:34.000000 bonsai_prp-0.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:04:43.721355 bonsai_prp-0.8.2/bonsai_prp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-20 12:04:43.000000 bonsai_prp-0.8.2/bonsai_prp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-20 12:04:43.000000 bonsai_prp-0.8.2/bonsai_prp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 12:04:43.000000 bonsai_prp-0.8.2/bonsai_prp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-20 12:04:43.000000 bonsai_prp-0.8.2/bonsai_prp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-20 12:04:43.000000 bonsai_prp-0.8.2/bonsai_prp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-20 12:04:43.000000 bonsai_prp-0.8.2/bonsai_prp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:04:43.717355 bonsai_prp-0.8.2/prp/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-20 12:04:34.000000 bonsai_prp-0.8.2/prp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-20 12:04:34.000000 bonsai_prp-0.8.2/prp/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17673 2024-05-20 12:04:34.000000 bonsai_prp-0.8.2/prp/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:04:43.717355 bonsai_prp-0.8.2/prp/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-20 12:04:34.000000 bonsai_prp-0.8.2/prp/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-20 12:04:34.000000 bonsai_prp-0.8.2/prp/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-20 12:04:34.000000 bonsai_prp-0.8.2/prp/models/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-05-20 12:04:34.000000 bonsai_prp-0.8.2/prp/models/phenotype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-20 12:04:34.000000 bonsai_prp-0.8.2/prp/models/qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-20 12:04:34.000000 bonsai_prp-0.8.2/prp/models/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-20 12:04:34.000000 bonsai_prp-0.8.2/prp/models/species.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-20 12:04:34.000000 bonsai_prp-0.8.2/prp/models/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-20 12:04:34.000000 bonsai_prp-0.8.2/prp/models/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:04:43.717355 bonsai_prp-0.8.2/prp/parse/
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-20 12:04:34.000000 bonsai_prp-0.8.2/prp/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-20 12:04:34.000000 bonsai_prp-0.8.2/prp/parse/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-20 12:04:34.000000 bonsai_prp-0.8.2/prp/parse/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:04:43.721355 bonsai_prp-0.8.2/prp/parse/phenotype/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-20 12:04:34.000000 bonsai_prp-0.8.2/prp/parse/phenotype/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7084 2024-05-20 12:04:34.000000 bonsai_prp-0.8.2/prp/parse/phenotype/amrfinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-20 12:04:34.000000 bonsai_prp-0.8.2/prp/parse/phenotype/mykrobe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14440 2024-05-20 12:04:34.000000 bonsai_prp-0.8.2/prp/parse/phenotype/resfinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-20 12:04:34.000000 bonsai_prp-0.8.2/prp/parse/phenotype/serotypefinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-05-20 12:04:34.000000 bonsai_prp-0.8.2/prp/parse/phenotype/tbprofiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-20 12:04:34.000000 bonsai_prp-0.8.2/prp/parse/phenotype/virulencefinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11232 2024-05-20 12:04:34.000000 bonsai_prp-0.8.2/prp/parse/qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-20 12:04:34.000000 bonsai_prp-0.8.2/prp/parse/species.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-05-20 12:04:34.000000 bonsai_prp-0.8.2/prp/parse/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10933 2024-05-20 12:04:34.000000 bonsai_prp-0.8.2/prp/parse/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-20 12:04:34.000000 bonsai_prp-0.8.2/prp/parse/variant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-20 12:04:34.000000 bonsai_prp-0.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 12:04:43.721355 bonsai_prp-0.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:04:43.721355 bonsai_prp-0.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7892 2024-05-20 12:04:34.000000 bonsai_prp-0.8.2/tests/test_cli.py
```

### Comparing `bonsai_prp-0.8.1/LICENSE` & `bonsai_prp-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.1/PKG-INFO` & `bonsai_prp-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bonsai-prp
-Version: 0.8.1
+Version: 0.8.2
 Summary: Pipline result processing program for the JASEN pipeline and Bonsai tool.
 Author-email: Markus Johansson <markus.h.johansson@skane.se>, Ryan Kennedy <Ryan.Kennedy@skane.se>
 Project-URL: Repository, https://github.com/Clinical-Genomics-Lund/
 Project-URL: Issues, https://github.com/Clinical-Genomics-Lund/bonsai-prp/issues
 Project-URL: Changelog, https://github.com/Clinical-Genomics-Lund/CHANGELOG.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
```

### Comparing `bonsai_prp-0.8.1/README.md` & `bonsai_prp-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.1/bonsai_prp.egg-info/PKG-INFO` & `bonsai_prp-0.8.2/bonsai_prp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bonsai-prp
-Version: 0.8.1
+Version: 0.8.2
 Summary: Pipline result processing program for the JASEN pipeline and Bonsai tool.
 Author-email: Markus Johansson <markus.h.johansson@skane.se>, Ryan Kennedy <Ryan.Kennedy@skane.se>
 Project-URL: Repository, https://github.com/Clinical-Genomics-Lund/
 Project-URL: Issues, https://github.com/Clinical-Genomics-Lund/bonsai-prp/issues
 Project-URL: Changelog, https://github.com/Clinical-Genomics-Lund/CHANGELOG.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
```

### Comparing `bonsai_prp-0.8.1/bonsai_prp.egg-info/SOURCES.txt` & `bonsai_prp-0.8.2/bonsai_prp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.1/prp/cli.py` & `bonsai_prp-0.8.2/prp/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,16 @@
     parse_resfinder_amr_pred,
     parse_serotypefinder_oh_typing,
     parse_tbprofiler_amr_pred,
     parse_tbprofiler_lineage_results,
     parse_virulencefinder_stx_typing,
     parse_virulencefinder_vir_pred,
 )
-from .parse.species import get_mykrobe_spp_prediction
 from .parse.metadata import get_database_info, get_gb_genome_version, parse_run_info
+from .parse.species import get_mykrobe_spp_prediction
 from .parse.utils import _get_path, get_db_version, parse_input_dir
 from .parse.variant import annotate_delly_variants
 
 logging.basicConfig(
     level=logging.INFO, format="[%(asctime)s] %(levelname)s in %(module)s: %(message)s"
 )
 LOG = logging.getLogger(__name__)
@@ -258,21 +258,19 @@
             SoupVersion(
                 name="mykrobe-predictor",
                 version=pred_res[0]["mykrobe_version"],
                 type=SoupType.DB,
             )
         )
         # parse mykrobe result
-        amr_res = parse_mykrobe_amr_pred(pred_res, ElementType.AMR)
+        amr_res = parse_mykrobe_amr_pred(pred_res)
         if amr_res is not None:
             results["element_type_result"].append(amr_res)
 
-        lin_res: MethodIndex | None = parse_mykrobe_lineage_results(
-            pred_res, TypingMethod.LINEAGE
-        )
+        lin_res: MethodIndex | None = parse_mykrobe_lineage_results(pred_res)
         if lin_res is not None:
             results["typing_result"].append(lin_res)
 
         # parse mykrobe species prediction result
         results["species_prediction"].append(get_mykrobe_spp_prediction(pred_res))
 
     # tbprofiler
@@ -285,19 +283,17 @@
                 SoupVersion(
                     name=pred_res["pipeline"]["db_version"]["name"],
                     version=get_db_version(pred_res["pipeline"]["db_version"]),
                     type=SoupType.DB,
                 )
             ]
             results["run_metadata"]["databases"].extend(db_info)
-            lin_res: MethodIndex = parse_tbprofiler_lineage_results(
-                pred_res, TypingMethod.LINEAGE
-            )
+            lin_res: MethodIndex = parse_tbprofiler_lineage_results(pred_res)
             results["typing_result"].append(lin_res)
-            amr_res: MethodIndex = parse_tbprofiler_amr_pred(pred_res, ElementType.AMR)
+            amr_res: MethodIndex = parse_tbprofiler_amr_pred(pred_res)
             results["element_type_result"].append(amr_res)
 
     # parse SNV and SV variants.
     if snv_vcf:
         results["snv_variants"] = load_variants(snv_vcf)
 
     if sv_vcf:
```

### Comparing `bonsai_prp-0.8.1/prp/models/metadata.py` & `bonsai_prp-0.8.2/prp/models/metadata.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.1/prp/models/phenotype.py` & `bonsai_prp-0.8.2/prp/models/phenotype.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.1/prp/models/qc.py` & `bonsai_prp-0.8.2/prp/models/qc.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.1/prp/models/sample.py` & `bonsai_prp-0.8.2/prp/models/sample.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,34 +5,36 @@
 
 from .base import RWModel
 from .metadata import RunMetadata
 from .phenotype import ElementType, ElementTypeResult, PredictionSoftware, VariantBase
 from .qc import QcMethodIndex
 from .species import SppMethodIndex
 from .typing import (
+    ResultLineageBase,
+    TbProfilerLineage,
     TypingMethod,
     TypingResultCgMlst,
     TypingResultGeneAllele,
-    TypingResultLineage,
     TypingResultMlst,
     TypingSoftware,
 )
 
 
 class MethodIndex(RWModel):
     """Container for key-value lookup of analytical results."""
 
     type: Union[ElementType, TypingMethod]
     software: PredictionSoftware | TypingSoftware | None
     result: Union[
         ElementTypeResult,
         TypingResultMlst,
         TypingResultCgMlst,
-        TypingResultLineage,
         TypingResultGeneAllele,
+        ResultLineageBase,
+        TbProfilerLineage,
     ]
 
 
 class SampleBase(RWModel):
     """Base datamodel for sample data structure"""
 
     run_metadata: RunMetadata = Field(..., alias="runMetadata")
```

### Comparing `bonsai_prp-0.8.1/prp/models/species.py` & `bonsai_prp-0.8.2/prp/models/species.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Species related data models."""
 
 from enum import Enum
 from typing import List
 
 from pydantic import Field
-from .phenotype import ElementTypeResult, PredictionSoftware
 
 from .base import RWModel
+from .phenotype import ElementTypeResult, PredictionSoftware
 
 
 class TaxLevel(Enum):
     """Braken phylogenetic level."""
 
     P = "phylum"
     C = "class"
```

### Comparing `bonsai_prp-0.8.1/prp/models/tags.py` & `bonsai_prp-0.8.2/prp/models/tags.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.1/prp/models/typing.py` & `bonsai_prp-0.8.2/prp/models/typing.py`

 * *Files 23% similar despite different names*

```diff
@@ -47,67 +47,56 @@
 class MlstErrors(str, Enum):
     """MLST error codes."""
 
     NOVEL = "novel"
     PARTIAL = "partial"
 
 
-class LineageInformation(RWModel):
-    """Base class for storing lineage information typing results"""
-
-    lin: str | None = None
-    family: str | None = None
-    spoligotype: str | None = None
-    rd: str | None = None
-    fraction: float | None = None
-    variant: str | None = None
-    coverage: Dict[str, Any] | None = None
-
-
 class ResultMlstBase(RWModel):
     """Base class for storing MLST-like typing results"""
 
     alleles: Dict[str, Union[int, str, List, None]]
 
 
-class ResultLineageBase(RWModel):
-    """Base class for storing MLST-like typing results"""
-
-    lineages: List[LineageInformation]
-
-
 class TypingResultMlst(ResultMlstBase):
     """MLST results"""
 
     scheme: str
     sequence_type: Optional[int] = Field(None, alias="sequenceType")
 
 
 class TypingResultCgMlst(ResultMlstBase):
     """MLST results"""
 
     n_novel: int = Field(0, alias="nNovel")
     n_missing: int = Field(0, alias="nNovel")
 
 
-class TypingResultLineage(ResultLineageBase):
+class ResultLineageBase(RWModel):
     """Lineage results"""
 
     lineage_depth: float | None = None
-    main_lin: str
-    sublin: str
+    main_lineage: str
+    sublineage: str
+
 
+class LineageInformation(RWModel):
+    """Base class for storing lineage information typing results"""
 
-class TypingResultPhylogenetics(TypingResultLineage):
-    """Phylogenetics results"""
+    lineage: str | None
+    family: str | None
+    rd: str | None
+    fraction: float | None
+    support: List[Dict[str, Any]] | None = None
 
-    phylo_group_depth: float | None = None
-    phylo_group: str | None = None
-    species_depth: float | None = None
-    species: str | None = None
+
+class TbProfilerLineage(ResultLineageBase):
+    """Base class for storing MLST-like typing results"""
+
+    lineages: List[LineageInformation]
 
 
 class TypingResultGeneAllele(VirulenceGene, SerotypeGene):
     """Identification of individual gene alleles."""
 
 
 CgmlstAlleles = Dict[str, int | None | ChewbbacaErrors | MlstErrors | List[int]]
```

### Comparing `bonsai_prp-0.8.1/prp/parse/__init__.py` & `bonsai_prp-0.8.2/prp/parse/__init__.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.1/prp/parse/metadata.py` & `bonsai_prp-0.8.2/prp/parse/metadata.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.1/prp/parse/phenotype/amrfinder.py` & `bonsai_prp-0.8.2/prp/parse/phenotype/amrfinder.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.1/prp/parse/phenotype/mykrobe.py` & `bonsai_prp-0.8.2/prp/parse/phenotype/mykrobe.py`

 * *Files 3% similar despite different names*

```diff
@@ -138,26 +138,24 @@
     # sort variants
     variants = sorted(
         results, key=lambda entry: (entry.reference_sequence, entry.start)
     )
     return variants
 
 
-def parse_mykrobe_amr_pred(
-    prediction: Dict[str, Any], resistance_category
-) -> ElementTypeResult | None:
+def parse_mykrobe_amr_pred(prediction: Dict[str, Any]) -> ElementTypeResult | None:
     """Parse mykrobe resistance prediction results."""
     LOG.info("Parsing mykrobe prediction")
     resistance = ElementTypeResult(
         phenotypes=_get_mykrobe_amr_sr_profie(prediction),
         genes=[],
         variants=_parse_mykrobe_amr_variants(prediction),
     )
 
     # verify prediction result
     if is_prediction_result_empty(resistance):
         result = None
     else:
         result = MethodIndex(
-            type=resistance_category, software=Software.MYKROBE, result=resistance
+            type=ElementType.AMR, software=Software.MYKROBE, result=resistance
         )
     return result
```

### Comparing `bonsai_prp-0.8.1/prp/parse/phenotype/resfinder.py` & `bonsai_prp-0.8.2/prp/parse/phenotype/resfinder.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.1/prp/parse/phenotype/serotypefinder.py` & `bonsai_prp-0.8.2/prp/parse/phenotype/serotypefinder.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.1/prp/parse/phenotype/tbprofiler.py` & `bonsai_prp-0.8.2/prp/parse/phenotype/tbprofiler.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,19 +125,20 @@
     phenotypes = []
     for drug in drugs:
         # assign element type
         if drug["type"] == "drug_resistance" or drug["type"] == "who_confidence":
             drug_type = ElementType.AMR
         else:
             drug_type = ElementType.AMR
-            LOG.warning((
-                "Unknown TbProfiler drug; drug: %s"
-                ", confers resistance with confidence"
-                ": %s; default to %s"
-            ),
+            LOG.warning(
+                (
+                    "Unknown TbProfiler drug; drug: %s"
+                    ", confers resistance with confidence"
+                    ": %s; default to %s"
+                ),
                 drug["type"],
                 drug["confidence"],
                 drug_type,
             )
         reference = drug.get("comment")
         phenotypes.append(
             PhenotypeInfo(
@@ -150,19 +151,19 @@
                 source=drug.get("source"),
             )
         )
     return phenotypes
 
 
 def parse_tbprofiler_amr_pred(
-    prediction: Dict[str, Any], resistance_category
+    prediction: Dict[str, Any]
 ) -> Tuple[SoupVersions, ElementTypeResult]:
     """Parse tbprofiler resistance prediction results."""
     LOG.info("Parsing tbprofiler prediction")
     resistance = ElementTypeResult(
         phenotypes=_get_tbprofiler_amr_sr_profie(prediction),
         genes=[],
         variants=_parse_tbprofiler_amr_variants(prediction),
     )
     return MethodIndex(
-        type=resistance_category, software=Software.TBPROFILER, result=resistance
+        type=ElementType.AMR, software=Software.TBPROFILER, result=resistance
     )
```

### Comparing `bonsai_prp-0.8.1/prp/parse/phenotype/virulencefinder.py` & `bonsai_prp-0.8.2/prp/parse/phenotype/virulencefinder.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.1/prp/parse/qc.py` & `bonsai_prp-0.8.2/prp/parse/qc.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.1/prp/parse/species.py` & `bonsai_prp-0.8.2/prp/parse/species.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 """Parsers for species prediction tools."""
 
 import logging
-from typing import Dict, Any, List
+from typing import Any, Dict, List
 
 import pandas as pd
-from prp.models.species import SppMethodIndex, SppPredictionSoftware, MykrobeSpeciesPrediction
+
+from prp.models.species import (
+    MykrobeSpeciesPrediction,
+    SppMethodIndex,
+    SppPredictionSoftware,
+)
 
 LOG = logging.getLogger(__name__)
 
 
 def parse_kraken_result(file: str, cutoff: float = 0.0001) -> SppMethodIndex:
     """parse_species_pred""Parse species prediciton result"""
     tax_lvl_dict = {
@@ -29,21 +34,19 @@
     )
     # cast as method index
     return SppMethodIndex(
         software=SppPredictionSoftware.BRACKEN,
         result=species_pred.to_dict(orient="records"),
     )
 
+
 def get_mykrobe_spp_prediction(prediction: List[Dict[str, Any]]) -> SppMethodIndex:
     """Get species prediction result from Mykrobe."""
     LOG.info("Parsing Mykrobe spp result.")
     spp_pred = MykrobeSpeciesPrediction(
         scientific_name=prediction[0]["species"].replace("_", " "),
         taxonomy_id=None,
         phylogenetic_group=prediction[0]["phylo_group"].replace("_", " "),
         phylogenetic_group_coverage=prediction[0]["phylo_group_per_covg"],
         species_coverage=prediction[0]["species_per_covg"],
     )
-    return SppMethodIndex(
-        software=SppPredictionSoftware.MYKROBE,
-        result=[spp_pred]
-    )
+    return SppMethodIndex(software=SppPredictionSoftware.MYKROBE, result=[spp_pred])
```

### Comparing `bonsai_prp-0.8.1/prp/parse/typing.py` & `bonsai_prp-0.8.2/prp/parse/typing.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 import json
 import logging
 from typing import List
 
 from ..models.sample import MethodIndex
 from ..models.typing import (
     LineageInformation,
+    ResultLineageBase,
+    TbProfilerLineage,
     TypingMethod,
     TypingResultCgMlst,
     TypingResultGeneAllele,
     TypingResultMlst,
-    TypingResultPhylogenetics,
 )
 from ..models.typing import TypingSoftware as Software
 from .phenotype.serotypefinder import parse_serotype_gene
 from .phenotype.virulencefinder import parse_vir_gene
 
 LOG = logging.getLogger(__name__)
 
@@ -40,29 +41,31 @@
 def parse_mlst_results(mlst_fpath: str) -> TypingResultMlst:
     """Parse mlst results from mlst to json object."""
     LOG.info("Parsing mlst results")
     with open(mlst_fpath, "r", encoding="utf-8") as jsonfile:
         result = json.load(jsonfile)[0]
         result_obj = TypingResultMlst(
             scheme=result["scheme"],
-            sequence_type=None
-            if result["sequence_type"] == "-"
-            else result["sequence_type"],
+            sequence_type=(
+                None if result["sequence_type"] == "-" else result["sequence_type"]
+            ),
             alleles={
                 gene: _process_allele_call(allele)
                 for gene, allele in result["alleles"].items()
             },
         )
     return MethodIndex(
         type=TypingMethod.MLST, software=Software.MLST, result=result_obj
     )
 
 
 def parse_cgmlst_results(
-    chewbacca_res_path: str, include_novel_alleles: bool = True, correct_alleles: bool = False
+    chewbacca_res_path: str,
+    include_novel_alleles: bool = True,
+    correct_alleles: bool = False,
 ) -> TypingResultCgMlst:
     """Parse chewbbaca cgmlst prediction results to json results.
 
     Chewbbaca reports errors in allele profile.
     See: https://github.com/B-UMMI/chewBBACA
     -------------------
     INF-<allele name>, inferred new allele
@@ -100,15 +103,15 @@
         return allele
 
     LOG.info(
         "Parsing cgmslt results, %s including novel alleles",
         "not" if not include_novel_alleles else "",
     )
 
-    with open(chewbacca_res_path, encoding='utf-8') as fileh:
+    with open(chewbacca_res_path, encoding="utf-8") as fileh:
         creader = csv.reader(fileh, delimiter="\t")
         _, *allele_names = (colname.rstrip(".fasta") for colname in next(creader))
         # parse alleles
         _, *alleles = next(creader)
     corrected_alleles = (replace_errors(a) for a in alleles)
     results = TypingResultCgMlst(
         n_novel=sum(1 for a in alleles if a.startswith("INF")),
@@ -116,64 +119,55 @@
         alleles=dict(zip(allele_names, corrected_alleles)),
     )
     return MethodIndex(
         type=TypingMethod.CGMLST, software=Software.CHEWBBACA, result=results
     )
 
 
-def parse_tbprofiler_lineage_results(
-    pred_res: dict, method
-) -> TypingResultPhylogenetics:
+def parse_tbprofiler_lineage_results(pred_res: dict) -> MethodIndex:
     """Parse tbprofiler results for lineage object."""
     LOG.info("Parsing lineage results")
-    result_obj = TypingResultPhylogenetics(
-        phylo_group_depth=None,
-        species_depth=None,
-        lineage_depth=None,
-        phylo_group=None,
-        species=None,
-        main_lin=pred_res["main_lineage"],
-        sublin=pred_res["sub_lineage"],
-        lineages=pred_res["lineage"],
-    )
-    return MethodIndex(type=method, software=Software.TBPROFILER, result=result_obj)
-
-
-def parse_mykrobe_lineage_results(
-    pred_res: dict, method
-) -> TypingResultPhylogenetics | None:
+    # lineages
+    lineages = [
+        LineageInformation(
+            lineage=lin["lineage"],
+            family=lin["family"],
+            rd=lin["rd"],
+            fraction=lin["fraction"],
+            support=lin["support"],
+        )
+        for lin in pred_res["lineage"]
+    ]
+    # combine into result
+    result_obj = TbProfilerLineage(
+        main_lineage=pred_res["main_lineage"],
+        sublineage=pred_res["sub_lineage"],
+        lineages=lineages,
+    )
+    # store result as a method index
+    return MethodIndex(
+        type=TypingMethod.LINEAGE,
+        software=Software.TBPROFILER,
+        result=result_obj,
+    )
+
+
+def parse_mykrobe_lineage_results(pred_res: dict) -> MethodIndex | None:
     """Parse mykrobe results for lineage object."""
     LOG.info("Parsing lineage results")
     if pred_res:
-        lineage = pred_res[0]
-        phylo_group_depth = lineage["phylo_group_depth"]
-        species_depth = lineage["species_depth"]
-        lineage_depth = lineage["lineage_depth"]
-        split_lin = lineage["lineage"].split(".")
-        main_lin = split_lin[0]
-        sublin = lineage["lineage"]
-        lin_idxs = lineage["lineage"].lstrip("lineage").split(".")
-        lineages = [
-            LineageInformation(lineage="lineage" + ".".join(lin_idxs[: idx + 1]))
-            for idx in range(len(lin_idxs))
-        ]
+        lineage = pred_res[0]["lineage"]
         # cast to lineage object
-        result_obj = TypingResultPhylogenetics(
-            phylo_group_depth=float(phylo_group_depth)
-            if phylo_group_depth
-            else phylo_group_depth,
-            species_depth=float(species_depth) if species_depth else species_depth,
-            lineage_depth=float(lineage_depth) if lineage_depth else lineage_depth,
-            phylo_group=lineage["phylo_group"],
-            species=lineage["species"],
-            main_lin=main_lin,
-            sublin=sublin,
-            lineages=lineages,
+        result_obj = ResultLineageBase(
+            main_lineage=lineage.split(".")[0],
+            sublineage=lineage,
+        )
+        return MethodIndex(
+            type=TypingMethod.LINEAGE, software=Software.MYKROBE, result=result_obj
         )
-        return MethodIndex(type=method, software=Software.MYKROBE, result=result_obj)
     return None
 
 
 def parse_virulencefinder_stx_typing(path: str) -> MethodIndex | None:
     """Parse virulencefinder's output re stx typing"""
     with open(path, "rb") as inpt:
         pred_obj = json.load(inpt)
```

### Comparing `bonsai_prp-0.8.1/prp/parse/utils.py` & `bonsai_prp-0.8.2/prp/parse/utils.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.1/prp/parse/variant.py` & `bonsai_prp-0.8.2/prp/parse/variant.py`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.1/pyproject.toml` & `bonsai_prp-0.8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bonsai_prp-0.8.1/tests/test_cli.py` & `bonsai_prp-0.8.2/tests/test_cli.py`

 * *Files identical despite different names*

