# Comparing `tmp/cellxgene_lamin-0.2.1.tar.gz` & `tmp/cellxgene_lamin-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellxgene_lamin-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cellxgene_lamin-0.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cellxgene_lamin-0.2.1.tar` & `cellxgene_lamin-0.2.2.tar`

### file list

```diff
@@ -1,37 +1,40 @@
--rw-r--r--   0        0        0     5051 2024-04-02 09:35:42.292041 cellxgene_lamin-0.2.1/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2024-03-19 12:35:39.229740 cellxgene_lamin-0.2.1/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2024-03-19 12:35:39.233074 cellxgene_lamin-0.2.1/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1252 2024-03-19 12:35:39.233074 cellxgene_lamin-0.2.1/.gitignore
--rw-r--r--   0        0        0     1444 2024-03-27 14:52:05.525051 cellxgene_lamin-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2024-03-19 12:35:39.233074 cellxgene_lamin-0.2.1/LICENSE
--rw-r--r--   0        0        0      607 2024-03-19 12:35:39.233074 cellxgene_lamin-0.2.1/README.md
--rw-r--r--   0        0        0      444 2024-04-02 09:49:14.604374 cellxgene_lamin-0.2.1/cellxgene_lamin/__init__.py
--rw-r--r--   0        0        0     6951 2024-04-02 09:35:42.292041 cellxgene_lamin-0.2.1/cellxgene_lamin/_annotate.py
--rw-r--r--   0        0        0      538 2024-03-19 12:35:39.233074 cellxgene_lamin-0.2.1/cellxgene_lamin/_curate.py
--rw-r--r--   0        0        0      796 2024-03-19 12:35:39.233074 cellxgene_lamin-0.2.1/cellxgene_lamin/_cxg_rest.py
--rw-r--r--   0        0        0     1834 2024-03-19 12:35:39.233074 cellxgene_lamin-0.2.1/cellxgene_lamin/_features.py
--rw-r--r--   0        0        0     1409 2024-03-19 12:35:39.233074 cellxgene_lamin-0.2.1/cellxgene_lamin/_fields.py
--rw-r--r--   0        0        0     2024 2024-03-19 12:35:39.233074 cellxgene_lamin-0.2.1/cellxgene_lamin/_gene.py
--rw-r--r--   0        0        0     1435 2024-03-26 15:16:11.446346 cellxgene_lamin-0.2.1/cellxgene_lamin/_labels.py
--rw-r--r--   0        0        0     3819 2024-03-26 15:16:11.446346 cellxgene_lamin-0.2.1/cellxgene_lamin/_ontology.py
--rw-r--r--   0        0        0     1538 2024-03-26 15:16:11.446346 cellxgene_lamin-0.2.1/cellxgene_lamin/_organism.py
--rw-r--r--   0        0        0     1334 2024-03-19 12:35:39.233074 cellxgene_lamin-0.2.1/cellxgene_lamin/datasets.py
--rw-r--r--   0        0        0    11323 2024-04-02 09:35:42.292041 cellxgene_lamin-0.2.1/docs/cellxgene-annotate.ipynb
--rw-r--r--   0        0        0    17787 2024-03-28 12:38:15.901980 cellxgene_lamin-0.2.1/docs/cellxgene.ipynb
--rw-r--r--   0        0        0     6674 2024-04-02 09:49:41.607896 cellxgene_lamin-0.2.1/docs/changelog.md
--rw-r--r--   0        0        0      148 2024-03-28 12:38:15.901980 cellxgene_lamin-0.2.1/docs/index.md
--rw-r--r--   0        0        0      594 2024-03-19 12:35:39.233074 cellxgene_lamin-0.2.1/docs/notebooks.md
--rw-r--r--   0        0        0   443766 2024-03-19 17:00:30.489432 cellxgene_lamin-0.2.1/docs/notebooks/cencus-release-2023-12-15-LTS.ipynb
--rw-r--r--   0        0        0    71734 2024-03-19 17:00:30.489432 cellxgene_lamin-0.2.1/docs/notebooks/census-release-2023-07-25.ipynb
--rw-r--r--   0        0        0   351322 2024-03-19 17:00:30.492765 cellxgene_lamin-0.2.1/docs/notebooks/census-release-2023-11-13.ipynb
--rw-r--r--   0        0        0   104755 2024-03-19 17:00:30.492765 cellxgene_lamin-0.2.1/docs/notebooks/census-release-2023-12-06.ipynb
--rw-r--r--   0        0        0    33056 2024-03-19 17:00:30.492765 cellxgene_lamin-0.2.1/docs/notebooks/files-meta.ipynb
--rw-r--r--   0        0        0    20552 2024-03-19 17:00:30.492765 cellxgene_lamin-0.2.1/docs/notebooks/files.ipynb
--rw-r--r--   0        0        0    36950 2024-03-19 17:00:30.492765 cellxgene_lamin-0.2.1/docs/notebooks/meta-human.ipynb
--rw-r--r--   0        0        0  1299626 2024-03-19 17:00:30.496099 cellxgene_lamin-0.2.1/docs/notebooks/meta-mouse.ipynb
--rw-r--r--   0        0        0     8775 2024-03-27 14:56:24.485955 cellxgene_lamin-0.2.1/docs/query-census.ipynb
--rw-r--r--   0        0        0      176 2024-03-19 12:35:39.259740 cellxgene_lamin-0.2.1/lamin-project.yaml
--rw-r--r--   0        0        0     1927 2024-04-02 09:35:42.292041 cellxgene_lamin-0.2.1/noxfile.py
--rw-r--r--   0        0        0     3860 2024-04-02 09:49:20.917752 cellxgene_lamin-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      464 2024-03-28 12:38:15.901980 cellxgene_lamin-0.2.1/tests/test_notebooks.py
--rw-r--r--   0        0        0     1472 1970-01-01 00:00:00.000000 cellxgene_lamin-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     4714 2024-04-24 11:56:35.004410 cellxgene_lamin-0.2.2/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-09-05 14:07:08.719114 cellxgene_lamin-0.2.2/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-09-05 14:07:08.719576 cellxgene_lamin-0.2.2/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1266 2024-04-15 15:55:14.484689 cellxgene_lamin-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1521 2024-04-18 07:38:18.332861 cellxgene_lamin-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-09-05 14:07:08.699075 cellxgene_lamin-0.2.2/LICENSE
+-rw-r--r--   0        0        0      607 2024-03-26 16:54:13.778817 cellxgene_lamin-0.2.2/README.md
+-rw-r--r--   0        0        0      444 2024-05-20 11:09:57.044595 cellxgene_lamin-0.2.2/cellxgene_lamin/__init__.py
+-rw-r--r--   0        0        0     7561 2024-04-24 11:40:52.019559 cellxgene_lamin-0.2.2/cellxgene_lamin/_annotate.py
+-rw-r--r--   0        0        0      538 2024-03-19 11:05:18.090849 cellxgene_lamin-0.2.2/cellxgene_lamin/_curate.py
+-rw-r--r--   0        0        0      796 2024-01-17 12:35:32.450804 cellxgene_lamin-0.2.2/cellxgene_lamin/_cxg_rest.py
+-rw-r--r--   0        0        0     1834 2024-01-17 12:35:32.451118 cellxgene_lamin-0.2.2/cellxgene_lamin/_features.py
+-rw-r--r--   0        0        0     1409 2024-03-19 11:05:18.091120 cellxgene_lamin-0.2.2/cellxgene_lamin/_fields.py
+-rw-r--r--   0        0        0     2024 2024-02-01 06:48:25.424516 cellxgene_lamin-0.2.2/cellxgene_lamin/_gene.py
+-rw-r--r--   0        0        0     1435 2024-03-26 16:54:13.779949 cellxgene_lamin-0.2.2/cellxgene_lamin/_labels.py
+-rw-r--r--   0        0        0     3819 2024-03-26 16:54:13.780676 cellxgene_lamin-0.2.2/cellxgene_lamin/_ontology.py
+-rw-r--r--   0        0        0     1538 2024-03-26 16:54:13.781190 cellxgene_lamin-0.2.2/cellxgene_lamin/_organism.py
+-rw-r--r--   0        0        0     1334 2024-03-19 11:05:18.091640 cellxgene_lamin-0.2.2/cellxgene_lamin/datasets.py
+-rw-r--r--   0        0        0        0 2024-04-18 07:38:18.333538 cellxgene_lamin-0.2.2/cellxgene_lamin/schemas/__init__.py
+-rw-r--r--   0        0        0      810 2024-04-18 07:38:18.333743 cellxgene_lamin-0.2.2/cellxgene_lamin/schemas/_schema_versions.py
+-rw-r--r--   0        0        0     1136 2024-04-18 07:38:18.333881 cellxgene_lamin-0.2.2/cellxgene_lamin/schemas/schema_versions.yml
+-rw-r--r--   0        0        0    11325 2024-04-16 07:57:46.620429 cellxgene_lamin-0.2.2/docs/cellxgene-annotate.ipynb
+-rw-r--r--   0        0        0    16617 2024-05-20 11:09:44.149538 cellxgene_lamin-0.2.2/docs/cellxgene.ipynb
+-rw-r--r--   0        0        0     7578 2024-05-20 11:09:52.313754 cellxgene_lamin-0.2.2/docs/changelog.md
+-rw-r--r--   0        0        0      148 2024-03-28 11:40:09.464328 cellxgene_lamin-0.2.2/docs/index.md
+-rw-r--r--   0        0        0      594 2024-01-17 12:35:32.452724 cellxgene_lamin-0.2.2/docs/notebooks.md
+-rw-r--r--   0        0        0   443766 2024-01-30 09:11:06.175677 cellxgene_lamin-0.2.2/docs/notebooks/cencus-release-2023-12-15-LTS.ipynb
+-rw-r--r--   0        0        0    71734 2024-01-30 09:11:06.176308 cellxgene_lamin-0.2.2/docs/notebooks/census-release-2023-07-25.ipynb
+-rw-r--r--   0        0        0   351322 2023-12-13 19:44:16.010428 cellxgene_lamin-0.2.2/docs/notebooks/census-release-2023-11-13.ipynb
+-rw-r--r--   0        0        0   104755 2024-01-08 15:58:36.215190 cellxgene_lamin-0.2.2/docs/notebooks/census-release-2023-12-06.ipynb
+-rw-r--r--   0        0        0    33056 2023-11-16 10:21:52.333881 cellxgene_lamin-0.2.2/docs/notebooks/files-meta.ipynb
+-rw-r--r--   0        0        0    20552 2023-11-20 21:49:43.209635 cellxgene_lamin-0.2.2/docs/notebooks/files.ipynb
+-rw-r--r--   0        0        0    36950 2023-11-16 15:44:17.995317 cellxgene_lamin-0.2.2/docs/notebooks/meta-human.ipynb
+-rw-r--r--   0        0        0  1299626 2023-11-16 15:44:17.997804 cellxgene_lamin-0.2.2/docs/notebooks/meta-mouse.ipynb
+-rw-r--r--   0        0        0     8775 2024-03-15 08:45:18.041258 cellxgene_lamin-0.2.2/docs/query-census.ipynb
+-rw-r--r--   0        0        0      176 2023-11-23 20:23:34.120310 cellxgene_lamin-0.2.2/lamin-project.yaml
+-rw-r--r--   0        0        0     1987 2024-04-24 11:56:35.004786 cellxgene_lamin-0.2.2/noxfile.py
+-rw-r--r--   0        0        0     3860 2024-04-15 15:55:14.487786 cellxgene_lamin-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      464 2024-03-28 11:40:09.465624 cellxgene_lamin-0.2.2/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1472 1970-01-01 00:00:00.000000 cellxgene_lamin-0.2.2/PKG-INFO
```

