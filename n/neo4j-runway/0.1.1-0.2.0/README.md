# Comparing `tmp/neo4j_runway-0.1.1.tar.gz` & `tmp/neo4j_runway-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neo4j_runway-0.1.1.tar", max compression
+gzip compressed data, was "neo4j_runway-0.2.0.tar", max compression
```

## Comparing `neo4j_runway-0.1.1.tar` & `neo4j_runway-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11354 2024-05-01 12:35:47.639470 neo4j_runway-0.1.1/LICENSE
--rw-r--r--   0        0        0     4725 2024-05-01 18:05:02.618828 neo4j_runway-0.1.1/README.md
--rw-r--r--   0        0        0      205 2024-05-01 12:25:23.214243 neo4j_runway-0.1.1/neo4j_runway/__init__.py
--rw-r--r--   0        0        0       33 2024-04-29 23:04:42.985466 neo4j_runway-0.1.1/neo4j_runway/discovery/__init__.py
--rw-r--r--   0        0        0     3211 2024-05-02 13:25:34.948014 neo4j_runway-0.1.1/neo4j_runway/discovery/discovery.py
--rw-r--r--   0        0        0       79 2024-04-29 23:04:42.986387 neo4j_runway-0.1.1/neo4j_runway/ingestion/__init__.py
--rw-r--r--   0        0        0    11693 2024-05-09 14:23:16.900284 neo4j_runway-0.1.1/neo4j_runway/ingestion/generate_ingest.py
--rwxr-xr-x   0        0        0     3503 2024-05-01 12:25:23.215248 neo4j_runway-0.1.1/neo4j_runway/ingestion/pyingest.py
--rw-r--r--   0        0        0       21 2024-04-29 23:04:42.987658 neo4j_runway-0.1.1/neo4j_runway/llm/__init__.py
--rw-r--r--   0        0        0     4543 2024-05-01 12:25:23.215746 neo4j_runway-0.1.1/neo4j_runway/llm/llm.py
--rw-r--r--   0        0        0       38 2024-04-29 23:04:42.988650 neo4j_runway-0.1.1/neo4j_runway/modeler/__init__.py
--rw-r--r--   0        0        0     7948 2024-05-02 13:25:34.960509 neo4j_runway-0.1.1/neo4j_runway/modeler/modeler.py
--rw-r--r--   0        0        0      229 2024-05-02 11:43:53.434393 neo4j_runway-0.1.1/neo4j_runway/objects/__init__.py
--rw-r--r--   0        0        0     5681 2024-05-09 15:42:41.632781 neo4j_runway-0.1.1/neo4j_runway/objects/arrows.py
--rw-r--r--   0        0        0    11004 2024-05-09 15:42:40.024287 neo4j_runway-0.1.1/neo4j_runway/objects/data_model.py
--rw-r--r--   0        0        0     3320 2024-05-09 16:05:18.875638 neo4j_runway-0.1.1/neo4j_runway/objects/node.py
--rw-r--r--   0        0        0     2851 2024-05-09 16:05:18.876065 neo4j_runway-0.1.1/neo4j_runway/objects/property.py
--rw-r--r--   0        0        0     3587 2024-05-09 16:05:18.876546 neo4j_runway-0.1.1/neo4j_runway/objects/relationship.py
--rw-r--r--   0        0        0      904 2024-05-02 11:43:53.436909 neo4j_runway-0.1.1/neo4j_runway/objects/user_input.py
--rw-r--r--   0        0        0     2205 2024-04-29 23:04:42.992114 neo4j_runway-0.1.1/neo4j_runway/resources/prompts/prompts.py
--rw-r--r--   0        0        0      138 2024-04-29 23:04:43.003742 neo4j_runway-0.1.1/neo4j_runway/utils/__init__.py
--rw-r--r--   0        0        0     3429 2024-04-29 23:04:43.003938 neo4j_runway-0.1.1/neo4j_runway/utils/naming_conventions.py
--rw-r--r--   0        0        0      917 2024-05-01 12:25:23.223161 neo4j_runway-0.1.1/neo4j_runway/utils/test_connection.py
--rw-r--r--   0        0        0     1116 2024-05-09 16:05:34.918238 neo4j_runway-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6015 1970-01-01 00:00:00.000000 neo4j_runway-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11354 2024-05-01 12:35:47.639470 neo4j_runway-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4713 2024-05-15 19:25:39.876076 neo4j_runway-0.2.0/README.md
+-rw-r--r--   0        0        0      205 2024-05-01 12:25:23.214243 neo4j_runway-0.2.0/neo4j_runway/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-29 23:04:42.985466 neo4j_runway-0.2.0/neo4j_runway/discovery/__init__.py
+-rw-r--r--   0        0        0     4373 2024-05-20 15:27:42.152492 neo4j_runway-0.2.0/neo4j_runway/discovery/discovery.py
+-rw-r--r--   0        0        0       79 2024-04-29 23:04:42.986387 neo4j_runway-0.2.0/neo4j_runway/ingestion/__init__.py
+-rw-r--r--   0        0        0    15503 2024-05-20 16:02:28.192255 neo4j_runway-0.2.0/neo4j_runway/ingestion/generate_ingest.py
+-rwxr-xr-x   0        0        0     4922 2024-05-20 15:50:27.701057 neo4j_runway-0.2.0/neo4j_runway/ingestion/pyingest.py
+-rw-r--r--   0        0        0       21 2024-04-29 23:04:42.987658 neo4j_runway-0.2.0/neo4j_runway/llm/__init__.py
+-rw-r--r--   0        0        0     4962 2024-05-20 18:43:19.227627 neo4j_runway-0.2.0/neo4j_runway/llm/llm.py
+-rw-r--r--   0        0        0       38 2024-04-29 23:04:42.988650 neo4j_runway-0.2.0/neo4j_runway/modeler/__init__.py
+-rw-r--r--   0        0        0    10072 2024-05-20 18:43:19.231514 neo4j_runway-0.2.0/neo4j_runway/modeler/modeler.py
+-rw-r--r--   0        0        0      229 2024-05-02 11:43:53.434393 neo4j_runway-0.2.0/neo4j_runway/objects/__init__.py
+-rw-r--r--   0        0        0     2990 2024-05-15 19:25:52.037594 neo4j_runway-0.2.0/neo4j_runway/objects/arrows.py
+-rw-r--r--   0        0        0    11786 2024-05-20 18:43:19.232422 neo4j_runway-0.2.0/neo4j_runway/objects/data_model.py
+-rw-r--r--   0        0        0     4828 2024-05-15 19:25:52.038524 neo4j_runway-0.2.0/neo4j_runway/objects/node.py
+-rw-r--r--   0        0        0     2934 2024-05-15 19:25:52.039220 neo4j_runway-0.2.0/neo4j_runway/objects/property.py
+-rw-r--r--   0        0        0     5438 2024-05-20 15:27:42.186513 neo4j_runway-0.2.0/neo4j_runway/objects/relationship.py
+-rw-r--r--   0        0        0      904 2024-05-02 11:43:53.436909 neo4j_runway-0.2.0/neo4j_runway/objects/user_input.py
+-rw-r--r--   0        0        0     2393 2024-05-20 18:43:19.233382 neo4j_runway-0.2.0/neo4j_runway/resources/prompts/prompts.py
+-rw-r--r--   0        0        0      138 2024-04-29 23:04:43.003742 neo4j_runway-0.2.0/neo4j_runway/utils/__init__.py
+-rw-r--r--   0        0        0     3429 2024-04-29 23:04:43.003938 neo4j_runway-0.2.0/neo4j_runway/utils/naming_conventions.py
+-rw-r--r--   0        0        0      917 2024-05-01 12:25:23.223161 neo4j_runway-0.2.0/neo4j_runway/utils/test_connection.py
+-rw-r--r--   0        0        0     1133 2024-05-20 18:56:18.317163 neo4j_runway-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5993 1970-01-01 00:00:00.000000 neo4j_runway-0.2.0/PKG-INFO
```

### Comparing `neo4j_runway-0.1.1/LICENSE` & `neo4j_runway-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.1.1/README.md` & `neo4j_runway-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -52,38 +52,38 @@
 ```Python
 llm = LLM()
 ```
 
 And we run discovery on our data.
 ```Python
 disc = Discovery(llm=llm, user_input=USER_GENERATED_INPUT, data=data)
-discovery = disc.run()
+disc.run()
 ```
 
 ### Data Modeling
 We can now pass our Discovery object to a GraphDataModeler to generate our initial data model. A Discovery object isn't required here, but it provides rich context to the LLM to achieve the best results.
 ```Python
 gdm = GraphDataModeler(llm=llm, discovery=disc)
 initial_model = gdm.create_initial_model()
 ```
 If we have graphviz installed, we can take a look at our model.
 ```Python
 gdm.current_model.visualize()
 ```
