# Comparing `tmp/aiida_workgraph-0.2.4.tar.gz` & `tmp/aiida_workgraph-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida_workgraph-0.2.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiida_workgraph-0.2.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiida_workgraph-0.2.4.tar` & `aiida_workgraph-0.2.5.tar`

### file list

```diff
@@ -1,119 +1,123 @@
--rw-r--r--   0        0        0     1066 2023-12-11 16:36:18.395013 aiida_workgraph-0.2.4/LICENSE
--rw-r--r--   0        0        0     5318 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.4/README.md
--rw-r--r--   0        0        0      175 2024-05-15 13:46:15.010509 aiida_workgraph-0.2.4/aiida_workgraph/__init__.py
--rw-r--r--   0        0        0      279 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/cli/__init__.py
--rw-r--r--   0        0        0    12112 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/cli/cmd_graph.py
--rw-r--r--   0        0        0     1937 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/cli/cmd_web.py
--rw-r--r--   0        0        0      714 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/cli/cmd_workgraph.py
--rw-r--r--   0        0        0     6587 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/cli/query_workgraph.py
--rw-r--r--   0        0        0     2342 2024-05-07 20:56:57.572283 aiida_workgraph-0.2.4/aiida_workgraph/collection.py
--rw-r--r--   0        0        0    17099 2024-05-15 13:45:10.407702 aiida_workgraph-0.2.4/aiida_workgraph/decorator.py
--rw-r--r--   0        0        0        0 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/engine/__init__.py
--rw-r--r--   0        0        0    47604 2024-05-14 15:37:34.242235 aiida_workgraph-0.2.4/aiida_workgraph/engine/workgraph.py
--rw-r--r--   0        0        0        0 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/executors/__init__.py
--rw-r--r--   0        0        0      897 2024-05-07 20:56:57.572283 aiida_workgraph-0.2.4/aiida_workgraph/executors/builtin.py
--rw-r--r--   0        0        0      740 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.4/aiida_workgraph/executors/qe.py
--rw-r--r--   0        0        0      768 2024-05-07 20:56:57.572283 aiida_workgraph-0.2.4/aiida_workgraph/executors/test.py
--rw-r--r--   0        0        0     4151 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.4/aiida_workgraph/node.py
--rw-r--r--   0        0        0      847 2024-05-15 13:45:10.407702 aiida_workgraph-0.2.4/aiida_workgraph/nodes/__init__.py
--rw-r--r--   0        0        0     3957 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.4/aiida_workgraph/nodes/builtin.py
--rw-r--r--   0        0        0     2168 2024-05-15 13:45:10.407702 aiida_workgraph-0.2.4/aiida_workgraph/nodes/qe.py
--rw-r--r--   0        0        0     7233 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.4/aiida_workgraph/nodes/test.py
--rw-r--r--   0        0        0     1214 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/orm/worktree.py
--rw-r--r--   0        0        0      115 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/properties/__init__.py
--rw-r--r--   0        0        0    10647 2024-05-15 13:45:10.407702 aiida_workgraph-0.2.4/aiida_workgraph/properties/built_in.py
--rw-r--r--   0        0        0     2131 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.4/aiida_workgraph/property.py
--rw-r--r--   0        0        0     1386 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.4/aiida_workgraph/socket.py
--rw-r--r--   0        0        0      111 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/sockets/__init__.py
--rw-r--r--   0        0        0     3760 2024-05-15 13:45:10.407702 aiida_workgraph-0.2.4/aiida_workgraph/sockets/built_in.py
--rw-r--r--   0        0        0     7824 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.4/aiida_workgraph/utils/__init__.py
--rw-r--r--   0        0        0     6132 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.4/aiida_workgraph/utils/analysis.py
--rw-r--r--   0        0        0     1754 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.4/aiida_workgraph/utils/graph.py
--rw-r--r--   0        0        0      763 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/web/README.md
--rw-r--r--   0        0        0        0 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/web/backend/app/__init__.py
--rw-r--r--   0        0        0     2395 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/web/backend/app/api.py
--rw-r--r--   0        0        0     3638 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/web/backend/app/daemon.py
--rw-r--r--   0        0        0     2208 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.4/aiida_workgraph/web/backend/app/datanode.py
--rw-r--r--   0        0        0     6618 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.4/aiida_workgraph/web/backend/app/utils.py
--rw-r--r--   0        0        0     5130 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/web/backend/app/workgraph.py
--rw-r--r--   0        0        0      115 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/web/backend/main.py
--rw-r--r--   0        0        0      310 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/.gitignore
--rw-r--r--   0        0        0       62 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/.rete-patch
--rw-r--r--   0        0        0     2136 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/README.md
--rw-r--r--   0        0        0      517 2024-05-07 20:57:48.891725 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/asset-manifest.json
--rw-r--r--   0        0        0     3870 2024-05-07 20:57:23.435997 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/favicon.ico
--rw-r--r--   0        0        0      654 2024-05-07 20:57:48.891725 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/index.html
--rw-r--r--   0        0        0      306 2024-05-07 20:57:23.439997 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/manifest.json
--rw-r--r--   0        0        0       67 2024-05-07 20:57:23.439997 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/robots.txt
--rw-r--r--   0        0        0    18033 2024-05-07 20:57:48.915725 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/static/css/main.8ddb8b68.css
--rw-r--r--   0        0        0    46655 2024-05-07 20:57:48.915725 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/static/css/main.8ddb8b68.css.map
--rw-r--r--   0        0        0     4518 2024-05-07 20:57:48.915725 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/static/js/787.095790c7.chunk.js
--rw-r--r--   0        0        0    10597 2024-05-07 20:57:48.915725 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/static/js/787.095790c7.chunk.js.map
--rw-r--r--   0        0        0  3614868 2024-05-07 20:57:48.915725 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js
--rw-r--r--   0        0        0     3456 2024-05-07 20:57:48.915725 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js.LICENSE.txt
--rw-r--r--   0        0        0 13934230 2024-05-07 20:57:48.915725 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js.map
--rw-r--r--   0        0        0  1408324 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/package-lock.json
--rw-r--r--   0        0        0     2249 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/package.json
--rw-r--r--   0        0        0     3870 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/public/favicon.ico
--rw-r--r--   0        0        0     1324 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/public/index.html
--rw-r--r--   0        0        0      306 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/public/manifest.json
--rw-r--r--   0        0        0       67 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/public/robots.txt
--rw-r--r--   0        0        0     2443 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/App.css
--rw-r--r--   0        0        0     1143 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/App.js
--rw-r--r--   0        0        0      273 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/App.test.tsx
--rw-r--r--   0        0        0     1675 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/AtomsItem.js
--rw-r--r--   0        0        0       94 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/Data.js
--rw-r--r--   0        0        0      106 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/DataNode.js
--rw-r--r--   0        0        0      505 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/DataNodeItem.css
--rw-r--r--   0        0        0     1458 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/DataNodeItem.tsx
--rw-r--r--   0        0        0     5593 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/DataNodeTable.js
--rw-r--r--   0        0        0      116 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/Home.js
--rw-r--r--   0        0        0     1324 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/Layout.css
--rw-r--r--   0        0        0     1067 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/Layout.js
--rw-r--r--   0        0        0     5792 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/NodeDetails.js
--rw-r--r--   0        0        0     2784 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/Settings.js
--rw-r--r--   0        0        0     1025 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphDetail.js
--rw-r--r--   0        0        0     2631 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphDuration.js
--rw-r--r--   0        0        0     1129 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphIndicator.js
--rw-r--r--   0        0        0     8796 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphItem.tsx
--rw-r--r--   0        0        0     1064 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphItemStyles.ts
--rw-r--r--   0        0        0      837 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphLog.js
--rw-r--r--   0        0        0     3434 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphSummary.js
--rw-r--r--   0        0        0      990 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphTable.css
--rw-r--r--   0        0        0     7518 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphTable.js
--rw-r--r--   0        0        0      366 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/index.css
--rw-r--r--   0        0        0      554 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/index.tsx
--rw-r--r--   0        0        0     6007 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/logo.svg
--rw-r--r--   0        0        0       40 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/react-app-env.d.ts
--rw-r--r--   0        0        0      425 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/reportWebVitals.ts
--rw-r--r--   0        0        0      160 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete.css
--rw-r--r--   0        0        0     2787 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/customization.ts
--rw-r--r--   0        0        0      813 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/customization/CustomConnection.tsx
--rw-r--r--   0        0        0     4981 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/customization/CustomNode.tsx
--rw-r--r--   0        0        0      566 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/customization/CustomSocket.tsx
--rw-r--r--   0        0        0      540 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/customization/StyledNode.tsx
--rw-r--r--   0        0        0      602 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/customization/background.css
--rw-r--r--   0        0        0      378 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/customization/custom-background.ts
--rw-r--r--   0        0        0       94 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/customization/vars.ts
--rw-r--r--   0        0        0     4864 2024-05-04 20:38:47.853168 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/default.ts
--rw-r--r--   0        0        0      603 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/index.ts
--rw-r--r--   0        0        0      241 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/setupTests.ts
--rw-r--r--   0        0        0      535 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/tsconfig.json
--rw-r--r--   0        0        0       94 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/widget/.gitignore
--rw-r--r--   0        0        0      488 2024-04-13 07:05:41.907170 aiida_workgraph-0.2.4/aiida_workgraph/widget/.ipynb_checkpoints/example-checkpoint.ipynb
--rw-r--r--   0        0        0      552 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/widget/README.md
--rw-r--r--   0        0        0       71 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/widget/__init__.py
--rw-r--r--   0        0        0     7122 2024-05-03 14:17:12.929117 aiida_workgraph-0.2.4/aiida_workgraph/widget/js/default_rete.ts
--rw-r--r--   0        0        0      565 2024-04-22 20:35:00.919099 aiida_workgraph-0.2.4/aiida_workgraph/widget/js/widget.css
--rw-r--r--   0        0        0     5905 2024-04-22 20:35:00.919099 aiida_workgraph-0.2.4/aiida_workgraph/widget/js/widget.tsx
--rw-r--r--   0        0        0   148687 2024-04-22 20:35:00.923099 aiida_workgraph-0.2.4/aiida_workgraph/widget/package-lock.json
--rw-r--r--   0        0        0      851 2024-04-22 20:35:00.923099 aiida_workgraph-0.2.4/aiida_workgraph/widget/package.json
--rw-r--r--   0        0        0      765 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/widget/pyproject.toml
--rw-r--r--   0        0        0     1981 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.4/aiida_workgraph/widget/src/widget/__init__.py
--rw-r--r--   0        0        0      429 2024-05-07 20:57:15.636082 aiida_workgraph-0.2.4/aiida_workgraph/widget/src/widget/static/widget.css
--rw-r--r--   0        0        0  1796776 2024-05-07 20:57:15.640082 aiida_workgraph-0.2.4/aiida_workgraph/widget/src/widget/static/widget.js
--rw-r--r--   0        0        0      897 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.4/aiida_workgraph/widget/src/widget/utils.py
--rw-r--r--   0        0        0      453 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.4/aiida_workgraph/widget/tsconfig.json
--rw-r--r--   0        0        0    14889 2024-05-13 04:17:07.626646 aiida_workgraph-0.2.4/aiida_workgraph/workgraph.py
--rw-r--r--   0        0        0     2505 2024-05-15 13:45:46.436692 aiida_workgraph-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     7358 1970-01-01 00:00:00.000000 aiida_workgraph-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-12-11 16:36:18.395013 aiida_workgraph-0.2.5/LICENSE
+-rw-r--r--   0        0        0     5318 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.5/README.md
+-rw-r--r--   0        0        0      175 2024-05-20 19:34:02.324876 aiida_workgraph-0.2.5/aiida_workgraph/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 19:33:14.095414 aiida_workgraph-0.2.5/aiida_workgraph/calculations/__init__.py
+-rw-r--r--   0        0        0     2468 2024-05-20 19:33:14.095414 aiida_workgraph-0.2.5/aiida_workgraph/calculations/general_data.py
+-rw-r--r--   0        0        0     7811 2024-05-20 19:33:14.095414 aiida_workgraph-0.2.5/aiida_workgraph/calculations/python.py
+-rw-r--r--   0        0        0     1391 2024-05-20 19:33:14.095414 aiida_workgraph-0.2.5/aiida_workgraph/calculations/python_parser.py
+-rw-r--r--   0        0        0      279 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/cli/__init__.py
+-rw-r--r--   0        0        0    12112 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/cli/cmd_graph.py
+-rw-r--r--   0        0        0     1937 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/cli/cmd_web.py
+-rw-r--r--   0        0        0      714 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/cli/cmd_workgraph.py
+-rw-r--r--   0        0        0     6599 2024-05-18 09:24:02.309034 aiida_workgraph-0.2.5/aiida_workgraph/cli/query_workgraph.py
+-rw-r--r--   0        0        0     2679 2024-05-20 19:33:14.095414 aiida_workgraph-0.2.5/aiida_workgraph/collection.py
+-rw-r--r--   0        0        0    18544 2024-05-20 19:33:14.095414 aiida_workgraph-0.2.5/aiida_workgraph/decorator.py
+-rw-r--r--   0        0        0        0 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/engine/__init__.py
+-rw-r--r--   0        0        0    49863 2024-05-20 19:33:14.095414 aiida_workgraph-0.2.5/aiida_workgraph/engine/workgraph.py
+-rw-r--r--   0        0        0        0 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/executors/__init__.py
+-rw-r--r--   0        0        0      897 2024-05-07 20:56:57.572283 aiida_workgraph-0.2.5/aiida_workgraph/executors/builtin.py
+-rw-r--r--   0        0        0      740 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.5/aiida_workgraph/executors/qe.py
+-rw-r--r--   0        0        0      768 2024-05-07 20:56:57.572283 aiida_workgraph-0.2.5/aiida_workgraph/executors/test.py
+-rw-r--r--   0        0        0     4151 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.5/aiida_workgraph/node.py
+-rw-r--r--   0        0        0      847 2024-05-15 13:45:10.407702 aiida_workgraph-0.2.5/aiida_workgraph/nodes/__init__.py
+-rw-r--r--   0        0        0     3957 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.5/aiida_workgraph/nodes/builtin.py
+-rw-r--r--   0        0        0     2168 2024-05-15 13:45:10.407702 aiida_workgraph-0.2.5/aiida_workgraph/nodes/qe.py
+-rw-r--r--   0        0        0     7233 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.5/aiida_workgraph/nodes/test.py
+-rw-r--r--   0        0        0     1214 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/orm/worktree.py
+-rw-r--r--   0        0        0      115 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/properties/__init__.py
+-rw-r--r--   0        0        0    10647 2024-05-15 13:45:10.407702 aiida_workgraph-0.2.5/aiida_workgraph/properties/built_in.py
+-rw-r--r--   0        0        0     2131 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.5/aiida_workgraph/property.py
+-rw-r--r--   0        0        0     1386 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.5/aiida_workgraph/socket.py
+-rw-r--r--   0        0        0      111 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/sockets/__init__.py
+-rw-r--r--   0        0        0     3760 2024-05-15 13:45:10.407702 aiida_workgraph-0.2.5/aiida_workgraph/sockets/built_in.py
+-rw-r--r--   0        0        0     7824 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.5/aiida_workgraph/utils/__init__.py
+-rw-r--r--   0        0        0     6132 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.5/aiida_workgraph/utils/analysis.py
+-rw-r--r--   0        0        0     1754 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.5/aiida_workgraph/utils/graph.py
+-rw-r--r--   0        0        0      763 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/web/README.md
+-rw-r--r--   0        0        0        0 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/web/backend/app/__init__.py
+-rw-r--r--   0        0        0     2395 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/web/backend/app/api.py
+-rw-r--r--   0        0        0     3638 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/web/backend/app/daemon.py
+-rw-r--r--   0        0        0     2208 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.5/aiida_workgraph/web/backend/app/datanode.py
+-rw-r--r--   0        0        0     6618 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.5/aiida_workgraph/web/backend/app/utils.py
+-rw-r--r--   0        0        0     5130 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/web/backend/app/workgraph.py
+-rw-r--r--   0        0        0      115 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/web/backend/main.py
+-rw-r--r--   0        0        0      310 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/.gitignore
+-rw-r--r--   0        0        0       62 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/.rete-patch
+-rw-r--r--   0        0        0     2136 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/README.md
+-rw-r--r--   0        0        0      517 2024-05-20 19:35:26.142370 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/asset-manifest.json
+-rw-r--r--   0        0        0     3870 2024-05-20 19:34:56.150973 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/favicon.ico
+-rw-r--r--   0        0        0      654 2024-05-20 19:35:26.142370 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/index.html
+-rw-r--r--   0        0        0      306 2024-05-20 19:34:56.150973 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/manifest.json
+-rw-r--r--   0        0        0       67 2024-05-20 19:34:56.150973 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/robots.txt
+-rw-r--r--   0        0        0    18033 2024-05-20 19:35:26.170373 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/static/css/main.8ddb8b68.css
+-rw-r--r--   0        0        0    46655 2024-05-20 19:35:26.170373 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/static/css/main.8ddb8b68.css.map
+-rw-r--r--   0        0        0     4518 2024-05-20 19:35:26.170373 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/static/js/787.095790c7.chunk.js
+-rw-r--r--   0        0        0    10597 2024-05-20 19:35:26.170373 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/static/js/787.095790c7.chunk.js.map
+-rw-r--r--   0        0        0  3614868 2024-05-20 19:35:26.142370 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js
+-rw-r--r--   0        0        0     3456 2024-05-20 19:35:26.170373 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js.LICENSE.txt
+-rw-r--r--   0        0        0 13934230 2024-05-20 19:35:26.170373 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js.map
+-rw-r--r--   0        0        0  1408324 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/package-lock.json
+-rw-r--r--   0        0        0     2249 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/package.json
+-rw-r--r--   0        0        0     3870 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/public/favicon.ico
+-rw-r--r--   0        0        0     1324 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/public/index.html
+-rw-r--r--   0        0        0      306 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/public/manifest.json
+-rw-r--r--   0        0        0       67 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/public/robots.txt
+-rw-r--r--   0        0        0     2443 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/App.css
+-rw-r--r--   0        0        0     1143 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/App.js
+-rw-r--r--   0        0        0      273 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/App.test.tsx
+-rw-r--r--   0        0        0     1675 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/AtomsItem.js
+-rw-r--r--   0        0        0       94 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/Data.js
+-rw-r--r--   0        0        0      106 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/DataNode.js
+-rw-r--r--   0        0        0      505 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/DataNodeItem.css
+-rw-r--r--   0        0        0     1458 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/DataNodeItem.tsx
+-rw-r--r--   0        0        0     5593 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/DataNodeTable.js
+-rw-r--r--   0        0        0      116 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/Home.js
+-rw-r--r--   0        0        0     1324 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/Layout.css
+-rw-r--r--   0        0        0     1067 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/Layout.js
+-rw-r--r--   0        0        0     5792 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/NodeDetails.js
+-rw-r--r--   0        0        0     2784 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/Settings.js
+-rw-r--r--   0        0        0     1025 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphDetail.js
+-rw-r--r--   0        0        0     2631 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphDuration.js
+-rw-r--r--   0        0        0     1129 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphIndicator.js
+-rw-r--r--   0        0        0     8796 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphItem.tsx
+-rw-r--r--   0        0        0     1064 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphItemStyles.ts
+-rw-r--r--   0        0        0      837 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphLog.js
+-rw-r--r--   0        0        0     3434 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphSummary.js
+-rw-r--r--   0        0        0      990 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphTable.css
+-rw-r--r--   0        0        0     7518 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphTable.js
+-rw-r--r--   0        0        0      366 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/index.css
+-rw-r--r--   0        0        0      554 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/index.tsx
+-rw-r--r--   0        0        0     6007 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/logo.svg
+-rw-r--r--   0        0        0       40 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/react-app-env.d.ts
+-rw-r--r--   0        0        0      425 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/reportWebVitals.ts
+-rw-r--r--   0        0        0      160 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete.css
+-rw-r--r--   0        0        0     2787 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/customization.ts
+-rw-r--r--   0        0        0      813 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/customization/CustomConnection.tsx
+-rw-r--r--   0        0        0     4981 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/customization/CustomNode.tsx
+-rw-r--r--   0        0        0      566 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/customization/CustomSocket.tsx
+-rw-r--r--   0        0        0      540 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/customization/StyledNode.tsx
+-rw-r--r--   0        0        0      602 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/customization/background.css
+-rw-r--r--   0        0        0      378 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/customization/custom-background.ts
+-rw-r--r--   0        0        0       94 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/customization/vars.ts
+-rw-r--r--   0        0        0     4864 2024-05-04 20:38:47.853168 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/default.ts
+-rw-r--r--   0        0        0      603 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/index.ts
+-rw-r--r--   0        0        0      241 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/setupTests.ts
+-rw-r--r--   0        0        0      535 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/tsconfig.json
+-rw-r--r--   0        0        0       94 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/widget/.gitignore
+-rw-r--r--   0        0        0      488 2024-04-13 07:05:41.907170 aiida_workgraph-0.2.5/aiida_workgraph/widget/.ipynb_checkpoints/example-checkpoint.ipynb
+-rw-r--r--   0        0        0      552 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/widget/README.md
+-rw-r--r--   0        0        0       71 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/widget/__init__.py
+-rw-r--r--   0        0        0     7122 2024-05-03 14:17:12.929117 aiida_workgraph-0.2.5/aiida_workgraph/widget/js/default_rete.ts
+-rw-r--r--   0        0        0      565 2024-04-22 20:35:00.919099 aiida_workgraph-0.2.5/aiida_workgraph/widget/js/widget.css
+-rw-r--r--   0        0        0     5905 2024-04-22 20:35:00.919099 aiida_workgraph-0.2.5/aiida_workgraph/widget/js/widget.tsx
+-rw-r--r--   0        0        0   148687 2024-04-22 20:35:00.923099 aiida_workgraph-0.2.5/aiida_workgraph/widget/package-lock.json
+-rw-r--r--   0        0        0      851 2024-04-22 20:35:00.923099 aiida_workgraph-0.2.5/aiida_workgraph/widget/package.json
+-rw-r--r--   0        0        0      765 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/widget/pyproject.toml
+-rw-r--r--   0        0        0     1981 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.5/aiida_workgraph/widget/src/widget/__init__.py
+-rw-r--r--   0        0        0      429 2024-05-20 19:36:16.932122 aiida_workgraph-0.2.5/aiida_workgraph/widget/src/widget/static/widget.css
+-rw-r--r--   0        0        0  1796776 2024-05-20 19:36:16.932122 aiida_workgraph-0.2.5/aiida_workgraph/widget/src/widget/static/widget.js
+-rw-r--r--   0        0        0      897 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.5/aiida_workgraph/widget/src/widget/utils.py
+-rw-r--r--   0        0        0      453 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/widget/tsconfig.json
+-rw-r--r--   0        0        0    14913 2024-05-20 19:33:14.095414 aiida_workgraph-0.2.5/aiida_workgraph/workgraph.py
+-rw-r--r--   0        0        0     2853 2024-05-20 19:33:14.095414 aiida_workgraph-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     7358 1970-01-01 00:00:00.000000 aiida_workgraph-0.2.5/PKG-INFO
```

