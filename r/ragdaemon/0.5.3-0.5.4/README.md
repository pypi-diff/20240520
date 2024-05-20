# Comparing `tmp/ragdaemon-0.5.3.tar.gz` & `tmp/ragdaemon-0.5.4.tar.gz`

## Comparing `ragdaemon-0.5.3.tar` & `ragdaemon-0.5.4.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/scratch.ipynb
--rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/tutorial.ipynb
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/__main__.py
--rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/app.py
--rw-r--r--   0        0        0    10876 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/context.py
--rw-r--r--   0        0        0     8200 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/daemon.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/errors.py
--rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/get_paths.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/graph.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/locate.py
--rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/utils.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/annotators/__init__.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/annotators/base_annotator.py
--rw-r--r--   0        0        0    10676 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/annotators/call_graph.py
--rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/annotators/chunker.py
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/annotators/chunker_line.py
--rw-r--r--   0        0        0    10009 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/annotators/chunker_llm.py
--rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/annotators/diff.py
--rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/annotators/hierarchy.py
--rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/annotators/layout_hierarchy.py
--rw-r--r--   0        0        0    12042 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/annotators/summarizer.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/database/__init__.py
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/database/chroma_database.py
--rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/database/database.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/database/lite_database.py
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/prompts/call_graph.toml
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/prompts/chunker_llm.toml
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/prompts/locate.toml
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/prompts/summarizer/base.txt
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/prompts/summarizer/chunk.txt
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/prompts/summarizer/directory.txt
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/prompts/summarizer/file.txt
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/prompts/summarizer/root.txt
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/prompts/summarizer/user.txt
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/static/favicon.ico
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/static/js/controlPanel.js
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/static/js/main.js
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/static/js/three/camera.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/static/js/three/controls.js
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/static/js/three/edge.js
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/static/js/three/node.js
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/static/js/three/raycaster.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/static/js/three/renderer.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/static/js/three/scene.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/templates/index.html
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/ragdaemon/templates/search_results.html
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/tests/conftest.py
--rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/tests/test_comments.py
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/tests/test_context.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/tests/test_daemon.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/tests/test_database.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/tests/test_get_paths.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/tests/test_sample.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/tests/annotators/test_chunker.py
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/tests/annotators/test_chunker_llm.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/tests/annotators/test_diff.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/tests/annotators/test_hierarchy.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/tests/annotators/test_layout_hierarchy.py
--rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/tests/annotators/test_summarizer.py
--rw-r--r--   0        0        0     8531 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/tests/data/chunker_graph.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/tests/data/context_message.txt
--rw-r--r--   0        0        0    10570 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/tests/data/diff_graph.json
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/tests/data/hard_to_chunk.txt
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/tests/data/hierarchy_graph.json
--rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/tests/data/layout_hierarchy_graph.json
--rw-r--r--   0        0        0    17458 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/tests/data/summarizer_graph.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/tests/sample/README.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/tests/sample/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/tests/sample/src/__init__.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/tests/sample/src/interface.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/tests/sample/src/operations.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/.gitignore
--rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/LICENSE
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/README.md
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     6985 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/scratch.ipynb
+-rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tutorial.ipynb
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/__main__.py
+-rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/app.py
+-rw-r--r--   0        0        0    10876 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/context.py
+-rw-r--r--   0        0        0     8200 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/daemon.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/errors.py
+-rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/get_paths.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/graph.py
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/locate.py
+-rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/utils.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/annotators/__init__.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/annotators/base_annotator.py
+-rw-r--r--   0        0        0    10676 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/annotators/call_graph.py
+-rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/annotators/chunker.py
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/annotators/chunker_line.py
+-rw-r--r--   0        0        0    10250 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/annotators/chunker_llm.py
+-rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/annotators/diff.py
+-rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/annotators/hierarchy.py
+-rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/annotators/layout_hierarchy.py
+-rw-r--r--   0        0        0    12309 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/annotators/summarizer.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/database/__init__.py
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/database/chroma_database.py
+-rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/database/database.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/database/lite_database.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/prompts/call_graph.toml
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/prompts/chunker_llm.toml
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/prompts/locate.toml
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/prompts/summarizer/base.txt
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/prompts/summarizer/chunk.txt
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/prompts/summarizer/directory.txt
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/prompts/summarizer/file.txt
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/prompts/summarizer/root.txt
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/prompts/summarizer/user.txt
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/static/favicon.ico
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/static/js/controlPanel.js
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/static/js/main.js
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/static/js/three/camera.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/static/js/three/controls.js
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/static/js/three/edge.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/static/js/three/node.js
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/static/js/three/raycaster.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/static/js/three/renderer.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/static/js/three/scene.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/templates/index.html
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/templates/search_results.html
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/conftest.py
+-rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/test_comments.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/test_context.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/test_daemon.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/test_database.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/test_get_paths.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/test_sample.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/annotators/test_chunker.py
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/annotators/test_chunker_llm.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/annotators/test_diff.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/annotators/test_hierarchy.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/annotators/test_layout_hierarchy.py
+-rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/annotators/test_summarizer.py
+-rw-r--r--   0        0        0     8531 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/data/chunker_graph.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/data/context_message.txt
+-rw-r--r--   0        0        0    10570 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/data/diff_graph.json
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/data/hard_to_chunk.txt
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/data/hierarchy_graph.json
+-rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/data/layout_hierarchy_graph.json
+-rw-r--r--   0        0        0    17458 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/data/summarizer_graph.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/sample/README.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/sample/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/sample/src/__init__.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/sample/src/interface.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/sample/src/operations.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/.gitignore
+-rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/README.md
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/PKG-INFO
```

### Comparing `ragdaemon-0.5.3/tutorial.ipynb` & `ragdaemon-0.5.4/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/.github/workflows/run-tests.yml` & `ragdaemon-0.5.4/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/ragdaemon/app.py` & `ragdaemon-0.5.4/ragdaemon/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,19 +35,18 @@
 refresh = args.refresh
 verbose = True  # Always verbose in server mode
 code_extensions = None if args.code_extensions is None else set(args.code_extensions)
 diff = args.diff
 annotators = {
     "hierarchy": {},
     "chunker_llm": {"chunk_extensions": code_extensions},
-    # "summarizer": {},
-    # "clusterer_binary": {},
-    # "call_graph": {"call_extensions": code_extensions},
-    "diff": {"diff": diff},
-    "layout_hierarchy": {},
+    "call_graph": {"call_extensions": code_extensions},
+    "summarizer": {},
+    # "diff": {"diff": diff},
+    # "layout_hierarchy": {},
 }
 daemon = Daemon(Path.cwd(), annotators=annotators, verbose=verbose)
 
 
 # Start/run daemon in the background
 @asynccontextmanager
 async def lifespan(app: FastAPI):