### Comparing `cellxgene_lamin-0.2.1/.github/workflows/build.yml` & `cellxgene_lamin-0.2.2/.github/workflows/build.yml`

 * *Files 6% similar despite different names*

```diff
@@ -25,16 +25,14 @@
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
-          cache: "pip"
-          cache-dependency-path: ".github/workflows/build.yml" # See dependencies below
       - name: cache pre-commit
         uses: actions/cache@v3
         with:
           path: ~/.cache/pre-commit
           key: pre-commit-${{ runner.os }}-${{ hashFiles('.pre-commit-config.yaml') }}
       - name: Cache postgres
         id: cache-postgres
@@ -50,35 +48,34 @@
       - name: Cache postgres miss
         if: steps.cache-postgres.outputs.cache-hit != 'true'
         run: docker pull postgres:latest && docker image save postgres:latest --output ~/postgres.tar
       - name: Cache postgres use
         if: steps.cache-postgres.outputs.cache-hit == 'true'
         run: docker image load --input ~/postgres.tar
       - run: |
-          python -m pip install -U pip
           pip install -U laminci
           sudo apt-get -y install graphviz
       - run: nox -s lint
         if: ${{ matrix.python-version == '3.10' && matrix.group == 'validator' }}
       - run: nox -s "install(group='${{ matrix.group }}')"
       - run: nox -s "build(group='${{ matrix.group }}')"
       - uses: voxmedia/github-action-slack-notify-build@v1
         if: ${{ success() && github.event_name == 'repository_dispatch' }}
         env:
           SLACK_BOT_TOKEN: ${{ secrets.SLACK_GITHUB_ACTION }}
         with:
-          channel: lamindb-mirror-github-actions
+          channel: mirror-github-actions-lamindb
           status: SUCCESS
           color: good
       - uses: voxmedia/github-action-slack-notify-build@v1
         if: ${{ failure() && github.event_name == 'repository_dispatch' }}
         env:
           SLACK_BOT_TOKEN: ${{ secrets.SLACK_GITHUB_ACTION }}
         with:
-          channel: lamindb-mirror-github-actions
+          channel: mirror-github-actions-lamindb
           status: FAILURE
           color: danger
       - name: upload docs
         if: ${{ matrix.group == 'census' || matrix.group == 'validator' }}
         uses: actions/upload-artifact@v2
         with:
           name: docs_${{ matrix.group }}
@@ -102,22 +99,17 @@
         with:
           aws-access-key-id: ${{ secrets.AWS_ACCESS_KEY_ID }}
           aws-secret-access-key: ${{ secrets.AWS_SECRET_ACCESS_KEY }}
           aws-region: us-east-1
       - uses: actions/setup-python@v5
         with:
           python-version: "3.10"
-          cache: "pip"
-          cache-dependency-path: ".github/workflows/build.yml"
 
       - name: install Python deps
-        run: |
-          python -m pip install --upgrade pip
-          pip install laminci
-          sudo apt-get -y install graphviz
+        run: pip install laminci
 
       - run: nox -s "install(group='docs')"
       - uses: actions/download-artifact@v2
       - run: nox -s docs
       - uses: nwtgck/actions-netlify@v1.2
         with:
           publish-dir: "_build/html"
```