-![countries-first-model.svg](./images/countries-first-model.svg)
+![countries-first-model.png](./images/countries-first-model.png)
 
 Let's make some corrections to our model and view the results.
 ```Python
 gdm.iterate_model(user_corrections="""
 Make Region node have a HAS_SUBREGION relationship with Subregion node. 
 Remove The relationship between Country and Region.
 """)
 gdm.current_model.visualize()
 ```
-![countries-second-model.svg](./images/countries-second-model.svg)
+![countries-second-model.png](./images/countries-second-model.png)
 
 ### Code Generation
 We can now use our data model to generate some ingestion code.
 
 ```Python
 gen = IngestionGenerator(data_model=gdm.current_model, 
                          username="neo4j", password="password",
```

### Comparing `neo4j_runway-0.1.1/neo4j_runway/discovery/discovery.py` & `neo4j_runway-0.2.0/neo4j_runway/discovery/discovery.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import io
+import os
 from typing import Dict, Union
 
 import pandas as pd
 
 from ..llm.llm import LLM
 from ..objects.user_input import UserInput
 
@@ -89,7 +90,58 @@
             formatted_prompt=self._generate_discovery_prompt()
         )
 
         self._discovery_ran = True
         self.discovery = response
 
         return response
+
+    def to_txt(self, file_dir: str = "./", file_name: str = "discovery") -> None:
+        """
+        Save the generated discovery to a .txt file.
+        """
+
+        if file_dir != "./":
+            os.makedirs(file_dir, exist_ok=True)
+
+        with open(f"./{file_dir}{file_name}.txt", "w") as f:
+
+            f.write(
+                f"""
+Data General Info
+{self.df_info}
+
+Numeric Data Descriptions
+{self.numeric_data_description}
+
+Categorical Data Descriptions
+{self.categorical_data_description}
+
+LLM Generated Discovery
+{self.discovery}
+            """
+            )
+
+    def to_markdown(self, file_dir: str = "./", file_name: str = "discovery") -> None:
+        """
+        Save the generated discovery to a .md file.
+        """
+
+        if file_dir != "./":
+            os.makedirs(file_dir, exist_ok=True)
+
+        with open(f"./{file_dir}{file_name}.md", "w") as f:
+            f.write(
+                f"""
+Data General Info
+{self.df_info}
+
+Numeric Data Descriptions
+{self.numeric_data_description}
+
+Categorical Data Descriptions
+{self.categorical_data_description}
+
+LLM Generated Discovery
+{self.discovery}
+            """
+            )
```

### Comparing `neo4j_runway-0.1.1/neo4j_runway/ingestion/generate_ingest.py` & `neo4j_runway-0.2.0/neo4j_runway/ingestion/generate_ingest.py`

 * *Files 17% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 
 class IngestionGenerator:
 
     def __init__(
         self,
         data_model: DataModel,
-        csv_name: str,
+        csv_name: str = "",
         username: Union[str, None] = None,
         password: Union[str, None] = None,
         uri: Union[str, None] = None,
         database: Union[str, None] = None,
         csv_dir: str = "",
         file_output_dir: str = "",
     ):
@@ -63,70 +63,93 @@
         self._config_files_list: Union[List[Dict[str, Any]], None] = []
         self._constraints: Dict[str, str] = {}
         self._cypher_map: Dict[str, Dict[str, Any]] = {}
 
     def _generate_base_information(self, method: str = "api", batch_size: int = 100):
         for node in self.data_model.nodes:
             if len(node.unique_properties_column_mapping) > 0:
+                # unique constraints
                 for unique_property in node.unique_properties:
                     self._constraints[
                         generate_constraints_key(
                             label_or_type=node.label, unique_property=unique_property
                         )
                     ] = generate_constraint(
                         label_or_type=node.label, unique_property=unique_property
                     )
+            # node keys
+            if node.node_keys:
+                self._constraints[
+                    generate_constraints_key(
+                        label_or_type=node.label, unique_property=node.node_keys
+                    )
+                ] = generate_node_key_constraint(
+                    label=node.label, unique_property=node.node_keys
+                )
 
             # add to cypher map
             self._cypher_map[lowercase_first_letter(node.label)] = {
                 "cypher": literal_unicode(
                     generate_merge_node_clause_standard(node=node)
                 ),
                 "cypher_loadcsv": literal_unicode(
                     generate_merge_node_load_csv_clause(
                         node=node,
-                        csv_name=self.csv_name,
+                        csv_name=(
+                            node.csv_name if self.csv_name == "" else self.csv_name
+                        ),
                         method=method,
                         batch_size=batch_size,
                     )
                 ),
-                "csv": f"$BASE/{self.csv_dir}{self.csv_name}",
+                "csv": f"$BASE/{self.csv_dir}{node.csv_name if self.csv_name == '' else self.csv_name}",
             }
 
         ## get relationships
         for rel in self.data_model.relationships:
             if len(rel.unique_properties_column_mapping) > 0:
+                # unique constraints
                 for unique_property in rel.unique_properties:
                     self._constraints[
                         generate_constraints_key(
                             label_or_type=rel.type, unique_property=unique_property
                         )
                     ] = generate_constraint(
                         label_or_type=rel.type, unique_property=unique_property
                     )
 
+            # relationship keys
+            if rel.relationship_keys:
+                self._constraints[
+                    generate_constraints_key(
+                        label_or_type=node.label, unique_property=node.node_keys
+                    )
+                ] = generate_relationship_key_constraint(
+                    type=rel.type, unique_property=rel.relationship_keys
+                )
+
             source = self.data_model.node_dict[rel.source]
             target = self.data_model.node_dict[rel.target]
             self._cypher_map[f"{rel.source}_{rel.target}"] = {
                 "cypher": literal_unicode(
                     generate_merge_relationship_clause_standard(
                         relationship=rel, source_node=source, target_node=target
                     )
                 ),
                 "cypher_loadcsv": literal_unicode(
                     generate_merge_relationship_load_csv_clause(
                         relationship=rel,
                         source_node=source,
                         target_node=target,
-                        csv_name=self.csv_name,
+                        csv_name=rel.csv_name if self.csv_name == "" else self.csv_name,
                         method=method,
                         batch_size=batch_size,
                     )
                 ),
-                "csv": f"$BASE/{self.csv_dir}{self.csv_name}",
+                "csv": f"$BASE/{self.csv_dir}{rel.csv_name if self.csv_name == '' else self.csv_name}",
             }
 
         self._config_files_list = []
         for item in self._cypher_map:
             file_dict = {}
             if self._cypher_map[item]["csv"]:
                 file_dict["url"] = self._cypher_map[item]["csv"]
@@ -159,15 +182,15 @@
         config_dump = yaml.dump(final_yaml)
 
         to_return = (
             f"server_uri: {self.uri}\n"
             + f"admin_user: {self.username}\n"
             + f"admin_pass: {self.password}\n"
             + f"database: {self.database}\n"
-            + "basepath: file:./\n\n"
+            + "basepath: ./\n\n"
             + "pre_ingest:\n"
         )
         for constraint in self._constraints:
             to_return += f"  - {self._constraints[constraint]}"
         to_return += config_dump
 
         return to_return
@@ -231,20 +254,26 @@
 
         for item in self._cypher_map:
             to_return = to_return + self._cypher_map[item]["cypher_loadcsv"]
 
         return to_return
 
 
-def generate_constraints_key(label_or_type: str, unique_property: str) -> str:
+def generate_constraints_key(
+    label_or_type: str, unique_property: Union[str, List[str]]
+) -> str:
     """
-    Generate the key for a unique constraint.
+    Generate the key for a unique or node key constraint.
     """
-
-    return f"{label_or_type.lower()}_{unique_property.lower()}"
+    if isinstance(unique_property, str):
+        return f"{label_or_type.lower()}_{unique_property.lower()}"
+    else:
+        return (
+            f"{label_or_type.lower()}_{'_'.join([x.lower() for x in unique_property])}"
+        )
 
 
 def generate_constraint(label_or_type: str, unique_property: str) -> str:
     """
     Generate a constrant string.
     """
 
@@ -256,19 +285,39 @@
     Generate a MATCH node clause.
     """
 
     return (
         "MATCH (n:"
         + node.label
         + " {"
-        + f"{generate_set_unique_property(node.unique_properties_column_mapping)}"
+        + f"{generate_set_unique_property(node.node_key_mapping or node.unique_properties_column_mapping)}"
         + "})"
     )
 
 
+def generate_match_same_node_labels_clause(node: Node) -> str:
+    """
+    Generate the two match statements for node with two unique csv mappings.
+    This is used when a relationship connects two nodes with the same label.
+    An example: (:Person{name: row.person_name})-[:KNOWS]->(:Person{name:row.knows_person})
+    """
+
+    from_unique, to_unique = [
+        (
+            "{" + f"{prop}: row.{csv_mapping[0]}" + "}",
+            "{" + f"{prop}: row.{csv_mapping[1]}" + "}",
+        )
+        for prop, csv_mapping in node.unique_properties_column_mapping.items()
+        if isinstance(csv_mapping, list)
+    ][0]
+
+    return f"""MATCH (source:{node.label} {from_unique})
+MATCH (target:{node.label} {to_unique})"""
+
+
 def generate_set_property(property_column_mapping: Dict[str, str]) -> str:
     """
     Generate a set property string.
     """
 
     temp_set_list = []
 
@@ -280,37 +329,41 @@
     if not result == "":
         result = f"SET {result}"
 
     return result
 
 
 def generate_set_unique_property(
-    unique_properties_column_mapping: Dict[str, str]
+    unique_properties_column_mapping: Dict[str, Union[str, List[str]]]
 ) -> str:
     """
     Generate the unique properties to match a node on within a MERGE statement.
     Returns: unique_property_match_component
     """
 
     res = [
-        f"{prop}: row.{csv_mapping}"
+        (
+            f"{prop}: row.{csv_mapping[0]}"
+            if isinstance(csv_mapping, list)
+            else f"{prop}: row.{csv_mapping}"
+        )
         for prop, csv_mapping in unique_properties_column_mapping.items()
     ]
     return ", ".join(res)
 
 
 def generate_merge_node_clause_standard(node: Node) -> str:
     """
     Generate a MERGE node clause.
     """
 
     return f"""WITH $dict.rows AS rows
 UNWIND rows AS row
-MERGE (n:{node.label} {{{generate_set_unique_property(node.unique_properties_column_mapping)}}})
-{generate_set_property(node.nonunique_properties_column_mapping)}"""
+MERGE (n:{node.label} {{{generate_set_unique_property(node.node_key_mapping or node.unique_properties_column_mapping)}}})
+{generate_set_property(node.nonunique_properties_mapping_for_set_clause)}"""
 
 
 def generate_merge_node_load_csv_clause(
     node: Node,
     csv_name: str,
     method: str = "api",
     batch_size: int = 10000,
@@ -319,33 +372,39 @@
     Generate a MERGE node clause for the LOAD CSV method.
     """
 
     command = ":auto " if method == "browser" else ""
     return f"""{command}LOAD CSV WITH HEADERS FROM 'file:///{csv_name}' as row
 CALL {{
     WITH row
-    MERGE (n:{node.label} {{{generate_set_unique_property(node.unique_properties_column_mapping)}}})
-    {generate_set_property(node.nonunique_properties_column_mapping)}
+    MERGE (n:{node.label} {{{generate_set_unique_property(node.node_key_mapping or node.unique_properties_column_mapping)}}})
+    {generate_set_property(node.nonunique_properties_mapping_for_set_clause)}
 }} IN TRANSACTIONS OF {str(batch_size)} ROWS;
 """
 
 
 def generate_merge_relationship_clause_standard(
     relationship: Relationship, source_node: Node, target_node: Node
 ) -> str:
     """
     Generate a MERGE relationship clause.
     """
-
-    return f"""WITH $dict.rows AS rows
+    if source_node.label == target_node.label:
+        return f"""WITH $dict.rows AS rows
+UNWIND rows as row
+{generate_match_same_node_labels_clause(node=source_node)}
+MERGE (source)-[n:{relationship.type}]->(target)
+{generate_set_property(relationship.nonunique_properties_mapping_for_set_clause)}"""
+    else:
+        return f"""WITH $dict.rows AS rows
 UNWIND rows as row
 {generate_match_node_clause(source_node).replace('(n:', '(source:')}
 {generate_match_node_clause(target_node).replace('(n:', '(target:')}
 MERGE (source)-[n:{relationship.type}]->(target)
-{generate_set_property(relationship.nonunique_properties_column_mapping)}"""
+{generate_set_property(relationship.nonunique_properties_mapping_for_set_clause)}"""
 
 
 def generate_merge_relationship_load_csv_clause(
     relationship: Relationship,
     source_node: Node,
     target_node: Node,
     csv_name: str,
@@ -353,16 +412,46 @@
     batch_size: int = 10000,
 ) -> str:
     """
     Generate a MERGE relationship clause for the LOAD CSV method.
     """
 
     command = ":auto " if method == "browser" else ""
-    return f"""{command}LOAD CSV WITH HEADERS FROM 'file:///{csv_name}' as row
+    if source_node.label == target_node.label:
+        return f"""{command}LOAD CSV WITH HEADERS FROM 'file:///{csv_name}' as row
+CALL {{
+    WITH row
+    {generate_match_same_node_labels_clause(node=source_node)}
+    MERGE (source)-[n:{relationship.type}]->(target)
+    {generate_set_property(relationship.nonunique_properties_mapping_for_set_clause)}
+}} IN TRANSACTIONS OF {str(batch_size)} ROWS;
+"""
+    else:
+        return f"""{command}LOAD CSV WITH HEADERS FROM 'file:///{csv_name}' as row
 CALL {{
     WITH row
     {generate_match_node_clause(source_node).replace('(n:', '(source:')}
     {generate_match_node_clause(target_node).replace('(n:', '(target:')}
     MERGE (source)-[n:{relationship.type}]->(target)
-    {generate_set_property(relationship.nonunique_properties_column_mapping)}
+    {generate_set_property(relationship.nonunique_properties_mapping_for_set_clause)}
 }} IN TRANSACTIONS OF {str(batch_size)} ROWS;
 """
+
+
+def generate_node_key_constraint(
+    label: str, unique_property: Union[str, List[str]]
+) -> str:
+    """
+    Generate a node key constraint.
+    """
+    props = "(" + ", ".join([f"n.{x}" for x in unique_property]) + ")"
+    return f"""CREATE CONSTRAINT {generate_constraints_key(label_or_type=label, unique_property=unique_property)} IF NOT EXISTS FOR (n:{label}) REQUIRE {props} IS NODE KEY;\n"""
+
+
+def generate_relationship_key_constraint(
+    type: str, unique_property: Union[str, List[str]]
+) -> str:
+    """
+    Generate a relationship key constraint.
+    """
+    props = "(" + ", ".join([f"r.{x}" for x in unique_property]) + ")"
+    return f"""CREATE CONSTRAINT {generate_constraints_key(label_or_type=type, unique_property=unique_property)} IF NOT EXISTS FOR ()-[r:{type}]-() REQUIRE {props} IS RELATIONSHIP KEY;\n"""
```