```

### Comparing `ragdaemon-0.5.3/ragdaemon/context.py` & `ragdaemon-0.5.4/ragdaemon/context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/ragdaemon/daemon.py` & `ragdaemon-0.5.4/ragdaemon/daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/ragdaemon/get_paths.py` & `ragdaemon-0.5.4/ragdaemon/get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/ragdaemon/graph.py` & `ragdaemon-0.5.4/ragdaemon/graph.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/ragdaemon/locate.py` & `ragdaemon-0.5.4/ragdaemon/locate.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/ragdaemon/utils.py` & `ragdaemon-0.5.4/ragdaemon/utils.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/ragdaemon/annotators/__init__.py` & `ragdaemon-0.5.4/ragdaemon/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/ragdaemon/annotators/base_annotator.py` & `ragdaemon-0.5.4/ragdaemon/annotators/base_annotator.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/ragdaemon/annotators/call_graph.py` & `ragdaemon-0.5.4/ragdaemon/annotators/call_graph.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/ragdaemon/annotators/chunker.py` & `ragdaemon-0.5.4/ragdaemon/annotators/chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/ragdaemon/annotators/chunker_line.py` & `ragdaemon-0.5.4/ragdaemon/annotators/chunker_line.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/ragdaemon/annotators/chunker_llm.py` & `ragdaemon-0.5.4/ragdaemon/annotators/chunker_llm.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,67 +30,75 @@
     if not isinstance(chunks, list):
         return False
     if not all(isinstance(chunk, dict) for chunk in chunks):
         return False
 
     for chunk in chunks:
         if not set(chunk.keys()) == {"id", "start_line", "end_line"}:
-            return False  # Chunk is missing fields
+            return False
 
         halves = chunk["id"].split(":")
         if len(halves) != 2 or not halves[0] or not halves[1]:
-            return False  # Chunk ID is not in the correct format
+            return False
         if halves[0] != file:
             return False
 
         start, end = chunk.get("start_line"), chunk.get("end_line")
         if start is None or end is None:
