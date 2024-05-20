# Comparing `tmp/digitalhub_ml-0.4.0b8.tar.gz` & `tmp/digitalhub_ml-0.5.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalhub_ml-0.4.0b8.tar", last modified: Tue May 14 11:02:36 2024, max compression
+gzip compressed data, was "digitalhub_ml-0.5.0b0.tar", last modified: Mon May 20 12:49:20 2024, max compression
```

## Comparing `digitalhub_ml-0.4.0b8.tar` & `digitalhub_ml-0.5.0b0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 11:02:36.945569 digitalhub_ml-0.4.0b8/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)      938 2024-05-14 11:02:36.945569 digitalhub_ml-0.4.0b8/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      462 2024-04-23 09:36:04.000000 digitalhub_ml-0.4.0b8/README.md
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 11:02:36.941569 digitalhub_ml-0.4.0b8/digitalhub_ml/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      304 2024-05-14 10:46:36.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 11:02:36.941569 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:38:37.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      436 2024-05-06 11:22:14.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/entity_types.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 11:02:36.945569 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/models/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:40:22.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/models/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6328 2024-05-14 10:46:36.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/models/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     7285 2024-05-14 10:46:36.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/models/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      318 2024-04-23 09:36:04.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/models/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      557 2024-05-06 10:38:24.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/models/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      209 2024-02-15 10:15:41.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/models/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 11:02:36.945569 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/projects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:33:48.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/projects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6049 2024-05-14 10:46:36.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/projects/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5869 2024-05-14 10:46:36.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/projects/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      988 2024-05-14 10:46:36.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/projects/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      730 2024-05-06 11:19:46.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/registries.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 11:02:36.945569 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/runs/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-23 14:34:03.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/runs/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-03-07 13:39:55.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/runs/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      405 2024-05-14 10:46:36.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/runs/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      313 2024-03-14 13:46:16.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/runs/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 11:02:36.945569 digitalhub_ml-0.4.0b8/digitalhub_ml.egg-info/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)      938 2024-05-14 11:02:36.000000 digitalhub_ml-0.4.0b8/digitalhub_ml.egg-info/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      903 2024-05-14 11:02:36.000000 digitalhub_ml-0.4.0b8/digitalhub_ml.egg-info/SOURCES.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-05-14 11:02:36.000000 digitalhub_ml-0.4.0b8/digitalhub_ml.egg-info/dependency_links.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-05-14 11:02:36.000000 digitalhub_ml-0.4.0b8/digitalhub_ml.egg-info/requires.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       19 2024-05-14 11:02:36.000000 digitalhub_ml-0.4.0b8/digitalhub_ml.egg-info/top_level.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1054 2024-05-13 12:41:00.000000 digitalhub_ml-0.4.0b8/pyproject.toml
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-05-14 11:02:36.945569 digitalhub_ml-0.4.0b8/setup.cfg
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:49:20.762657 digitalhub_ml-0.5.0b0/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)      938 2024-05-20 12:49:20.762657 digitalhub_ml-0.5.0b0/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      462 2024-04-23 09:36:04.000000 digitalhub_ml-0.5.0b0/README.md
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:49:20.758657 digitalhub_ml-0.5.0b0/digitalhub_ml/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      304 2024-05-20 09:51:09.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:49:20.758657 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:38:37.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      436 2024-05-06 11:22:14.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/entity_types.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:49:20.758657 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/models/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:40:22.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/models/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6328 2024-05-20 09:51:09.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/models/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    12517 2024-05-20 09:55:25.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/models/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      318 2024-04-23 09:36:04.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/models/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      996 2024-05-20 07:16:51.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/models/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      209 2024-02-15 10:15:41.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/models/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:49:20.762657 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/projects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:33:48.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/projects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6049 2024-05-20 09:51:09.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/projects/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5869 2024-05-20 09:51:09.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/projects/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      988 2024-05-20 09:51:09.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/projects/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      730 2024-05-06 11:19:46.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/registries.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:49:20.762657 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/runs/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-23 14:34:03.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/runs/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-03-07 13:39:55.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/runs/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      405 2024-05-20 09:51:09.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/runs/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      313 2024-03-14 13:46:16.000000 digitalhub_ml-0.5.0b0/digitalhub_ml/entities/runs/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:49:20.762657 digitalhub_ml-0.5.0b0/digitalhub_ml.egg-info/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)      938 2024-05-20 12:49:20.000000 digitalhub_ml-0.5.0b0/digitalhub_ml.egg-info/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      903 2024-05-20 12:49:20.000000 digitalhub_ml-0.5.0b0/digitalhub_ml.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-05-20 12:49:20.000000 digitalhub_ml-0.5.0b0/digitalhub_ml.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-05-20 12:49:20.000000 digitalhub_ml-0.5.0b0/digitalhub_ml.egg-info/requires.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       19 2024-05-20 12:49:20.000000 digitalhub_ml-0.5.0b0/digitalhub_ml.egg-info/top_level.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1054 2024-05-20 07:16:51.000000 digitalhub_ml-0.5.0b0/pyproject.toml
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-05-20 12:49:20.762657 digitalhub_ml-0.5.0b0/setup.cfg
```

### Comparing `digitalhub_ml-0.4.0b8/PKG-INFO` & `digitalhub_ml-0.5.0b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: digitalhub-ml
-Version: 0.4.0b8
+Version: 0.5.0b0
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 Keywords: data,dataops,kubernetes
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: digitalhub-data~=0.3
+Requires-Dist: digitalhub-data~=0.5
 
 # Digitalhub-ml Library
 
 The Digitalhub-ml SDK library is used to manage entities and executions in Digitalhub from Python.
 The Digitalhub-ml layer is the third layer of the Digitalhub ml platform, focused on machine learning functions.
 It contains the ml entities and objects (Models) and the methods to manage them.