### Comparing `cellxgene_lamin-0.2.1/.github/workflows/latest-changes.yml` & `cellxgene_lamin-0.2.2/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.1/.gitignore` & `cellxgene_lamin-0.2.2/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -104,7 +104,9 @@
 _build
 docs/cellxgene_census_lamin.*
 lamin_sphinx
 docs/conf.py
 _docs_tmp*
 test-cellxgene-registries/
 test-cellxgene/
+*.lndb
+*.h5ad
```

### Comparing `cellxgene_lamin-0.2.1/.pre-commit-config.yaml` & `cellxgene_lamin-0.2.2/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -45,12 +45,17 @@
       - id: check-case-conflict
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.7.1
     hooks:
       - id: mypy
         args: [--no-strict-optional, --ignore-missing-imports]
         additional_dependencies:
-          ["types-pkg-resources", "types-requests", "types-attrs"]
+          [
+            "types-pkg-resources",
+            "types-requests",
+            "types-attrs",
+            "types-PyYAML",
+          ]
         exclude: |
           (?x)(
               test_notebooks.py
           )
```

### Comparing `cellxgene_lamin-0.2.1/LICENSE` & `cellxgene_lamin-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.1/README.md` & `cellxgene_lamin-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.1/cellxgene_lamin/_annotate.py` & `cellxgene_lamin-0.2.2/cellxgene_lamin/_annotate.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import re
+from importlib import resources
 from pathlib import Path
 from typing import Dict, Optional, Union
 
 import anndata as ad
 import bionty as bt
+import pandas as pd
 from lamin_utils import logger
 from lamindb._annotate import AnnDataAnnotator, validate_categories_in_df
 from lnschema_core.types import FieldAttr
 
 from ._curate import convert_name_to_ontology_id
 from ._fields import CellxGeneFields
+from .schemas._schema_versions import read_schema_versions
 
 
 def _restrict_obs_fields(adata: ad.AnnData, obs_fields: Dict[str, FieldAttr]):
     """Restrict the obs fields so that there's no duplications."""
     obs_fields_unique = {k: v for k, v in obs_fields.items() if k in adata.obs.columns}
     for name, field in obs_fields.items():
         if name.endswith("_ontology_term_id"):