-            return False  # Chunk lines are missing
+            return False
 
         # Sometimes output is int, sometimes string. This accomodates either.
         start, end = str(start), str(end)
         if not start.isdigit() or not end.isdigit():
-            return False  # Chunk lines are not valid
+            return False
         start, end = int(start), int(end)
 
         if not 1 <= start <= end <= max_line:
-            return False  # Chunk lines are out of bounds
-        # TODO: Validate the ref, i.e. a parent chunk exists
+            return False
 
     if last_chunk is not None:
         if not any(chunk["id"] == last_chunk["id"] for chunk in chunks):
             return False
 
-    # Sometimes the model returns chunks with invalid parents. Most of the time
-    # this is an error so we want to retry. If it keeps getting it wrong though,
-    # we'd rather accept the incorrect ones (they'll be linked to BASE later on)
-    # so we can bypass this check by passing file_chunks=None.
-    if file_chunks is not None:
+    """
+    The LLM sometimes returns invalid parents (i.e. path/to/file.ext:parent.chunk).
+    There are 3 cases why they might be invalid:
+    A) The LLM made a typo here. In that case, return False to try again.
+    B) The LLM made a typo when parsing the parent in a previous batch. In that case,
+       go back and redo the previous batch. We distinguish this from case A) by checking
+       if multiple chunks reference the same invalid parent.
+    C) An edge case where our schema breaks down, e.g. Javascript event handlers 
+       usually try to set "document" as their parent, but that won't be a node.
+    
+    Case A) should be resolved by Spice's validator loop, i.e. this function returning 
+    "False". For Case B), raise a special exception and step back one batch in the 
+    chunk_document loop. Any chunks still referencing invalid parents after these two 
+    loops are exhausted (including case C)) will just be accepted and linked to 
+    path/to/file.ext:BASE.
+    """
+    if file_chunks:  # else, loops exhausted or Case C)
         valid_parents = file_chunks.copy()
         chunks_shortest_first = sorted(chunks, key=lambda x: len(x["id"]))
         chunks_missing_parents = set()
         for chunk in chunks_shortest_first:
             if not resolve_chunk_parent(chunk["id"], valid_parents):
                 chunks_missing_parents.add(chunk["id"])
             valid_parents.add(chunk["id"])
 
-        # If multiple chunks are missing the same parent, it's likely an
-        # issue with the prior chunk. Raise an error to revert the outer loop
-        # one step and try the previous chunk again.
         if len(chunks_missing_parents) > 1:
             missing_parents = []
             for chunk in chunks_missing_parents:
                 file, chunk_str = chunk.split(":")
                 parts = chunk_str.split(".")
                 missing_parents.append(f"{file}:{'.'.join(parts[:-1])}")
             mp_counts = Counter(missing_parents)
             parent, count = mp_counts.most_common(1)[0]
             if count > 1:
-                raise ChunkErrorInPreviousBatch(parent)
-            return False
+                raise ChunkErrorInPreviousBatch(parent)  # Case B)
+            return False  # Case A)
 
     return True
 
 
 class ChunkerLLM(Chunker):
     name = "chunker_llm"
     chunk_field_id = "chunks_llm"
@@ -143,21 +151,19 @@
                     response_format={"type": "json_object"},
                     validator=validator,
                     retries=2,
                 )
                 return json.loads(response.text).get("chunks")
             except ValueError:
                 pass