```

### Comparing `digitalhub_ml-0.4.0b8/digitalhub_ml/entities/models/crud.py` & `digitalhub_ml-0.5.0b0/digitalhub_ml/entities/models/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.4.0b8/digitalhub_ml/entities/models/entity.py` & `digitalhub_ml-0.5.0b0/digitalhub_ml/entities/projects/entity.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,278 +1,235 @@
-"""
-Model module.
-"""
 from __future__ import annotations
 
 import typing
-from pathlib import Path
 
-from digitalhub_core.context.builder import get_context
-from digitalhub_core.entities._base.entity import Entity
 from digitalhub_core.entities._builders.metadata import build_metadata
 from digitalhub_core.entities._builders.spec import build_spec
 from digitalhub_core.entities._builders.status import build_status
-from digitalhub_core.utils.api import api_ctx_create, api_ctx_read, api_ctx_update
-from digitalhub_core.utils.generic_utils import build_uuid, get_timestamp
-from digitalhub_core.utils.io_utils import write_yaml
+from digitalhub_core.utils.generic_utils import build_uuid
+from digitalhub_data.entities.projects.entity import CTX_ENTITIES, FUNC_MAP, ProjectData
 from digitalhub_ml.entities.entity_types import EntityTypes
+from digitalhub_ml.entities.models.crud import create_model_from_dict, delete_model, get_model, list_models, new_model
 
 if typing.TYPE_CHECKING:
-    from digitalhub_core.context.context import Context
-    from digitalhub_ml.entities.models.metadata import ModelMetadata
-    from digitalhub_ml.entities.models.spec import ModelSpec
-    from digitalhub_ml.entities.models.status import ModelStatus
+    from digitalhub_ml.entities.models.entity import Model
 
+MODELS = EntityTypes.MODELS.value
+CTX_ENTITIES.append(MODELS)
+FUNC_MAP[MODELS] = create_model_from_dict
 
-class Model(Entity):
+
+class ProjectMl(ProjectData):
     """
-    A class representing a model.
+    ProjectMl class.
     """
 
-    ENTITY_TYPE = EntityTypes.MODELS.value
+    #############################
+    #  Models
+    #############################
 
-    def __init__(
-        self,
-        project: str,
-        name: str,
-        uuid: str,
-        kind: str,
-        metadata: ModelMetadata,
-        spec: ModelSpec,
-        status: ModelStatus,
-        user: str | None = None,
-    ) -> None:
+    def new_model(self, **kwargs) -> Model:
         """
-        Constructor.
+        Create a Model.
 
         Parameters
         ----------
-        project : str
-            Project name.
-        name : str
-            Name of the object.
-        uuid : str
-            Version of the object.
-        kind : str
-            Kind of the object.
-        metadata : ModelMetadata
-            Metadata of the object.
-        spec : ModelSpec
-            Specification of the object.
-        status : ModelStatus
-            Status of the object.
-        user : str
-            Owner of the object.
-        """
-        super().__init__()
-        self.project = project
-        self.name = name
-        self.id = uuid
-        self.kind = kind
-        self.key = f"store://{project}/{self.ENTITY_TYPE}/{kind}/{name}:{uuid}"
-        self.metadata = metadata
-        self.spec = spec
-        self.status = status
-        self.user = user
-
-        # Add attributes to be used in the to_dict method
-        self._obj_attr.extend(["project", "name", "id", "key"])
+        **kwargs
+            Keyword arguments.
 