### Comparing `neo4j_runway-0.1.1/neo4j_runway/ingestion/pyingest.py` & `neo4j_runway-0.2.0/neo4j_runway/ingestion/pyingest.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 This is a modified PyIngest file for Neo4j Runway. It currently only supports Pandas DataFrame ingestion.
 """
 
 import datetime
+from typing import Optional
 
 from neo4j import GraphDatabase
 import numpy as np
 import pandas as pd
 import yaml
 
 
@@ -28,16 +29,14 @@
     def close(self):
         self._driver.close()
 
     def get_params(self, file):
         params = dict()
         params["skip_records"] = file.get("skip_records") or 0
         params["compression"] = file.get("compression") or "none"
-        # if params["compression"] not in supported_compression_formats:
-        #     print("Unsupported compression format: {}", params["compression"])
 
         file_url = file["url"]
         if self.basepath and file_url.startswith("$BASE"):
             file_url = file_url.replace("$BASE", self.basepath, 1)
         params["url"] = file_url
         print("File {}", params["url"])
         params["cql"] = file["cql"]
@@ -58,14 +57,47 @@
                 print("loading...", i, datetime.datetime.now(), flush=True)
                 # Chunk up the rows to enable additional fastness :-)
                 rows_dict = {"rows": rows.fillna(value="").to_dict("records")}
                 session.run(params["cql"], dict=rows_dict).consume()
 
         print("{} : Completed file", datetime.datetime.now())
 
+    def load_csv(self, file):
+        with self._driver.session(**self.db_config) as session:
+            params = self.get_params(file)
+
+            with open(params["url"]) as openfile:
+                # Grab the header from the file and pass that to pandas.  This allow the header
+                # to be applied even if we are skipping lines of the file
+                header = str(openfile.readline()).strip().split(params['field_sep'])
+
+                # Pandas' read_csv method is highly optimized and fast :-)
+                row_chunks = pd.read_csv(
+                    openfile,
+                    dtype=str,
+                    sep=params["field_sep"],
+                    on_bad_lines="skip",
+                    index_col=False,
+                    skiprows=params["skip_records"],
+                    names=header,
+                    low_memory=False,
+                    engine="c",
+                    compression="infer",
+                    header=None,
+                    chunksize=params["chunk_size"],
+                )
+
+                for i, rows in enumerate(row_chunks):
+                    print(params["url"], i, datetime.datetime.now(), flush=True)
+                    # Chunk up the rows to enable additional fastness :-)
+                    rows_dict = {"rows": rows.fillna(value="").to_dict("records")}
+                    session.run(params["cql"], dict=rows_dict).consume()
+
+        print("{} : Completed file", datetime.datetime.now())
+
     def pre_ingest(self):
         if "pre_ingest" in config:
             statements = config["pre_ingest"]
             if len(statements) > 0:
                 with self._driver.session(**self.db_config) as session:
                     for statement in statements:
                         session.run(statement)
@@ -84,17 +116,19 @@
 
 
 def load_config(configuration):
     global config
     config = yaml.safe_load(configuration)
 
 
-def PyIngest(yaml_string: str, dataframe: pd.DataFrame) -> None:
-    # configuration = sys.argv[1]
+def PyIngest(yaml_string: str, dataframe: Optional[pd.DataFrame] = None) -> None:
     load_config(yaml_string)
     server = LocalServer()
     server.pre_ingest()
     file_list = config["files"]
     for file in file_list:
-        server.load_dataframe(file, dataframe=dataframe)
+        if dataframe is not None:
+            server.load_dataframe(file, dataframe=dataframe)
+        else:
+            server.load_csv(file)
     server.post_ingest()
     server.close()
```

### Comparing `neo4j_runway-0.1.1/neo4j_runway/llm/llm.py` & `neo4j_runway-0.2.0/neo4j_runway/llm/llm.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import instructor
 
 from ..objects.data_model import DataModel
 from ..resources.prompts.prompts import system_prompts
 from ..resources.prompts.prompts import model_generation_rules
 
 MODEL_OPTIONS = [
+    "gpt-4o",
+    "gpt-4o-2024-05-13",
     "gpt-4",
     "gpt-3.5-turbo",
     "gpt-4-0125-preview",
     "gpt-4-turbo-preview",
     "gpt-4-1106-preview",
     "gpt-4-0613",
     "gpt-4-32k",
@@ -23,18 +25,24 @@
     "gpt-3.5-turbo-0125",
 ]
 
 
 class LLM:
     """
     Interface for interacting with different LLMs.
