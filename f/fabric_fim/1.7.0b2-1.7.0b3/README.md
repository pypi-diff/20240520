# Comparing `tmp/fabric_fim-1.7.0b2.tar.gz` & `tmp/fabric_fim-1.7.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric_fim-1.7.0b2.tar", last modified: Sun May 12 16:07:43 2024, max compression
+gzip compressed data, was "fabric_fim-1.7.0b3.tar", last modified: Mon May 20 21:31:27 2024, max compression
```

## Comparing `fabric_fim-1.7.0b2.tar` & `fabric_fim-1.7.0b3.tar`

### file list

```diff
@@ -1,114 +1,114 @@
--rw-r--r--   0        0        0     2208 2024-05-10 20:24:43.795008 fabric_fim-1.7.0b2/.gitignore
--rw-r--r--   0        0        0       26 2024-05-10 20:24:43.795488 fabric_fim-1.7.0b2/AUTHORS
--rw-r--r--   0        0        0     1071 2024-05-10 20:24:43.795857 fabric_fim-1.7.0b2/LICENSE
--rw-r--r--   0        0        0    11110 2024-05-10 20:24:43.796169 fabric_fim-1.7.0b2/README.md
--rw-r--r--   0        0        0    18690 2024-05-10 20:24:43.796534 fabric_fim-1.7.0b2/figs/fim-structure.png
--rw-r--r--   0        0        0      557 2024-05-10 20:24:43.796847 fabric_fim-1.7.0b2/fim/README.md
--rw-r--r--   0        0        0      105 2024-05-12 16:06:38.841363 fabric_fim-1.7.0b2/fim/__init__.py
--rw-r--r--   0        0        0        1 2024-05-10 20:24:43.797256 fabric_fim-1.7.0b2/fim/authz/__init__.py
--rw-r--r--   0        0        0    16139 2024-05-10 20:24:43.797491 fabric_fim-1.7.0b2/fim/authz/attribute_collector.py
--rw-r--r--   0        0        0      334 2024-05-10 20:24:43.797655 fabric_fim-1.7.0b2/fim/graph/README.md
--rw-r--r--   0        0        0        1 2024-05-10 20:24:43.797759 fabric_fim-1.7.0b2/fim/graph/__init__.py
--rw-r--r--   0        0        0    69847 2024-05-12 16:06:12.493690 fabric_fim-1.7.0b2/fim/graph/abc_property_graph.py
--rw-r--r--   0        0        0     4093 2024-05-10 20:24:43.798314 fabric_fim-1.7.0b2/fim/graph/abc_property_graph_constants.py
--rw-r--r--   0        0        0        1 2024-05-10 20:24:43.798489 fabric_fim-1.7.0b2/fim/graph/data/__init__.py
--rw-r--r--   0        0        0      283 2024-05-10 20:24:43.798716 fabric_fim-1.7.0b2/fim/graph/data/capacity_types.json
--rw-r--r--   0        0        0      100 2024-05-10 20:24:43.798819 fabric_fim-1.7.0b2/fim/graph/data/constraint_types.json
--rw-r--r--   0        0        0     3886 2024-05-10 20:24:43.798958 fabric_fim-1.7.0b2/fim/graph/data/graph_validation_rules.json
--rw-r--r--   0        0        0     3845 2024-05-10 20:24:43.799082 fabric_fim-1.7.0b2/fim/graph/data/graph_validation_rules_neo4j_v4.json
--rw-r--r--   0        0        0      547 2024-05-10 20:24:43.799191 fabric_fim-1.7.0b2/fim/graph/data/label_types.json
--rw-r--r--   0        0        0       91 2024-05-10 20:24:43.799336 fabric_fim-1.7.0b2/fim/graph/data/location_types.json
--rw-r--r--   0        0        0      861 2024-05-10 20:24:43.799537 fabric_fim-1.7.0b2/fim/graph/data/neo4j_indexes.json
--rw-r--r--   0        0        0     3320 2024-05-10 20:24:43.799684 fabric_fim-1.7.0b2/fim/graph/graph_util.py
--rw-r--r--   0        0        0    44293 2024-05-10 20:24:43.799917 fabric_fim-1.7.0b2/fim/graph/neo4j_property_graph.py
--rw-r--r--   0        0        0     6160 2024-05-10 20:24:43.800266 fabric_fim-1.7.0b2/fim/graph/networkx_mixin.py
--rw-r--r--   0        0        0    42211 2024-05-10 20:24:43.800923 fabric_fim-1.7.0b2/fim/graph/networkx_property_graph.py
--rw-r--r--   0        0        0     8354 2024-05-10 20:24:43.801320 fabric_fim-1.7.0b2/fim/graph/networkx_property_graph_disjoint.py
--rw-r--r--   0        0        0     1501 2024-05-10 20:24:43.801540 fabric_fim-1.7.0b2/fim/graph/resources/README.md
--rw-r--r--   0        0        0        1 2024-05-10 20:24:43.801659 fabric_fim-1.7.0b2/fim/graph/resources/__init__.py
--rw-r--r--   0        0        0     4484 2024-05-10 20:24:43.801834 fabric_fim-1.7.0b2/fim/graph/resources/abc_adm.py
--rw-r--r--   0        0        0    13570 2024-05-10 20:24:43.802071 fabric_fim-1.7.0b2/fim/graph/resources/abc_arm.py
--rw-r--r--   0        0        0     2991 2024-05-10 20:24:43.802244 fabric_fim-1.7.0b2/fim/graph/resources/abc_bqm.py
--rw-r--r--   0        0        0     5284 2024-05-10 20:24:43.802417 fabric_fim-1.7.0b2/fim/graph/resources/abc_cbm.py
--rw-r--r--   0        0        0     2297 2024-05-10 20:24:43.802620 fabric_fim-1.7.0b2/fim/graph/resources/neo4j_adm.py
--rw-r--r--   0        0        0     2106 2024-05-10 20:24:43.802756 fabric_fim-1.7.0b2/fim/graph/resources/neo4j_arm.py
--rw-r--r--   0        0        0    20998 2024-05-10 20:24:43.802902 fabric_fim-1.7.0b2/fim/graph/resources/neo4j_cbm.py
--rw-r--r--   0        0        0     5017 2024-05-10 20:24:43.803159 fabric_fim-1.7.0b2/fim/graph/resources/networkx_abqm.py
--rw-r--r--   0        0        0     2341 2024-05-10 20:24:43.803301 fabric_fim-1.7.0b2/fim/graph/resources/networkx_adm.py
--rw-r--r--   0        0        0     2122 2024-05-10 20:24:43.803584 fabric_fim-1.7.0b2/fim/graph/resources/networkx_arm.py
--rw-r--r--   0        0        0      301 2024-05-10 20:24:43.803783 fabric_fim-1.7.0b2/fim/graph/slices/README.md
--rw-r--r--   0        0        0        1 2024-05-10 20:24:43.803907 fabric_fim-1.7.0b2/fim/graph/slices/__init__.py
--rw-r--r--   0        0        0     8223 2024-05-10 20:24:43.804168 fabric_fim-1.7.0b2/fim/graph/slices/abc_asm.py
--rw-r--r--   0        0        0     3733 2024-05-10 20:24:43.804392 fabric_fim-1.7.0b2/fim/graph/slices/neo4j_asm.py
--rw-r--r--   0        0        0     4298 2024-05-10 20:24:43.804598 fabric_fim-1.7.0b2/fim/graph/slices/networkx_asm.py
--rw-r--r--   0        0        0     8615 2024-05-10 20:24:43.804937 fabric_fim-1.7.0b2/fim/graph/typed_tuples.py
--rw-r--r--   0        0        0        0 2024-05-10 20:24:43.805038 fabric_fim-1.7.0b2/fim/logging/__init__.py
--rw-r--r--   0        0        0     1526 2024-05-10 20:24:43.805280 fabric_fim-1.7.0b2/fim/logging/fim_logger.py
--rw-r--r--   0        0        0     9592 2024-05-10 20:24:43.805573 fabric_fim-1.7.0b2/fim/logging/log_collector.py
--rw-r--r--   0        0        0     9555 2024-05-10 20:24:43.805926 fabric_fim-1.7.0b2/fim/pluggable.py
--rw-r--r--   0        0        0      189 2024-05-10 20:24:43.806235 fabric_fim-1.7.0b2/fim/slivers/README.md
--rw-r--r--   0        0        0      217 2024-05-10 20:24:43.806437 fabric_fim-1.7.0b2/fim/slivers/__init__.py
--rw-r--r--   0        0        0     3641 2024-05-10 20:24:43.806672 fabric_fim-1.7.0b2/fim/slivers/attached_components.py
--rw-r--r--   0        0        0    13021 2024-05-10 20:24:43.806968 fabric_fim-1.7.0b2/fim/slivers/base_sliver.py
--rw-r--r--   0        0        0    26012 2024-05-10 20:24:43.807097 fabric_fim-1.7.0b2/fim/slivers/capacities_labels.py
--rw-r--r--   0        0        0    11537 2024-05-10 20:24:43.807400 fabric_fim-1.7.0b2/fim/slivers/component_catalog.py
--rw-r--r--   0        0        0        1 2024-05-10 20:24:43.807559 fabric_fim-1.7.0b2/fim/slivers/data/__init__.py
--rw-r--r--   0        0        0     1691 2024-05-10 20:24:43.807676 fabric_fim-1.7.0b2/fim/slivers/data/component_catalog.json
--rw-r--r--   0        0        0    77237 2024-05-10 20:24:43.807928 fabric_fim-1.7.0b2/fim/slivers/data/instance_sizes.json
--rw-r--r--   0        0        0    23524 2024-05-10 20:24:43.808314 fabric_fim-1.7.0b2/fim/slivers/delegations.py
--rw-r--r--   0        0        0     3593 2024-05-10 20:24:43.808521 fabric_fim-1.7.0b2/fim/slivers/gateway.py
--rw-r--r--   0        0        0     1193 2024-05-10 20:44:16.037631 fabric_fim-1.7.0b2/fim/slivers/identifiers.py
--rw-r--r--   0        0        0     3444 2024-05-10 20:24:43.808901 fabric_fim-1.7.0b2/fim/slivers/instance_catalog.py
--rw-r--r--   0        0        0     3225 2024-05-10 20:24:43.809015 fabric_fim-1.7.0b2/fim/slivers/interface_info.py
--rw-r--r--   0        0        0     2702 2024-05-10 20:24:43.809319 fabric_fim-1.7.0b2/fim/slivers/json.py
--rw-r--r--   0        0        0     3869 2024-05-10 20:24:43.809455 fabric_fim-1.7.0b2/fim/slivers/json_data.py
--rw-r--r--   0        0        0     5983 2024-05-10 20:24:43.809634 fabric_fim-1.7.0b2/fim/slivers/maintenance_mode.py
--rw-r--r--   0        0        0     1566 2024-05-10 20:24:43.809805 fabric_fim-1.7.0b2/fim/slivers/network_attached_storage.py
--rw-r--r--   0        0        0     3910 2024-05-10 20:24:43.809960 fabric_fim-1.7.0b2/fim/slivers/network_link.py
--rw-r--r--   0        0        0    10283 2024-05-10 20:24:43.810194 fabric_fim-1.7.0b2/fim/slivers/network_node.py
--rw-r--r--   0        0        0    22076 2024-05-10 20:24:43.810476 fabric_fim-1.7.0b2/fim/slivers/network_service.py
--rw-r--r--   0        0        0     6795 2024-05-10 20:24:43.810725 fabric_fim-1.7.0b2/fim/slivers/path_info.py
--rw-r--r--   0        0        0     3024 2024-05-10 20:24:43.811079 fabric_fim-1.7.0b2/fim/slivers/tags.py
--rw-r--r--   0        0        0     2622 2024-05-10 20:24:43.811250 fabric_fim-1.7.0b2/fim/slivers/topology_diff.py
--rw-r--r--   0        0        0     8706 2024-05-10 20:24:43.811562 fabric_fim-1.7.0b2/fim/user/README.md
--rw-r--r--   0        0        0     1914 2024-05-10 20:24:43.811680 fabric_fim-1.7.0b2/fim/user/__init__.py
--rw-r--r--   0        0        0    11730 2024-05-10 20:24:43.811887 fabric_fim-1.7.0b2/fim/user/component.py
--rw-r--r--   0        0        0     6781 2024-05-10 20:24:43.812130 fabric_fim-1.7.0b2/fim/user/composite_node.py
--rw-r--r--   0        0        0     7660 2024-05-10 20:24:43.812358 fabric_fim-1.7.0b2/fim/user/interface.py
--rw-r--r--   0        0        0     8381 2024-05-10 20:24:43.812688 fabric_fim-1.7.0b2/fim/user/link.py
--rw-r--r--   0        0        0     1219 2024-05-10 20:24:43.812907 fabric_fim-1.7.0b2/fim/user/measurement.py
--rw-r--r--   0        0        0     9668 2024-05-10 20:24:43.813172 fabric_fim-1.7.0b2/fim/user/model_element.py
--rw-r--r--   0        0        0    28472 2024-05-10 20:24:43.813369 fabric_fim-1.7.0b2/fim/user/network_service.py
--rw-r--r--   0        0        0    22636 2024-05-10 20:24:43.813557 fabric_fim-1.7.0b2/fim/user/node.py
--rw-r--r--   0        0        0    63341 2024-05-10 20:26:26.617594 fabric_fim-1.7.0b2/fim/user/topology.py
--rw-r--r--   0        0        0        2 2024-05-10 20:24:43.814024 fabric_fim-1.7.0b2/fim/util/__init__.py
--rw-r--r--   0        0        0    14680 2024-05-10 20:24:43.814211 fabric_fim-1.7.0b2/fim/util/fim_util.py
--rw-r--r--   0        0        0      595 2024-05-10 20:24:43.814379 fabric_fim-1.7.0b2/fim/view_only_dict.py
--rw-r--r--   0        0        0        0 2024-05-10 20:24:43.816925 fabric_fim-1.7.0b2/neo4j/data/.empty
--rw-r--r--   0        0        0        0 2024-05-10 20:24:43.817057 fabric_fim-1.7.0b2/neo4j/imports/.empty
--rw-r--r--   0        0        0      861 2024-05-10 20:24:43.817205 fabric_fim-1.7.0b2/pyproject.toml
--rw-r--r--   0        0        0     4632 2024-05-10 20:24:43.817434 fabric_fim-1.7.0b2/test/ad_topology_test.py
--rw-r--r--   0        0        0     4834 2024-05-10 20:24:43.817571 fabric_fim-1.7.0b2/test/after.graphml
--rw-r--r--   0        0        0    17550 2024-05-10 20:24:43.817695 fabric_fim-1.7.0b2/test/attribute_collector_test.py
--rw-r--r--   0        0        0     4696 2024-05-10 20:24:43.817868 fabric_fim-1.7.0b2/test/before.graphml
--rw-r--r--   0        0        0     2729 2024-05-10 20:24:43.818052 fabric_fim-1.7.0b2/test/catalog_test.py
--rw-r--r--   0        0        0     4319 2024-05-10 20:24:43.818232 fabric_fim-1.7.0b2/test/delegation_label_test.py
--rw-r--r--   0        0        0     1653 2024-05-10 20:24:43.818351 fabric_fim-1.7.0b2/test/maintenance_test.py
--rw-r--r--   0        0        0    51613 2024-05-10 20:24:43.818614 fabric_fim-1.7.0b2/test/models/advertised_topo.graphml
--rw-r--r--   0        0        0    49696 2024-05-10 20:24:43.818816 fabric_fim-1.7.0b2/test/models/graph-template.graphml
--rw-r--r--   0        0        0    82994 2024-05-10 20:24:43.819152 fabric_fim-1.7.0b2/test/models/network-am-ad.graphml
--rw-r--r--   0        0        0    57411 2024-05-10 20:24:43.819362 fabric_fim-1.7.0b2/test/models/site-2-am-1broker-ad.graphml
--rw-r--r--   0        0        0    52887 2024-05-10 20:24:43.819564 fabric_fim-1.7.0b2/test/models/site-3-am-1broker-ad.graphml
--rw-r--r--   0        0        0   131407 2024-05-10 20:24:43.819871 fabric_fim-1.7.0b2/test/models/site-am-2broker-ad.graphml
--rw-r--r--   0        0        0    18708 2024-05-10 20:24:43.820055 fabric_fim-1.7.0b2/test/modify_test.py
--rw-r--r--   0        0        0    13135 2024-05-10 20:24:43.820298 fabric_fim-1.7.0b2/test/networkxx_pg_disjoint_test.py
--rw-r--r--   0        0        0    14091 2024-05-10 20:24:43.820588 fabric_fim-1.7.0b2/test/networkxx_pg_test.py
--rw-r--r--   0        0        0     2572 2024-05-10 20:24:43.820714 fabric_fim-1.7.0b2/test/pluggable_test.py
--rw-r--r--   0        0        0    48631 2024-05-10 20:26:50.309360 fabric_fim-1.7.0b2/test/slice_topology_test.py
--rw-r--r--   0        0        0     1869 2024-05-10 20:24:43.821046 fabric_fim-1.7.0b2/test/sliver_json_test.py
--rw-r--r--   0        0        0     6030 2024-05-10 20:24:43.821189 fabric_fim-1.7.0b2/test/sliver_test.py
--rw-r--r--   0        0        0    98404 2024-05-10 20:27:01.881851 fabric_fim-1.7.0b2/test/substrate_topology_test.py
--rw-r--r--   0        0        0      654 2024-05-10 20:24:43.821690 fabric_fim-1.7.0b2/test/test_load.py
--rw-r--r--   0        0        0     2362 2024-05-10 20:24:43.821803 fabric_fim-1.7.0b2/test/tuple_test.py
--rw-r--r--   0        0        0    15663 2024-05-11 02:39:28.968543 fabric_fim-1.7.0b2/test/zz_neo4j_pg_test.py
--rw-r--r--   0        0        0    11890 1970-01-01 00:00:00.000000 fabric_fim-1.7.0b2/PKG-INFO
+-rw-r--r--   0        0        0     2208 2024-05-10 20:24:43.795008 fabric_fim-1.7.0b3/.gitignore
+-rw-r--r--   0        0        0       26 2024-05-10 20:24:43.795488 fabric_fim-1.7.0b3/AUTHORS
+-rw-r--r--   0        0        0     1071 2024-05-10 20:24:43.795857 fabric_fim-1.7.0b3/LICENSE
+-rw-r--r--   0        0        0    11110 2024-05-10 20:24:43.796169 fabric_fim-1.7.0b3/README.md
+-rw-r--r--   0        0        0    18690 2024-05-10 20:24:43.796534 fabric_fim-1.7.0b3/figs/fim-structure.png
+-rw-r--r--   0        0        0      557 2024-05-10 20:24:43.796847 fabric_fim-1.7.0b3/fim/README.md
+-rw-r--r--   0        0        0      105 2024-05-20 21:31:08.393928 fabric_fim-1.7.0b3/fim/__init__.py
+-rw-r--r--   0        0        0        1 2024-05-10 20:24:43.797256 fabric_fim-1.7.0b3/fim/authz/__init__.py
+-rw-r--r--   0        0        0    16139 2024-05-10 20:24:43.797491 fabric_fim-1.7.0b3/fim/authz/attribute_collector.py
+-rw-r--r--   0        0        0      334 2024-05-10 20:24:43.797655 fabric_fim-1.7.0b3/fim/graph/README.md
+-rw-r--r--   0        0        0        1 2024-05-10 20:24:43.797759 fabric_fim-1.7.0b3/fim/graph/__init__.py
+-rw-r--r--   0        0        0    69847 2024-05-12 16:06:12.493690 fabric_fim-1.7.0b3/fim/graph/abc_property_graph.py
+-rw-r--r--   0        0        0     4093 2024-05-10 20:24:43.798314 fabric_fim-1.7.0b3/fim/graph/abc_property_graph_constants.py
+-rw-r--r--   0        0        0        1 2024-05-10 20:24:43.798489 fabric_fim-1.7.0b3/fim/graph/data/__init__.py
+-rw-r--r--   0        0        0      283 2024-05-10 20:24:43.798716 fabric_fim-1.7.0b3/fim/graph/data/capacity_types.json
+-rw-r--r--   0        0        0      100 2024-05-10 20:24:43.798819 fabric_fim-1.7.0b3/fim/graph/data/constraint_types.json
+-rw-r--r--   0        0        0     3886 2024-05-10 20:24:43.798958 fabric_fim-1.7.0b3/fim/graph/data/graph_validation_rules.json
+-rw-r--r--   0        0        0     3845 2024-05-10 20:24:43.799082 fabric_fim-1.7.0b3/fim/graph/data/graph_validation_rules_neo4j_v4.json
+-rw-r--r--   0        0        0      547 2024-05-10 20:24:43.799191 fabric_fim-1.7.0b3/fim/graph/data/label_types.json
+-rw-r--r--   0        0        0       91 2024-05-10 20:24:43.799336 fabric_fim-1.7.0b3/fim/graph/data/location_types.json
+-rw-r--r--   0        0        0      861 2024-05-10 20:24:43.799537 fabric_fim-1.7.0b3/fim/graph/data/neo4j_indexes.json
+-rw-r--r--   0        0        0     3320 2024-05-10 20:24:43.799684 fabric_fim-1.7.0b3/fim/graph/graph_util.py
+-rw-r--r--   0        0        0    44293 2024-05-10 20:24:43.799917 fabric_fim-1.7.0b3/fim/graph/neo4j_property_graph.py
+-rw-r--r--   0        0        0     6160 2024-05-10 20:24:43.800266 fabric_fim-1.7.0b3/fim/graph/networkx_mixin.py
+-rw-r--r--   0        0        0    42211 2024-05-10 20:24:43.800923 fabric_fim-1.7.0b3/fim/graph/networkx_property_graph.py
+-rw-r--r--   0        0        0     8354 2024-05-10 20:24:43.801320 fabric_fim-1.7.0b3/fim/graph/networkx_property_graph_disjoint.py
+-rw-r--r--   0        0        0     1501 2024-05-10 20:24:43.801540 fabric_fim-1.7.0b3/fim/graph/resources/README.md
+-rw-r--r--   0        0        0        1 2024-05-10 20:24:43.801659 fabric_fim-1.7.0b3/fim/graph/resources/__init__.py
+-rw-r--r--   0        0        0     4484 2024-05-10 20:24:43.801834 fabric_fim-1.7.0b3/fim/graph/resources/abc_adm.py
+-rw-r--r--   0        0        0    13570 2024-05-10 20:24:43.802071 fabric_fim-1.7.0b3/fim/graph/resources/abc_arm.py
+-rw-r--r--   0        0        0     2991 2024-05-10 20:24:43.802244 fabric_fim-1.7.0b3/fim/graph/resources/abc_bqm.py
+-rw-r--r--   0        0        0     5284 2024-05-10 20:24:43.802417 fabric_fim-1.7.0b3/fim/graph/resources/abc_cbm.py
+-rw-r--r--   0        0        0     2297 2024-05-10 20:24:43.802620 fabric_fim-1.7.0b3/fim/graph/resources/neo4j_adm.py
+-rw-r--r--   0        0        0     2106 2024-05-10 20:24:43.802756 fabric_fim-1.7.0b3/fim/graph/resources/neo4j_arm.py
+-rw-r--r--   0        0        0    20998 2024-05-10 20:24:43.802902 fabric_fim-1.7.0b3/fim/graph/resources/neo4j_cbm.py
+-rw-r--r--   0        0        0     5017 2024-05-10 20:24:43.803159 fabric_fim-1.7.0b3/fim/graph/resources/networkx_abqm.py
+-rw-r--r--   0        0        0     2341 2024-05-10 20:24:43.803301 fabric_fim-1.7.0b3/fim/graph/resources/networkx_adm.py
+-rw-r--r--   0        0        0     2122 2024-05-10 20:24:43.803584 fabric_fim-1.7.0b3/fim/graph/resources/networkx_arm.py
+-rw-r--r--   0        0        0      301 2024-05-10 20:24:43.803783 fabric_fim-1.7.0b3/fim/graph/slices/README.md
+-rw-r--r--   0        0        0        1 2024-05-10 20:24:43.803907 fabric_fim-1.7.0b3/fim/graph/slices/__init__.py
+-rw-r--r--   0        0        0     8223 2024-05-10 20:24:43.804168 fabric_fim-1.7.0b3/fim/graph/slices/abc_asm.py
+-rw-r--r--   0        0        0     3733 2024-05-10 20:24:43.804392 fabric_fim-1.7.0b3/fim/graph/slices/neo4j_asm.py
+-rw-r--r--   0        0        0     4298 2024-05-10 20:24:43.804598 fabric_fim-1.7.0b3/fim/graph/slices/networkx_asm.py
+-rw-r--r--   0        0        0     8615 2024-05-10 20:24:43.804937 fabric_fim-1.7.0b3/fim/graph/typed_tuples.py
+-rw-r--r--   0        0        0        0 2024-05-10 20:24:43.805038 fabric_fim-1.7.0b3/fim/logging/__init__.py
+-rw-r--r--   0        0        0     1526 2024-05-10 20:24:43.805280 fabric_fim-1.7.0b3/fim/logging/fim_logger.py
+-rw-r--r--   0        0        0     9592 2024-05-10 20:24:43.805573 fabric_fim-1.7.0b3/fim/logging/log_collector.py
+-rw-r--r--   0        0        0     9555 2024-05-10 20:24:43.805926 fabric_fim-1.7.0b3/fim/pluggable.py
+-rw-r--r--   0        0        0      189 2024-05-10 20:24:43.806235 fabric_fim-1.7.0b3/fim/slivers/README.md
+-rw-r--r--   0        0        0      217 2024-05-10 20:24:43.806437 fabric_fim-1.7.0b3/fim/slivers/__init__.py
+-rw-r--r--   0        0        0     3641 2024-05-10 20:24:43.806672 fabric_fim-1.7.0b3/fim/slivers/attached_components.py
+-rw-r--r--   0        0        0    13021 2024-05-10 20:24:43.806968 fabric_fim-1.7.0b3/fim/slivers/base_sliver.py
+-rw-r--r--   0        0        0    26210 2024-05-20 21:29:56.026701 fabric_fim-1.7.0b3/fim/slivers/capacities_labels.py
+-rw-r--r--   0        0        0    11537 2024-05-10 20:24:43.807400 fabric_fim-1.7.0b3/fim/slivers/component_catalog.py
+-rw-r--r--   0        0        0        1 2024-05-10 20:24:43.807559 fabric_fim-1.7.0b3/fim/slivers/data/__init__.py
+-rw-r--r--   0        0        0     1691 2024-05-10 20:24:43.807676 fabric_fim-1.7.0b3/fim/slivers/data/component_catalog.json
+-rw-r--r--   0        0        0    77237 2024-05-10 20:24:43.807928 fabric_fim-1.7.0b3/fim/slivers/data/instance_sizes.json
+-rw-r--r--   0        0        0    23524 2024-05-10 20:24:43.808314 fabric_fim-1.7.0b3/fim/slivers/delegations.py
+-rw-r--r--   0        0        0     3593 2024-05-10 20:24:43.808521 fabric_fim-1.7.0b3/fim/slivers/gateway.py
+-rw-r--r--   0        0        0     1193 2024-05-10 20:44:16.037631 fabric_fim-1.7.0b3/fim/slivers/identifiers.py
+-rw-r--r--   0        0        0     3444 2024-05-10 20:24:43.808901 fabric_fim-1.7.0b3/fim/slivers/instance_catalog.py
+-rw-r--r--   0        0        0     3225 2024-05-10 20:24:43.809015 fabric_fim-1.7.0b3/fim/slivers/interface_info.py
+-rw-r--r--   0        0        0     2702 2024-05-10 20:24:43.809319 fabric_fim-1.7.0b3/fim/slivers/json.py
+-rw-r--r--   0        0        0     3869 2024-05-10 20:24:43.809455 fabric_fim-1.7.0b3/fim/slivers/json_data.py
+-rw-r--r--   0        0        0     5983 2024-05-10 20:24:43.809634 fabric_fim-1.7.0b3/fim/slivers/maintenance_mode.py
+-rw-r--r--   0        0        0     1566 2024-05-10 20:24:43.809805 fabric_fim-1.7.0b3/fim/slivers/network_attached_storage.py
+-rw-r--r--   0        0        0     3910 2024-05-10 20:24:43.809960 fabric_fim-1.7.0b3/fim/slivers/network_link.py
+-rw-r--r--   0        0        0    10283 2024-05-10 20:24:43.810194 fabric_fim-1.7.0b3/fim/slivers/network_node.py
+-rw-r--r--   0        0        0    22076 2024-05-10 20:24:43.810476 fabric_fim-1.7.0b3/fim/slivers/network_service.py
+-rw-r--r--   0        0        0     6795 2024-05-10 20:24:43.810725 fabric_fim-1.7.0b3/fim/slivers/path_info.py
+-rw-r--r--   0        0        0     3024 2024-05-10 20:24:43.811079 fabric_fim-1.7.0b3/fim/slivers/tags.py
+-rw-r--r--   0        0        0     2622 2024-05-10 20:24:43.811250 fabric_fim-1.7.0b3/fim/slivers/topology_diff.py
+-rw-r--r--   0        0        0     8706 2024-05-10 20:24:43.811562 fabric_fim-1.7.0b3/fim/user/README.md
+-rw-r--r--   0        0        0     1914 2024-05-10 20:24:43.811680 fabric_fim-1.7.0b3/fim/user/__init__.py
+-rw-r--r--   0        0        0    11730 2024-05-10 20:24:43.811887 fabric_fim-1.7.0b3/fim/user/component.py
+-rw-r--r--   0        0        0     6781 2024-05-10 20:24:43.812130 fabric_fim-1.7.0b3/fim/user/composite_node.py
+-rw-r--r--   0        0        0     7660 2024-05-10 20:24:43.812358 fabric_fim-1.7.0b3/fim/user/interface.py
+-rw-r--r--   0        0        0     8381 2024-05-10 20:24:43.812688 fabric_fim-1.7.0b3/fim/user/link.py
+-rw-r--r--   0        0        0     1219 2024-05-10 20:24:43.812907 fabric_fim-1.7.0b3/fim/user/measurement.py
+-rw-r--r--   0        0        0     9668 2024-05-10 20:24:43.813172 fabric_fim-1.7.0b3/fim/user/model_element.py
+-rw-r--r--   0        0        0    28472 2024-05-10 20:24:43.813369 fabric_fim-1.7.0b3/fim/user/network_service.py
+-rw-r--r--   0        0        0    22636 2024-05-10 20:24:43.813557 fabric_fim-1.7.0b3/fim/user/node.py
+-rw-r--r--   0        0        0    63341 2024-05-10 20:26:26.617594 fabric_fim-1.7.0b3/fim/user/topology.py
+-rw-r--r--   0        0        0        2 2024-05-10 20:24:43.814024 fabric_fim-1.7.0b3/fim/util/__init__.py
+-rw-r--r--   0        0        0    14680 2024-05-10 20:24:43.814211 fabric_fim-1.7.0b3/fim/util/fim_util.py
+-rw-r--r--   0        0        0      595 2024-05-10 20:24:43.814379 fabric_fim-1.7.0b3/fim/view_only_dict.py
+-rw-r--r--   0        0        0        0 2024-05-10 20:24:43.816925 fabric_fim-1.7.0b3/neo4j/data/.empty
+-rw-r--r--   0        0        0        0 2024-05-10 20:24:43.817057 fabric_fim-1.7.0b3/neo4j/imports/.empty
+-rw-r--r--   0        0        0      861 2024-05-10 20:24:43.817205 fabric_fim-1.7.0b3/pyproject.toml
+-rw-r--r--   0        0        0     4632 2024-05-10 20:24:43.817434 fabric_fim-1.7.0b3/test/ad_topology_test.py
+-rw-r--r--   0        0        0     4834 2024-05-10 20:24:43.817571 fabric_fim-1.7.0b3/test/after.graphml
+-rw-r--r--   0        0        0    17550 2024-05-10 20:24:43.817695 fabric_fim-1.7.0b3/test/attribute_collector_test.py
+-rw-r--r--   0        0        0     4696 2024-05-10 20:24:43.817868 fabric_fim-1.7.0b3/test/before.graphml
+-rw-r--r--   0        0        0     2729 2024-05-10 20:24:43.818052 fabric_fim-1.7.0b3/test/catalog_test.py
+-rw-r--r--   0        0        0     4319 2024-05-10 20:24:43.818232 fabric_fim-1.7.0b3/test/delegation_label_test.py
+-rw-r--r--   0        0        0     1653 2024-05-10 20:24:43.818351 fabric_fim-1.7.0b3/test/maintenance_test.py
+-rw-r--r--   0        0        0    51613 2024-05-10 20:24:43.818614 fabric_fim-1.7.0b3/test/models/advertised_topo.graphml
+-rw-r--r--   0        0        0    49696 2024-05-10 20:24:43.818816 fabric_fim-1.7.0b3/test/models/graph-template.graphml
+-rw-r--r--   0        0        0    82994 2024-05-10 20:24:43.819152 fabric_fim-1.7.0b3/test/models/network-am-ad.graphml
+-rw-r--r--   0        0        0    57411 2024-05-10 20:24:43.819362 fabric_fim-1.7.0b3/test/models/site-2-am-1broker-ad.graphml
+-rw-r--r--   0        0        0    52887 2024-05-10 20:24:43.819564 fabric_fim-1.7.0b3/test/models/site-3-am-1broker-ad.graphml
+-rw-r--r--   0        0        0   131407 2024-05-10 20:24:43.819871 fabric_fim-1.7.0b3/test/models/site-am-2broker-ad.graphml
+-rw-r--r--   0        0        0    18708 2024-05-10 20:24:43.820055 fabric_fim-1.7.0b3/test/modify_test.py
+-rw-r--r--   0        0        0    13135 2024-05-10 20:24:43.820298 fabric_fim-1.7.0b3/test/networkxx_pg_disjoint_test.py
+-rw-r--r--   0        0        0    14091 2024-05-10 20:24:43.820588 fabric_fim-1.7.0b3/test/networkxx_pg_test.py
+-rw-r--r--   0        0        0     2572 2024-05-10 20:24:43.820714 fabric_fim-1.7.0b3/test/pluggable_test.py
+-rw-r--r--   0        0        0    48631 2024-05-10 20:26:50.309360 fabric_fim-1.7.0b3/test/slice_topology_test.py
+-rw-r--r--   0        0        0     1869 2024-05-10 20:24:43.821046 fabric_fim-1.7.0b3/test/sliver_json_test.py
+-rw-r--r--   0        0        0     6030 2024-05-10 20:24:43.821189 fabric_fim-1.7.0b3/test/sliver_test.py
+-rw-r--r--   0        0        0    98404 2024-05-10 20:27:01.881851 fabric_fim-1.7.0b3/test/substrate_topology_test.py
+-rw-r--r--   0        0        0      654 2024-05-10 20:24:43.821690 fabric_fim-1.7.0b3/test/test_load.py
+-rw-r--r--   0        0        0     2362 2024-05-10 20:24:43.821803 fabric_fim-1.7.0b3/test/tuple_test.py
+-rw-r--r--   0        0        0    15663 2024-05-11 02:39:28.968543 fabric_fim-1.7.0b3/test/zz_neo4j_pg_test.py
+-rw-r--r--   0        0        0    11890 1970-01-01 00:00:00.000000 fabric_fim-1.7.0b3/PKG-INFO
```

### Comparing `fabric_fim-1.7.0b2/.gitignore` & `fabric_fim-1.7.0b3/.gitignore`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/LICENSE` & `fabric_fim-1.7.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/README.md` & `fabric_fim-1.7.0b3/README.md`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/figs/fim-structure.png` & `fabric_fim-1.7.0b3/figs/fim-structure.png`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/README.md` & `fabric_fim-1.7.0b3/fim/README.md`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/authz/attribute_collector.py` & `fabric_fim-1.7.0b3/fim/authz/attribute_collector.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/graph/abc_property_graph.py` & `fabric_fim-1.7.0b3/fim/graph/abc_property_graph.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/graph/abc_property_graph_constants.py` & `fabric_fim-1.7.0b3/fim/graph/abc_property_graph_constants.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/graph/data/graph_validation_rules.json` & `fabric_fim-1.7.0b3/fim/graph/data/graph_validation_rules.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/graph/data/graph_validation_rules_neo4j_v4.json` & `fabric_fim-1.7.0b3/fim/graph/data/graph_validation_rules_neo4j_v4.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/graph/data/label_types.json` & `fabric_fim-1.7.0b3/fim/graph/data/label_types.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/graph/data/neo4j_indexes.json` & `fabric_fim-1.7.0b3/fim/graph/data/neo4j_indexes.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/graph/graph_util.py` & `fabric_fim-1.7.0b3/fim/graph/graph_util.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/graph/neo4j_property_graph.py` & `fabric_fim-1.7.0b3/fim/graph/neo4j_property_graph.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/graph/networkx_mixin.py` & `fabric_fim-1.7.0b3/fim/graph/networkx_mixin.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/graph/networkx_property_graph.py` & `fabric_fim-1.7.0b3/fim/graph/networkx_property_graph.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/graph/networkx_property_graph_disjoint.py` & `fabric_fim-1.7.0b3/fim/graph/networkx_property_graph_disjoint.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/graph/resources/README.md` & `fabric_fim-1.7.0b3/fim/graph/resources/README.md`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/graph/resources/abc_adm.py` & `fabric_fim-1.7.0b3/fim/graph/resources/abc_adm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/graph/resources/abc_arm.py` & `fabric_fim-1.7.0b3/fim/graph/resources/abc_arm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/graph/resources/abc_bqm.py` & `fabric_fim-1.7.0b3/fim/graph/resources/abc_bqm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/graph/resources/abc_cbm.py` & `fabric_fim-1.7.0b3/fim/graph/resources/abc_cbm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/graph/resources/neo4j_adm.py` & `fabric_fim-1.7.0b3/fim/graph/resources/neo4j_adm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/graph/resources/neo4j_arm.py` & `fabric_fim-1.7.0b3/fim/graph/resources/neo4j_arm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/graph/resources/neo4j_cbm.py` & `fabric_fim-1.7.0b3/fim/graph/resources/neo4j_cbm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/graph/resources/networkx_abqm.py` & `fabric_fim-1.7.0b3/fim/graph/resources/networkx_abqm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/graph/resources/networkx_adm.py` & `fabric_fim-1.7.0b3/fim/graph/resources/networkx_adm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/graph/resources/networkx_arm.py` & `fabric_fim-1.7.0b3/fim/graph/resources/networkx_arm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/graph/slices/abc_asm.py` & `fabric_fim-1.7.0b3/fim/graph/slices/abc_asm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/graph/slices/neo4j_asm.py` & `fabric_fim-1.7.0b3/fim/graph/slices/neo4j_asm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/graph/slices/networkx_asm.py` & `fabric_fim-1.7.0b3/fim/graph/slices/networkx_asm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/graph/typed_tuples.py` & `fabric_fim-1.7.0b3/fim/graph/typed_tuples.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/logging/fim_logger.py` & `fabric_fim-1.7.0b3/fim/logging/fim_logger.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/logging/log_collector.py` & `fabric_fim-1.7.0b3/fim/logging/log_collector.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/pluggable.py` & `fabric_fim-1.7.0b3/fim/pluggable.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/slivers/attached_components.py` & `fabric_fim-1.7.0b3/fim/slivers/attached_components.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/slivers/base_sliver.py` & `fabric_fim-1.7.0b3/fim/slivers/base_sliver.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/slivers/capacities_labels.py` & `fabric_fim-1.7.0b3/fim/slivers/capacities_labels.py`

 * *Files 1% similar despite different names*