-    #############################
-    #  Save / Refresh / Export
-    #############################
+        Returns
+        -------
+        Model
+           Object instance.
+        """
+        kwargs["project"] = self.name
+        kwargs["kind"] = "model"
+        obj = new_model(**kwargs)
+        self._add_object(obj, MODELS)
+        return obj
 
-    def save(self, update: bool = False) -> Model:
+    def get_model(self, entity_name: str | None = None, entity_id: str | None = None, **kwargs) -> Model:
         """
-        Save entity into backend.
+        Get object from backend.
 
         Parameters
         ----------
-        update : bool
-            Flag to indicate update.
+        entity_name : str
+            Entity name.
+        entity_id : str
+            Entity ID.
+        **kwargs : dict
+            Parameters to pass to the API call.
 
         Returns
         -------
         Model
-            Entity saved.
+            Instance of Model class.
         """
-        obj = self.to_dict()
-
-        if not update:
-            api = api_ctx_create(self.project, self.ENTITY_TYPE)
-            new_obj = self._context().create_object(api, obj)
-            self._update_attributes(new_obj)
-            return self
-
-        self.metadata.updated = obj["metadata"]["updated"] = get_timestamp()
-        api = api_ctx_update(self.project, self.ENTITY_TYPE, self.id)
-        new_obj = self._context().update_object(api, obj)
-        self._update_attributes(new_obj)
-        return self
+        obj = get_model(self.name, entity_name=entity_name, entity_id=entity_id, **kwargs)
+        self._add_object(obj, MODELS)
+        return obj
 
-    def refresh(self) -> Model:
+    def delete_model(self, entity_name: str | None = None, entity_id: str | None = None, **kwargs) -> None:
         """
-        Refresh object from backend.
+        Delete a Model from project.
+
+        Parameters
+        ----------
+        entity_name : str
+            Entity name.
+        entity_id : str
+            Entity ID.
+        **kwargs : dict
+            Parameters to pass to the API call.
 
         Returns
         -------
-        Model
-            Entity refreshed.
+        None
         """
-        api = api_ctx_read(self.project, self.ENTITY_TYPE, self.id)
-        obj = self._context().read_object(api)
-        self._update_attributes(obj)
-        return self
+        delete_model(self.name, entity_name=entity_name, entity_id=entity_id, **kwargs)
+        self._delete_object(MODELS, entity_name, entity_id)
 
-    def export(self, filename: str | None = None) -> None:
+    def set_model(self, model: Model) -> None:
         """
-        Export object as a YAML file.
+        Set a Model.
 
         Parameters
         ----------
-        filename : str
-            Name of the export YAML file. If not specified, the default value is used.
+        model : Model
+            Model to set.
 
         Returns
         -------
         None
         """
-        obj = self.to_dict()
-        if filename is None:
-            filename = f"{self.kind}_{self.name}_{self.id}.yml"
-        pth = Path(self._context().project_dir) / filename
-        pth.parent.mkdir(parents=True, exist_ok=True)
-        write_yaml(pth, obj)
-
-    #############################
-    #  Context
-    #############################
+        self._add_object(model, MODELS)
 
-    def _context(self) -> Context:
+    def list_models(self, **kwargs) -> list[dict]:
         """
-        Get context.
+        List models associated with the project.
+
+        Parameters
+        ----------
+        **kwargs : dict
+            Filters to apply to the list. Shold be params={"filter": "value"}.
 
         Returns
         -------
-        Context
-            Context.
+        list[dict]
+            List of objects related to project.
         """
-        return get_context(self.project)
-
-    #############################
-    #  Static interface methods
-    #############################
+        return list_models(self.name, **kwargs)
 
     @staticmethod
     def _parse_dict(obj: dict, validate: bool = True) -> dict:
         """
         Get dictionary and parse it to a valid entity dictionary.
 
         Parameters
         ----------
+        entity : str
+            Entity type.
         obj : dict
             Dictionary to parse.
 
         Returns
         -------
         dict
             A dictionary containing the attributes of the entity instance.
         """
-        project = obj.get("project")
-        name = obj.get("name")
+        # Override methods to search in digitalhub_ml
+        name = build_uuid(obj.get("name"))
         kind = obj.get("kind")
-        uuid = build_uuid(obj.get("id"))
         metadata = build_metadata(kind, **obj.get("metadata", {}))
         spec = build_spec(kind, validate=validate, **obj.get("spec", {}))
         status = build_status(kind, **obj.get("status", {}))
         user = obj.get("user")
+        local = obj.get("local", False)
         return {
-            "project": project,
             "name": name,
-            "uuid": uuid,
             "kind": kind,
             "metadata": metadata,
             "spec": spec,
             "status": status,
             "user": user,
+            "local": local,
         }
 
 
-def model_from_parameters(
-    project: str,
+def project_from_parameters(
     name: str,
     kind: str,
-    uuid: str | None = None,
     description: str | None = None,
     source: str | None = None,
     labels: list[str] | None = None,
-    embedded: bool = True,
+    local: bool = False,
+    context: str | None = None,
     **kwargs,
-) -> Model:
+) -> ProjectData:
     """