-            # It's possible the parent chunk just doens't exist. So try once more and
-            # disregard that - it will just be linked to the BASE chunk instead.
             validator = partial(
                 validate,
                 file=file,
                 max_line=max_line,
-                file_chunks=None,
+                file_chunks=None,  # Skip parent chunk validation
                 last_chunk=last_chunk,
             )
             try:
                 response = await self.spice_client.get_response(
                     messages=messages,
                     model=self.model,
                     response_format={"type": "json_object"},
@@ -190,17 +196,18 @@
         while i < n_batches:
             while retries_by_batch[i] >= 0:
                 batch_lines = file_lines[
                     i * self.batch_size : (i + 1) * self.batch_size
                 ]
                 chunk_index_by_batch[i] = len(chunks)
                 last_chunk = chunks.pop() if chunks else None
-                file_chunks = (
-                    {c["id"] for c in chunks} if retries_by_batch[i] > 0 else None
-                )
+                if retries_by_batch[i] > 0:
+                    file_chunks = {c["id"] for c in chunks}
+                else:
+                    file_chunks = None  # Skip parent chunk validation
                 try:
                     _chunks = await self.get_llm_response(
                         file, batch_lines, file_chunks, last_chunk
                     )
                     chunks.extend(_chunks)
                     i += 1
                     break
```

### Comparing `ragdaemon-0.5.3/ragdaemon/annotators/diff.py` & `ragdaemon-0.5.4/ragdaemon/annotators/diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/ragdaemon/annotators/hierarchy.py` & `ragdaemon-0.5.4/ragdaemon/annotators/hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/ragdaemon/annotators/layout_hierarchy.py` & `ragdaemon-0.5.4/ragdaemon/annotators/layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/ragdaemon/annotators/summarizer.py` & `ragdaemon-0.5.4/ragdaemon/annotators/summarizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from ragdaemon.annotators.base_annotator import Annotator
 from ragdaemon.context import ContextBuilder
 from ragdaemon.database import Database, remove_update_db_duplicates
 from ragdaemon.graph import KnowledgeGraph
 from ragdaemon.errors import RagdaemonError
 from ragdaemon.utils import (
     DEFAULT_COMPLETION_MODEL,
-    hash_str,
     match_refresh,
     semaphore,
     truncate,
 )
 
 
 def count_leaf_nodes_any_depth(
@@ -208,23 +207,23 @@
 
     def is_complete(self, graph: KnowledgeGraph, db: Database) -> bool:
         for node, data in graph.nodes(data=True):
             if data is None:
                 raise RagdaemonError(f"Node {node} has no data.")
             if data.get("type") not in self.summarize_nodes:
                 continue
+            if data.get("checksum") is None:
+                raise RagdaemonError(f"Node {node} missing checksum.")
             if data.get(self.summary_field_id) is None:
                 return False
-            document, context = get_document_and_context(
-                node,
-                graph,
-                summary_field_id=self.summary_field_id,
-                model=self.model,
-            )
-            summary_checksum = hash_str(document + context)
+            # Checksum used to be hash_str(document + context) using the above method. This is
+            # technically more correct, because the summary context includes adjacent summaries
+            # so the whole system updates iteratively. In practice it was just too much looping
+            # so for now we just reuse the checksum generated in hierarchy (hash_str(document)).
+            summary_checksum = data["checksum"]
             if summary_checksum != data.get(self.checksum_field_id):
                 return False
         return True
 
     async def generate_summary(
         self,
         node: str,
@@ -232,25 +231,25 @@
         loading_bar: Optional[tqdm] = None,
         refresh: str | bool = False,
     ):
         """Asynchronously generate summary and update graph"""
         if self.spice_client is None:
             raise RagdaemonError("Spice client not initialized")
 
-        document, context = get_document_and_context(
-            node, graph, summary_field_id=self.summary_field_id, model=self.model
-        )
-        summary_checksum = hash_str(document + context)
         data = graph.nodes[node]
+        summary_checksum = data["checksum"]
         _refresh = match_refresh(refresh, node)
         if (
             _refresh
             or data.get(self.summary_field_id) is None
             or summary_checksum != data.get(self.checksum_field_id)
         ):
+            document, context = get_document_and_context(
+                node, graph, summary_field_id=self.summary_field_id, model=self.model
+            )
             subprompt = "root" if node == "ROOT" else data.get("type", "")
             previous_summary = "" if _refresh else data.get(self.summary_field_id, "")
 
             messages = SpiceMessages(self.spice_client)
             messages.add_system_prompt(
                 name=f"summarizer.{subprompt}", previous_summary=previous_summary
             )
```

### Comparing `ragdaemon-0.5.3/ragdaemon/database/__init__.py` & `ragdaemon-0.5.4/ragdaemon/database/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/ragdaemon/database/chroma_database.py` & `ragdaemon-0.5.4/ragdaemon/database/chroma_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/ragdaemon/database/database.py` & `ragdaemon-0.5.4/ragdaemon/database/database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/ragdaemon/database/lite_database.py` & `ragdaemon-0.5.4/ragdaemon/database/lite_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/ragdaemon/prompts/call_graph.toml` & `ragdaemon-0.5.4/ragdaemon/prompts/call_graph.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/ragdaemon/prompts/chunker_llm.toml` & `ragdaemon-0.5.4/ragdaemon/prompts/chunker_llm.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/ragdaemon/prompts/locate.toml` & `ragdaemon-0.5.4/ragdaemon/prompts/locate.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/ragdaemon/prompts/summarizer/base.txt` & `ragdaemon-0.5.4/ragdaemon/prompts/summarizer/base.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/ragdaemon/prompts/summarizer/chunk.txt` & `ragdaemon-0.5.4/ragdaemon/prompts/summarizer/chunk.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/ragdaemon/prompts/summarizer/directory.txt` & `ragdaemon-0.5.4/ragdaemon/prompts/summarizer/directory.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/ragdaemon/prompts/summarizer/file.txt` & `ragdaemon-0.5.4/ragdaemon/prompts/summarizer/file.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/ragdaemon/prompts/summarizer/root.txt` & `ragdaemon-0.5.4/ragdaemon/prompts/summarizer/root.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/ragdaemon/static/favicon.ico` & `ragdaemon-0.5.4/ragdaemon/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/ragdaemon/static/js/controlPanel.js` & `ragdaemon-0.5.4/ragdaemon/static/js/controlPanel.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/ragdaemon/static/js/main.js` & `ragdaemon-0.5.4/ragdaemon/static/js/main.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/ragdaemon/static/js/three/edge.js` & `ragdaemon-0.5.4/ragdaemon/static/js/three/edge.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/ragdaemon/static/js/three/node.js` & `ragdaemon-0.5.4/ragdaemon/static/js/three/node.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/ragdaemon/static/js/three/raycaster.js` & `ragdaemon-0.5.4/ragdaemon/static/js/three/raycaster.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/ragdaemon/templates/index.html` & `ragdaemon-0.5.4/ragdaemon/templates/index.html`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/tests/conftest.py` & `ragdaemon-0.5.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/tests/test_comments.py` & `ragdaemon-0.5.4/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/tests/test_context.py` & `ragdaemon-0.5.4/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/tests/test_daemon.py` & `ragdaemon-0.5.4/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/tests/test_get_paths.py` & `ragdaemon-0.5.4/tests/test_get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/tests/test_sample.py` & `ragdaemon-0.5.4/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/tests/annotators/test_chunker.py` & `ragdaemon-0.5.4/tests/annotators/test_chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/tests/annotators/test_chunker_llm.py` & `ragdaemon-0.5.4/tests/annotators/test_chunker_llm.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/tests/annotators/test_diff.py` & `ragdaemon-0.5.4/tests/annotators/test_diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/tests/annotators/test_hierarchy.py` & `ragdaemon-0.5.4/tests/annotators/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/tests/annotators/test_layout_hierarchy.py` & `ragdaemon-0.5.4/tests/annotators/test_layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/tests/annotators/test_summarizer.py` & `ragdaemon-0.5.4/tests/annotators/test_summarizer.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/tests/data/chunker_graph.json` & `ragdaemon-0.5.4/tests/data/chunker_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/tests/data/context_message.txt` & `ragdaemon-0.5.4/tests/data/context_message.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/tests/data/diff_graph.json` & `ragdaemon-0.5.4/tests/data/diff_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/tests/data/hard_to_chunk.txt` & `ragdaemon-0.5.4/tests/data/hard_to_chunk.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/tests/data/hierarchy_graph.json` & `ragdaemon-0.5.4/tests/data/hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/tests/data/layout_hierarchy_graph.json` & `ragdaemon-0.5.4/tests/data/layout_hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/tests/data/summarizer_graph.json` & `ragdaemon-0.5.4/tests/data/summarizer_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/tests/sample/src/interface.py` & `ragdaemon-0.5.4/tests/sample/src/interface.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/LICENSE` & `ragdaemon-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/README.md` & `ragdaemon-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.3/pyproject.toml` & `ragdaemon-0.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages=["ragdaemon"]
 
 [project]
 name = "ragdaemon"
-version = "0.5.3"
+version = "0.5.4"
 description = "Generate and render a call graph for a Python project."
 readme = "README.md"
 dependencies = [
     "chromadb==0.4.24",
     "dict2xml==1.7.5",
     "fastapi==0.109.2",
     "Jinja2==3.1.3",
```

### Comparing `ragdaemon-0.5.3/PKG-INFO` & `ragdaemon-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragdaemon
-Version: 0.5.3
+Version: 0.5.4
 Summary: Generate and render a call graph for a Python project.
 Project-URL: Homepage, https://github.com/AbanteAI/ragdaemon
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