+    Attributes
+    ----------
+    model: str
+        The OpenAI LLM to use.
+    open_ai_key: Union[str, None] = None
+        Your OpenAI API key if it is not declared in an environment variable.
     """
 
     def __init__(
-        self, model: str = "gpt-4-0125-preview", open_ai_key: Union[str, None] = None
+        self, model: str = "gpt-4o-2024-05-13", open_ai_key: Union[str, None] = None
     ) -> None:
 
         if model not in MODEL_OPTIONS:
             raise ValueError("model must be one of the following: ", MODEL_OPTIONS)
         self.llm_instance = instructor.patch(
             OpenAI(
                 api_key=(
@@ -42,15 +50,15 @@
                     if open_ai_key is not None
                     else os.environ.get("OPENAI_API_KEY")
                 )
             )
         )
         self.model = model
 
-    def get_discovery_response(self, formatted_prompt: str) -> DataModel:
+    def get_discovery_response(self, formatted_prompt: str) -> str:
         """
         Get a discovery response from the LLM.
         """
 
         response = self.llm_instance.chat.completions.create(
             model=self.model,
             temperature=0,
@@ -58,27 +66,31 @@
                 {"role": "system", "content": system_prompts["discovery"]},
                 {"role": "user", "content": formatted_prompt},
             ],
         )
         return response.choices[0].message.content
 
     def get_data_model_response(
-        self, formatted_prompt: str, csv_columns: List[str], max_retries: int = 3
+        self,
+        formatted_prompt: str,
+        csv_columns: List[str],
+        max_retries: int = 3,
+        use_yaml_data_model: bool = False,
     ) -> DataModel:
         """
         Get a data model response from the LLM.
         """
 
         retries = 0
         valid_response = False
         while retries < max_retries and not valid_response:
 
             retries += 1  # increment retries each pass
 
-            response = self.llm_instance.chat.completions.create(
+            response: DataModel = self.llm_instance.chat.completions.create(
                 model=self.model,
                 temperature=0,
                 response_model=DataModel,
                 messages=[
                     {"role": "system", "content": system_prompts["data_model"]},
                     {"role": "user", "content": formatted_prompt},
                 ],
@@ -90,17 +102,20 @@
                 cot = self.get_chain_of_thought_response(
                     formatted_prompt=validation["message"]
                 )
                 # formatted_prompt = validation['message']
                 formatted_prompt = self._generate_retry_prompt(
                     chain_of_thought_response=cot,
                     errors_to_fix=validation["errors"],
-                    model_to_fix=response,
+                    model_to_fix=(
+                        response.to_yaml(write_file=False)
+                        if use_yaml_data_model
+                        else response
+                    ),
                 )
-                print("retry prompt: ", formatted_prompt)
             elif validation["valid"]:
                 print("recieved a valid response")
                 valid_response = True
 
         return response
 
     def get_chain_of_thought_response(self, formatted_prompt: str) -> str:
@@ -118,15 +133,15 @@
         )
         return response.choices[0].message.content
 
     def _generate_retry_prompt(
         self,
         chain_of_thought_response: str,
         errors_to_fix: str,
-        model_to_fix: DataModel,
+        model_to_fix: Union[DataModel, str],
     ) -> str:
         """
         Generate a prompt to fix the data model using the errors found in previous model
         and the chain of thought response containing ideas on how to fix the errors.
         """
 
         return f"""