### Comparing `aiida_workgraph-0.2.4/LICENSE` & `aiida_workgraph-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/README.md` & `aiida_workgraph-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/cli/cmd_graph.py` & `aiida_workgraph-0.2.5/aiida_workgraph/cli/cmd_graph.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/cli/cmd_web.py` & `aiida_workgraph-0.2.5/aiida_workgraph/cli/cmd_web.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/cli/cmd_workgraph.py` & `aiida_workgraph-0.2.5/aiida_workgraph/cli/cmd_workgraph.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/cli/query_workgraph.py` & `aiida_workgraph-0.2.5/aiida_workgraph/cli/query_workgraph.py`

 * *Files 4% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         :param limit: Limit the query set to this number of entries.
         :return: The query set, a list of dictionaries.
         """
         import datetime
 
         from aiida import orm
         from aiida.common import timezone
-        from aiida_workgraph.engine.workgraph import WorkGraph
+        from aiida_workgraph.engine.workgraph import WorkGraphEngine
 
         # Define the list of projections for the QueryBuilder, which are all valid minus the compound projections
         projected_attributes = [
             self.mapper.get_attribute(projection)
             for projection in self._valid_projections
             if projection not in self._compound_projections
         ]
@@ -153,15 +153,15 @@
         if past_days is not None:
             filters["ctime"] = {
                 ">": timezone.now() - datetime.timedelta(days=past_days)
             }
 
         builder = orm.QueryBuilder()
         builder.append(
-            WorkGraph, filters=filters, project=unique_projections, tag="process"
+            WorkGraphEngine, filters=filters, project=unique_projections, tag="process"
         )
 
         if relationships is not None:
             for tag, entity in relationships.items():
                 builder.append(
                     cls=type(entity), filters={"id": entity.pk}, **{tag: "process"}
                 )
```

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/collection.py` & `aiida_workgraph-0.2.5/aiida_workgraph/collection.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,21 +9,28 @@
 
 class WorkGraphNodeCollection(NodeCollection):
     def new(
         self,
         identifier: Union[Callable, str],
         name: Optional[str] = None,
         uuid: Optional[str] = None,
+        on_remote: Optional[bool] = False,
         **kwargs: Any
     ) -> Any:
-        from aiida_workgraph.decorator import build_node_from_callable
+        from aiida_workgraph.decorator import (
+            build_node_from_callable,
+            build_PythonJob_node,
+        )
 
         # build the node on the fly if the identifier is a callable
         if callable(identifier):
             identifier = build_node_from_callable(identifier)
+        if isinstance(identifier, str) and identifier.upper() == "PYTHONJOB":
+            # copy the inputs and outputs from the function node to the PythonJob node
+            identifier = build_PythonJob_node(kwargs.pop("function"))
         # Call the original new method
         return super().new(identifier, name, uuid, **kwargs)
 
 
 class WorkGraphPropertyCollection(PropertyCollection):
     def new(
         self,
```

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/decorator.py` & `aiida_workgraph-0.2.5/aiida_workgraph/decorator.py`

 * *Files 7% similar despite different names*

```diff
@@ -145,28 +145,28 @@
         return executor
     ndata = {}
     if inspect.isfunction(executor):
         # calcfunction and workfunction
         if getattr(executor, "node_class", False):
             ndata["node_type"] = node_types.get(executor.node_class, "NORMAL")
             ndata["executor"] = executor
-            return build_node_from_AiiDA(ndata, inputs=inputs, outputs=outputs)
+            return build_node_from_AiiDA(ndata, inputs=inputs, outputs=outputs)[0]
         else:
             ndata["node_type"] = "NORMAL"
             ndata["executor"] = executor
             return build_node_from_function(executor, inputs=inputs, outputs=outputs)
     else:
         if issubclass(executor, CalcJob):
             ndata["node_type"] = "CALCJOB"
             ndata["executor"] = executor
-            return build_node_from_AiiDA(ndata, inputs=inputs, outputs=outputs)
+            return build_node_from_AiiDA(ndata, inputs=inputs, outputs=outputs)[0]
         elif issubclass(executor, WorkChain):
             ndata["node_type"] = "WORKCHAIN"
             ndata["executor"] = executor
-            return build_node_from_AiiDA(ndata, inputs=inputs, outputs=outputs)
+            return build_node_from_AiiDA(ndata, inputs=inputs, outputs=outputs)[0]
     raise ValueError("The executor is not supported.")
 
 
 def build_node_from_function(
     executor: Callable,
     inputs: Optional[List[str]] = None,
     outputs: Optional[List[str]] = None,
@@ -226,15 +226,42 @@
     executor = {
         "executor": pickle.dumps(executor),
         "type": ndata["node_type"],
         "is_pickle": True,
     }
     ndata["executor"] = executor
     node = create_node(ndata)
-    return node
+    return node, ndata
+
+
+def build_PythonJob_node(func: Callable) -> Node:
+    """Build PythonJob node from function."""
+    from aiida_workgraph.calculations.python import PythonJob
+
+    ndata = {"executor": PythonJob, "node_type": "CALCJOB"}
+    _, ndata_py = build_node_from_AiiDA(ndata)
+    ndata = func.ndata
+    # merge the inputs and outputs from the PythonJob node to the function node
+    # skip the already existed inputs and outputs
+    inputs = ndata["inputs"]
+    outputs = ndata["outputs"]
+    for input in ndata_py["inputs"]:
+        if input not in inputs:
+            inputs.append(input)
+    for output in ndata_py["outputs"]:
+        if output not in outputs:
+            outputs.append(output)
+    # append the kwargs of the PythonJob node to the function node
+    kwargs = ndata["kwargs"]
+    kwargs.extend(ndata_py["kwargs"])
+    ndata["inputs"] = inputs
+    ndata["outputs"] = outputs
+    ndata["kwargs"] = kwargs
+    ndata["node_type"] = "PYTHONJOB"
+    return create_node(ndata)
 
 
 def build_node_from_workgraph(wg: any) -> Node:
     """Build node from workgraph."""
     from aiida_workgraph.node import Node
 
     ndata = {"node_type": "workgraph"}
@@ -259,14 +286,15 @@
                 [f"{node.name}.{socket.name}", f"{node.name}.{socket.name}"]
             )
     kwargs = [input[1] for input in inputs]
     # add built-in sockets
     outputs.append(["General", "_outputs"])
     outputs.append(["General", "_wait"])
     inputs.append(["General", "_wait", {"link_limit": 1e6}])
+    inputs.append(["General", "_code"])
     ndata["node_class"] = Node
     ndata["kwargs"] = kwargs
     ndata["inputs"] = inputs
     ndata["outputs"] = outputs
     ndata["identifier"] = wg.name
     # TODO In order to reload the WorkGraph from process, "is_pickle" should be True
     # so I pickled the function here, but this is not necessary
@@ -282,19 +310,27 @@
     node.group_outputs = group_outputs
     return node
 
 
 def serialize_function(func: Callable) -> Dict[str, Any]:
     """Serialize a function for storage or transmission."""
     import cloudpickle as pickle
+    import inspect
+    import textwrap
+
+    source_code = inspect.getsource(func)
+    source_code_lines = source_code.split("\n")
+    function_source_code = "\n".join(source_code_lines[1:])
+    function_source_code = textwrap.dedent(function_source_code)
 
     return {
         "executor": pickle.dumps(func),
         "type": "function",
         "is_pickle": True,
+        "function_source_code": function_source_code,
     }
 
 
 def generate_ndata(
     func: Callable,
     identifier: str,
     inputs: List[Tuple[str, str]],
@@ -310,14 +346,16 @@
 
     args, kwargs, var_args, var_kwargs, _inputs = generate_input_sockets(
         func, inputs, properties
     )
     node_outputs = outputs
     # add built-in sockets
     _inputs.append(["General", "_wait", {"link_limit": 1e6}])
+    _inputs.append(["General", "_code"])
+    kwargs.append("_code")
     node_outputs.append(["General", "_wait"])
     node_outputs.append(["General", "_outputs"])
     ndata = {
         "node_class": Node,
         "identifier": identifier,
         "args": args,
         "kwargs": kwargs,
@@ -378,14 +416,15 @@
                 properties or [],
                 catalog,
                 node_type,
             )
             node = create_node(ndata)
             func.identifier = identifier
             func.node = node
+            func.ndata = ndata
             return func
 
         return decorator
 
     # decorator with arguments indentifier, args, kwargs, properties, inputs, outputs, executor
     @staticmethod
     def decorator_graph_builder(
```

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/engine/workgraph.py` & `aiida_workgraph-0.2.5/aiida_workgraph/engine/workgraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 __all__ = "WorkGraph"
 
 
 MAX_NUMBER_AWAITABLES_MSG = "The maximum number of subprocesses has been reached: {}. Cannot launch the job: {}."
 
 
 @auto_persist("_awaitables")
-class WorkGraph(Process, metaclass=Protect):
+class WorkGraphEngine(Process, metaclass=Protect):
     """The `WorkGraph` class is used to construct workflows in AiiDA."""
 
     # used to create a process node that represents what happened in this process.
     _node_class = WorkChainNode
     _spec_class = WorkChainSpec
     _CONTEXT = "CONTEXT"
 
@@ -569,14 +569,15 @@
             in [
                 "CALCFUNCTION",
                 "WORKFUNCTION",
                 "CALCJOB",
                 "WORKCHAIN",
                 "GRAPH_BUILDER",
                 "WORKGRAPH",
+                "PYTHONJOB",
             ]
             and node["state"] == "RUNNING"
         ):
             self.set_node_result(node)
 
     def is_workgraph_finished(self) -> bool:
         """Check if the workgraph is finished.