```diff
@@ -563,25 +563,27 @@
 
 class Location(JSONField):
     """
     Location representation (as address, coordinates or any other useful way)
     """
     def __init__(self, **kwargs):
         self.postal = None
+        self.lat = None
+        self.lon = None
         self._set_fields(**kwargs)
 
     def _set_fields(self, forgiving=False, **kwargs):
         """
         Universal setter for location fields. Values are strings.
         :param kwargs:
         :return:
         """
         for k, v in kwargs.items():
             assert v is not None
-            assert isinstance(v, str)
+            assert isinstance(v, str) or isinstance(v, float)
             try:
                 # will throw exception if field is not defined
                 self.__getattribute__(k)
                 self.__setattr__(k, v)
             except AttributeError:
                 report = f"Unable to set field {k} of location, no such field available"
                 if forgiving:
@@ -592,31 +594,35 @@
 
     def to_latlon(self) -> Tuple[float, float]:
         """
         Return a tuple of floats indicating Lat/Lon of the location. Uses Nomatim OpenStreetMaps
         service.
         :return:
         """
+        if self.lat and self.lon:
+            return self.lat, self.lon
         url = 'https://nominatim.openstreetmap.org/search?q=' + urllib.parse.quote(self.postal) + '&format=json'
         # per terms of service set user agent
-        headers = {'User-Agent': 'FABRIC FIM Utility'}
+        headers = {'User-Agent': 'FABRIC FIM Utility v2'}
         response = requests.get(url, headers)
         if response.status_code != 200:
             raise LocationException(f"Unable to convert address to Lat/Lon via OpenStreetmaps due "
                                     f"to: {response.reason}")
         try:
             response_json = response.json()
             if not isinstance(response_json, list):
                 raise ValueError
             if len(response_json) < 1:
                 raise ValueError
         except ValueError:
             raise LocationException(f"Unable to interpret response from OpenStreetmaps for address {self.postal}")
 
-        return float(response_json[0]['lat']), float(response_json[0]['lon'])
+        self.lat = float(response_json[0]['lat'])
+        self.lon = (response_json[0]['lon'])
+        return self.lat, self.lon
 
 
 class Flags(JSONField):
     """
     JSON-ified representation of various flags that can be attached to slivers
     """
     def __init__(self, **kwargs):
```