```

### Comparing `neo4j_runway-0.1.1/neo4j_runway/modeler/modeler.py` & `neo4j_runway-0.2.0/neo4j_runway/modeler/modeler.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,58 @@
-from typing import Dict, Any, Union
+from typing import Dict, Any, Union, List
 import warnings
 
 from graphviz import Digraph
 
 from ..discovery import Discovery
 from ..llm import LLM
-from ..objects import DataModel
+from ..objects import DataModel, UserInput
 from ..resources.prompts.prompts import model_generation_rules, model_format
 
 
 class GraphDataModeler:
+    """
+    Attributes
+    ----------
+    llm : LLM
+        The LLM used to generate data models.
+    discovery : Union[str, Discovery] = ""
+        Either a string containing the LLM generated discovery or a Discovery object that has been ran.
+        If a Discovery object is provided then the remaining discovery attributes don't need to be provided.
+    user_input : Dict[str, UserInput] = {}
+        Either a dictionary with keys general_description and column names with descriptions or a UserInput object.
+        Not required.
+    general_data_description : str = ""
+        A general data description provided by Discovery. Not required.
+    numeric_data_description : str = ""
+        A numeric data description provided by Discovery. Not required.
+    categorical_data_description : str = ""
+        A categorical data description provided by Discovery. Not required.
+    feature_descriptions : str = ""
+        Feature descriptions provided by Discovery. Not required.
+    """
 
     def __init__(
         self,
         llm: LLM,
         discovery: Union[str, Discovery] = "",
-        user_input: Dict[str, str] = {},
+        user_input: Union[Dict[str, str], UserInput] = {},
         general_data_description: str = "",
         numeric_data_description: str = "",
         categorical_data_description: str = "",
         feature_descriptions: str = "",
     ) -> None:
         """
-        Takes an LLM instance and Discovery information. Either a Discovery object can be provided, or each field can be provided individually.
+        Takes an LLM instance and Discovery information.
+        Either a Discovery object can be provided, or each field can be provided individually.
         """
 
         self.llm = llm
 
         if isinstance(discovery, Discovery):
-            # print("discovery instance")
             self.user_input = discovery.user_input
 
             assert "general_description" in self.user_input.keys(), (
                 "user_input must include key:value pair {general_description: ...}. "
                 + f"Found keys {self.user_input.keys()}"
             )
 
@@ -41,55 +61,76 @@
             self.discovery = discovery.discovery
             self.general_info = discovery.df_info
             self.description_numeric = discovery.numeric_data_description
             self.description_categorical = discovery.categorical_data_description
             self.feature_descriptions = discovery.feature_descriptions
 
         else:
-            # print("no discovery instance")
-            self.user_input = user_input
 
-            assert "general_description" in self.user_input.keys(), (
-                "user_input must include key:value pair {general_description: ...}. "
-                + f"Found keys {self.user_input.keys()}"
-            )
+            if isinstance(user_input, UserInput):
+                self.user_input = user_input.formatted_dict
+            else:
+                self.user_input = user_input
+                assert "general_description" in self.user_input.keys(), (
+                    "user_input must include key:value pair {general_description: ...}. "
+                    + f"Found keys {self.user_input.keys()}"
+                )
+
+            # self.user_input = user_input
 
-            self.columns_of_interest = list(user_input.keys())
+            # assert "general_description" in self.user_input.keys(), (
+            #     "user_input must include key:value pair {general_description: ...}. "
+            #     + f"Found keys {self.user_input.keys()}"
+            # )
+
+            self.columns_of_interest = list(self.user_input.keys())
             self.columns_of_interest.remove("general_description")
 
             self.discovery = discovery
             self.general_info = general_data_description
             self.description_numeric = numeric_data_description
             self.description_categorical = categorical_data_description
             self.feature_descriptions = feature_descriptions
 
         if self.discovery == "":
             warnings.warn(
                 "It is highly recommended to provide discovery generated from the Discovery module."
             )
 
-        self._initial_model_created = False
-        self.model_iterations = 0
-        self.model_history = []
+        self._initial_model_created: bool = False
+        self.model_iterations: int = 0
+        self.model_history: List[DataModel] = []
 
     @property
     def current_model(self) -> DataModel:
         """
         The current data model.
         """
 
         assert len(self.model_history) > 0, "No models found in history."
 
         return self.model_history[-1]
 