@@ -675,14 +676,15 @@
             print("-" * 60)
             node = self.ctx.nodes[name]
             if node["metadata"]["node_type"].upper() in [
                 "CALCJOB",
                 "WORKCHAIN",
                 "GRAPH_BUILDER",
                 "WORKGRAPH",
+                "PYTHONJOB",
             ]:
                 if len(self._awaitables) > self.ctx.max_number_awaitables:
                     print(
                         MAX_NUMBER_AWAITABLES_MSG.format(
                             self.ctx.max_number_awaitables, name
                         )
                     )
@@ -808,23 +810,68 @@
                         wgdata["nodes"][node_name]["properties"][socket_name][
                             "value"
                         ] = value
                 # merge the properties
                 merge_properties(wgdata)
                 metadata = {"call_link_label": name}
                 inputs = {"wg": wgdata, "metadata": metadata}
-                process_inited = WorkGraph(inputs=inputs)
+                process_inited = WorkGraphEngine(inputs=inputs)
                 process_inited.runner.persister.save_checkpoint(process_inited)
                 saver = WorkGraphSaver(process_inited.node, wgdata)
                 saver.save()
                 print("submit workgraph: ")
                 process = self.submit(process_inited)
                 node["process"] = process
                 self.ctx.nodes[name]["state"] = "RUNNING"
                 self.to_context(**{name: process})