-    Create a new Model instance with the specified parameters.
+    Create project.
 
     Parameters
     ----------
-    project : str
-        A string representing the project associated with this model.
     name : str
-        The name of the model.
+        Name that identifies the object.
     kind : str
         Kind of the object.
-    uuid : str
-        ID of the object in form of UUID.
+    description : str
+        Description of the object.
     source : str
         Remote git source for object.
     labels : list[str]
         List of labels.
-    description : str
-        A description of the model.
-    embedded : bool
-        Flag to determine if object must be embedded in project.
+    local : bool
+        Flag to determine if object will be exported to backend.
+    context : str
+        The context of the project.
     **kwargs
         Spec keyword arguments.
 
     Returns
     -------
-    Model
-        An instance of the created model.
+    ProjectData
+        ProjectData object.
     """
-    uuid = build_uuid(uuid)
+    name = build_uuid(name)
+    spec = build_spec(
+        kind,
+        context=context,
+        **kwargs,
+    )
     metadata = build_metadata(
         kind,
-        project=project,
+        project=name,
         name=name,
-        version=uuid,
         description=description,
-        source=source,
         labels=labels,
-        embedded=embedded,
+        source=source,
     )
-    spec = build_spec(kind, **kwargs)
     status = build_status(kind)
-    return Model(
-        project=project,
+    return ProjectData(
         name=name,
-        uuid=uuid,
         kind=kind,
         metadata=metadata,
         spec=spec,
         status=status,
+        local=local,
     )
 
 
-def model_from_dict(obj: dict) -> Model:
+def project_from_dict(obj: dict) -> ProjectData:
     """
-    Create Model instance from a dictionary.
+    Create project from dictionary.
 
     Parameters
     ----------
     obj : dict
         Dictionary to create object from.
 
     Returns
     -------
-    Model
-        Model instance.
+    ProjectData
+        ProjectData object.
     """
-    return Model.from_dict(obj, validate=False)
+    return ProjectData.from_dict(obj, validate=False)
```

### Comparing `digitalhub_ml-0.4.0b8/digitalhub_ml/entities/projects/crud.py` & `digitalhub_ml-0.5.0b0/digitalhub_ml/entities/projects/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.4.0b8/digitalhub_ml/entities/projects/spec.py` & `digitalhub_ml-0.5.0b0/digitalhub_ml/entities/projects/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.4.0b8/digitalhub_ml/entities/registries.py` & `digitalhub_ml-0.5.0b0/digitalhub_ml/entities/registries.py`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.4.0b8/digitalhub_ml.egg-info/PKG-INFO` & `digitalhub_ml-0.5.0b0/digitalhub_ml.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: digitalhub-ml
-Version: 0.4.0b8
+Version: 0.5.0b0
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 Keywords: data,dataops,kubernetes
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: digitalhub-data~=0.3
+Requires-Dist: digitalhub-data~=0.5
 
 # Digitalhub-ml Library
 
 The Digitalhub-ml SDK library is used to manage entities and executions in Digitalhub from Python.
 The Digitalhub-ml layer is the third layer of the Digitalhub ml platform, focused on machine learning functions.
 It contains the ml entities and objects (Models) and the methods to manage them.
```

### Comparing `digitalhub_ml-0.4.0b8/digitalhub_ml.egg-info/SOURCES.txt` & `digitalhub_ml-0.5.0b0/digitalhub_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.4.0b8/pyproject.toml` & `digitalhub_ml-0.5.0b0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digitalhub-ml"
-version = "0.4.0b8"
+version = "0.5.0b0"
 description = "Python SDK for DHCore"
 readme = "README.md"
 authors = [
     { name = "Fondazione Bruno Kessler", email = "dslab@fbk.eu" },
     { name = "Matteo Martini", email = "mmartini@fbk.eu" }
 ]
 license = { file = "LICENSE.txt" }
@@ -16,22 +16,22 @@
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10"
 ]
 keywords = ["data", "dataops", "kubernetes"]
 requires-python = ">=3.9"
 dependencies = [
-    "digitalhub-data~=0.3",
+    "digitalhub-data~=0.5",
 ]
 
 [tool.setuptools.packages.find]
 exclude = ["modules*"]
 
 [tool.bumpver]
-current_version = "0.4.0b8"
+current_version = "0.5.0b0"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = false
 tag             = false
 push            = false
 
 [tool.bumpver.file_patterns]
```