+    def load_model(self, data_model: DataModel) -> None:
+        """
+        Append a new data model to the end of the model_history.
+        This will become the new current_model.
+        """
+
+        if not isinstance(data_model, DataModel):
+            raise ValueError("Provided data model is not of type <DataModel>!")
+
+        self.model_history.append(data_model)
+        self._initial_model_created = True
+
     def get_model(
         self, version: int = -1, as_dict: bool = False
     ) -> Union[DataModel, Dict[str, Any]]:
         """
-        Returns the data model version specified.
+        Returns the data model version specified. Example: Version 1 will return model_history index 0.
         By default will return the most recent model.
         Allows access to the intial model.
         """
 
         assert len(self.model_history) > 0, "No models found in history."
         assert version != 0, "No model version 0."
         if version < 0:
@@ -141,15 +182,17 @@
             {model_generation_rules}
 
             {model_format}
             """
         return prompt
 
     def _generate_data_model_iteration_prompt(
-        self, user_corrections: Union[str, None] = None
+        self,
+        user_corrections: Union[str, None] = None,
+        use_yaml_data_model: bool = False,
     ) -> str:
         """
         Generate the prompt to iterate on the previous data model.
         """
 
         if user_corrections is not None:
             user_corrections = (
@@ -175,58 +218,63 @@
             {self.feature_descriptions}
 
             Here is the initial discovery findings:
             {self.discovery}
 
             Based on your experience building high-quality graph data
             models, are there any improvements you would suggest to this model?
-            {self.current_model}
+            {self.current_model.to_yaml(write_file=False) if use_yaml_data_model else self.current_model}
 
             {user_corrections}
 
             {model_generation_rules}
             """
 
         return prompt
 
     def create_initial_model(self) -> str:
         """
         Create the initial model.
         """
 
-        # assert self._discovery_ran, "Run discovery before creating the initial model."
-
         response = self.llm.get_data_model_response(
             formatted_prompt=self._generate_initial_data_model_prompt(),
             csv_columns=self.columns_of_interest,
         )
 
         self.model_history.append(response)
 
         self._initial_model_created = True
 
         return response
 
     def iterate_model(
-        self, iterations: int = 1, user_corrections: Union[str, None] = None
+        self,
+        iterations: int = 1,
+        user_corrections: Union[str, None] = None,
+        use_yaml_data_model: bool = False,
     ) -> str:
         """
         Iterate on the previous data model the number times indicated.
         """
 
         assert self._initial_model_created, "No data model present to iterate on."
 
-        def iterate():
+        def iterate() -> DataModel:
             for i in range(0, iterations):
                 response = self.llm.get_data_model_response(
                     formatted_prompt=self._generate_data_model_iteration_prompt(
-                        user_corrections=user_corrections
+                        user_corrections=user_corrections,
+                        use_yaml_data_model=use_yaml_data_model,
                     ),
                     csv_columns=self.columns_of_interest,
+                    use_yaml_data_model=use_yaml_data_model,
                 )
 
                 self.model_history.append(response)
                 self.model_iterations += 1
-                yield response
 
-        for iteration in iterate():
-            return iteration
+            return response
+        
+        current_model = iterate()
+        
+        return current_model
```

### Comparing `neo4j_runway-0.1.1/neo4j_runway/objects/data_model.py` & `neo4j_runway-0.2.0/neo4j_runway/objects/data_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from ast import literal_eval
-from typing import List, Dict, Union
+from typing import List, Dict, Union, Self
 
 from graphviz import Digraph
 from pydantic import BaseModel