+            elif node["metadata"]["node_type"].upper() in ["PYTHONJOB"]:
+                from aiida_workgraph.calculations.python import PythonJob
+                from aiida_workgraph.calculations.general_data import GeneralData
+
+                print("node  type: Python.")
+                # normal function does not have a process
+                code = kwargs.pop("code")
+                parent_folder = kwargs.pop("parent_folder", None)
+                metadata = kwargs.pop("metadata", {})
+                metadata.update({"call_link_label": name})
+                # get the source code of the function
+                function_name = executor.__name__
+                function_source_code = node["executor"]["function_source_code"]
+                inputs = {}
+                # save all kwargs to inputs port
+                for key, value in kwargs.items():
+                    if isinstance(value, orm.Node):
+                        if not hasattr(value, "value"):
+                            raise ValueError(
+                                "Only AiiDA data Node with a value attribute is allowed."
+                            )
+                        inputs[key] = value
+                    else:
+                        inputs[key] = GeneralData(value)
+                print("inputs: ", inputs)
+                # outputs
+                output_name_list = [output["name"] for output in node["outputs"]]
+
+                # transfer the args to kwargs
+                process = self.submit(
+                    PythonJob,
+                    inputs={
+                        "function_source_code": orm.Str(function_source_code),
+                        "function_name": orm.Str(function_name),
+                        "code": code,
+                        "kwargs": inputs,
+                        "output_name_list": orm.List(output_name_list),
+                        "parent_folder": parent_folder,
+                        "metadata": metadata,
+                    },
+                )
+                process.label = name
+                node["process"] = process
+                self.ctx.nodes[name]["state"] = "RUNNING"
+                self.to_context(**{name: process})
             elif node["metadata"]["node_type"].upper() in ["NORMAL"]:
                 print("node  type: Normal.")
                 # normal function does not have a process
                 if "context" in node["metadata"]["kwargs"]:
                     self.ctx.node_name = name
                     kwargs.update({"context": self.ctx})
                 for key in self.ctx.nodes[name]["metadata"]["args"]:
```

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/executors/builtin.py` & `aiida_workgraph-0.2.5/aiida_workgraph/executors/builtin.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/executors/qe.py` & `aiida_workgraph-0.2.5/aiida_workgraph/executors/qe.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/executors/test.py` & `aiida_workgraph-0.2.5/aiida_workgraph/executors/test.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/node.py` & `aiida_workgraph-0.2.5/aiida_workgraph/node.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/nodes/__init__.py` & `aiida_workgraph-0.2.5/aiida_workgraph/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/nodes/builtin.py` & `aiida_workgraph-0.2.5/aiida_workgraph/nodes/builtin.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/nodes/qe.py` & `aiida_workgraph-0.2.5/aiida_workgraph/nodes/qe.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/nodes/test.py` & `aiida_workgraph-0.2.5/aiida_workgraph/nodes/test.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/orm/worktree.py` & `aiida_workgraph-0.2.5/aiida_workgraph/orm/worktree.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/properties/built_in.py` & `aiida_workgraph-0.2.5/aiida_workgraph/properties/built_in.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/property.py` & `aiida_workgraph-0.2.5/aiida_workgraph/property.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/socket.py` & `aiida_workgraph-0.2.5/aiida_workgraph/socket.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/sockets/built_in.py` & `aiida_workgraph-0.2.5/aiida_workgraph/sockets/built_in.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/utils/__init__.py` & `aiida_workgraph-0.2.5/aiida_workgraph/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/utils/analysis.py` & `aiida_workgraph-0.2.5/aiida_workgraph/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/utils/graph.py` & `aiida_workgraph-0.2.5/aiida_workgraph/utils/graph.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/README.md` & `aiida_workgraph-0.2.5/aiida_workgraph/web/README.md`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/backend/app/api.py` & `aiida_workgraph-0.2.5/aiida_workgraph/web/backend/app/api.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/backend/app/daemon.py` & `aiida_workgraph-0.2.5/aiida_workgraph/web/backend/app/daemon.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/backend/app/datanode.py` & `aiida_workgraph-0.2.5/aiida_workgraph/web/backend/app/datanode.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/backend/app/utils.py` & `aiida_workgraph-0.2.5/aiida_workgraph/web/backend/app/utils.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/backend/app/workgraph.py` & `aiida_workgraph-0.2.5/aiida_workgraph/web/backend/app/workgraph.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/README.md` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/README.md`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/asset-manifest.json` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/favicon.ico` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/index.html` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/static/css/main.8ddb8b68.css` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/static/css/main.8ddb8b68.css`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/static/css/main.8ddb8b68.css.map` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/static/css/main.8ddb8b68.css.map`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/static/js/787.095790c7.chunk.js` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/static/js/787.095790c7.chunk.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/static/js/787.095790c7.chunk.js.map` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/static/js/787.095790c7.chunk.js.map`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js.LICENSE.txt` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js.map` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js.map`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/package-lock.json` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/package.json` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/package.json`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/public/favicon.ico` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/public/index.html` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/public/index.html`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/App.css` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/App.css`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/App.js` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/App.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/AtomsItem.js` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/AtomsItem.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/DataNodeItem.tsx` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/DataNodeItem.tsx`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/DataNodeTable.js` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/DataNodeTable.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/Layout.css` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/Layout.css`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/Layout.js` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/Layout.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/NodeDetails.js` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/NodeDetails.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/Settings.js` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/Settings.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphDetail.js` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphDetail.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphDuration.js` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphDuration.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphIndicator.js` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphIndicator.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphItem.tsx` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphItem.tsx`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphItemStyles.ts` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphItemStyles.ts`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphLog.js` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphLog.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphSummary.js` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphSummary.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphTable.css` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphTable.css`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/components/WorkGraphTable.js` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphTable.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/index.tsx` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/index.tsx`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/logo.svg` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/logo.svg`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/customization.ts` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/customization.ts`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/customization/CustomConnection.tsx` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/customization/CustomConnection.tsx`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/customization/CustomNode.tsx` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/customization/CustomNode.tsx`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/customization/CustomSocket.tsx` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/customization/CustomSocket.tsx`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/customization/StyledNode.tsx` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/customization/StyledNode.tsx`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/customization/background.css` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/customization/background.css`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/default.ts` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/default.ts`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/src/rete/index.ts` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/index.ts`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/web/frontend/tsconfig.json` & `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/widget/README.md` & `aiida_workgraph-0.2.5/aiida_workgraph/widget/README.md`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/widget/js/default_rete.ts` & `aiida_workgraph-0.2.5/aiida_workgraph/widget/js/default_rete.ts`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/widget/js/widget.css` & `aiida_workgraph-0.2.5/aiida_workgraph/widget/js/widget.css`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/widget/js/widget.tsx` & `aiida_workgraph-0.2.5/aiida_workgraph/widget/js/widget.tsx`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/widget/package-lock.json` & `aiida_workgraph-0.2.5/aiida_workgraph/widget/package-lock.json`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/widget/package.json` & `aiida_workgraph-0.2.5/aiida_workgraph/widget/package.json`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/widget/pyproject.toml` & `aiida_workgraph-0.2.5/aiida_workgraph/widget/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/widget/src/widget/__init__.py` & `aiida_workgraph-0.2.5/aiida_workgraph/widget/src/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/widget/src/widget/static/widget.js` & `aiida_workgraph-0.2.5/aiida_workgraph/widget/src/widget/static/widget.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/widget/src/widget/utils.py` & `aiida_workgraph-0.2.5/aiida_workgraph/widget/src/widget/utils.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.4/aiida_workgraph/workgraph.py` & `aiida_workgraph-0.2.5/aiida_workgraph/workgraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     link_deletion_hook,
 )
 from aiida_workgraph.widget import NodeGraphWidget
 from typing import Any, Dict, List, Optional
 
 
 class WorkGraph(node_graph.NodeGraph):
-    """Build a node-based workflow AiiDA's workgraph engine.
+    """Build a node-based workflow AiiDA's workgraph.
 
     The class extends from NodeGraph and provides methods to run,
     submit tasks, wait for tasks to finish, and update the process status.
     It is used to handle various states of a workgraph process and provides
     convenient operations to interact with it.
 
     Attributes:
@@ -57,15 +57,15 @@
         self._widget = NodeGraphWidget(parent=self)
 
     def run(self, inputs: Optional[Dict[str, Any]] = None) -> Any:
         """
         Run the AiiDA workgraph process and update the process status. The method uses AiiDA's engine to run
         the process and then calls the update method to update the state of the process.
         """
-        from aiida_workgraph.engine.workgraph import WorkGraph as WorkGraphEngine
+        from aiida_workgraph.engine.workgraph import WorkGraphEngine
         from aiida_workgraph.utils import merge_properties
 
         # set node inputs
         if inputs is not None:
             for name, input in inputs.items():
                 if name not in self.nodes.keys():
                     raise KeyError(f"Node {name} not found in WorkGraph.")
@@ -132,15 +132,15 @@
         return self.process
 
     def save(self, metadata: Optional[Dict[str, Any]] = None) -> None:
         """Save the udpated workgraph to the process
         This is only used for a running workgraph.
         Save the AiiDA workgraph process and update the process status.
         """
-        from aiida_workgraph.engine.workgraph import WorkGraph as WorkGraphEngine
+        from aiida_workgraph.engine.workgraph import WorkGraphEngine
         from aiida_workgraph.utils import merge_properties
 
         wgdata = self.to_dict()
         merge_properties(wgdata)
         metadata = metadata or {}
         inputs = {"wg": wgdata, "metadata": metadata}
         if self.process is None:
@@ -227,23 +227,25 @@
                 self.nodes[link.link_label].state = node.process_state.value.upper()
                 self.nodes[link.link_label].node = node
                 self.nodes[link.link_label].pk = node.pk
                 self.nodes[link.link_label].ctime = node.ctime
                 self.nodes[link.link_label].mtime = node.mtime
                 if self.nodes[link.link_label].state == "FINISHED":
                     # update the output sockets
+                    i = 0
                     for socket in self.nodes[link.link_label].outputs:
                         if self.nodes[link.link_label].node_type == "graph_builder":
                             if not getattr(node.outputs, "group_outputs", False):
                                 continue
                             socket.value = getattr(
                                 node.outputs.group_outputs, socket.name, None
                             )
                         else:
                             socket.value = getattr(node.outputs, socket.name, None)
+                        i += 1
             elif isinstance(node, aiida.orm.Data):
                 if link.link_label.startswith(
                     "group_outputs__"
                 ) or link.link_label.startswith("new_data__"):
                     label = link.link_label.split("__", 1)[1]
                     if label in self.nodes.keys():
                         self.nodes[label].state = "FINISHED"
```