### Comparing `fabric_fim-1.7.0b2/fim/slivers/component_catalog.py` & `fabric_fim-1.7.0b3/fim/slivers/component_catalog.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/slivers/data/component_catalog.json` & `fabric_fim-1.7.0b3/fim/slivers/data/component_catalog.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/slivers/data/instance_sizes.json` & `fabric_fim-1.7.0b3/fim/slivers/data/instance_sizes.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/slivers/delegations.py` & `fabric_fim-1.7.0b3/fim/slivers/delegations.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/slivers/gateway.py` & `fabric_fim-1.7.0b3/fim/slivers/gateway.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/slivers/identifiers.py` & `fabric_fim-1.7.0b3/fim/slivers/identifiers.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/slivers/instance_catalog.py` & `fabric_fim-1.7.0b3/fim/slivers/instance_catalog.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/slivers/interface_info.py` & `fabric_fim-1.7.0b3/fim/slivers/interface_info.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/slivers/json.py` & `fabric_fim-1.7.0b3/fim/slivers/json.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/slivers/json_data.py` & `fabric_fim-1.7.0b3/fim/slivers/json_data.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/slivers/maintenance_mode.py` & `fabric_fim-1.7.0b3/fim/slivers/maintenance_mode.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/slivers/network_attached_storage.py` & `fabric_fim-1.7.0b3/fim/slivers/network_attached_storage.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/slivers/network_link.py` & `fabric_fim-1.7.0b3/fim/slivers/network_link.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/slivers/network_node.py` & `fabric_fim-1.7.0b3/fim/slivers/network_node.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/slivers/network_service.py` & `fabric_fim-1.7.0b3/fim/slivers/network_service.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/slivers/path_info.py` & `fabric_fim-1.7.0b3/fim/slivers/path_info.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/slivers/tags.py` & `fabric_fim-1.7.0b3/fim/slivers/tags.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/slivers/topology_diff.py` & `fabric_fim-1.7.0b3/fim/slivers/topology_diff.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/user/README.md` & `fabric_fim-1.7.0b3/fim/user/README.md`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/user/__init__.py` & `fabric_fim-1.7.0b3/fim/user/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/user/component.py` & `fabric_fim-1.7.0b3/fim/user/component.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/user/composite_node.py` & `fabric_fim-1.7.0b3/fim/user/composite_node.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/user/interface.py` & `fabric_fim-1.7.0b3/fim/user/interface.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/user/link.py` & `fabric_fim-1.7.0b3/fim/user/link.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/user/measurement.py` & `fabric_fim-1.7.0b3/fim/user/measurement.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/user/model_element.py` & `fabric_fim-1.7.0b3/fim/user/model_element.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/user/network_service.py` & `fabric_fim-1.7.0b3/fim/user/network_service.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/user/node.py` & `fabric_fim-1.7.0b3/fim/user/node.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/user/topology.py` & `fabric_fim-1.7.0b3/fim/user/topology.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/util/fim_util.py` & `fabric_fim-1.7.0b3/fim/util/fim_util.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/fim/view_only_dict.py` & `fabric_fim-1.7.0b3/fim/view_only_dict.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/pyproject.toml` & `fabric_fim-1.7.0b3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/test/ad_topology_test.py` & `fabric_fim-1.7.0b3/test/ad_topology_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/test/after.graphml` & `fabric_fim-1.7.0b3/test/after.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/test/attribute_collector_test.py` & `fabric_fim-1.7.0b3/test/attribute_collector_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/test/before.graphml` & `fabric_fim-1.7.0b3/test/before.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/test/catalog_test.py` & `fabric_fim-1.7.0b3/test/catalog_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/test/delegation_label_test.py` & `fabric_fim-1.7.0b3/test/delegation_label_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/test/maintenance_test.py` & `fabric_fim-1.7.0b3/test/maintenance_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/test/models/advertised_topo.graphml` & `fabric_fim-1.7.0b3/test/models/advertised_topo.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/test/models/graph-template.graphml` & `fabric_fim-1.7.0b3/test/models/graph-template.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/test/models/network-am-ad.graphml` & `fabric_fim-1.7.0b3/test/models/network-am-ad.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/test/models/site-2-am-1broker-ad.graphml` & `fabric_fim-1.7.0b3/test/models/site-2-am-1broker-ad.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/test/models/site-3-am-1broker-ad.graphml` & `fabric_fim-1.7.0b3/test/models/site-3-am-1broker-ad.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/test/models/site-am-2broker-ad.graphml` & `fabric_fim-1.7.0b3/test/models/site-am-2broker-ad.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/test/modify_test.py` & `fabric_fim-1.7.0b3/test/modify_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/test/networkxx_pg_disjoint_test.py` & `fabric_fim-1.7.0b3/test/networkxx_pg_disjoint_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/test/networkxx_pg_test.py` & `fabric_fim-1.7.0b3/test/networkxx_pg_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/test/pluggable_test.py` & `fabric_fim-1.7.0b3/test/pluggable_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/test/slice_topology_test.py` & `fabric_fim-1.7.0b3/test/slice_topology_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/test/sliver_json_test.py` & `fabric_fim-1.7.0b3/test/sliver_json_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/test/sliver_test.py` & `fabric_fim-1.7.0b3/test/sliver_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/test/substrate_topology_test.py` & `fabric_fim-1.7.0b3/test/substrate_topology_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/test/test_load.py` & `fabric_fim-1.7.0b3/test/test_load.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/test/tuple_test.py` & `fabric_fim-1.7.0b3/test/tuple_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/test/zz_neo4j_pg_test.py` & `fabric_fim-1.7.0b3/test/zz_neo4j_pg_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.7.0b2/PKG-INFO` & `fabric_fim-1.7.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric_fim
-Version: 1.7.0b2
+Version: 1.7.0b3
 Summary: FABRIC Information Model library and utilities
 Keywords: Neo4j
 Author-email: Ilya Baldin <ibaldin@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