@@ -61,36 +64,45 @@
         categoricals: Dict[str, FieldAttr] = CellxGeneFields.OBS_FIELDS,
         using: str = "laminlabs/cellxgene",
         verbosity: str = "hint",
         **kwargs,
     ):
         add_defaults_to_obs_fields(adata, **kwargs)
         super().__init__(
-            adata=adata,
+            data=adata,
             var_index=var_index,
             categoricals=_restrict_obs_fields(adata, categoricals),
             using=using,
             verbosity=verbosity,
         )
-        self._schema_version = "5.1.0"
-        self._schema_reference = "https://github.com/chanzuckerberg/single-cell-curation/blob/main/schema/5.1.0/schema.md"
-        self._pinned_ontologies: Dict[str, str] = {
-            "cl": "2024-01-04",
-            "efo": "3.62.0",
-            "hancestro": "3.0",
-            "hsapdv": "2020-03-10",
-            "mmusdv": "2020-03-10",
-            "mondo": "2024-01-03",
-            "ncbitaxon": "2023-06-20",
-            "pato": "2023-05-18",
-            "uberon": "2024-01-18",
-        }
+        self._schema_version = "5.0.0"
+        self._schema_reference = "https://github.com/chanzuckerberg/single-cell-curation/blob/main/schema/5.0.0/schema.md"
+        try:
+            import cellxgene_schema
+
+            major_minor_installed = cellxgene_schema.__version__.rsplit(".", 1)[0]
+            major_minor_expected = self._schema_version.rsplit(".", 1)[0]
+
+            if major_minor_installed != major_minor_expected:
+                logger.warn(
+                    f"installed cellxgene-schema version {cellxgene_schema.__version__} does not match expected major and minor version {self._schema_version}"
+                )
+        except ImportError:
+            pass
+
+        with resources.path(
+            "cellxgene_lamin.schemas", "schema_versions.yml"
+        ) as schema_versions_path:
+            self._pinned_ontologies = read_schema_versions(schema_versions_path)[
+                self._schema_version
+            ]
 
     @property