### Comparing `aiida_workgraph-0.2.4/pyproject.toml` & `aiida_workgraph-0.2.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -66,14 +66,23 @@
 
 [project.scripts]
 workgraph = "aiida_workgraph.cli.cmd_workgraph:workgraph"
 
 [project.entry-points."aiida.cmdline"]
 "workgraph" = "aiida_workgraph.cli.cmd_workgraph:workgraph"
 
+[project.entry-points."aiida.calculations"]
+"workgraph.python" = "aiida_workgraph.calculations.python:PythonJob"
+
+[project.entry-points."aiida.parsers"]
+"workgraph.python" = "aiida_workgraph.calculations.python_parser:PythonParser"
+
+[project.entry-points."aiida.data"]
+"workgraph.general" = "aiida_workgraph.calculations.general_data:GeneralData"
+
 [project.entry-points."aiida.node"]
 "process.workflow.workgraph" = "aiida_workgraph.orm.workgraph:WorkgraphNode"
 
 [project.entry-points."aiida_workgraph.node"]
 "aiida" = "aiida_workgraph.nodes:node_list"
 
 [project.entry-points."aiida_workgraph.property"]
```

### Comparing `aiida_workgraph-0.2.4/PKG-INFO` & `aiida_workgraph-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-workgraph
-Version: 0.2.4
+Version: 0.2.5
 Summary: Design flexible node-based workflow for AiiDA calculation.
 Keywords: aiida,workflows
 Author-email: Xing Wang <xingwang1991@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 1 - Planning
 Classifier: Framework :: AiiDA
```