+import yaml
 
 from ..objects.arrows import ArrowsNode, ArrowsRelationship, ArrowsDataModel
 from ..objects.node import Node
 from ..objects.relationship import Relationship
 from ..resources.prompts.prompts import model_generation_rules
 from ..utils.naming_conventions import (
     fix_node_label,
@@ -14,14 +15,23 @@
     fix_relationship_type,
 )
 
 
 class DataModel(BaseModel):
     """
     Graph Data Model representation.
+
+    Attributes
+    ----------
+    nodes : List<Node>
+        A list of the nodes in the data model.
+    relationships : List<Relationship>
+        A list of the relationships in the data model.
+    use_neo4j_naming_conventions : bool
+        Whether to convert labels, relationships and properties to Neo4j naming conventions.
     """
 
     nodes: List[Node]
     relationships: List[Relationship]
 
     def __init__(
         self,
@@ -123,31 +133,36 @@
         return errors
 
     def _validate_csv_features_used_only_once(self) -> List[Union[str, None]]:
         """
         Validate that each property is used no more than one time in the data model.
         """
 
-        used_features = {}
-        errors = []
+        used_features: Dict[str, List[str]] = {}
+        errors: List[str] = []
 
         for node in self.nodes:
             for prop in node.properties:
-                if prop.csv_mapping not in list(used_features.keys()):
-                    used_features[prop.csv_mapping] = [node.label]
+                if isinstance(prop.csv_mapping, list):
+                    for csv_map in prop.csv_mapping:
+                        if csv_map not in list(used_features.keys()):
+                            used_features[csv_map] = [node.label]
+                        else:
+                            used_features[csv_map].append(node.label)
                 else:
-                    used_features[prop.csv_mapping].append(node.label)
-                    # errors.append(f"The property {prop} is used for {used_features[prop]} in the data model. Each node or relationship must use a different csv column as a property instead.")
+                    if prop.csv_mapping not in list(used_features.keys()):
+                        used_features[prop.csv_mapping] = [node.label]
+                    else:
+                        used_features[prop.csv_mapping].append(node.label)
         for rel in self.relationships:
             for prop in rel.properties:
                 if prop.csv_mapping not in used_features:
                     used_features[prop.csv_mapping] = [rel.type]
                 else:
                     used_features[prop.csv_mapping].append(rel.type)
-                    # errors.append(f"The property {prop} is used for {used_features[prop]} in the data model. Each node or relationship must use a different csv column as a property instead.")
         for prop, labels_or_types in used_features.items():
             if len(labels_or_types) > 1:
                 errors.append(
                     f"The property csv_mapping {prop} is used for {labels_or_types} in the data model. Each of these must use a different csv column as a property csv_mapping instead. Find alternative property csv_mappings from the column options or remove."
                 )
 
         return errors
@@ -174,27 +189,25 @@
     @staticmethod
     def _generate_node_text(node: Node) -> str:
         """
         Generate the label, property and unique constraints displayed on a node.
         """
 
         result = node.label
-        # print(result)
         if len(node.properties) > 0:
             result += "\n\nproperties:\n"
-            # print(result)
         for prop in node.properties:
             result = (
                 result
                 + prop.name
                 + f": {prop.csv_mapping}"
                 + (" *unique*" if prop.is_unique else "")
+                + (" *key*" if prop.part_of_key else "")
                 + "\n"
             )
-            # print(result)
 
         return result
 
     @staticmethod
     def _generate_relationship_text(relationship: Relationship) -> str:
         """
         Generate the label, property and unique constraints displayed on a relationship.
@@ -205,14 +218,15 @@
             result += "\n\nproperties:\n"
         for prop in relationship.properties:
             result = (
                 result
                 + prop.name
                 + f": {prop.csv_mapping}"
                 + (" *unique*" if prop.is_unique else "")
+                + (" *key*" if prop.part_of_key else "")
                 + "\n"
             )
 
         return result
 
     def apply_neo4j_naming_conventions(self) -> None:
         """
@@ -239,14 +253,27 @@
         """
 
         with open(f"./{file_name}.json", "w") as f:
             f.write(self.model_dump_json())
 
         return self.model_dump_json()
 
+    def to_yaml(self, file_name: str = "data-model", write_file: bool = True) -> str:
+        """
+        Output the data model to a yaml file and / or yaml string.
+        """
+
+        yaml_string = yaml.dump(self.model_dump())
+
+        if write_file:
+            with open(f"./{file_name}.yaml", "w") as f:
+                f.write(yaml_string)
+
+        return yaml_string
+
     def to_arrows(
         self, file_name: str = "data-model", write_file: bool = True
     ) -> ArrowsDataModel:
         """
         Output the data model to arrows compatible JSON file.
         """
 
@@ -268,15 +295,15 @@
         if write_file:
             with open(f"./{file_name}.json", "w") as f:
                 f.write(arrows_data_model.model_dump_json())
 
         return arrows_data_model
 
     @classmethod
-    def from_arrows(cls, file_path: str) -> None:
+    def from_arrows(cls, file_path: str) -> Self:
         """
         Construct a DataModel from an arrows data model JSON file.
         """
 
         with open(f"{file_path}", "r") as f:
             content = literal_eval(f.read())
             node_id_label_map = {n["id"]: n["labels"][0] for n in content["nodes"]}
```

### Comparing `neo4j_runway-0.1.1/neo4j_runway/objects/property.py` & `neo4j_runway-0.2.0/neo4j_runway/objects/property.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import List, Dict, Union, Any
+from typing import List, Dict, Union, Any, Self
 
 from pydantic import BaseModel, field_validator
 
 
 TYPES_MAP_NEO4J_KEYS = {
     "LIST": "list",
     "MAP": "dict",
@@ -30,16 +30,17 @@
 class Property(BaseModel):
     """
     Property representation.
     """
 
     name: str
     type: str
-    csv_mapping: str
+    csv_mapping: Union[str, List[str]]
     is_unique: bool = False
+    part_of_key: bool = False
     # is_indexed: bool
     # must_exist: bool
 
     @field_validator("type")
     def validate_type(cls, v):
         if v.lower() == "object" or v.lower() == "string":
             return "str"
@@ -59,37 +60,37 @@
     def neo4j_type(self) -> str:
         """
         The Neo4j property type.
         """
         return TYPES_MAP_PYTHON_KEYS[self.type]
 
     @classmethod
-    def from_arrows(cls, arrows_property: Dict[str, str], caption: str = "") -> None:
+    def from_arrows(cls, arrows_property: Dict[str, str], caption: str = "") -> Self:
         """
         Parse the arrows property representation into a standard Property model.
         Arrow property values are formatted as <csv_mapping> | <python_type> | <unique>.
         """
 
         if "|" in list(arrows_property.values())[0]:
             prop_props = [
                 x.strip() for x in list(arrows_property.values())[0].split("|")
             ]
-            csv_mapping = prop_props[0]
+            if "," in prop_props[0]:
+                csv_mapping: List[str] = [x.strip() for x in prop_props[0].split(",")]
+            else:
+                csv_mapping: str = prop_props[0]
             python_type = prop_props[1]
             is_unique = "unique" in prop_props
+            node_key = "nodekey" in prop_props
         else:
-            csv_mapping = list(arrows_property.values())[0]
+            csv_mapping: str = list(arrows_property.values())[0]
             python_type = "unknown"
             is_unique = False
-
-        # support identifying uniqueness in caption for now, this will be depreciated.
-        if caption:
-            is_unique = list(arrows_property.keys())[0] in [
-                x.strip() for x in caption.split(",")
-            ]
+            node_key = False
 
         return cls(
             name=list(arrows_property.keys())[0],
             csv_mapping=csv_mapping,
             type=python_type,
             is_unique=is_unique,
+            part_of_key=node_key,
         )
```

### Comparing `neo4j_runway-0.1.1/neo4j_runway/objects/relationship.py` & `neo4j_runway-0.2.0/neo4j_runway/objects/relationship.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,59 @@
-from typing import List, Dict, Union, Any
+from typing import List, Dict, Union, Any, Self
 
-from pydantic import BaseModel
+from pydantic import BaseModel, field_validator
 
+from ..objects.node import Node
 from ..objects.property import Property
 from ..objects.arrows import ArrowsRelationship
 
 
 class Relationship(BaseModel):
     """
     Relationship representation.
     """
 
     type: str
     properties: List[Property] = []
     source: str
     target: str
+    csv_name: str = ""
 
-    def __init__(self, *a, **kw) -> None:
-        super().__init__(*a, **kw)
+    def __init__(
+        self,
+        type: str,
+        source: str,
+        target: str,
+        properties: List[Property] = [],
+        csv_name: str = "",
+    ) -> None:
+        super().__init__(
+            type=type,
+            source=source,
+            target=target,
+            properties=properties,
+            csv_name=csv_name,
+        )
 
         if self.properties is None:
             self.properties = []
 
+    @field_validator("csv_name")
+    def validate_csv_name(cls, v: str) -> str:
+        """
+        Validate the CSV name provided.
+        """
+
+        if v == "":
+            return v
+        else:
+            if not v.endswith(".csv"):
+                return v + ".csv"
+        return v
+
     @property
     def property_names(self) -> List[str]:
         """
         The relationship's property names.
         """
 
         return [prop.name for prop in self.properties]
@@ -72,54 +100,97 @@
 
         return {
             prop.name: prop.csv_mapping
             for prop in self.properties
             if not prop.is_unique
         }
 
+    @property
+    def relationship_keys(self) -> List[str]:
+        """
+        The relationship's keys.
+        """
+
+        return [prop.name for prop in self.properties if prop.part_of_key]
+
+    @property
+    def relationship_key_mapping(self) -> Dict[str, str]:
+        """
+        Map of relationship keys to their respective csv columns.
+        """
+
+        return {
+            prop.name: prop.csv_mapping for prop in self.properties if prop.part_of_key
+        }
+
+    @property
+    def nonunique_properties_mapping_for_set_clause(self) -> Dict[str, str]:
+        """
+        Map of nonunique properties to their respective csv columns if a property is not unique or a node key.
+        """
+
+        return {
+            prop.name: prop.csv_mapping
+            for prop in self.properties
+            if not prop.is_unique and not prop.part_of_key
+        }
+
     def validate_properties(self, csv_columns: List[str]) -> List[Union[str, None]]:
         errors = []
         if self.properties is not None:
             for prop in self.properties:
                 if prop.csv_mapping not in csv_columns:
-                    # raise ValueError(
                     errors.append(
                         f"The relationship {self.type} the property {prop.name} mapped to csv column {prop.csv_mapping} which does not exist. {prop} should be edited or removed from relationship {self.type}."
                     )
-                    # )
         return errors
 
     def to_arrows(self) -> ArrowsRelationship:
         """
         Return an arrows.app compatible relationship.
         """
 
-        props = {x.name: x.csv_mapping + " | " + x.type for x in self.properties}
+        props = {
+            x.name: (
+                x.csv_mapping + " | " + x.type + " | unique"
+                if x.is_unique
+                else "" + " | nodekey" if x.is_unique else ""
+            )
+            for x in self.properties
+            if x != "csv"
+        }
         arrows_id = self.type + self.source + self.target
         return ArrowsRelationship(
             id=arrows_id,
             fromId=self.source,
             toId=self.target,
             type=self.type,
             properties=props,
         )
 
     @classmethod
     def from_arrows(
         cls, arrows_relationship: ArrowsRelationship, node_id_label_map: Dict[str, str]
-    ):
+    ) -> Self:
         """
         Initialize a relationship from an arrows relationship.
         """
 
         props = [
-            Property.from_arrows(
-                arrows_property={k: v}
-            )
+            Property.from_arrows(arrows_property={k: v})
             for k, v in arrows_relationship.properties.items()
+            if k != "csv"
         ]
+
+        csv_name = (
+            arrows_relationship.properties["csv"]
+            if "csv" in arrows_relationship.properties.keys()
+            else ""
+        )
+
         return cls(
             type=arrows_relationship.type,
             source=node_id_label_map[arrows_relationship.fromId],
             target=node_id_label_map[arrows_relationship.toId],
             properties=props,
-        )
+            csv_name=csv_name,
+        )
```

### Comparing `neo4j_runway-0.1.1/neo4j_runway/objects/user_input.py` & `neo4j_runway-0.2.0/neo4j_runway/objects/user_input.py`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.1.1/neo4j_runway/resources/prompts/prompts.py` & `neo4j_runway-0.2.0/neo4j_runway/resources/prompts/prompts.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,16 @@
     "retry": retry_model,
 }
 
 
 model_generation_rules = """
 Please follow these rules strictly! Billions of dollars depend on you.
 A uniqueness constraint is what makes the associated node or relationship unique.
-Each node must have one property with a unique constraint.
+A node key is a unique combination of two properties that distinguishes a node.
+Each node must have one property with a unique constraint or two properties that make a node key.
 Each node must have at least one property.
 A node must have a relationship to at least one other node.
 Property csv_mappings should be exact matches to features in the .csv file.
 A property csv_mapping should only be used once in the data model. Nodes must not share property csv_mappings.
 Nodes must not share property unique constraints.
 Include only nodes, relationships, and properties derived from features from my .csv file.
 Do not include all properties in a single Node!
@@ -37,15 +38,16 @@
 model_format = """
 Return your data model in JSON format. 
 Format properties as:
 {
     "name": <property name>,
     "type": <Python type>,
     "csv_mapping": <csv column that maps to property>,
-    "is_unique": <property has a unique constraint>
+    "is_unique": <property has a unique constraint>,
+    "part_of_key": <property is part of a node or relationship key>
 }
 Format nodes as:
 {
     "label": <node label>,
     "properties": [properties]
 }
 Format relationships as:
```

### Comparing `neo4j_runway-0.1.1/neo4j_runway/utils/naming_conventions.py` & `neo4j_runway-0.2.0/neo4j_runway/utils/naming_conventions.py`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.1.1/neo4j_runway/utils/test_connection.py` & `neo4j_runway-0.2.0/neo4j_runway/utils/test_connection.py`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.1.1/pyproject.toml` & `neo4j_runway-0.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neo4j-runway"
-version = "0.1.1"
+version = "0.2.0"
 description = "A Python library that contains tools for data discovery, data model generation and ingestion for the Neo4j graph database."
 authors = ["Alex Gilmore", "Jason Booth", "Dan Bukowski"]
 license = "MIT"
 readme = "README.md"
 keywords = ["graph", "neo4j", "data model"]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -12,27 +12,27 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: Apache Software License',
     'Programming Language :: Python',
     'Topic :: Software Development :: Libraries :: Python Modules',
     "Programming Language :: Python :: 3",
     "Topic :: Database",
 ]
-exclude = ["neo4j_runway/tests*", "images/*"]
+exclude = ["neo4j_runway/tests*", "images/*", "test.ipynb", "data/"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 graphviz = "^0.20.1"
-instructor = "^0.5.2"
+instructor = "^1.2.0"
 neo4j = "^5.19.0"
 openai = "^1.12.0"
 pandas = "^2.0.3"
 pydantic = "^2.6.1"
 pyyaml = "^6.0.1"
 numpy = "^1.26.3"
-regex= "^2022.10.31"
+regex= "~2024"
 
 
 [tool.poetry.group.dev.dependencies]
 python-dotenv = "^1.0.1"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `neo4j_runway-0.1.1/PKG-INFO` & `neo4j_runway-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo4j-runway
-Version: 0.1.1
+Version: 0.2.0
 Summary: A Python library that contains tools for data discovery, data model generation and ingestion for the Neo4j graph database.
 License: MIT
 Keywords: graph,neo4j,data model
 Author: Alex Gilmore
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -15,22 +15,22 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: graphviz (>=0.20.1,<0.21.0)
-Requires-Dist: instructor (>=0.5.2,<0.6.0)
+Requires-Dist: instructor (>=1.2.0,<2.0.0)
 Requires-Dist: neo4j (>=5.19.0,<6.0.0)
 Requires-Dist: numpy (>=1.26.3,<2.0.0)
 Requires-Dist: openai (>=1.12.0,<2.0.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: pydantic (>=2.6.1,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
-Requires-Dist: regex (>=2022.10.31,<2023.0.0)
+Requires-Dist: regex (>=2024,<2025)
 Description-Content-Type: text/markdown
 
 # Neo4j Runway
 Neo4j Runway is a Python library that simplifies the process of migrating your relational data into a graph. It provides tools that abstract communication with OpenAI to run discovery on your data and generate a data model, as well as tools to generate ingestion code and load your data into a Neo4j instance.
 
 ## Key Features
 
@@ -83,38 +83,38 @@
 ```Python
 llm = LLM()
 ```
 
 And we run discovery on our data.
 ```Python
 disc = Discovery(llm=llm, user_input=USER_GENERATED_INPUT, data=data)
-discovery = disc.run()
+disc.run()
 ```
 
 ### Data Modeling
 We can now pass our Discovery object to a GraphDataModeler to generate our initial data model. A Discovery object isn't required here, but it provides rich context to the LLM to achieve the best results.
 ```Python
 gdm = GraphDataModeler(llm=llm, discovery=disc)
 initial_model = gdm.create_initial_model()
 ```
 If we have graphviz installed, we can take a look at our model.
 ```Python
 gdm.current_model.visualize()
 ```
-![countries-first-model.svg](./images/countries-first-model.svg)
+![countries-first-model.png](./images/countries-first-model.png)
 
 Let's make some corrections to our model and view the results.
 ```Python
 gdm.iterate_model(user_corrections="""
 Make Region node have a HAS_SUBREGION relationship with Subregion node. 
 Remove The relationship between Country and Region.
 """)
 gdm.current_model.visualize()
 ```
-![countries-second-model.svg](./images/countries-second-model.svg)
+![countries-second-model.png](./images/countries-second-model.png)
 
 ### Code Generation
 We can now use our data model to generate some ingestion code.
 
 ```Python
 gen = IngestionGenerator(data_model=gdm.current_model, 
                          username="neo4j", password="password",
```