-    def pinned_ontologies(self) -> Dict[str, str]:
+    def pinned_ontologies(self) -> pd.DataFrame:
+        print(f"Currently used schema version: {self._schema_version}")
         return self._pinned_ontologies
 
     def to_cellxgene(
         self, is_primary_data: bool, title: Optional[str] = None
     ) -> ad.AnnData:
         """Converts the AnnData object to the cellxgene-schema input format.
 
@@ -166,16 +178,16 @@
         if self._collection is None:
             if title is None:
                 raise ValueError("please pass a title!")
             else:
                 adata_cxg.uns["title"] = title
         else:
             adata_cxg.uns["title"] = self._collection.name
-        adata_cxg.uns["schema_reference"] = self._schema_reference
-        adata_cxg.uns["schema_version"] = self._schema_version
+        adata_cxg.uns["cxg_lamin_schema_reference"] = self._schema_reference
+        adata_cxg.uns["cxg_lamin_schema_version"] = self._schema_version
 
         embedding_pattern = r"^[a-zA-Z][a-zA-Z0-9_.-]*$"
         exclude_key = "spatial"
         matching_keys = [
             key
             for key in adata_cxg.obsm.keys()
             if re.match(embedding_pattern, key) and key != exclude_key
```

### Comparing `cellxgene_lamin-0.2.1/cellxgene_lamin/_curate.py` & `cellxgene_lamin-0.2.2/cellxgene_lamin/_curate.py`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.1/cellxgene_lamin/_cxg_rest.py` & `cellxgene_lamin-0.2.2/cellxgene_lamin/_cxg_rest.py`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.1/cellxgene_lamin/_features.py` & `cellxgene_lamin-0.2.2/cellxgene_lamin/_features.py`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.1/cellxgene_lamin/_fields.py` & `cellxgene_lamin-0.2.2/cellxgene_lamin/_fields.py`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.1/cellxgene_lamin/_gene.py` & `cellxgene_lamin-0.2.2/cellxgene_lamin/_gene.py`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.1/cellxgene_lamin/_labels.py` & `cellxgene_lamin-0.2.2/cellxgene_lamin/_labels.py`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.1/cellxgene_lamin/_ontology.py` & `cellxgene_lamin-0.2.2/cellxgene_lamin/_ontology.py`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.1/cellxgene_lamin/_organism.py` & `cellxgene_lamin-0.2.2/cellxgene_lamin/_organism.py`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.1/cellxgene_lamin/datasets.py` & `cellxgene_lamin-0.2.2/cellxgene_lamin/datasets.py`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.1/docs/cellxgene-annotate.ipynb` & `cellxgene_lamin-0.2.2/docs/cellxgene-annotate.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998937074829932%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, 'This guide shows how to validate and curate an AnnData "*

 * *            'object using the metadata registries of '*

 * *            '[`laminlabs/cellxgene`](https://lamin.ai/laminlabs/cellxgene), based on the '*

 * *            '[CELLxGENE schema version '*

 * *            "5.1.0](https://github.com/chanzuckerberg/single-cell-curation/blob/main/schema/5.1.0/schema.md).\\n')], "*

 * *            'delete: [2]}}}'}*

```diff
@@ -3,15 +3,15 @@
         {
             "cell_type": "markdown",
             "id": "1d2cd769",
             "metadata": {},
             "source": [
                 "# Annotate an h5ad file based on CELLxGENE schema\n",
                 "\n",
-                "This guide shows how to validate and curate an AnnData object using the metadata registries of [laminlabs/cellxgene](https://lamin.ai/laminlabs/cellxgene), based on the [CELLxGENE schema version 5.1.0](https://github.com/chanzuckerberg/single-cell-curation/blob/main/schema/5.1.0/schema.md).\n",
+                "This guide shows how to validate and curate an AnnData object using the metadata registries of [`laminlabs/cellxgene`](https://lamin.ai/laminlabs/cellxgene), based on the [CELLxGENE schema version 5.1.0](https://github.com/chanzuckerberg/single-cell-curation/blob/main/schema/5.1.0/schema.md).\n",
                 "\n",
                 "The validated object can be subsequently registered as an artifact in your LaminDB instance."
             ]
         },
         {
             "cell_type": "markdown",
             "id": "772175fbe2c41932",
```

### Comparing `cellxgene_lamin-0.2.1/docs/cellxgene.ipynb` & `cellxgene_lamin-0.2.2/docs/cellxgene.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9788898108838585%*

 * *Differences: {"'cells'": "{0: {'source': "*

 * *            "['[![hub](https://img.shields.io/badge/Source%20%26%20report%20on%20LaminHub-mediumseagreen)](https://lamin.ai/laminlabs/cellxgene/transform/5FUyJ6RkVk0Dz8)']}, "*

 * *            "2: {'source': {insert: [(7, '2. If you want to use these in your own LaminDB "*

 * *            "instance, see the [transfer guide](inv:docs#transfer).\\n'), (12, '1. See the [scRNA "*

 * *            'guide](inv:docs#scrna) for how to create a growing versioned queryable scRNA-seq '*

 * *            "datas […]*

```diff
@@ -1,15 +1,15 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "id": "c71502b7",
             "metadata": {},
             "source": [
-                "[![hub](https://img.shields.io/badge/Source%20%26%20report%20on%20LaminHub-mediumseagreen)](https://lamin.ai/laminlabs/cellxgene/record/core/Transform?uid=5FUyJ6RkVk0Dz8)"
+                "[![hub](https://img.shields.io/badge/Source%20%26%20report%20on%20LaminHub-mediumseagreen)](https://lamin.ai/laminlabs/cellxgene/transform/5FUyJ6RkVk0Dz8)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "7f26a335-cf1c-4e69-be3b-0c26b154606a",
             "metadata": {},
             "source": [
@@ -24,22 +24,22 @@
                 "[CZ CELLxGENE](https://cellxgene.cziscience.com/) hosts the globally largest standardized collection of scRNA-seq datasets.\n",
                 "\n",
                 "LaminDB makes it easy to query the CELLxGENE data and integrate it with in-house data of any kind (omics, phenotypes, pdfs, notebooks, ML models, ...).\n",
                 "\n",
                 "You can use the CELLxGENE data in three ways:\n",
                 "\n",
                 "1. In the current guide, you'll see how to query metadata and data based on `AnnData` objects.\n",
-                "2. If you want to use these in your own LaminDB instance, see the [transfer guide](docs:transfer).\n",
+                "2. If you want to use these in your own LaminDB instance, see the [transfer guide](inv:docs#transfer).\n",
                 "3. If you'd like to leverage the TileDB-SOMA API for the data subset of [CELLxGENE Census](https://chanzuckerberg.github.io/cellxgene-census), see the [Census guide](query-census).\n",
                 "\n",
                 "If you are interested in building similar data assets in-house:\n",
                 "\n",
-                "1. See the [scRNA guide](docs:scrna) for how to create a growing versioned queryable scRNA-seq dataset.\n",
+                "1. See the [scRNA guide](inv:docs#scrna) for how to create a growing versioned queryable scRNA-seq dataset.\n",
                 "2. See the [Annotate](./cellxgene-annotate) for validating, curating and registering your own AnnData objects.\n",
-                "3. [Reach out](https://lamin.ai/contact) if you are interested in a full zero-copy clone of `laminlabs/cellxgene` to accelerate building your in-house LaminDB instances.\n"
+                "3. [Reach out](https://lamin.ai/contact) if you are interested in a full zero-copy clone of [`laminlabs/cellxgene`](https://lamin.ai/laminlabs/cellxgene) to accelerate building your in-house LaminDB instances.\n"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "5dde5525",
             "metadata": {},
             "source": [
@@ -92,15 +92,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "c380296b",
             "metadata": {},
             "source": [
-                "You can create look-up objects for any registry in LaminDB, including [basic biological entities](docs:bionty) and things like users or storage locations.\n",
+                "You can create look-up objects for any registry in LaminDB, including [basic biological entities](https://lamin.ai/laminlabs/docs/bionty) and things like users or storage locations.\n",
                 "\n",
                 "Let's use auto-complete to look up cell types:\n",
                 "\n",
                 ":::{dropdown} Show me a screenshot\n",
                 "\n",
                 "<img src=\"https://lamin-site-assets.s3.amazonaws.com/.lamindb/lgRNHNtMxjU0y8nIagt7.png\" width=\"400px\">\n",
                 "\n",
@@ -129,23 +129,18 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "eb81f096",
             "metadata": {},
             "outputs": [],
             "source": [
-                "organisms = bt.Organism.lookup()  # species\n",
-                "genes = bt.Gene.filter(organism=organisms.human).lookup()  # ~60k human genes\n",
-                "features = ln.Feature.lookup()  # non-gene features, like `cell_type`, `assay`, etc.\n",
+                "organisms = bt.Organism.lookup()\n",
                 "experimental_factors = bt.ExperimentalFactor.lookup()  # labels for experimental factors\n",
                 "tissues = bt.Tissue.lookup()  # tissue labels\n",
-                "ulabels = ln.ULabel.lookup()  # universal labels, e.g. dataset collections\n",
-                "suspension_types = (\n",
-                "    ulabels.is_suspension_type.children.all().lookup()\n",
-                ")  # suspension types"
+                "suspension_types = ln.ULabel.filter(name=\"is_suspension_type\").one().children.lookup()  # suspension types"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "e75a5614",
             "metadata": {},
             "source": [
@@ -260,36 +255,46 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "c2384c0e",
             "metadata": {},
             "source": [
-                "Unlike in the [SOMA guide](query-census), here, we'll query sets of `h5ad` files, which correspond to `AnnData` objects.\n",
+                "Unlike in the [SOMA guide](query-census), here, we'll query sets of `.h5ad` files, which correspond to `AnnData` objects.\n",
                 "\n",
-                "To access them, we query the {class}`~lamindb.Collection` record that links the latest LTS set of h5ad files:"
+                "To access them, we query the {class}`~lamindb.Collection` record that links the latest LTS set of `.h5ad` artifacts:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "0884ba0a",
             "metadata": {},
             "outputs": [],
             "source": [
-                "collection = ln.Collection.filter(name=\"cellxgene-census\", version=\"2023-07-25\").one()\n",
+                "collection = ln.Collection.filter(name=\"cellxgene-census\", version=\"2023-12-15\").one()\n",
                 "collection"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "8fa78cce",
             "metadata": {},
             "source": [
-                "You can get all linked files as a dataframe - there are 850 files in `cellxgene-census` version `2023-07-25`."
+                "You can get all linked artifacts as a dataframe - there are >1000 h5ad files in `cellxgene-census` version `2023-12-15`."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "b60003a3",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "collection.artifacts.count()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "bd413016",
             "metadata": {
@@ -303,30 +308,30 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "9ef4133d",
             "metadata": {},
             "source": [
-                "You can query across files by arbitrary metadata combinations, for instance:"
+                "You can query across artifacts by arbitrary metadata combinations, for instance:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "fa6437ee",
             "metadata": {
                 "tags": [
                     "hide-output"
                 ]
             },
             "outputs": [],
             "source": [
                 "query = collection.artifacts.filter(\n",
-                "    organism=organisms.human,\n",
+                "    organisms=organisms.human,\n",
                 "    cell_types__in=[cell_types.dendritic_cell, cell_types.neutrophil],\n",
                 "    tissues=tissues.kidney,\n",
                 "    ulabels=suspension_types.cell,\n",
                 "    experimental_factors=experimental_factors.ln_10x_3_v2,\n",
                 ")\n",
                 "query = query.order_by(\"size\")  # order by size\n",
                 "query.df().head()  # convert to DataFrame"
@@ -341,17 +346,17 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "ba8914bc",
             "metadata": {},
             "source": [
-                "Each file stores an array in form of an annotated data matrix, an `AnnData` object.\n",
+                "Each artifact stores an array in form of an annotated data matrix, an `AnnData` object.\n",
                 "\n",
-                "Let's look at the first array in the file query and show metadata using `.describe()`:"
+                "Let's look at the first array in the artifact query and show metadata using `.describe()`:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "524ed16e",
             "metadata": {
@@ -405,23 +410,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "e3b104c9",
             "metadata": {},
             "source": [
-                "### 1. Cache & load"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "b8974508",
-            "metadata": {},
-            "source": [
-                "Let us first consider option 1:"
+                "Cache & load:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "271f05ea",
             "metadata": {
@@ -436,69 +433,56 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "9290545c",
             "metadata": {},
             "source": [
-                "Now we have an `AnnData` object, which stores observation annotations matching our file-level query in the `.obs` slot, and we can re-use almost the same query on the array-level:\n",
+                "Now we have an `AnnData` object, which stores observation annotations matching our artifact-level query in the `.obs` slot, and we can re-use almost the same query on the array-level.\n",
+                "\n",
+                ":::{dropdown} See the array-level query\n",
+                "\n",
+                "```\n",
+                "adata_slice = adata[\n",
+                "    adata.obs.cell_type.isin(\n",
+                "        [cell_types.dendritic_cell.name, cell_types.neutrophil.name]\n",
+                "    )\n",
+                "    & (adata.obs.tissue == tissues.kidney.name)\n",
+                "    & (adata.obs.suspension_type == suspension_types.cell.name)\n",
+                "    & (adata.obs.assay == experimental_factors.ln_10x_3_v2.name)\n",
+                "]\n",
+                "adata_slice\n",
+                "```\n",
+                "\n",
+                ":::\n",
+                "\n",
                 "\n",
-                ":::{dropdown} See the file-level query for comparison\n",
+                ":::{dropdown} See the artifact-level query for comparison\n",
                 "\n",
                 "```\n",
-                "query = collection.files.filter(\n",
+                "query = collection.artifacts.filter(\n",
                 "    organism=organisms.human,\n",
                 "    cell_types__in=[cell_types.dendritic_cell, cell_types.neutrophil],\n",
                 "    tissues=tissues.kidney,\n",
                 "    ulabels=suspension_types.cell,\n",
                 "    experimental_factors=experimental_factors.ln_10x_3_v2,\n",
                 ")\n",
                 "```\n",
                 "\n",
                 "`AnnData` uses pandas to manage metadata and the syntax differs slightly. However, the same metadata records are used.\n",
                 "\n",
                 ":::"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "1a1e25c5",
-            "metadata": {
-                "tags": [
-                    "hide-output"
-                ]
-            },
-            "outputs": [],
-            "source": [
-                "adata_slice = adata[\n",
-                "    adata.obs.cell_type.isin(\n",
-                "        [cell_types.dendritic_cell.name, cell_types.neutrophil.name]\n",
-                "    )\n",
-                "    & (adata.obs.tissue == tissues.kidney.name)\n",
-                "    & (adata.obs.suspension_type == suspension_types.cell.name)\n",
-                "    & (adata.obs.assay == experimental_factors.ln_10x_3_v2.name)\n",
-                "]\n",
-                "adata_slice"
-            ]
-        },
-        {
             "cell_type": "markdown",
             "id": "618aea87",
             "metadata": {},
             "source": [
-                "### 2. Stream"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "ff667e7c",
-            "metadata": {},
-            "source": [
-                "Let us now consider option 2:"
+                "Stream:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "963f51c0",
             "metadata": {
@@ -513,74 +497,29 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "53cb9209",
             "metadata": {},
             "source": [
-                "We now have an `AnnDataAccessor` object, which behaves much like an `AnnData`, and the query looks the same:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "34dd9231",
-            "metadata": {
-                "tags": [
-                    "hide-output"
-                ]
-            },
-            "outputs": [],
-            "source": [
+                "We now have an `AnnDataAccessor` object, which behaves much like an `AnnData`, and the query looks the same.\n",
+                "\n",
+                ":::{dropdown} See the query\n",
+                "\n",
+                "```\n",
                 "adata_backed_slice = adata_backed[\n",
                 "    adata_backed.obs.cell_type.isin(\n",
                 "        [cell_types.dendritic_cell.name, cell_types.neutrophil.name]\n",
                 "    )\n",
                 "    & (adata_backed.obs.tissue == tissues.kidney.name)\n",
                 "    & (adata_backed.obs.suspension_type == suspension_types.cell.name)\n",
                 "    & (adata_backed.obs.assay == experimental_factors.ln_10x_3_v2.name)\n",
                 "]\n",
                 "\n",
-                "adata_backed_slice.to_memory()"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "dc7efac3",
-            "metadata": {},
-            "source": [
-                "### 3. Concatenate slices "
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "69c8ade3",
-            "metadata": {},
-            "source": [
-                "If we want to concatenate these individual file-level slices, loop over all files in `query` and concatenate the results.\n",
-                "\n",
-                ":::{dropdown} How would this look like?\n",
-                "\n",
-                "```\n",
-                "adata_slices = []\n",
-                "for file in query:\n",
-                "    adata_backed = artifact.backed()\n",
-                "    adata_slice = adata_backed[\n",
-                "        adata_backed.obs.cell_type.isin(\n",
-                "            [cell_types.dendritic_cell.name, cell_types.neutrophil.name]\n",
-                "        )\n",
-                "        & (adata_backed.obs.tissue == tissues.kidney.name)\n",
-                "        & (adata_backed.obs.suspension_type == suspension_types.cell.name)\n",
-                "        & (adata_backed.obs.assay == experimental_factors.ln_10x_3_v2.name)\n",
-                "    ]\n",
-                "    adata_slices.append(adata_slice.to_memory())\n",
-                "\n",
-                "import anndata as ad\n",
-                "\n",
-                "adata_query = ad.concat(adata_slices)\n",
+                "adata_backed_slice.to_memory()\n",
                 "```\n",
                 "\n",
                 ":::"
             ]
         },
         {
             "cell_type": "markdown",
@@ -591,14 +530,16 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "73b06fe6",
             "metadata": {},
             "source": [
+                "You can directly train an ML models on the entire collection.\n",
+                "\n",
                 "See {doc}`docs:scrna5`."
             ]
         },
         {
             "cell_type": "markdown",
             "id": "0d40b93e",
             "metadata": {},
@@ -609,35 +550,35 @@
         {
             "cell_type": "markdown",
             "id": "8299ecdc",
             "metadata": {},
             "source": [
                 "Alternatively, \n",
                 "\n",
-                "- [you can search a file on the LaminHub UI](https://lamin.ai/laminlabs/cellxgene/records/core/Artifact?offset=0&limit=50) and fetch it through: \n",
-                "`ln.Artifact.filter(uid=\"...\").one()`\n",
+                "- [you can search a file on the LaminHub UI](https://lamin.ai/laminlabs/cellxgene/artifacts) and fetch it through: \n",
+                "`ln.Artifact.get(uid)`\n",
                 "- or query for a collection you found on [CZ CELLxGENE Discover](https://cellxgene.cziscience.com/collections)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "8b537df8",
             "metadata": {},
             "source": [
-                "Let's search the collections from CELLxGENE:"
+                "Let's search the collections from CELLxGENE within the 2023-12-15 release:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "3710084a",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.Collection.search(\"immune human kidney\", limit=10)"
+                "ln.Collection.filter(version=\"2023-12-15\").search(\"immune human kidney\", limit=10)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "0a707588",
             "metadata": {},
             "source": [
@@ -647,29 +588,47 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "c49c302d",
             "metadata": {},
             "outputs": [],
             "source": [
-                "collection = ln.Collection.filter(uid=\"kqiPjpzpK9H9rdtnHWas\").one()\n",
+                "collection = ln.Collection.filter(uid=\"kqiPjpzpK9H9rdtnV67f\").one()\n",
                 "\n",
                 "collection"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "5a36be6f",
             "metadata": {},
             "source": [
                 "We see it's a Science paper and we could find more information using the [DOI](https://doi.org/10.1126/science.aat5031) or CELLxGENE [collection id](https://cellxgene.cziscience.com/collections/120e86b4-1195-48c5-845b-b98054105eec)."
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "11bce898",
+            "metadata": {},
+            "source": [
+                "Check different versions of this collection:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "f97538e2",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "collection.versions.df()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "id": "19f32e23",
             "metadata": {},
             "source": [
                 "Each collection has at least one {class}`~lamindb.Artifact` file associated to it. Let's get the associated artifacts:"
             ]
         },
         {
```

### Comparing `cellxgene_lamin-0.2.1/docs/changelog.md` & `cellxgene_lamin-0.2.2/docs/changelog.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+♻️ Fixes for lamindb 0.72 | [54](https://github.com/laminlabs/cellxgene-lamin/pull/54) | [falexwolf](https://github.com/falexwolf) | 2024-05-19 | 0.2.2
+👷 Use uv | [53](https://github.com/laminlabs/cellxgene-lamin/pull/53) | [sunnyosun](https://github.com/sunnyosun) | 2024-04-24 |
+💚 Fix data arg | [52](https://github.com/laminlabs/cellxgene-lamin/pull/52) | [sunnyosun](https://github.com/sunnyosun) | 2024-04-24 |
+♻️ Simplify guide | [51](https://github.com/laminlabs/cellxgene-lamin/pull/51) | [falexwolf](https://github.com/falexwolf) | 2024-04-19 |
+:sparkles: Pinned ontologies schema | [50](https://github.com/laminlabs/cellxgene-lamin/pull/50) | [Zethson](https://github.com/Zethson) | 2024-04-16 |
+:sparkles: Compare installed and expected cellxgene-schema versions | [49](https://github.com/laminlabs/cellxgene-lamin/pull/49) | [Zethson](https://github.com/Zethson) | 2024-04-15 |
 :sparkles: Pin lamindb 0.69.5 | [47](https://github.com/laminlabs/cellxgene-lamin/pull/47) | [Zethson](https://github.com/Zethson) | 2024-04-02 |
 ⬆️ Update Annotate | [46](https://github.com/laminlabs/cellxgene-lamin/pull/46) | [sunnyosun](https://github.com/sunnyosun) | 2024-03-31 |
 :art: Run census & annotate in parallel | [45](https://github.com/laminlabs/cellxgene-lamin/pull/45) | [Zethson](https://github.com/Zethson) | 2024-03-30 |
 ⬆️ Pin lamindb to 0.69.3 | [42](https://github.com/laminlabs/cellxgene-lamin/pull/42) | [Zethson](https://github.com/Zethson) | 2024-03-28 | 0.2.0
 🚚 Rename Validate to Annotate | [43](https://github.com/laminlabs/cellxgene-lamin/pull/43) | [sunnyosun](https://github.com/sunnyosun) | 2024-03-28 |
 Fix census notebook execution not being shown | [41](https://github.com/laminlabs/cellxgene-lamin/pull/41) | [Zethson](https://github.com/Zethson) | 2024-03-27 |
 Fix notebook execution rendering | [39](https://github.com/laminlabs/cellxgene-lamin/pull/39) | [Zethson](https://github.com/Zethson) | 2024-03-27 |
```

### Comparing `cellxgene_lamin-0.2.1/docs/notebooks.md` & `cellxgene_lamin-0.2.2/docs/notebooks.md`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.1/docs/notebooks/cencus-release-2023-12-15-LTS.ipynb` & `cellxgene_lamin-0.2.2/docs/notebooks/cencus-release-2023-12-15-LTS.ipynb`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.1/docs/notebooks/census-release-2023-07-25.ipynb` & `cellxgene_lamin-0.2.2/docs/notebooks/census-release-2023-07-25.ipynb`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.1/docs/notebooks/census-release-2023-11-13.ipynb` & `cellxgene_lamin-0.2.2/docs/notebooks/census-release-2023-11-13.ipynb`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.1/docs/notebooks/census-release-2023-12-06.ipynb` & `cellxgene_lamin-0.2.2/docs/notebooks/census-release-2023-12-06.ipynb`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.1/docs/notebooks/files-meta.ipynb` & `cellxgene_lamin-0.2.2/docs/notebooks/files-meta.ipynb`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.1/docs/notebooks/files.ipynb` & `cellxgene_lamin-0.2.2/docs/notebooks/files.ipynb`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.1/docs/notebooks/meta-human.ipynb` & `cellxgene_lamin-0.2.2/docs/notebooks/meta-human.ipynb`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.1/docs/notebooks/meta-mouse.ipynb` & `cellxgene_lamin-0.2.2/docs/notebooks/meta-mouse.ipynb`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.1/docs/query-census.ipynb` & `cellxgene_lamin-0.2.2/docs/query-census.ipynb`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.1/noxfile.py` & `cellxgene_lamin-0.2.2/noxfile.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,23 +23,25 @@
     "group",
     ["census", "validator", "docs"],
 )
 def install(session: nox.Session, group: str) -> None:
     extra = ""
     if group == "census":
         extra = ",jupyter,aws"
-        session.run(*"pip install cellxgene-census".split())
+        session.run(*"uv pip install --system cellxgene-census".split())
     elif group == "validator":
         extra = ",jupyter,aws,zarr"
-        session.run(*"pip install cellxgene-schema".split())
-        session.run(*"pip install anndata==0.9.0".split())
-    session.run(*"pip install .[dev]".split())
+        session.run(*"uv pip install --system cellxgene-schema==5.0.2".split())
+        session.run(*"uv pip install --system anndata==0.9.0".split())
+    session.run(*"uv pip install --system .[dev]".split())
     session.run(
+        "uv",
         "pip",
         "install",
+        "--system",
         f"lamindb[bionty{extra}] @ git+https://github.com/laminlabs/lamindb@release",
     )
 
 
 @nox.session
 @nox.parametrize(
     "group",
@@ -60,11 +62,10 @@
 @nox.session
 def docs(session):
     # Recover executed notebooks
     for group in ["census", "validator"]:
         for path in Path(f"./docs_{group}").glob("*"):
             path.rename(f"./docs/{path.name}")
 
-    login_testuser1(session)
     session.run(*"lamin init --storage ./docsbuild --schema bionty".split())
     build_docs(session, strict=False)
     upload_docs_artifact(aws=True)
```

### Comparing `cellxgene_lamin-0.2.1/pyproject.toml` & `cellxgene_lamin-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cellxgene_lamin-0.2.1/PKG-INFO` & `cellxgene_lamin-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellxgene_lamin
-Version: 0.2.1
+Version: 0.2.2
 Summary: Manage cellxgene metadata using LaminDB.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

