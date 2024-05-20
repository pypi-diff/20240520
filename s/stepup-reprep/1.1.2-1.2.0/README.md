# Comparing `tmp/stepup_reprep-1.1.2.tar.gz` & `tmp/stepup_reprep-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stepup_reprep-1.1.2.tar", last modified: Thu May 16 11:29:58 2024, max compression
+gzip compressed data, was "stepup_reprep-1.2.0.tar", last modified: Mon May 20 13:32:39 2024, max compression
```

## Comparing `stepup_reprep-1.1.2.tar` & `stepup_reprep-1.2.0.tar`

### file list

```diff
@@ -1,366 +1,357 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.627519 stepup_reprep-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.563519 stepup_reprep-1.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.571519 stepup_reprep-1.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/.github/workflows/mkdocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-16 11:29:58.627519 stepup_reprep-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.571519 stepup_reprep-1.1.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.575519 stepup_reprep-1.1.2/docs/advanced_topics/
--rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/advanced_topics/good_practices.md
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/advanced_topics/manifest_files.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.575519 stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    22692 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs/figure.png
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs/hexagon.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)      114 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs/pentagon.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)      278 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs/square.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs/stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      413 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs/tile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs/triangle.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs.md
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/clean_stdout.sed
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/development.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.575519 stepup_reprep-1.1.2/docs/from_scratch/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/from_scratch/introduction.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.575519 stepup_reprep-1.1.2/docs/from_template/
--rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/from_template/before_you_begin.md
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/from_template/create_or_clone_a_project.md
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/from_template/introduction.md
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/from_template/working_on_a_project.md
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/license.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.575519 stepup_reprep-1.1.2/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/reference/stepup.reprep.api.md
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/reference/stepup.reprep.tile_pdf.md
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 11:29:58.627519 stepup_reprep-1.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.567519 stepup_reprep-1.1.2/stepup/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.579519 stepup_reprep-1.1.2/stepup/reprep/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/add_notes_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    25407 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/bibtex_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/check_hrefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/check_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/convert_inkscape.py
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/convert_markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/latex.py
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/latex_deps.py
--rw-r--r--   0 runner    (1001) docker     (127)     7006 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/latex_flat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/latex_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/make_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/normalize_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/nup_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/pytest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/raster_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/render.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/tile_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/zip_manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.627519 stepup_reprep-1.1.2/stepup_reprep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-16 11:29:58.000000 stepup_reprep-1.1.2/stepup_reprep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12175 2024-05-16 11:29:58.000000 stepup_reprep-1.1.2/stepup_reprep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 11:29:58.000000 stepup_reprep-1.1.2/stepup_reprep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-16 11:29:58.000000 stepup_reprep-1.1.2/stepup_reprep.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-16 11:29:58.000000 stepup_reprep-1.1.2/stepup_reprep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 11:29:58.000000 stepup_reprep-1.1.2/stepup_reprep.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.583519 stepup_reprep-1.1.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.571519 stepup_reprep-1.1.2/tests/cases/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.583519 stepup_reprep-1.1.2/tests/cases/add_notes_pdf/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/add_notes_pdf/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/add_notes_pdf/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/add_notes_pdf/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/add_notes_pdf/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1108 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/add_notes_pdf/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/add_notes_pdf/notes.pdf
--rwxr-xr-x   0 runner    (1001) docker     (127)      182 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/add_notes_pdf/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/add_notes_pdf/src.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.583519 stepup_reprep-1.1.2/tests/cases/cat_pdf/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/cat_pdf/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/cat_pdf/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/cat_pdf/doc1.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/cat_pdf/doc2.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/cat_pdf/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/cat_pdf/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1108 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/cat_pdf/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      172 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/cat_pdf/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.587519 stepup_reprep-1.1.2/tests/cases/check_hrefs_html/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_html/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_html/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_html/check_hrefs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_html/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_html/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      749 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_html/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_html/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_html/test.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.587519 stepup_reprep-1.1.2/tests/cases/check_hrefs_md/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_md/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_md/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_md/check_hrefs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_md/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_md/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      749 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_md/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      174 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_md/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_md/test.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.587519 stepup_reprep-1.1.2/tests/cases/check_hrefs_pdf/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_pdf/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_pdf/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_pdf/check_hrefs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_pdf/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_pdf/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      881 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_pdf/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_pdf/main.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      202 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_pdf/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.591519 stepup_reprep-1.1.2/tests/cases/convert_inkscape/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape/expected_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape/glasses.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1332 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      244 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape/smile.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.595519 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_050.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_055.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_060.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_065.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_070.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_075.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_080.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_085.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_090.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_095.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_100.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_105.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_110.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_115.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_120.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5907 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_125.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_130.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_135.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_140.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_145.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2045 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      163 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.595519 stepup_reprep-1.1.2/tests/cases/convert_libreoffice/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_libreoffice/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_libreoffice/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_libreoffice/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_libreoffice/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1141 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_libreoffice/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      153 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_libreoffice/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)    13660 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_libreoffice/slide.odp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.595519 stepup_reprep-1.1.2/tests/cases/convert_libreoffice_concurrency/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_libreoffice_concurrency/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)     2039 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_libreoffice_concurrency/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      242 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_libreoffice_concurrency/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)    10286 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_libreoffice_concurrency/something.odt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.599519 stepup_reprep-1.1.2/tests/cases/convert_markdown/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_markdown/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_markdown/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_markdown/demo.md
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_markdown/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_markdown/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1129 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_markdown/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      151 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_markdown/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.599519 stepup_reprep-1.1.2/tests/cases/convert_mutool/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_mutool/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_mutool/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_mutool/example.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_mutool/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_mutool/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1110 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_mutool/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      173 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_mutool/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.599519 stepup_reprep-1.1.2/tests/cases/convert_weasyprint/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_weasyprint/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_weasyprint/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_weasyprint/doc.html
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_weasyprint/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_weasyprint/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1116 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_weasyprint/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      157 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_weasyprint/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.603519 stepup_reprep-1.1.2/tests/cases/latex_diff/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_diff/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_diff/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_diff/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_diff/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1057 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_diff/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_diff/new.tex
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_diff/old.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      173 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_diff/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.603519 stepup_reprep-1.1.2/tests/cases/latex_flat/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat/article_structured.tex
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat/expected_article.tex
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1423 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat/part1.tex
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat/part2.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat/plan_01.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      249 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat/plan_02.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.603519 stepup_reprep-1.1.2/tests/cases/latex_flat/sub/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat/sub/original.tex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.603519 stepup_reprep-1.1.2/tests/cases/latex_flat_subdir/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat_subdir/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat_subdir/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat_subdir/expected_article.tex
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat_subdir/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat_subdir/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      877 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat_subdir/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      238 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat_subdir/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.607519 stepup_reprep-1.1.2/tests/cases/latex_flat_subdir/sub/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat_subdir/sub/article_structured.tex
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat_subdir/sub/part1.tex
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat_subdir/sub/part2.tex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.607519 stepup_reprep-1.1.2/tests/cases/lualatex_simple/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/lualatex_simple/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/lualatex_simple/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/lualatex_simple/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1256 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/lualatex_simple/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/lualatex_simple/paper.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      134 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/lualatex_simple/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.607519 stepup_reprep-1.1.2/tests/cases/make_manifest_in/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_in/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_in/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_in/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_in/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_in/expected_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_in/hello.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      787 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_in/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      180 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_in/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.611519 stepup_reprep-1.1.2/tests/cases/make_manifest_in_sub/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_in_sub/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_in_sub/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_in_sub/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_in_sub/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      838 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_in_sub/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      187 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_in_sub/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.611519 stepup_reprep-1.1.2/tests/cases/make_manifest_in_sub/sub/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_in_sub/sub/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_in_sub/sub/hello.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.611519 stepup_reprep-1.1.2/tests/cases/make_manifest_list/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_list/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_list/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_list/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_list/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      787 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_list/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      166 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_list/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.611519 stepup_reprep-1.1.2/tests/cases/nup_pdf/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/nup_pdf/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/nup_pdf/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/nup_pdf/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/nup_pdf/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1078 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/nup_pdf/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/nup_pdf/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     9122 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/nup_pdf/src.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.615519 stepup_reprep-1.1.2/tests/cases/pdflatex_bbl/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_bbl/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_bbl/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_bbl/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1224 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_bbl/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_bbl/paper.bbl
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_bbl/paper.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      172 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_bbl/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.615519 stepup_reprep-1.1.2/tests/cases/pdflatex_bibtex/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_bibtex/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_bibtex/bibsane.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_bibtex/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_bibtex/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1503 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_bibtex/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_bibtex/paper.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      190 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_bibtex/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_bibtex/references.bib
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.615519 stepup_reprep-1.1.2/tests/cases/pdflatex_input/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_input/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_input/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_input/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1269 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_input/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_input/paper.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      224 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_input/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_input/smile.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.619520 stepup_reprep-1.1.2/tests/cases/raster_pdf/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/raster_pdf/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/raster_pdf/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/raster_pdf/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/raster_pdf/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1157 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/raster_pdf/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      181 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/raster_pdf/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/raster_pdf/smile.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.619520 stepup_reprep-1.1.2/tests/cases/render_basic/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_basic/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_basic/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_basic/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_basic/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      849 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_basic/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      188 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_basic/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_basic/template.md
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_basic/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.619520 stepup_reprep-1.1.2/tests/cases/render_relpath/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_relpath/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     9195 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_relpath/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_relpath/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1084 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_relpath/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      270 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_relpath/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.619520 stepup_reprep-1.1.2/tests/cases/render_relpath/static/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_relpath/static/main.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      213 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_relpath/static/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_relpath/static/preamble.inc.tex
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_relpath/static/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_relpath/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.623520 stepup_reprep-1.1.2/tests/cases/tile_pdf/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/tile_pdf/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/tile_pdf/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    15675 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/tile_pdf/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/tile_pdf/expected_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/tile_pdf/hexagon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/tile_pdf/horizontal.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1526 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/tile_pdf/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/tile_pdf/pentagon.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)      227 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/tile_pdf/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/tile_pdf/square.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)      674 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/tile_pdf/tile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/tile_pdf/triangle.svg
--rw-r--r--   0 runner    (1001) docker     (127)    65932 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/tile_pdf/vera.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/tile_pdf/vertical.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.623520 stepup_reprep-1.1.2/tests/cases/xelatex_input/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/xelatex_input/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/xelatex_input/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/xelatex_input/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1370 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/xelatex_input/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/xelatex_input/paper.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      348 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/xelatex_input/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/xelatex_input/smile.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.627519 stepup_reprep-1.1.2/tests/cases/zip_manifest/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/zip_manifest/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/zip_manifest/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/zip_manifest/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/zip_manifest/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1147 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/zip_manifest/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      290 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/zip_manifest/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/zip_manifest/static.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/reprep_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/test_bibtex_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/test_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/test_latex_deps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/test_latex_flat.py
--rw-r--r--   0 runner    (1001) docker     (127)    14002 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/test_latex_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/test_zip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.018039 stepup_reprep-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.966039 stepup_reprep-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.974039 stepup_reprep-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/.github/workflows/mkdocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-20 13:32:39.018039 stepup_reprep-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.974039 stepup_reprep-1.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.974039 stepup_reprep-1.2.0/docs/advanced_topics/
+-rw-r--r--   0 runner    (1001) docker     (127)     7573 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/advanced_topics/archive_git.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/advanced_topics/good_practices.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/advanced_topics/inventory_files.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.978039 stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    22692 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs/figure.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs/hexagon.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      114 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs/pentagon.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      278 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs/square.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs/stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      413 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs/tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs/triangle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/clean_stdout.sed
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/development.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.978039 stepup_reprep-1.2.0/docs/from_scratch/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/from_scratch/introduction.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.978039 stepup_reprep-1.2.0/docs/from_template/
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/from_template/before_you_begin.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/from_template/create_or_clone_a_project.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/from_template/introduction.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/from_template/working_on_a_project.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/license.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.978039 stepup_reprep-1.2.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/reference/stepup.reprep.api.md
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/docs/reference/stepup.reprep.tile_pdf.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 13:32:39.018039 stepup_reprep-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.966039 stepup_reprep-1.2.0/stepup/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.982039 stepup_reprep-1.2.0/stepup/reprep/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/add_notes_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24955 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/bibtex_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/check_hrefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/check_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/convert_inkscape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/convert_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/latex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/latex_deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7006 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/latex_flat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/latex_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7184 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/make_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/normalize_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/nup_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/pytest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/raster_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/tile_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/stepup/reprep/zip_inventory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.018039 stepup_reprep-1.2.0/stepup_reprep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-20 13:32:38.000000 stepup_reprep-1.2.0/stepup_reprep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11921 2024-05-20 13:32:38.000000 stepup_reprep-1.2.0/stepup_reprep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:32:38.000000 stepup_reprep-1.2.0/stepup_reprep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-20 13:32:38.000000 stepup_reprep-1.2.0/stepup_reprep.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-20 13:32:38.000000 stepup_reprep-1.2.0/stepup_reprep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 13:32:38.000000 stepup_reprep-1.2.0/stepup_reprep.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.982039 stepup_reprep-1.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.970039 stepup_reprep-1.2.0/tests/cases/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.982039 stepup_reprep-1.2.0/tests/cases/add_notes_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/add_notes_pdf/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/add_notes_pdf/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/add_notes_pdf/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/add_notes_pdf/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1113 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/add_notes_pdf/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/add_notes_pdf/notes.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (127)      182 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/add_notes_pdf/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/add_notes_pdf/src.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.986039 stepup_reprep-1.2.0/tests/cases/cat_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/cat_pdf/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/cat_pdf/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/cat_pdf/doc1.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/cat_pdf/doc2.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/cat_pdf/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/cat_pdf/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1113 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/cat_pdf/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      172 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/cat_pdf/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/cat_pdf/reproducibility_inventory.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.986039 stepup_reprep-1.2.0/tests/cases/check_hrefs_html/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_html/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_html/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_html/check_hrefs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_html/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_html/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      749 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_html/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_html/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_html/test.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.986039 stepup_reprep-1.2.0/tests/cases/check_hrefs_md/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_md/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_md/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_md/check_hrefs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_md/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_md/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      749 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_md/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      174 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_md/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_md/test.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.990039 stepup_reprep-1.2.0/tests/cases/check_hrefs_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_pdf/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_pdf/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_pdf/check_hrefs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_pdf/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_pdf/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      883 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_pdf/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_pdf/main.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      202 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/check_hrefs_pdf/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.990039 stepup_reprep-1.2.0/tests/cases/convert_inkscape/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape/glasses.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1340 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      244 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape/smile.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.994039 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_050.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_055.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_060.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_065.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_070.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_075.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_080.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_085.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_090.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_095.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_100.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_105.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_110.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_115.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_120.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5907 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_125.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_130.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_135.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_140.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_145.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2045 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      163 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.994039 stepup_reprep-1.2.0/tests/cases/convert_libreoffice/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_libreoffice/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_libreoffice/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_libreoffice/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_libreoffice/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1146 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_libreoffice/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      153 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_libreoffice/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13660 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_libreoffice/slide.odp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.994039 stepup_reprep-1.2.0/tests/cases/convert_libreoffice_concurrency/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_libreoffice_concurrency/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2039 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_libreoffice_concurrency/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      242 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_libreoffice_concurrency/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10286 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_libreoffice_concurrency/something.odt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.998039 stepup_reprep-1.2.0/tests/cases/convert_markdown/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_markdown/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_markdown/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_markdown/demo.css
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_markdown/demo.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_markdown/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_markdown/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_markdown/macros.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1134 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_markdown/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      202 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_markdown/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.998039 stepup_reprep-1.2.0/tests/cases/convert_mutool/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_mutool/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_mutool/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_mutool/example.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_mutool/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_mutool/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1115 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_mutool/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      173 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_mutool/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_mutool/reproducibility_inventory.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.998039 stepup_reprep-1.2.0/tests/cases/convert_weasyprint/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_weasyprint/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_weasyprint/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_weasyprint/doc.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_weasyprint/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_weasyprint/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1121 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_weasyprint/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      157 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/convert_weasyprint/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:38.998039 stepup_reprep-1.2.0/tests/cases/latex_diff/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_diff/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_diff/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_diff/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_diff/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1062 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_diff/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_diff/new.tex
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_diff/old.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      173 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_diff/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.002039 stepup_reprep-1.2.0/tests/cases/latex_flat/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat/article_structured.tex
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat/expected_article.tex
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1442 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat/part1.tex
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat/part2.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat/plan_01.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      249 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat/plan_02.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.002039 stepup_reprep-1.2.0/tests/cases/latex_flat/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat/sub/original.tex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.002039 stepup_reprep-1.2.0/tests/cases/latex_flat_subdir/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat_subdir/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat_subdir/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat_subdir/expected_article.tex
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat_subdir/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat_subdir/expected_inventory.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat_subdir/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat_subdir/inventory.def
+-rwxr-xr-x   0 runner    (1001) docker     (127)      969 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat_subdir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      238 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat_subdir/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.002039 stepup_reprep-1.2.0/tests/cases/latex_flat_subdir/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat_subdir/sub/article_structured.tex
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat_subdir/sub/part1.tex
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/latex_flat_subdir/sub/part2.tex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.006039 stepup_reprep-1.2.0/tests/cases/lualatex_simple/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/lualatex_simple/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/lualatex_simple/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/lualatex_simple/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1263 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/lualatex_simple/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/lualatex_simple/paper.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      134 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/lualatex_simple/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.006039 stepup_reprep-1.2.0/tests/cases/make_inventory_list/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/make_inventory_list/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/make_inventory_list/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/make_inventory_list/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/make_inventory_list/expected_inventory.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/make_inventory_list/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      790 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/make_inventory_list/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      171 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/make_inventory_list/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.006039 stepup_reprep-1.2.0/tests/cases/nup_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/nup_pdf/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/nup_pdf/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/nup_pdf/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/nup_pdf/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1083 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/nup_pdf/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/nup_pdf/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/nup_pdf/reproducibility_inventory.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9122 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/nup_pdf/src.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.006039 stepup_reprep-1.2.0/tests/cases/pdflatex_bbl/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_bbl/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_bbl/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_bbl/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1231 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_bbl/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_bbl/paper.bbl
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_bbl/paper.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      172 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_bbl/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.010039 stepup_reprep-1.2.0/tests/cases/pdflatex_bibtex/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_bibtex/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_bibtex/bibsane.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_bibtex/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_bibtex/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1513 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_bibtex/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_bibtex/paper.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      190 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_bibtex/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_bibtex/references.bib
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.010039 stepup_reprep-1.2.0/tests/cases/pdflatex_input/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_input/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_input/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_input/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1276 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_input/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_input/paper.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      224 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_input/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/pdflatex_input/smile.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.010039 stepup_reprep-1.2.0/tests/cases/raster_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/raster_pdf/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/raster_pdf/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/raster_pdf/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/raster_pdf/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1162 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/raster_pdf/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      181 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/raster_pdf/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/raster_pdf/smile.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.010039 stepup_reprep-1.2.0/tests/cases/render_basic/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_basic/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_basic/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_basic/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_basic/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      849 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_basic/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      188 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_basic/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_basic/template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_basic/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.014039 stepup_reprep-1.2.0/tests/cases/render_relpath/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_relpath/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_relpath/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_relpath/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1084 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_relpath/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      270 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_relpath/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.014039 stepup_reprep-1.2.0/tests/cases/render_relpath/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_relpath/static/main.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      213 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_relpath/static/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_relpath/static/preamble.inc.tex
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_relpath/static/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/render_relpath/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.014039 stepup_reprep-1.2.0/tests/cases/tile_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/tile_pdf/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/tile_pdf/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    15675 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/tile_pdf/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/tile_pdf/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/tile_pdf/hexagon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/tile_pdf/horizontal.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1531 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/tile_pdf/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/tile_pdf/pentagon.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      227 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/tile_pdf/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/tile_pdf/square.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      674 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/tile_pdf/tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/tile_pdf/triangle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    65932 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/tile_pdf/vera.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/tile_pdf/vertical.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.014039 stepup_reprep-1.2.0/tests/cases/xelatex_input/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/xelatex_input/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/xelatex_input/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/xelatex_input/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1377 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/xelatex_input/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/xelatex_input/paper.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      348 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/xelatex_input/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/xelatex_input/smile.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:32:39.018039 stepup_reprep-1.2.0/tests/cases/zip_inventory/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/zip_inventory/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/zip_inventory/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/zip_inventory/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/zip_inventory/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1153 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/zip_inventory/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      296 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/zip_inventory/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/cases/zip_inventory/static.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/reprep_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/test_bibtex_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/test_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/test_latex_deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/test_latex_flat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14002 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/test_latex_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-20 13:32:23.000000 stepup_reprep-1.2.0/tests/test_zip.py
```

### Comparing `stepup_reprep-1.1.2/.github/workflows/release.yaml` & `stepup_reprep-1.2.0/.github/workflows/release.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     steps:
     - name: Download all the dists
       uses: actions/download-artifact@v4
       with:
         name: python-package-distributions
         path: dist/
     - name: Sign the dists with Sigstore
-      uses: sigstore/gh-action-sigstore-python@v2
+      uses: sigstore/gh-action-sigstore-python@v2.1.1
       with:
         inputs: >-
           ./dist/*.tar.gz
           ./dist/*.whl
     - name: Create GitHub Release
       env:
         GITHUB_TOKEN: ${{ github.token }}
```

### Comparing `stepup_reprep-1.1.2/.pre-commit-config.yaml` & `stepup_reprep-1.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/LICENSE` & `stepup_reprep-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/PKG-INFO` & `stepup_reprep-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stepup-reprep
-Version: 1.1.2
+Version: 1.2.0
 Summary: StepUp RepRep is the StepUp extension for Reproducible Reporting
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 Project-URL: Documentation, https://reproducible-reporting.github.io/stepup-reprep/
 Project-URL: Issues, https://github.com/reproducible-reporting/stepup-reprep/issues
 Project-URL: Source, https://github.com/reproducible-reporting/stepup-reprep/
 Project-URL: Changelog, https://reproducible-reporting.github.io/stepup-reprep/changelog/
 Classifier: Environment :: Console
@@ -24,16 +24,15 @@
 Requires-Dist: markdown
 Requires-Dist: markdown_katex
 Requires-Dist: numpy
 Requires-Dist: path
 Requires-Dist: pymupdf
 Requires-Dist: pyyaml
 Requires-Dist: scipy
-Requires-Dist: setuptools
-Requires-Dist: stepup>=1.2.2
+Requires-Dist: stepup>=1.2.3
 Requires-Dist: weasyprint
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
```

### Comparing `stepup_reprep-1.1.2/README.md` & `stepup_reprep-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/docs/advanced_topics/good_practices.md` & `stepup_reprep-1.2.0/docs/advanced_topics/good_practices.md`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 ### Should
 
 - Some packages, like `todo`, are convenient while writing.
   Clearly separate these from other `\usepackage` lines, so they can be easily deleted
   when finalizing the manuscript.
 - Define as few commands as possible.
 - Avoid low-quality publisher article classes. (ACS has a decent one.)
-- Avoid `\subfigure`. Merge panels into one PDF instead. (See [Tiling PDFs](tiling_pdfs.md).)
+- Avoid `\subfigure`. Merge panels into one PDF instead. (See [Tile PDFs](tile_pdfs.md).)
 
 
 ## Figures
 
 ### Must
 
 - Separate data generation or collection from actual plotting:
```

### Comparing `stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs/figure.png` & `stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs/figure.png`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs/hexagon.svg` & `stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs/hexagon.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs/pentagon.svg` & `stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs/pentagon.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs/square.svg` & `stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs/square.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs/stdout.txt` & `stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs/triangle.svg` & `stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs/triangle.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs.md` & `stepup_reprep-1.2.0/docs/advanced_topics/tile_pdfs.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-# Tiling PDFs
+# Tile PDFs
 
-StepUp RepRep includes a tool for tiling panels (individual PDF figures) into a composite PDF figure.
+StepUp RepRep includes a tool to tile panels (individual PDF figures) into a composite PDF figure.
 
 The tiling code is based on the *script protocol* in StepUp Core,
 which is explained in the [StepUp Core "Getting Started" tutorials](https://reproducible-reporting.github.io/stepup-core/getting_started/introduction/).
 
 This tutorial provides a simple example that you can use as a starting point.
 For a more advanced example, see the [`tild_pdf` test case](https://github.com/reproducible-reporting/stepup-reprep/tree/main/tests/cases/tile_pdf) in the StepUp RepRep unit test suite.
 
 
 ## Example
 
-Example source files: [tutorials/tiling_pdfs/](https://github.com/reproducible-reporting/stepup-reprep/tree/main/docs/advanced_topics/tiling_pdfs)
+Example source files: [tutorials/tile_pdfs/](https://github.com/reproducible-reporting/stepup-reprep/tree/main/docs/advanced_topics/tile_pdfs)
 
 Create a `tile.py` script with the following code:
 
 ```python
-{% include 'advanced_topics/tiling_pdfs/tile.py' %}
+{% include 'advanced_topics/tile_pdfs/tile.py' %}
 ```
 
 Next, create a script `plan.py` as follows:
 
 ```python
-{% include 'advanced_topics/tiling_pdfs/plan.py' %}
+{% include 'advanced_topics/tile_pdfs/plan.py' %}
 ```
 
 For this example to work, you also need to create four SVG figures of the same size: `triangle.svg`, `square.svg`, `pentagon.svg` and  `hexagon.svg`.
 
 To run the example, make the scripts executable and run StepUp:
 
 ```bash
 chmod +x plan.py tile.py
 stepup -n -w1
 ```
 
 You should see the following terminal output:
 
 ```
-{% include 'advanced_topics/tiling_pdfs/stdout.txt' %}
+{% include 'advanced_topics/tile_pdfs/stdout.txt' %}
 ```
 
 This is the PNG conversion of the resulting PDF figure:
 
-![figure](tiling_pdfs/figure.png)
+![figure](tile_pdfs/figure.png)
```

### Comparing `stepup_reprep-1.1.2/docs/changelog.md` & `stepup_reprep-1.2.0/docs/changelog.md`

 * *Files 24% similar despite different names*

```diff
@@ -3,14 +3,39 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [1.2.0] - 2024-05-20
+
+### Added
+
+- `reprep-zip-inventory` command to manually create a reproducible ZIP file from an `inventory.txt` file.
+- More documentation on how to work with inventory files.
+- Tutorial for archiving StepUp publication Git repositories.
+
+### Changed
+
+- Renamed all `MANIFEST` and `manifest` occurrences to `inventory`
+  and removed dependency of setuptools for processing such files.
+- The API of `make_inventory` is made simpler than that of `make_manifest`.
+- The commands supported in `inventory.def` files now differ from those in setuptools:
+  `include`, `exclude`, `include-git`, `exclude-git`, `include-workflow` and `exclude-workflow`.
+- The css style has been made customizable in `convert_markdown`.
+- KaTeX is now optional in `convert_markdown`.
+
+### Fixed
+
+- An error message is raised when trying to a put a directory in an inventory file.
+- Symbolic links are no longer dereferenced when they are listed in an inventory file.
+- Symbolic links are archived in ZIP files without dereferencing.
+
+
 ## [1.1.2] - 2024-05-16
 
 ### Fixed
 
 - Nicer fix for concurrent Inkscape SVG to PDF or PNG conversion
   (with `SELF_CALL=x`).
   See: https://gitlab.com/inkscape/inkscape/-/issues/4716
```

### Comparing `stepup_reprep-1.1.2/docs/development.md` & `stepup_reprep-1.2.0/docs/development.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/docs/from_template/before_you_begin.md` & `stepup_reprep-1.2.0/docs/from_template/before_you_begin.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/docs/from_template/create_or_clone_a_project.md` & `stepup_reprep-1.2.0/docs/from_template/create_or_clone_a_project.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/docs/from_template/introduction.md` & `stepup_reprep-1.2.0/docs/from_template/introduction.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/docs/from_template/working_on_a_project.md` & `stepup_reprep-1.2.0/docs/from_template/working_on_a_project.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/docs/index.md` & `stepup_reprep-1.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/docs/installation.md` & `stepup_reprep-1.2.0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/docs/license.md` & `stepup_reprep-1.2.0/docs/license.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/mkdocs.yml` & `stepup_reprep-1.2.0/mkdocs.yml`

 * *Files 6% similar despite different names*

```diff
@@ -42,17 +42,18 @@
     - from_template/introduction.md
     - from_template/before_you_begin.md
     - from_template/create_or_clone_a_project.md
     - from_template/working_on_a_project.md
   - From Scratch:
     - from_scratch/introduction.md
   - Advanced Topics:
-    - advanced_topics/manifest_files.md
-    - advanced_topics/tiling_pdfs.md
+    - advanced_topics/inventory_files.md
+    - advanced_topics/tile_pdfs.md
     - advanced_topics/good_practices.md
+    - advanced_topics/archive_git.md
   - Reference:
     - reference/stepup.reprep.api.md
     - reference/stepup.reprep.tile_pdf.md
   - changelog.md
   - development.md
   - license.md
```

### Comparing `stepup_reprep-1.1.2/pyproject.toml` & `stepup_reprep-1.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -28,16 +28,15 @@
     "markdown",
     "markdown_katex",
     "numpy",
     "path",
     "pymupdf",
     "pyyaml",
     "scipy",
-    "setuptools",
-    "stepup>=1.2.2",
+    "stepup>=1.2.3",
     "weasyprint",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
     "pytest",
@@ -52,16 +51,17 @@
 [project.urls]
 Documentation = "https://reproducible-reporting.github.io/stepup-reprep/"
 Issues = "https://github.com/reproducible-reporting/stepup-reprep/issues"
 Source = "https://github.com/reproducible-reporting/stepup-reprep/"
 Changelog = "https://reproducible-reporting.github.io/stepup-reprep/changelog/"
 
 [project.scripts]
-reprep-make-manifest = "stepup.reprep.make_manifest:main"
-reprep-check-manifest = "stepup.reprep.check_manifest:main"
+reprep-check-inventory = "stepup.reprep.check_inventory:main"
+reprep-make-inventory = "stepup.reprep.make_inventory:main"
+reprep-zip-inventory = "stepup.reprep.zip_inventory:main"
 
 [tool.pytest.ini_options]
 addopts = "-n auto"
 
 [tool.black]
 line-length = 100
 target-version = ['py311']
```

### Comparing `stepup_reprep-1.1.2/stepup/reprep/__init__.py` & `stepup_reprep-1.2.0/stepup/reprep/__init__.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/stepup/reprep/add_notes_pdf.py` & `stepup_reprep-1.2.0/stepup/reprep/add_notes_pdf.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/stepup/reprep/api.py` & `stepup_reprep-1.2.0/stepup/reprep/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,19 +36,19 @@
     "convert_pdf_png",
     "convert_svg",
     "convert_svg_pdf",
     "convert_svg_png",
     "latex",
     "latex_diff",
     "latex_flat",
-    "make_manifest",
+    "make_inventory",
     "nup_pdf",
     "raster_pdf",
     "render",
-    "zip_manifest",
+    "zip_inventory",
 )
 
 
 def add_notes_pdf(
     path_src: str, path_notes: str, path_dst: str, optional: bool = False, block: bool = False
 ):
     """Add a notes page at every even page of a PDF file.
@@ -130,45 +130,59 @@
     inp_paths = [path_src]
     if path_config is not None:
         inp_paths.append(path_config)
         command += f" -c {path_config}"
     step(command, inp=inp_paths, block=block)
 
 
-pool("markdown", 1)
+pool("markdown_katex", 1)
 
 
 def convert_markdown(
     path_md: str,
     out: str | None = None,
     *,
+    katex: bool = False,
+    path_macro: str | None = None,
     optional: bool = False,
     block: bool = False,
 ):
     """Convert a markdown to HTML.
 
     Parameters
     ----------
     path_md
         The markdown input file.
     out
         Output destination: `None`, a directory or a file.
+    katex
+        Set to `True` to enable KaTeX support.
+    path_macro
+        A file with macro definitions for KaTeX.
     optional
         When `True`, the step is only executed when needed by other steps.
     block
         When `True`, the step will always remain pending.
     """
     with subs_env_vars() as subs:
         path_md = subs(path_md)
         out = subs(out)
     if not path_md.endswith(".md"):
         raise ValueError("The Markdown file must have extension .md")
     path_html = make_path_out(path_md, out, ".html")
-    command = "python -m stepup.reprep.convert_markdown ${inp} ${out}"
-    step(command, inp=path_md, out=path_html, pool="markdown", optional=optional, block=block)
+    inp = [path_md]
+    command = f"python -m stepup.reprep.convert_markdown {path_md} {path_html}"
+    pool = None
+    if katex:
+        command += " --katex"
+        pool = "markdown_katex"
+        if path_macro is not None:
+            command += f" --katex-macros={path_macro}"
+            inp.append(path_macro)
+    step(command, inp=inp, out=path_html, pool=pool, optional=optional, block=block)
 
 
 def convert_weasyprint(
     path_html: str,
     out: str | None = None,
     *,
     optional: bool = False,
@@ -503,15 +517,15 @@
             command += f" --bibsane={bibsane}"
         if bibsane_config is not None:
             command += f" --bibsane-config={bibsane_config}"
             inp_paths.append(workdir / bibsane_config)
     step(
         command,
         inp=inp_paths,
-        out=[workdir / path_pdf, workdir / f"{prefix}.aux", workdir / f"{prefix}.MANIFEST.txt"],
+        out=[workdir / path_pdf, workdir / f"{prefix}.aux", workdir / f"{prefix}-inventory.txt"],
         workdir=workdir,
         optional=optional,
         block=block,
     )
     return workdir / path_pdf
 
 
@@ -594,54 +608,37 @@
         inp=path_tex,
         out=path_flat,
         optional=optional,
         block=block,
     )
 
 
-def make_manifest(
-    path_manifest: str, paths: Collection[str] = (), *, optional: bool = False, block: bool = False
+def make_inventory(
+    paths: Collection[str], path_inventory: str, *, optional: bool = False, block: bool = False
 ):
-    """Create a `MANIFEST.txt` file.
+    """Create an `inventory.txt` file.
 
     Parameters
     ----------
-    path_manifest
-        This can be either a `MANIFEST.in` file, in which case it is processed and a corresponding
-        `MANIFEST.out` is created. The same syntax is used as in setuptools.
-        See https://setuptools.pypa.io/en/latest/userguide/miscellaneous.html
-        The other option is to provide a `MANIFEST.txt` file, which serves as output.
-        In this case, no `MANIFEST.in` is processed.
-        The distinction between the two is based on the file extension.
     paths
-        (Additional) paths to include in the `MANIFEST.txt` file.
+        Paths to include in the `inventory.txt` file.
+    path_inventory
+        The inventory file to write.
     optional
         When `True`, the step is only executed when needed by other steps.
     block
         When `True`, the step will always remain pending.
     """
-    if path_manifest.endswith(".in"):
-        path_txt = path_manifest[:-3] + ".txt"
-        step(
-            "reprep-make-manifest -i ${inp}",
-            inp=[path_manifest, *paths],
-            out=[path_txt],
-            optional=optional,
-            block=block,
-        )
-    elif path_manifest.endswith(".txt"):
-        step(
-            "reprep-make-manifest ${inp} -o ${out}",
-            inp=paths,
-            out=[path_manifest],
-            optional=optional,
-            block=block,
-        )
-    else:
-        raise ValueError("The path_manifest argument must either have the .in or .txt suffix")
+    step(
+        "reprep-make-inventory ${inp} -o ${out}",
+        inp=paths,
+        out=[path_inventory],
+        optional=optional,
+        block=block,
+    )
 
 
 def nup_pdf(
     path_src: str,
     path_dst: str,
     *,
     nrow: int | None = None,
@@ -768,29 +765,31 @@
         inp=[path_template, *paths_variables],
         out=path_out,
         optional=optional,
         block=block,
     )
 
 
-def zip_manifest(path_manifest: str, path_zip: str, *, optional: bool = False, block: bool = False):
-    """Create a ZIP file with all files listed in a `MANIFEST.txt` file + check digests before zip.
+def zip_inventory(
+    path_inventory: str, path_zip: str, *, optional: bool = False, block: bool = False
+):
+    """Create a ZIP file with all files listed in a `inventory.txt` file + check digests before zip.
 
     Parameters
     ----------
-    path_manifest
-        A file created with the `make_manifest` API or with the command-line script
-        `reprep-make-manifest`.
+    path_inventory
+        A file created with the `make_inventory` API or with the command-line script
+        `reprep-make-inventory`.
     path_zip
         The output ZIP file
     optional
         When `True`, the step is only executed when needed by other steps.
     block
         When `True`, the step will always remain pending.
     """
     step(
-        "python -m stepup.reprep.zip_manifest ${inp} ${out}",
-        inp=path_manifest,
+        "python -m stepup.reprep.zip_inventory ${inp} ${out}",
+        inp=path_inventory,
         out=path_zip,
         optional=optional,
         block=block,
     )
```

### Comparing `stepup_reprep-1.1.2/stepup/reprep/bibtex_log.py` & `stepup_reprep-1.2.0/stepup/reprep/bibtex_log.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/stepup/reprep/check_hrefs.py` & `stepup_reprep-1.2.0/stepup/reprep/check_hrefs.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/stepup/reprep/convert_inkscape.py` & `stepup_reprep-1.2.0/stepup/reprep/convert_inkscape.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/stepup/reprep/convert_markdown.py` & `stepup_reprep-1.2.0/stepup/reprep/convert_markdown.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,146 +18,104 @@
 #
 # --
 """Markdown to HTML conversion."""
 
 import argparse
 import re
 import sys
-import tempfile
 
 import markdown
 
+from .render import render
+
 __all__ = ("convert_markdown",)
 
 
-HTML_HEADER = """\
+HTML_TEMPLATE = """\
 <!DOCTYPE html>
-<html xmlns="http://www.w3.org/1999/xhtml" lang="" xml:lang="">
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes" />
-  <title>Preview</title>
-  <style>
-    html {
-      line-height: 1.3;
-      font-family: IBM Plex Sans, Georgia, serif;
-      font-size: 10pt;
-    }
-    h1, h2 {
-      margin-top: 1cm;
-      border-bottom: 1pt solid #DDDDDD;
-    }
-    h3, h4, p {
-      margin-top: 0.5cm;
-      padding-left: 1.0cm;
-    }
-    ul {
-      padding-left: 2.0cm;
-    }
-    ul ul {
-      padding-left: 1.0cm;
-    }
-    li {
-      margin-top: 2pt;
-      margin-bottom: 2pt;
-    }
-    code {
-      font-family: IBM Plex Mono;
-      background-color: rgba(175, 184, 193, 0.2);
-      padding: 2pt 5pt 2pt 5pt;
-      border-radius: 6pt;
-    }
-    table {
-      margin-left: auto;
-      margin-right: auto;
-      text-align: center;
-      border-collapse: collapse;
-    }
-    td, th {
-      border: 1pt solid #BBBBBB;
-      padding: 4pt;
-      font-size: 10pt;
-    }
-    @page {
-        size: A4;
-        margin: 1.5cm 1.5cm 1.5cm 1.5cm;
-    }
-  </style>
+  <title>{{ title }}</title>
+  {{ css | indent(width=2) }}
 </head>
 <body>
+  {{ body | indent(width=2) }}
+</body>
+</html>
 """
 
 
-HTML_FOOTER = "</body>"
-
-
-MACRO_TEXT = r"""\
-\bvec:\vec{\mathbf{#1}}
-\normvec:\hat{\mathbf{#1}}
-\d:\operatorname{d}\!{#1}
-\ihat:\hat{\mathbf{i}}
-\jhat:\hat{\mathbf{j}}
-\khat:\hat{\mathbf{k}}
-"""
-
-
-def convert_markdown(text_md: str) -> str:
+def convert_markdown(text_md: str, katex: bool = False, path_macro: str | None = None) -> str:
     """Convert Markdown to HTML with KaTeX support.
 
     Parameters
     ----------
     text_md
-        The markdown source text
+        The markdown source text.
+    katex
+        Set to `True` to enable KaTeX support.
+    path_macro
+        A file with KaTeX macro definitions.
 
     Returns
     -------
     html
         The HTML conversion.
     """
     # Convert conventional LaTeX equation syntax to make it compatible with markdown_katex
     text_md = re.sub(r"\B\$(\S|\S[^\n\r]*?\S)\$\B", r"$`\1`$", text_md)
 
-    # Write macros to temporary file for KaTeX.
-    with tempfile.NamedTemporaryFile(suffix=".tex") as f:
-        f.write(MACRO_TEXT.encode("ascii"))
-        f.flush()
-        fn_macro = f.name
-
-        md_ctx = markdown.Markdown(
-            extensions=[
-                "fenced_code",
-                "markdown_katex",
-                "tables",
-            ],
-            extension_configs={
-                "markdown_katex": {"insert_fonts_css": True, "macro-file": fn_macro}
-            },
-        )
-
-        # Convert to HTML
-        text_html = HTML_HEADER + md_ctx.convert(text_md) + HTML_FOOTER
+    extensions = [
+        "fenced_code",
+        "tables",
+        "meta",
+    ]
+    configs = {}
+
+    if katex:
+        extensions.append("markdown_katex")
+        configs["markdown_katex"] = {"insert_fonts_css": True}
+        if path_macro is not None:
+            configs["markdown_katex"]["macro-file"] = path_macro
+
+    md_ctx = markdown.Markdown(
+        extensions=extensions,
+        extension_configs=configs,
+    )
 
-    return text_html
+    # Convert to HTML
+    body = md_ctx.convert(text_md)
+    variables = {
+        "body": body,
+        "title": md_ctx.Meta.get("title", ["Untitled"])[0],
+        "css": "\n".join(
+            f'<link rel="stylesheet" href="{path_css}">' for path_css in md_ctx.Meta.get("css", [])
+        ),
+    }
+    return render("HTML_TEMPLATE", variables, str_in=HTML_TEMPLATE)
 
 
 def parse_args() -> argparse.Namespace:
     """Parse command-line arguments."""
     parser = argparse.ArgumentParser(
         prog="reprep-convert-markdown", description="Convert Markdown to HTML"
     )
     parser.add_argument("markdown", help="A Markdown file with extension `.md`")
     parser.add_argument("html", help="A HTML output filename")
+    parser.add_argument("--katex", default=False, action="store_true", help="Enable KaTeX")
+    parser.add_argument("--katex-macros", default=None, help="KaTeX macro file")
     return parser.parse_args()
 
 
 def main() -> int:
     """Main program."""
     args = parse_args()
     if not args.markdown.endswith(".md"):
         raise ValueError("The markdown file must end with the .md extension.")
     with open(args.markdown) as fm, open(args.html, "w") as fh:
-        fh.write(convert_markdown(fm.read()))
+        fh.write(convert_markdown(fm.read(), args.katex, args.katex_macros))
     return 0
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `stepup_reprep-1.1.2/stepup/reprep/latex.py` & `stepup_reprep-1.2.0/stepup/reprep/latex.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import subprocess
 import sys
 
 from path import Path
 
 from stepup.core.api import amend, getenv
 from stepup.core.hash import compute_file_digest
-from stepup.reprep.make_manifest import write_manifest
+from stepup.reprep.make_inventory import write_inventory
 
 from .bibtex_log import parse_bibtex_log
 from .latex_deps import scan_latex_deps
 from .latex_log import ErrorInfo, parse_latex_log
 
 
 def main() -> int:
@@ -61,15 +61,15 @@
     if args.latex is None:
         args.latex = getenv("REPREP_LATEX", "pdflatex")
 
     aux_digest_hist = []
     if len(bib) == 0:
         if not amend(inp=implicit):
             return 0
-        manifest_files = list(implicit)
+        inventory_files = list(implicit)
     elif args.run_bibtex:
         # Get other executables and files
         if args.bibtex is None:
             args.bibtex = getenv("REPREP_BIBTEX", "bibtex")
         if args.bibsane is None:
             args.bibsane = getenv("REPREP_BIBSANE", "bibsane")
         paths_config = []
@@ -78,15 +78,15 @@
             paths_config.append(args.bibsane_config)
 
         if not amend(
             inp=implicit + bib + paths_config,
             out=[f"{stem}.bbl"],
         ):
             return 0
-        manifest_files = [*implicit, *bib, f"{stem}.bbl"]
+        inventory_files = [*implicit, *bib, f"{stem}.bbl"]
 
         # LaTeX
         cp = subprocess.run(
             [
                 args.latex,
                 "-interaction=errorstopmode",
                 "-draftmode",
@@ -135,15 +135,15 @@
             error_info = ErrorInfo("BibSane", src=f"{workdir}/{stem}.aux")
             error_info.print()
             sys.stdout.write(cp.stdout)
             return 3
     else:
         if not amend(inp=[*implicit, f"{stem}.bbl"]):
             return 0
-        manifest_files = [*implicit, f"{stem}.bbl"]
+        inventory_files = [*implicit, f"{stem}.bbl"]
 
     for _ in range(args.maxrep):
         # LaTeX
         cp = subprocess.run(
             [args.latex, "-interaction=errorstopmode", stem],
             stdin=subprocess.DEVNULL,
             stdout=subprocess.DEVNULL,
@@ -165,22 +165,22 @@
             file=sys.stderr,
         )
         print(path_aux, file=sys.stderr)
         for digest in aux_digest_hist:
             print(digest.hex(), file=sys.stderr)
         return -3
 
-    manifest_files.extend([f"{stem}.tex", f"{stem}.aux", f"{stem}.pdf"])
-    path_manifest = f"{stem}.MANIFEST.txt"
-    write_manifest(path_manifest, manifest_files)
+    inventory_files.extend([f"{stem}.tex", f"{stem}.aux", f"{stem}.pdf"])
+    path_inventory = f"{stem}-inventory.txt"
+    write_inventory(path_inventory, inventory_files)
 
     vol_paths = []
     for path in Path(".").glob(f"{stem}.*"):
         path = path.normpath()
-        if not (path in manifest_files or path == path_manifest):
+        if not (path in inventory_files or path == path_inventory):
             vol_paths.append(path)
     amend(vol=vol_paths)
 
 
 def parse_args() -> argparse.Namespace:
     """Parse command-line arguments."""
     parser = argparse.ArgumentParser(
```

### Comparing `stepup_reprep-1.1.2/stepup/reprep/latex_deps.py` & `stepup_reprep-1.2.0/stepup/reprep/latex_deps.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/stepup/reprep/latex_flat.py` & `stepup_reprep-1.2.0/stepup/reprep/latex_flat.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/stepup/reprep/latex_log.py` & `stepup_reprep-1.2.0/stepup/reprep/latex_log.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/stepup/reprep/normalize_pdf.py` & `stepup_reprep-1.2.0/stepup/reprep/normalize_pdf.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/stepup/reprep/nup_pdf.py` & `stepup_reprep-1.2.0/stepup/reprep/nup_pdf.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/stepup/reprep/pytest.py` & `stepup_reprep-1.2.0/stepup/reprep/pytest.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,29 +18,29 @@
 #
 # --
 """Utilities for testing with pytest."""
 
 from path import Path
 
 from stepup.core.pytest import run_example as run_example_core
-from stepup.reprep.check_manifest import iter_manifest
+from stepup.reprep.check_inventory import iter_inventory
 
 __all__ = ("run_example",)
 
 
 async def run_example(srcdir, tmpdir, overwrite_expected=False):
     """Run an example use case in a temporary directory and check the outputs.
 
     See stepup.core.pytest.run_example for details.
     """
     await run_example_core(srcdir, tmpdir, overwrite_expected)
 
     # Reproducibility check
     workdir = Path(tmpdir) / "example"
-    for path_manifest in sorted(workdir.glob("reproducibility_*manifest.txt")):
-        records = list(iter_manifest(path_manifest))
-        sizes = {record[0] for record in records}
+    for path_inventory in sorted(workdir.glob("reproducibility_*inventory.txt")):
+        records = list(iter_inventory(path_inventory))
+        sizes = {record.size for record in records}
         if not len(sizes) == 1:
-            raise AssertionError(f"Not all file sizes in {path_manifest} are the same.")
-        digests = {record[1] for record in records}
+            raise AssertionError(f"Not all file sizes in {path_inventory} are the same.")
+        digests = {record.digest for record in records}
         if not len(digests) == 1:
-            raise AssertionError(f"Not all file digests in {path_manifest} are the same.")
+            raise AssertionError(f"Not all file digests in {path_inventory} are the same.")
```

### Comparing `stepup_reprep-1.1.2/stepup/reprep/raster_pdf.py` & `stepup_reprep-1.2.0/stepup/reprep/raster_pdf.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/stepup/reprep/render.py` & `stepup_reprep-1.2.0/stepup/reprep/render.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/stepup/reprep/tile_pdf.py` & `stepup_reprep-1.2.0/stepup/reprep/tile_pdf.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/stepup_reprep.egg-info/PKG-INFO` & `stepup_reprep-1.2.0/stepup_reprep.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stepup-reprep
-Version: 1.1.2
+Version: 1.2.0
 Summary: StepUp RepRep is the StepUp extension for Reproducible Reporting
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 Project-URL: Documentation, https://reproducible-reporting.github.io/stepup-reprep/
 Project-URL: Issues, https://github.com/reproducible-reporting/stepup-reprep/issues
 Project-URL: Source, https://github.com/reproducible-reporting/stepup-reprep/
 Project-URL: Changelog, https://reproducible-reporting.github.io/stepup-reprep/changelog/
 Classifier: Environment :: Console
@@ -24,16 +24,15 @@
 Requires-Dist: markdown
 Requires-Dist: markdown_katex
 Requires-Dist: numpy
 Requires-Dist: path
 Requires-Dist: pymupdf
 Requires-Dist: pyyaml
 Requires-Dist: scipy
-Requires-Dist: setuptools
-Requires-Dist: stepup>=1.2.2
+Requires-Dist: stepup>=1.2.3
 Requires-Dist: weasyprint
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
```

### Comparing `stepup_reprep-1.1.2/stepup_reprep.egg-info/SOURCES.txt` & `stepup_reprep-1.2.0/stepup_reprep.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -10,68 +10,70 @@
 .github/workflows/release.yaml
 docs/changelog.md
 docs/clean_stdout.sed
 docs/development.md
 docs/index.md
 docs/installation.md
 docs/license.md
+docs/advanced_topics/archive_git.md
 docs/advanced_topics/good_practices.md
-docs/advanced_topics/manifest_files.md
-docs/advanced_topics/tiling_pdfs.md
-docs/advanced_topics/tiling_pdfs/.gitignore
-docs/advanced_topics/tiling_pdfs/figure.png
-docs/advanced_topics/tiling_pdfs/hexagon.svg
-docs/advanced_topics/tiling_pdfs/main.sh
-docs/advanced_topics/tiling_pdfs/pentagon.svg
-docs/advanced_topics/tiling_pdfs/plan.py
-docs/advanced_topics/tiling_pdfs/square.svg
-docs/advanced_topics/tiling_pdfs/stdout.txt
-docs/advanced_topics/tiling_pdfs/tile.py
-docs/advanced_topics/tiling_pdfs/triangle.svg
+docs/advanced_topics/inventory_files.md
+docs/advanced_topics/tile_pdfs.md
+docs/advanced_topics/tile_pdfs/.gitignore
+docs/advanced_topics/tile_pdfs/figure.png
+docs/advanced_topics/tile_pdfs/hexagon.svg
+docs/advanced_topics/tile_pdfs/main.sh
+docs/advanced_topics/tile_pdfs/pentagon.svg
+docs/advanced_topics/tile_pdfs/plan.py
+docs/advanced_topics/tile_pdfs/square.svg
+docs/advanced_topics/tile_pdfs/stdout.txt
+docs/advanced_topics/tile_pdfs/tile.py
+docs/advanced_topics/tile_pdfs/triangle.svg
 docs/from_scratch/introduction.md
 docs/from_template/before_you_begin.md
 docs/from_template/create_or_clone_a_project.md
 docs/from_template/introduction.md
 docs/from_template/working_on_a_project.md
 docs/reference/stepup.reprep.api.md
 docs/reference/stepup.reprep.tile_pdf.md
 stepup/reprep/__init__.py
 stepup/reprep/add_notes_pdf.py
 stepup/reprep/api.py
 stepup/reprep/bibtex_log.py
 stepup/reprep/check_hrefs.py
-stepup/reprep/check_manifest.py
+stepup/reprep/check_inventory.py
 stepup/reprep/convert_inkscape.py
 stepup/reprep/convert_markdown.py
+stepup/reprep/inventory.py
 stepup/reprep/latex.py
 stepup/reprep/latex_deps.py
 stepup/reprep/latex_flat.py
 stepup/reprep/latex_log.py
-stepup/reprep/make_manifest.py
+stepup/reprep/make_inventory.py
 stepup/reprep/normalize_pdf.py
 stepup/reprep/nup_pdf.py
 stepup/reprep/pytest.py
 stepup/reprep/raster_pdf.py
 stepup/reprep/render.py
 stepup/reprep/tile_pdf.py
-stepup/reprep/zip_manifest.py
+stepup/reprep/zip_inventory.py
 stepup_reprep.egg-info/PKG-INFO
 stepup_reprep.egg-info/SOURCES.txt
 stepup_reprep.egg-info/dependency_links.txt
 stepup_reprep.egg-info/entry_points.txt
 stepup_reprep.egg-info/requires.txt
 stepup_reprep.egg-info/top_level.txt
 tests/conftest.py
 tests/reprep_common.py
 tests/test_bibtex_log.py
 tests/test_cases.py
+tests/test_inventory.py
 tests/test_latex_deps.py
 tests/test_latex_flat.py
 tests/test_latex_log.py
-tests/test_manifest.py
 tests/test_zip.py
 tests/cases/add_notes_pdf/.gitignore
 tests/cases/add_notes_pdf/README.md
 tests/cases/add_notes_pdf/expected_graph.txt
 tests/cases/add_notes_pdf/expected_stdout.txt
 tests/cases/add_notes_pdf/main.sh
 tests/cases/add_notes_pdf/notes.pdf
@@ -81,14 +83,15 @@
 tests/cases/cat_pdf/README.md
 tests/cases/cat_pdf/doc1.pdf
 tests/cases/cat_pdf/doc2.pdf
 tests/cases/cat_pdf/expected_graph.txt
 tests/cases/cat_pdf/expected_stdout.txt
 tests/cases/cat_pdf/main.sh
 tests/cases/cat_pdf/plan.py
+tests/cases/cat_pdf/reproducibility_inventory.txt
 tests/cases/check_hrefs_html/.gitignore
 tests/cases/check_hrefs_html/README.md
 tests/cases/check_hrefs_html/check_hrefs.yaml
 tests/cases/check_hrefs_html/expected_graph.txt
 tests/cases/check_hrefs_html/expected_stdout.txt
 tests/cases/check_hrefs_html/main.sh
 tests/cases/check_hrefs_html/plan.py
@@ -150,26 +153,29 @@
 tests/cases/convert_libreoffice/slide.odp
 tests/cases/convert_libreoffice_concurrency/.gitignore
 tests/cases/convert_libreoffice_concurrency/main.sh
 tests/cases/convert_libreoffice_concurrency/plan.py
 tests/cases/convert_libreoffice_concurrency/something.odt
 tests/cases/convert_markdown/.gitignore
 tests/cases/convert_markdown/README.md
+tests/cases/convert_markdown/demo.css
 tests/cases/convert_markdown/demo.md
 tests/cases/convert_markdown/expected_graph.txt
 tests/cases/convert_markdown/expected_stdout.txt
+tests/cases/convert_markdown/macros.tex
 tests/cases/convert_markdown/main.sh
 tests/cases/convert_markdown/plan.py
 tests/cases/convert_mutool/.gitignore
 tests/cases/convert_mutool/README.md
 tests/cases/convert_mutool/example.pdf
 tests/cases/convert_mutool/expected_graph.txt
 tests/cases/convert_mutool/expected_stdout.txt
 tests/cases/convert_mutool/main.sh
 tests/cases/convert_mutool/plan.py
+tests/cases/convert_mutool/reproducibility_inventory.txt
 tests/cases/convert_weasyprint/.gitignore
 tests/cases/convert_weasyprint/README.md
 tests/cases/convert_weasyprint/doc.html
 tests/cases/convert_weasyprint/expected_graph.txt
 tests/cases/convert_weasyprint/expected_stdout.txt
 tests/cases/convert_weasyprint/main.sh
 tests/cases/convert_weasyprint/plan.py
@@ -195,54 +201,42 @@
 tests/cases/latex_flat/plan_01.py
 tests/cases/latex_flat/plan_02.py
 tests/cases/latex_flat/sub/original.tex
 tests/cases/latex_flat_subdir/.gitignore
 tests/cases/latex_flat_subdir/README.md
 tests/cases/latex_flat_subdir/expected_article.tex
 tests/cases/latex_flat_subdir/expected_graph.txt
+tests/cases/latex_flat_subdir/expected_inventory.txt
 tests/cases/latex_flat_subdir/expected_stdout.txt
+tests/cases/latex_flat_subdir/inventory.def
 tests/cases/latex_flat_subdir/main.sh
 tests/cases/latex_flat_subdir/plan.py
 tests/cases/latex_flat_subdir/sub/article_structured.tex
 tests/cases/latex_flat_subdir/sub/part1.tex
 tests/cases/latex_flat_subdir/sub/part2.tex
 tests/cases/lualatex_simple/.gitignore
 tests/cases/lualatex_simple/expected_graph.txt
 tests/cases/lualatex_simple/expected_stdout.txt
 tests/cases/lualatex_simple/main.sh
 tests/cases/lualatex_simple/paper.tex
 tests/cases/lualatex_simple/plan.py
-tests/cases/make_manifest_in/.gitignore
-tests/cases/make_manifest_in/MANIFEST.in
-tests/cases/make_manifest_in/README.md
-tests/cases/make_manifest_in/expected_graph.txt
-tests/cases/make_manifest_in/expected_stdout.txt
-tests/cases/make_manifest_in/hello.txt
-tests/cases/make_manifest_in/main.sh
-tests/cases/make_manifest_in/plan.py
-tests/cases/make_manifest_in_sub/.gitignore
-tests/cases/make_manifest_in_sub/README.md
-tests/cases/make_manifest_in_sub/expected_graph.txt
-tests/cases/make_manifest_in_sub/expected_stdout.txt
-tests/cases/make_manifest_in_sub/main.sh
-tests/cases/make_manifest_in_sub/plan.py
-tests/cases/make_manifest_in_sub/sub/MANIFEST.in
-tests/cases/make_manifest_in_sub/sub/hello.txt
-tests/cases/make_manifest_list/.gitignore
-tests/cases/make_manifest_list/README.md
-tests/cases/make_manifest_list/expected_graph.txt
-tests/cases/make_manifest_list/expected_stdout.txt
-tests/cases/make_manifest_list/main.sh
-tests/cases/make_manifest_list/plan.py
+tests/cases/make_inventory_list/.gitignore
+tests/cases/make_inventory_list/README.md
+tests/cases/make_inventory_list/expected_graph.txt
+tests/cases/make_inventory_list/expected_inventory.txt
+tests/cases/make_inventory_list/expected_stdout.txt
+tests/cases/make_inventory_list/main.sh
+tests/cases/make_inventory_list/plan.py
 tests/cases/nup_pdf/.gitignore
 tests/cases/nup_pdf/README.md
 tests/cases/nup_pdf/expected_graph.txt
 tests/cases/nup_pdf/expected_stdout.txt
 tests/cases/nup_pdf/main.sh
 tests/cases/nup_pdf/plan.py
+tests/cases/nup_pdf/reproducibility_inventory.txt
 tests/cases/nup_pdf/src.pdf
 tests/cases/pdflatex_bbl/.gitignore
 tests/cases/pdflatex_bbl/expected_graph.txt
 tests/cases/pdflatex_bbl/expected_stdout.txt
 tests/cases/pdflatex_bbl/main.sh
 tests/cases/pdflatex_bbl/paper.bbl
 tests/cases/pdflatex_bbl/paper.tex
@@ -304,14 +298,14 @@
 tests/cases/xelatex_input/.gitignore
 tests/cases/xelatex_input/expected_graph.txt
 tests/cases/xelatex_input/expected_stdout.txt
 tests/cases/xelatex_input/main.sh
 tests/cases/xelatex_input/paper.tex
 tests/cases/xelatex_input/plan.py
 tests/cases/xelatex_input/smile.pdf
-tests/cases/zip_manifest/.gitignore
-tests/cases/zip_manifest/README.md
-tests/cases/zip_manifest/expected_graph.txt
-tests/cases/zip_manifest/expected_stdout.txt
-tests/cases/zip_manifest/main.sh
-tests/cases/zip_manifest/plan.py
-tests/cases/zip_manifest/static.txt
+tests/cases/zip_inventory/.gitignore
+tests/cases/zip_inventory/README.md
+tests/cases/zip_inventory/expected_graph.txt
+tests/cases/zip_inventory/expected_stdout.txt
+tests/cases/zip_inventory/main.sh
+tests/cases/zip_inventory/plan.py
+tests/cases/zip_inventory/static.txt
```

### Comparing `stepup_reprep-1.1.2/tests/cases/add_notes_pdf/expected_graph.txt` & `stepup_reprep-1.2.0/tests/cases/add_notes_pdf/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/add_notes_pdf/expected_stdout.txt` & `stepup_reprep-1.2.0/tests/cases/add_notes_pdf/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/add_notes_pdf/main.sh` & `stepup_reprep-1.2.0/tests/cases/add_notes_pdf/main.sh`

 * *Files 15% similar despite different names*

```diff
@@ -19,24 +19,24 @@
 graph("current_graph")
 EOD
 
 # Reproducibility test
 mv dst.pdf dst1.pdf
 python3 - << EOD
 from stepup.core.interact import *
-from stepup.reprep.make_manifest import write_manifest
+from stepup.reprep.make_inventory import write_inventory
 watch_delete("dst.pdf")
 run()
 join()
-write_manifest("reproducibility_manifest.txt", ["dst.pdf", "dst1.pdf"])
+write_inventory("reproducibility_inventory.txt", ["dst.pdf", "dst1.pdf"])
 EOD
 
 # Wait for background processes, if any.
 wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f src.pdf ]] || exit -1
 [[ -f notes.pdf ]] || exit -1
 [[ -f dst.pdf ]] || exit -1
 [[ -f dst1.pdf ]] || exit -1
-[[ -f reproducibility_manifest.txt ]] || exit -1
+[[ -f reproducibility_inventory.txt ]] || exit -1
```

### Comparing `stepup_reprep-1.1.2/tests/cases/add_notes_pdf/notes.pdf` & `stepup_reprep-1.2.0/tests/cases/add_notes_pdf/notes.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/add_notes_pdf/src.pdf` & `stepup_reprep-1.2.0/tests/cases/add_notes_pdf/src.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/cat_pdf/doc1.pdf` & `stepup_reprep-1.2.0/tests/cases/cat_pdf/doc1.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/cat_pdf/doc2.pdf` & `stepup_reprep-1.2.0/tests/cases/cat_pdf/doc2.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/cat_pdf/expected_graph.txt` & `stepup_reprep-1.2.0/tests/cases/cat_pdf/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/cat_pdf/expected_stdout.txt` & `stepup_reprep-1.2.0/tests/cases/cat_pdf/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/cat_pdf/main.sh` & `stepup_reprep-1.2.0/tests/cases/check_hrefs_pdf/main.sh`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,33 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
+export SOURCE_DATE_EPOCH="315532800"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
-EOD
-
-# Reproducibility test
-mv cat.pdf cat1.pdf
-python3 - << EOD
-from stepup.core.interact import *
-from stepup.reprep.make_manifest import write_manifest
-watch_delete("cat.pdf")
-run()
 join()
-write_manifest("reproducibility_manifest.txt", ["cat.pdf", "cat1.pdf"])
 EOD
 
 # Wait for background processes, if any.
 wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f doc1.pdf ]] || exit -1
-[[ -f doc2.pdf ]] || exit -1
-[[ -f cat.pdf ]] || exit -1
-[[ -f cat1.pdf ]] || exit -1
-[[ -f reproducibility_manifest.txt ]] || exit -1
+[[ -f main.pdf ]] || exit -1
+[[ -f main.log ]] || exit -1
+[[ -f main.aux ]] || exit -1
+[[ -f README.md ]] || exit -1
+reprep-check-inventory main-inventory.txt
```

### Comparing `stepup_reprep-1.1.2/tests/cases/check_hrefs_html/expected_graph.txt` & `stepup_reprep-1.2.0/tests/cases/check_hrefs_html/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/check_hrefs_html/expected_stdout.txt` & `stepup_reprep-1.2.0/tests/cases/check_hrefs_html/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/check_hrefs_html/main.sh` & `stepup_reprep-1.2.0/tests/cases/check_hrefs_html/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/check_hrefs_html/test.html` & `stepup_reprep-1.2.0/tests/cases/check_hrefs_html/test.html`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/check_hrefs_md/expected_graph.txt` & `stepup_reprep-1.2.0/tests/cases/check_hrefs_md/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/check_hrefs_md/expected_stdout.txt` & `stepup_reprep-1.2.0/tests/cases/check_hrefs_md/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/check_hrefs_md/main.sh` & `stepup_reprep-1.2.0/tests/cases/check_hrefs_md/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/check_hrefs_pdf/expected_graph.txt` & `stepup_reprep-1.2.0/tests/cases/check_hrefs_pdf/expected_graph.txt`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 file:./
                 path = ./
                state = STATIC
           created by   root:
             supplies   (file:BROKEN.md)
             supplies   file:README.md
             supplies   file:check_hrefs.yaml
-            supplies   file:main.MANIFEST.txt
+            supplies   file:main-inventory.txt
             supplies   file:main.aux
             supplies   file:main.log
             supplies   file:main.out
             supplies   file:main.pdf
             supplies   file:main.sh
             supplies   file:main.tex
             supplies   file:plan.py
@@ -72,29 +72,29 @@
   supplies (amended) = file:main.log
                      = file:main.out
                      = file:main.sh
    env_var (amended) = REPREP_LATEX
           created by   step:./plan.py
             consumes   file:./
             consumes   file:main.tex
-             creates   file:main.MANIFEST.txt
+             creates   file:main-inventory.txt
              creates   file:main.aux
              creates   file:main.log
              creates   file:main.out
              creates   file:main.pdf
              creates   file:main.sh
-            supplies   file:main.MANIFEST.txt
+            supplies   file:main-inventory.txt
             supplies   file:main.aux
             supplies   file:main.log
             supplies   file:main.out
             supplies   file:main.pdf
             supplies   file:main.sh
 
-file:main.MANIFEST.txt
-                path = main.MANIFEST.txt
+file:main-inventory.txt
+                path = main-inventory.txt
                state = BUILT
           created by   step:python -m stepup.reprep.latex main.tex --run-bibtex
             consumes   file:./
             consumes   step:python -m stepup.reprep.latex main.tex --run-bibtex
 
 file:main.aux
                 path = main.aux
```

### Comparing `stepup_reprep-1.1.2/tests/cases/check_hrefs_pdf/expected_stdout.txt` & `stepup_reprep-1.2.0/tests/cases/check_hrefs_pdf/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/check_hrefs_pdf/main.sh` & `stepup_reprep-1.2.0/tests/cases/make_inventory_list/main.sh`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
-export SOURCE_DATE_EPOCH="315532800"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
 
@@ -22,12 +21,10 @@
 EOD
 
 # Wait for background processes, if any.
 wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f main.pdf ]] || exit -1
-[[ -f main.log ]] || exit -1
-[[ -f main.aux ]] || exit -1
 [[ -f README.md ]] || exit -1
-reprep-check-manifest main.MANIFEST.txt
+[[ -f inventory.txt ]] || exit -1
+mv inventory.txt current_inventory.txt
```

### Comparing `stepup_reprep-1.1.2/tests/cases/check_hrefs_pdf/main.tex` & `stepup_reprep-1.2.0/tests/cases/check_hrefs_pdf/main.tex`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_inkscape/expected_graph.txt` & `stepup_reprep-1.2.0/tests/cases/convert_inkscape/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_inkscape/expected_stdout.txt` & `stepup_reprep-1.2.0/tests/cases/convert_inkscape/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_inkscape/glasses.svg` & `stepup_reprep-1.2.0/tests/cases/convert_inkscape/glasses.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_inkscape/main.sh` & `stepup_reprep-1.2.0/tests/cases/lualatex_simple/main.sh`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
 export SOURCE_DATE_EPOCH="315532800"
+export REPREP_LATEX="lualatex"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
 
@@ -17,30 +18,29 @@
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
 EOD
 
 # Reproducibility test
-mv final.pdf final1.pdf
-mv glasses.png glasses1.png
+rm paper.aux paper.log
+mv paper.pdf paper1.pdf
 python3 - << EOD
 from stepup.core.interact import *
-from stepup.reprep.make_manifest import write_manifest
-watch_delete("final.pdf")
-watch_delete("glasses.png")
+from stepup.reprep.make_inventory import write_inventory
+watch_delete("paper.pdf")
 run()
 join()
-write_manifest("reproducibility_png_manifest.txt", ["glasses.png", "glasses1.png"])
-write_manifest("reproducibility_pdf_manifest.txt", ["final.pdf", "final1.pdf"])
+write_inventory("reproducibility_inventory.txt", ["paper.pdf", "paper1.pdf"])
 EOD
 
 # Wait for background processes, if any.
 wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f smile.svg ]] || exit -1
-[[ -f final.pdf ]] || exit -1
-[[ -f final1.pdf ]] || exit -1
-[[ -f reproducibility_pdf_manifest.txt ]] || exit -1
-[[ -f reproducibility_png_manifest.txt ]] || exit -1
+[[ -f paper.pdf ]] || exit -1
+[[ -f paper.log ]] || exit -1
+[[ -f paper.aux ]] || exit -1
+[[ -f paper1.pdf ]] || exit -1
+[[ -f reproducibility_inventory.txt ]] || exit -1
+reprep-check-inventory paper-inventory.txt
```

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_inkscape/smile.svg` & `stepup_reprep-1.2.0/tests/cases/convert_inkscape/smile.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_050.svg` & `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_050.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_055.svg` & `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_055.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_060.svg` & `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_060.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_065.svg` & `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_065.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_070.svg` & `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_070.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_075.svg` & `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_075.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_080.svg` & `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_080.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_085.svg` & `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_085.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_090.svg` & `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_090.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_095.svg` & `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_095.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_100.svg` & `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_100.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_105.svg` & `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_105.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_110.svg` & `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_110.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_115.svg` & `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_115.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_120.svg` & `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_120.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_125.svg` & `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_125.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_130.svg` & `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_130.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_135.svg` & `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_135.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_140.svg` & `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_140.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_145.svg` & `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/dots_145.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/main.sh` & `stepup_reprep-1.2.0/tests/cases/convert_inkscape_concurrency/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_libreoffice/expected_graph.txt` & `stepup_reprep-1.2.0/tests/cases/convert_libreoffice/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_libreoffice/expected_stdout.txt` & `stepup_reprep-1.2.0/tests/cases/convert_libreoffice/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_libreoffice/main.sh` & `stepup_reprep-1.2.0/tests/cases/pdflatex_bbl/main.sh`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
-export SOURCE_DATE_EPOCH="315532800"
+export SOURCE_DATE_EPOCH"315532800"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
 
@@ -17,26 +17,29 @@
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
 EOD
 
 # Reproducibility test
-mv slide.pdf slide1.pdf
+rm paper.aux paper.log
+mv paper.pdf paper1.pdf
 python3 - << EOD
 from stepup.core.interact import *
-from stepup.reprep.make_manifest import write_manifest
-watch_delete("slide.pdf")
+from stepup.reprep.make_inventory import write_inventory
+watch_delete("paper.pdf")
 run()
 join()
-write_manifest("reproducibility_manifest_skip.txt", ["slide.pdf", "slide1.pdf"])
+write_inventory("reproducibility_inventory.txt", ["paper.pdf", "paper1.pdf"])
 EOD
 
 # Wait for background processes, if any.
 wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f slide.odp ]] || exit -1
-[[ -f slide.pdf ]] || exit -1
-[[ -f slide1.pdf ]] || exit -1
-[[ -f reproducibility_manifest_skip.txt ]] || exit -1
+[[ -f paper.pdf ]] || exit -1
+[[ -f paper.log ]] || exit -1
+[[ -f paper.aux ]] || exit -1
+[[ -f paper1.pdf ]] || exit -1
+[[ -f reproducibility_inventory.txt ]] || exit -1
+reprep-check-inventory paper-inventory.txt
```

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_libreoffice/slide.odp` & `stepup_reprep-1.2.0/tests/cases/convert_libreoffice/slide.odp`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_libreoffice_concurrency/main.sh` & `stepup_reprep-1.2.0/tests/cases/convert_libreoffice_concurrency/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_libreoffice_concurrency/something.odt` & `stepup_reprep-1.2.0/tests/cases/convert_libreoffice_concurrency/something.odt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_markdown/expected_stdout.txt` & `stepup_reprep-1.2.0/tests/cases/lualatex_simple/expected_stdout.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,17 @@
   DIRECTOR │ Launched worker 0
      PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
-     START │ python -m stepup.reprep.convert_markdown demo.md demo.html
-   SUCCESS │ python -m stepup.reprep.convert_markdown demo.md demo.html
+     START │ python -m stepup.reprep.latex paper.tex --run-bibtex
+   SUCCESS │ python -m stepup.reprep.latex paper.tex --run-bibtex
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
-   DELETED │ demo.html
+   DELETED │ paper.aux
+   DELETED │ paper.pdf
      PHASE │ run
-     START │ python -m stepup.reprep.convert_markdown demo.md demo.html
-   SUCCESS │ python -m stepup.reprep.convert_markdown demo.md demo.html
+     START │ python -m stepup.reprep.latex paper.tex --run-bibtex
+   SUCCESS │ python -m stepup.reprep.latex paper.tex --run-bibtex
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
   DIRECTOR │ Stopping workers.
   DIRECTOR │ See you!
```

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_markdown/main.sh` & `stepup_reprep-1.2.0/tests/cases/convert_mutool/main.sh`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
-export SOURCE_DATE_EPOCH="315532800"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
 
@@ -17,26 +16,26 @@
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
 EOD
 
 # Reproducibility test
-mv demo.html demo1.html
+mv example.png example1.png
 python3 - << EOD
 from stepup.core.interact import *
-from stepup.reprep.make_manifest import write_manifest
-watch_delete("demo.html")
+from stepup.reprep.make_inventory import write_inventory
+watch_delete("example.png")
 run()
 join()
-write_manifest("reproducibility_manifest.txt", ["demo.html", "demo1.html"])
+write_inventory("reproducibility_inventory.txt", ["example.png", "example1.png"])
 EOD
 
 # Wait for background processes, if any.
 wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f demo.md ]] || exit -1
-[[ -f demo.html ]] || exit -1
-[[ -f demo1.html ]] || exit -1
-[[ -f reproducibility_manifest.txt ]] || exit -1
+[[ -f example.pdf ]] || exit -1
+[[ -f example.png ]] || exit -1
+[[ -f example1.png ]] || exit -1
+[[ -f reproducibility_inventory.txt ]] || exit -1
```

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_mutool/example.pdf` & `stepup_reprep-1.2.0/tests/cases/convert_mutool/example.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_mutool/expected_graph.txt` & `stepup_reprep-1.2.0/tests/cases/convert_mutool/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_mutool/expected_stdout.txt` & `stepup_reprep-1.2.0/tests/cases/convert_mutool/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_mutool/main.sh` & `stepup_reprep-1.2.0/tests/cases/render_basic/main.sh`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,32 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
+export ENV_VAR_TEST_STEPUP_RENDER="cool"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
-EOD
-
-# Reproducibility test
-mv example.png example1.png
-python3 - << EOD
-from stepup.core.interact import *
-from stepup.reprep.make_manifest import write_manifest
-watch_delete("example.png")
-run()
 join()
-write_manifest("reproducibility_manifest.txt", ["example.png", "example1.png"])
 EOD
 
 # Wait for background processes, if any.
 wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f example.pdf ]] || exit -1
-[[ -f example.png ]] || exit -1
-[[ -f example1.png ]] || exit -1
-[[ -f reproducibility_manifest.txt ]] || exit -1
+[[ -f template.md ]] || exit -1
+[[ -f variables.py ]] || exit -1
+[[ -f rendered.md ]] || exit -1
+grep RepRep rendered.md
```

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_weasyprint/expected_graph.txt` & `stepup_reprep-1.2.0/tests/cases/convert_weasyprint/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_weasyprint/expected_stdout.txt` & `stepup_reprep-1.2.0/tests/cases/convert_weasyprint/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/convert_weasyprint/main.sh` & `stepup_reprep-1.2.0/tests/cases/zip_inventory/main.sh`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
-export SOURCE_DATE_EPOCH="315532800"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
 
@@ -17,26 +16,28 @@
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
 EOD
 
 # Reproducibility test
-mv doc.pdf doc1.pdf
+rm built.txt
+mv upload.zip upload1.zip
 python3 - << EOD
 from stepup.core.interact import *
-from stepup.reprep.make_manifest import write_manifest
-watch_delete("doc.pdf")
+from stepup.reprep.make_inventory import write_inventory
+watch_delete("upload.zip")
 run()
 join()
-write_manifest("reproducibility_manifest.txt", ["doc.pdf", "doc1.pdf"])
+write_inventory("reproducibility_inventory.txt", ["upload.zip", "upload1.zip"])
 EOD
 
 # Wait for background processes, if any.
 wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f doc.html ]] || exit -1
-[[ -f doc.pdf ]] || exit -1
-[[ -f doc1.pdf ]] || exit -1
-[[ -f reproducibility_manifest.txt ]] || exit -1
+[[ -f built.txt ]] || exit -1
+[[ -f inventory.txt ]] || exit -1
+[[ -f upload.zip ]] || exit -1
+[[ -f upload1.zip ]] || exit -1
+[[ -f reproducibility_inventory.txt ]] || exit -1
```

### Comparing `stepup_reprep-1.1.2/tests/cases/latex_diff/expected_graph.txt` & `stepup_reprep-1.2.0/tests/cases/latex_diff/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/latex_diff/expected_stdout.txt` & `stepup_reprep-1.2.0/tests/cases/latex_diff/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/latex_diff/main.sh` & `stepup_reprep-1.2.0/tests/cases/latex_flat/main.sh`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,56 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
-stepup -w 1 plan.py & # > current_stdout.txt &
+cp plan_01.py plan.py
+stepup -w 1 plan.py & # > current_stdout_01.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
+print("HERE")
 wait()
-graph("current_graph")
+graph("current_graph_01")
+join()
 EOD
 
-# Reproducibility test
-mv diff.tex diff1.tex
+# Check files that are expected to be present and/or missing.
+[[ -f plan.py ]] || exit -1
+[[ -f article_structured.tex ]] || exit -1
+[[ ! -f article.tex ]] || exit -1
+
+# Wait for background processes, if any.
+wait
+
+# Add the missing file and run again
+cp plan_02.py plan.py
+cp sub/original.tex sub/other.tex
+rm -r .stepup/logs
+stepup -w 1 plan.py & # > current_stdout_02.txt &
+
+# Wait for the director and get its socket.
+export STEPUP_DIRECTOR_SOCKET=$(
+  python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
+)
 python3 - << EOD
 from stepup.core.interact import *
-from stepup.reprep.make_manifest import write_manifest
-watch_delete("diff.tex")
-run()
+wait()
+graph("current_graph_02")
 join()
-write_manifest("reproducibility_manifest.txt", ["diff.tex", "diff1.tex"])
 EOD
 
-# Wait for background processes, if any.
-wait
-
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f diff.tex ]] || exit -1
-[[ -f diff1.tex ]] || exit -1
-[[ -f reproducibility_manifest.txt ]] || exit -1
+[[ -f article_structured.tex ]] || exit -1
+[[ -f article.tex ]] || exit -1
+
+# Wait for background processes, if any.
+wait
```

### Comparing `stepup_reprep-1.1.2/tests/cases/latex_flat/expected_graph_01.txt` & `stepup_reprep-1.2.0/tests/cases/latex_flat/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/latex_flat/expected_graph_02.txt` & `stepup_reprep-1.2.0/tests/cases/latex_flat/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/latex_flat/expected_stdout_01.txt` & `stepup_reprep-1.2.0/tests/cases/latex_flat/expected_stdout_01.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/latex_flat/main.sh` & `stepup_reprep-1.2.0/tests/cases/latex_flat_subdir/main.sh`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,35 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
-cp plan_01.py plan.py
-stepup -w 1 plan.py & # > current_stdout_01.txt &
+stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
-print("HERE")
 wait()
-graph("current_graph_01")
+graph("current_graph")
 join()
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f article_structured.tex ]] || exit -1
-[[ ! -f article.tex ]] || exit -1
+[[ -f sub/article_structured.tex ]] || exit -1
+[[ -f sub/part1.tex ]] || exit -1
+[[ -f sub/part2.tex ]] || exit -1
+[[ -f sub/article.tex ]] || exit -1
+cp sub/article.tex current_article.tex
 
-# Wait for background processes, if any.
-wait
-
-# Add the missing file and run again
-cp plan_02.py plan.py
-cp sub/original.tex sub/other.tex
-stepup -w 1 plan.py & # > current_stdout_02.txt &
-
-# Wait for the director and get its socket.
-export STEPUP_DIRECTOR_SOCKET=$(
-  python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
-)
-python3 - << EOD
-from stepup.core.interact import *
-wait()
-graph("current_graph_02")
-join()
-EOD
-
-# Check files that are expected to be present and/or missing.
-[[ -f plan.py ]] || exit -1
-[[ -f article_structured.tex ]] || exit -1
-[[ -f article.tex ]] || exit -1
+# Create an inventory file
+reprep-make-inventory -i inventory.def -o current_inventory.txt
 
 # Wait for background processes, if any.
 wait
```

### Comparing `stepup_reprep-1.1.2/tests/cases/latex_flat_subdir/expected_graph.txt` & `stepup_reprep-1.2.0/tests/cases/latex_flat_subdir/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/latex_flat_subdir/main.sh` & `stepup_reprep-1.2.0/tests/cases/render_relpath/main.sh`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
+export SOURCE_DATE_EPOCH="315532800"
+export PUBLIC="public/"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
 
@@ -16,17 +18,21 @@
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
 join()
 EOD
 
-# Check files that are expected to be present and/or missing.
-[[ -f plan.py ]] || exit -1
-[[ -f sub/article_structured.tex ]] || exit -1
-[[ -f sub/part1.tex ]] || exit -1
-[[ -f sub/part2.tex ]] || exit -1
-[[ -f sub/article.tex ]] || exit -1
-cp sub/article.tex current_article.tex
-
 # Wait for background processes, if any.
 wait
+
+# Check files that are expected to be present and/or missing.
+[[ -f plan.py ]] || exit -1
+[[ -f variables.py ]] || exit -1
+[[ -f static/main.tex ]] || exit -1
+[[ -f static/plan.py ]] || exit -1
+[[ -f static/preamble.inc.tex ]] || exit -1
+[[ -f static/variables.py ]] || exit -1
+[[ -f public/preamble.inc.tex ]] || exit -1
+[[ -f public/main.pdf ]] || exit -1
+[[ -f public/main.tex ]] || exit -1
+grep Everything public/main.tex
```

### Comparing `stepup_reprep-1.1.2/tests/cases/lualatex_simple/expected_graph.txt` & `stepup_reprep-1.2.0/tests/cases/lualatex_simple/expected_graph.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
             consumes   file:./
             supplies   step:./plan.py
 
 file:./
                 path = ./
                state = STATIC
           created by   root:
-            supplies   file:paper.MANIFEST.txt
+            supplies   file:paper-inventory.txt
             supplies   file:paper.aux
             supplies   file:paper.log
             supplies   file:paper.pdf
             supplies   file:paper.tex
             supplies   file:plan.py
             supplies   step:./plan.py
             supplies   step:python -m stepup.reprep.latex paper.tex --run-bibtex
@@ -46,25 +46,25 @@
              command = python -m stepup.reprep.latex paper.tex --run-bibtex
                state = SUCCEEDED
   supplies (amended) = file:paper.log
    env_var (amended) = REPREP_LATEX
           created by   step:./plan.py
             consumes   file:./
             consumes   file:paper.tex
-             creates   file:paper.MANIFEST.txt
+             creates   file:paper-inventory.txt
              creates   file:paper.aux
              creates   file:paper.log
              creates   file:paper.pdf
-            supplies   file:paper.MANIFEST.txt
+            supplies   file:paper-inventory.txt
             supplies   file:paper.aux
             supplies   file:paper.log
             supplies   file:paper.pdf
 
-file:paper.MANIFEST.txt
-                path = paper.MANIFEST.txt
+file:paper-inventory.txt
+                path = paper-inventory.txt
                state = BUILT
           created by   step:python -m stepup.reprep.latex paper.tex --run-bibtex
             consumes   file:./
             consumes   step:python -m stepup.reprep.latex paper.tex --run-bibtex
 
 file:paper.aux
                 path = paper.aux
```

### Comparing `stepup_reprep-1.1.2/tests/cases/lualatex_simple/expected_stdout.txt` & `stepup_reprep-1.2.0/tests/cases/pdflatex_bibtex/expected_stdout.txt`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
    SUCCESS │ ./plan.py
      START │ python -m stepup.reprep.latex paper.tex --run-bibtex
    SUCCESS │ python -m stepup.reprep.latex paper.tex --run-bibtex
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
    DELETED │ paper.aux
    DELETED │ paper.pdf
+   DELETED │ paper.bbl
      PHASE │ run
      START │ python -m stepup.reprep.latex paper.tex --run-bibtex
    SUCCESS │ python -m stepup.reprep.latex paper.tex --run-bibtex
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
   DIRECTOR │ Stopping workers.
   DIRECTOR │ See you!
```

### Comparing `stepup_reprep-1.1.2/tests/cases/lualatex_simple/main.sh` & `stepup_reprep-1.2.0/tests/cases/pdflatex_input/main.sh`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
 export SOURCE_DATE_EPOCH="315532800"
-export REPREP_LATEX="lualatex"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
 
@@ -18,29 +17,30 @@
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
 EOD
 
 # Reproducibility test
-rm paper.aux paper.log
+rm paper.aux paper.log generated.tex
 mv paper.pdf paper1.pdf
 python3 - << EOD
 from stepup.core.interact import *
-from stepup.reprep.make_manifest import write_manifest
+from stepup.reprep.make_inventory import write_inventory
 watch_delete("paper.pdf")
+watch_delete("generated.tex")
 run()
 join()
-write_manifest("reproducibility_manifest.txt", ["paper.pdf", "paper1.pdf"])
+write_inventory("reproducibility_inventory.txt", ["paper.pdf", "paper1.pdf"])
 EOD
 
 # Wait for background processes, if any.
 wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f paper.pdf ]] || exit -1
 [[ -f paper.log ]] || exit -1
 [[ -f paper.aux ]] || exit -1
 [[ -f paper1.pdf ]] || exit -1
-[[ -f reproducibility_manifest.txt ]] || exit -1
-reprep-check-manifest paper.MANIFEST.txt
+[[ -f reproducibility_inventory.txt ]] || exit -1
+reprep-check-inventory paper-inventory.txt
```

### Comparing `stepup_reprep-1.1.2/tests/cases/make_manifest_in/main.sh` & `stepup_reprep-1.2.0/tests/cases/cat_pdf/main.sh`

 * *Files 26% similar despite different names*

```diff
@@ -13,18 +13,30 @@
 )
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
+EOD
+
+# Reproducibility test
+mv cat.pdf cat1.pdf
+python3 - << EOD
+from stepup.core.interact import *
+from stepup.reprep.make_inventory import write_inventory
+watch_delete("cat.pdf")
+run()
 join()
+write_inventory("reproducibility_inventory.txt", ["cat.pdf", "cat1.pdf"])
 EOD
 
 # Wait for background processes, if any.
 wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f README.md ]] || exit -1
-[[ -f MANIFEST.txt ]] || exit -1
-mv MANIFEST.txt current_manifest.txt
+[[ -f doc1.pdf ]] || exit -1
+[[ -f doc2.pdf ]] || exit -1
+[[ -f cat.pdf ]] || exit -1
+[[ -f cat1.pdf ]] || exit -1
+[[ -f reproducibility_inventory.txt ]] || exit -1
```

### Comparing `stepup_reprep-1.1.2/tests/cases/make_manifest_in_sub/expected_graph.txt` & `stepup_reprep-1.2.0/tests/cases/pdflatex_bbl/expected_graph.txt`

 * *Files 24% similar despite different names*

```diff
@@ -11,64 +11,89 @@
             consumes   file:./
             supplies   step:./plan.py
 
 file:./
                 path = ./
                state = STATIC
           created by   root:
+            supplies   file:paper-inventory.txt
+            supplies   file:paper.aux
+            supplies   file:paper.bbl
+            supplies   file:paper.log
+            supplies   file:paper.pdf
+            supplies   file:paper.tex
             supplies   file:plan.py
-            supplies   file:sub/
             supplies   step:./plan.py
-            supplies   step:reprep-make-manifest -i sub/MANIFEST.in
+            supplies   step:python -m stepup.reprep.latex paper.tex
 
 step:./plan.py
              workdir = ./
              command = ./plan.py
                state = SUCCEEDED
           created by   root:
             consumes   file:./
             consumes   file:plan.py
-             creates   file:sub/
-             creates   file:sub/MANIFEST.in
-             creates   file:sub/hello.txt
-             creates   step:reprep-make-manifest -i sub/MANIFEST.in
+             creates   file:paper.bbl
+             creates   file:paper.tex
+             creates   step:python -m stepup.reprep.latex paper.tex
 
-file:sub/
-                path = sub/
+file:paper.tex
+                path = paper.tex
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
-            supplies   file:sub/MANIFEST.in
-            supplies   file:sub/MANIFEST.txt
-            supplies   file:sub/hello.txt
-            supplies   step:reprep-make-manifest -i sub/MANIFEST.in
+            supplies   step:python -m stepup.reprep.latex paper.tex
 
-file:sub/MANIFEST.in
-                path = sub/MANIFEST.in
+file:paper.bbl
+                path = paper.bbl
                state = STATIC
           created by   step:./plan.py
-            consumes   file:sub/
-            supplies   step:reprep-make-manifest -i sub/MANIFEST.in
-
-file:sub/hello.txt
-                path = sub/hello.txt
-               state = STATIC
-          created by   step:./plan.py
-            consumes   file:sub/
+            consumes   file:./
+            supplies   step:python -m stepup.reprep.latex paper.tex
 
-step:reprep-make-manifest -i sub/MANIFEST.in
+step:python -m stepup.reprep.latex paper.tex
              workdir = ./
-             command = reprep-make-manifest -i sub/MANIFEST.in
+             command = python -m stepup.reprep.latex paper.tex
                state = SUCCEEDED
+  consumes (amended) = file:paper.bbl
+  supplies (amended) = file:paper.log
+   env_var (amended) = REPREP_LATEX
           created by   step:./plan.py
             consumes   file:./
-            consumes   file:sub/
-            consumes   file:sub/MANIFEST.in
-             creates   file:sub/MANIFEST.txt
-            supplies   file:sub/MANIFEST.txt
+            consumes   file:paper.bbl
+            consumes   file:paper.tex
+             creates   file:paper-inventory.txt
+             creates   file:paper.aux
+             creates   file:paper.log
+             creates   file:paper.pdf
+            supplies   file:paper-inventory.txt
+            supplies   file:paper.aux
+            supplies   file:paper.log
+            supplies   file:paper.pdf
+
+file:paper-inventory.txt
+                path = paper-inventory.txt
+               state = BUILT
+          created by   step:python -m stepup.reprep.latex paper.tex
+            consumes   file:./
+            consumes   step:python -m stepup.reprep.latex paper.tex
 
-file:sub/MANIFEST.txt
-                path = sub/MANIFEST.txt
+file:paper.aux
+                path = paper.aux
                state = BUILT
-          created by   step:reprep-make-manifest -i sub/MANIFEST.in
-            consumes   file:sub/
-            consumes   step:reprep-make-manifest -i sub/MANIFEST.in
+          created by   step:python -m stepup.reprep.latex paper.tex
+            consumes   file:./
+            consumes   step:python -m stepup.reprep.latex paper.tex
+
+file:paper.pdf
+                path = paper.pdf
+               state = BUILT
+          created by   step:python -m stepup.reprep.latex paper.tex
+            consumes   file:./
+            consumes   step:python -m stepup.reprep.latex paper.tex
+
+file:paper.log
+                path = paper.log
+               state = VOLATILE
+          created by   step:python -m stepup.reprep.latex paper.tex
+            consumes   file:./
+            consumes   step:python -m stepup.reprep.latex paper.tex
```

### Comparing `stepup_reprep-1.1.2/tests/cases/make_manifest_list/expected_graph.txt` & `stepup_reprep-1.2.0/tests/cases/render_basic/expected_graph.txt`

 * *Files 20% similar despite different names*

```diff
@@ -11,46 +11,57 @@
             consumes   file:./
             supplies   step:./plan.py
 
 file:./
                 path = ./
                state = STATIC
           created by   root:
-            supplies   file:MANIFEST.txt
-            supplies   file:README.md
             supplies   file:plan.py
+            supplies   file:rendered.md
+            supplies   file:template.md
+            supplies   file:variables.py
             supplies   step:./plan.py
-            supplies   step:reprep-make-manifest README.md -o MANIFEST.txt
+            supplies   step:python -m stepup.reprep.render template.md variables.py rendered.md
 
 step:./plan.py
              workdir = ./
              command = ./plan.py
                state = SUCCEEDED
           created by   root:
             consumes   file:./
             consumes   file:plan.py
-             creates   file:README.md
-             creates   step:reprep-make-manifest README.md -o MANIFEST.txt
+             creates   file:template.md
+             creates   file:variables.py
+             creates   step:python -m stepup.reprep.render template.md variables.py rendered.md
 
-file:README.md
-                path = README.md
+file:template.md
+                path = template.md
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
-            supplies   step:reprep-make-manifest README.md -o MANIFEST.txt
+            supplies   step:python -m stepup.reprep.render template.md variables.py rendered.md
 
-step:reprep-make-manifest README.md -o MANIFEST.txt
+file:variables.py
+                path = variables.py
+               state = STATIC
+          created by   step:./plan.py
+            consumes   file:./
+            supplies   step:python -m stepup.reprep.render template.md variables.py rendered.md
+
+step:python -m stepup.reprep.render template.md variables.py rendered.md
              workdir = ./
-             command = reprep-make-manifest README.md -o MANIFEST.txt
+             command = python -m stepup.reprep.render template.md variables.py rendered.md
                state = SUCCEEDED
+   env_var (amended) = ENV_VAR_TEST_STEPUP_RENDER
           created by   step:./plan.py
             consumes   file:./
-            consumes   file:README.md
-             creates   file:MANIFEST.txt
-            supplies   file:MANIFEST.txt
+            consumes   file:template.md
+            consumes   file:variables.py
+             creates   file:rendered.md
+            supplies   file:rendered.md
 
-file:MANIFEST.txt
-                path = MANIFEST.txt
+file:rendered.md
+                path = rendered.md
                state = BUILT
-          created by   step:reprep-make-manifest README.md -o MANIFEST.txt
+          created by   step:python -m stepup.reprep.render template.md variables.py rendered.md
             consumes   file:./
-            consumes   step:reprep-make-manifest README.md -o MANIFEST.txt
+            consumes   step:python -m stepup.reprep.render template.md variables.py rendered.md
```

### Comparing `stepup_reprep-1.1.2/tests/cases/nup_pdf/expected_graph.txt` & `stepup_reprep-1.2.0/tests/cases/nup_pdf/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/nup_pdf/expected_stdout.txt` & `stepup_reprep-1.2.0/tests/cases/nup_pdf/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/nup_pdf/src.pdf` & `stepup_reprep-1.2.0/tests/cases/nup_pdf/src.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/pdflatex_bbl/expected_stdout.txt` & `stepup_reprep-1.2.0/tests/cases/pdflatex_bbl/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/pdflatex_bbl/main.sh` & `stepup_reprep-1.2.0/tests/cases/xelatex_input/main.sh`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
-export SOURCE_DATE_EPOCH"315532800"
+export SOURCE_DATE_EPOCH="315532800"
+export REPREP_LATEX="xelatex"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
 
@@ -17,29 +18,34 @@
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
 EOD
 
 # Reproducibility test
-rm paper.aux paper.log
+rm paper.aux
+rm paper.log
+rm subdir/generated.tex
+rm subdir/code.txt
 mv paper.pdf paper1.pdf
 python3 - << EOD
 from stepup.core.interact import *
-from stepup.reprep.make_manifest import write_manifest
+from stepup.reprep.make_inventory import write_inventory
 watch_delete("paper.pdf")
+watch_delete("subdir/generated.tex")
+watch_delete("subdir/code.txt")
 run()
 join()
-write_manifest("reproducibility_manifest.txt", ["paper.pdf", "paper1.pdf"])
+write_inventory("reproducibility_inventory.txt", ["paper.pdf", "paper1.pdf"])
 EOD
 
 # Wait for background processes, if any.
 wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f paper.pdf ]] || exit -1
 [[ -f paper.log ]] || exit -1
 [[ -f paper.aux ]] || exit -1
 [[ -f paper1.pdf ]] || exit -1
-[[ -f reproducibility_manifest.txt ]] || exit -1
-reprep-check-manifest paper.MANIFEST.txt
+[[ -f reproducibility_inventory.txt ]] || exit -1
+reprep-check-inventory paper-inventory.txt
```

### Comparing `stepup_reprep-1.1.2/tests/cases/pdflatex_bibtex/expected_graph.txt` & `stepup_reprep-1.2.0/tests/cases/pdflatex_bibtex/expected_graph.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
             supplies   step:./plan.py
 
 file:./
                 path = ./
                state = STATIC
           created by   root:
             supplies   file:bibsane.yaml
-            supplies   file:paper.MANIFEST.txt
+            supplies   file:paper-inventory.txt
             supplies   file:paper.aux
             supplies   file:paper.bbl
             supplies   file:paper.blg
             supplies   file:paper.log
             supplies   file:paper.pdf
             supplies   file:paper.tex
             supplies   file:plan.py
@@ -77,29 +77,29 @@
                      = REPREP_LATEX
                      = ROOT
           created by   step:./plan.py
             consumes   file:./
             consumes   file:bibsane.yaml
             consumes   file:paper.tex
             consumes   file:references.bib
-             creates   file:paper.MANIFEST.txt
+             creates   file:paper-inventory.txt
              creates   file:paper.aux
              creates   file:paper.bbl
              creates   file:paper.blg
              creates   file:paper.log
              creates   file:paper.pdf
-            supplies   file:paper.MANIFEST.txt
+            supplies   file:paper-inventory.txt
             supplies   file:paper.aux
             supplies   file:paper.bbl
             supplies   file:paper.blg
             supplies   file:paper.log
             supplies   file:paper.pdf
 
-file:paper.MANIFEST.txt
-                path = paper.MANIFEST.txt
+file:paper-inventory.txt
+                path = paper-inventory.txt
                state = BUILT
           created by   step:python -m stepup.reprep.latex paper.tex --run-bibtex
             consumes   file:./
             consumes   step:python -m stepup.reprep.latex paper.tex --run-bibtex
 
 file:paper.aux
                 path = paper.aux
```

### Comparing `stepup_reprep-1.1.2/tests/cases/pdflatex_bibtex/expected_stdout.txt` & `stepup_reprep-1.2.0/tests/cases/pdflatex_input/expected_stdout.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,30 @@
   DIRECTOR │ Launched worker 0
      PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ python -m stepup.reprep.latex paper.tex --run-bibtex
+RESCHEDULE │ python -m stepup.reprep.latex paper.tex --run-bibtex
+────────────────────────────────── Step info ───────────────────────────────────
+Command               python -m stepup.reprep.latex paper.tex --run-bibtex
+Return code           0
+──────────────── Rescheduling due to unavailable amended inputs ────────────────
+generated.tex
+────────────────────────────────────────────────────────────────────────────────
+     START │ echo 'Hi there!' > generated.tex
+   SUCCESS │ echo 'Hi there!' > generated.tex
+     START │ python -m stepup.reprep.latex paper.tex --run-bibtex
    SUCCESS │ python -m stepup.reprep.latex paper.tex --run-bibtex
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
    DELETED │ paper.aux
+   DELETED │ generated.tex
    DELETED │ paper.pdf
-   DELETED │ paper.bbl
      PHASE │ run
+     START │ echo 'Hi there!' > generated.tex
+   SUCCESS │ echo 'Hi there!' > generated.tex
      START │ python -m stepup.reprep.latex paper.tex --run-bibtex
    SUCCESS │ python -m stepup.reprep.latex paper.tex --run-bibtex
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
   DIRECTOR │ Stopping workers.
   DIRECTOR │ See you!
```

### Comparing `stepup_reprep-1.1.2/tests/cases/pdflatex_bibtex/main.sh` & `stepup_reprep-1.2.0/tests/cases/pdflatex_bibtex/main.sh`

 * *Files 14% similar despite different names*

```diff
@@ -23,30 +23,30 @@
 
 # Reproducibility test
 rm paper.aux paper.log
 mv paper.pdf paper1.pdf
 mv paper.bbl paper1.bbl
 python3 - << EOD
 from stepup.core.interact import *
-from stepup.reprep.make_manifest import write_manifest
+from stepup.reprep.make_inventory import write_inventory
 watch_delete("paper.pdf")
 watch_delete("paper.bbl")
 run()
 join()
-write_manifest("reproducibility_pdf_manifest.txt", ["paper.pdf", "paper1.pdf"])
-write_manifest("reproducibility_bbl_manifest.txt", ["paper.bbl", "paper1.bbl"])
+write_inventory("reproducibility_pdf_inventory.txt", ["paper.pdf", "paper1.pdf"])
+write_inventory("reproducibility_bbl_inventory.txt", ["paper.bbl", "paper1.bbl"])
 EOD
 
 # Wait for background processes, if any.
 wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f paper.pdf ]] || exit -1
 [[ -f paper.log ]] || exit -1
 [[ -f paper.aux ]] || exit -1
 [[ -f paper.bbl ]] || exit -1
 [[ -f paper1.pdf ]] || exit -1
 [[ -f paper1.bbl ]] || exit -1
-[[ -f reproducibility_pdf_manifest.txt ]] || exit -1
-[[ -f reproducibility_bbl_manifest.txt ]] || exit -1
-reprep-check-manifest paper.MANIFEST.txt
+[[ -f reproducibility_pdf_inventory.txt ]] || exit -1
+[[ -f reproducibility_bbl_inventory.txt ]] || exit -1
+reprep-check-inventory paper-inventory.txt
```

### Comparing `stepup_reprep-1.1.2/tests/cases/pdflatex_input/expected_graph.txt` & `stepup_reprep-1.2.0/tests/cases/pdflatex_input/expected_graph.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
             supplies   step:./plan.py
 
 file:./
                 path = ./
                state = STATIC
           created by   root:
             supplies   file:generated.tex
-            supplies   file:paper.MANIFEST.txt
+            supplies   file:paper-inventory.txt
             supplies   file:paper.aux
             supplies   file:paper.log
             supplies   file:paper.pdf
             supplies   file:paper.tex
             supplies   file:plan.py
             supplies   file:smile.pdf
             supplies   step:./plan.py
@@ -62,25 +62,25 @@
   supplies (amended) = file:paper.log
    env_var (amended) = REPREP_LATEX
           created by   step:./plan.py
             consumes   file:./
             consumes   file:generated.tex
             consumes   file:paper.tex
             consumes   file:smile.pdf
-             creates   file:paper.MANIFEST.txt
+             creates   file:paper-inventory.txt
              creates   file:paper.aux
              creates   file:paper.log
              creates   file:paper.pdf
-            supplies   file:paper.MANIFEST.txt
+            supplies   file:paper-inventory.txt
             supplies   file:paper.aux
             supplies   file:paper.log
             supplies   file:paper.pdf
 
-file:paper.MANIFEST.txt
-                path = paper.MANIFEST.txt
+file:paper-inventory.txt
+                path = paper-inventory.txt
                state = BUILT
           created by   step:python -m stepup.reprep.latex paper.tex --run-bibtex
             consumes   file:./
             consumes   step:python -m stepup.reprep.latex paper.tex --run-bibtex
 
 file:paper.aux
                 path = paper.aux
```

### Comparing `stepup_reprep-1.1.2/tests/cases/pdflatex_input/expected_stdout.txt` & `stepup_reprep-1.2.0/tests/cases/render_relpath/expected_stdout.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,27 @@
   DIRECTOR │ Launched worker 0
      PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
-     START │ python -m stepup.reprep.latex paper.tex --run-bibtex
-RESCHEDULE │ python -m stepup.reprep.latex paper.tex --run-bibtex
+     START │ mkdir -p public/
+   SUCCESS │ mkdir -p public/
+     START │ ./plan.py  # wd=static/
+   SUCCESS │ ./plan.py  # wd=static/
+     START │ python -m stepup.reprep.render main.tex ../variables.py variables.py ../public/main.tex  # wd=static/
+   SUCCESS │ python -m stepup.reprep.render main.tex ../variables.py variables.py ../public/main.tex  # wd=static/
+     START │ python -m stepup.reprep.latex main.tex --run-bibtex  # wd=public/
+RESCHEDULE │ python -m stepup.reprep.latex main.tex --run-bibtex  # wd=public/
 ────────────────────────────────── Step info ───────────────────────────────────
-Command               python -m stepup.reprep.latex paper.tex --run-bibtex
+Command               python -m stepup.reprep.latex main.tex --run-bibtex
+Working directory     public/
 Return code           0
 ──────────────── Rescheduling due to unavailable amended inputs ────────────────
-generated.tex
+public/preamble.inc.tex
 ────────────────────────────────────────────────────────────────────────────────
-     START │ echo 'Hi there!' > generated.tex
-   SUCCESS │ echo 'Hi there!' > generated.tex
-     START │ python -m stepup.reprep.latex paper.tex --run-bibtex
-   SUCCESS │ python -m stepup.reprep.latex paper.tex --run-bibtex
-  WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
-     PHASE │ watch
-   DELETED │ paper.aux
-   DELETED │ generated.tex
-   DELETED │ paper.pdf
-     PHASE │ run
-     START │ echo 'Hi there!' > generated.tex
-   SUCCESS │ echo 'Hi there!' > generated.tex
-     START │ python -m stepup.reprep.latex paper.tex --run-bibtex
-   SUCCESS │ python -m stepup.reprep.latex paper.tex --run-bibtex
+     START │ cp -aT static/preamble.inc.tex public/preamble.inc.tex
+   SUCCESS │ cp -aT static/preamble.inc.tex public/preamble.inc.tex
+     START │ python -m stepup.reprep.latex main.tex --run-bibtex  # wd=public/
+   SUCCESS │ python -m stepup.reprep.latex main.tex --run-bibtex  # wd=public/
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
   DIRECTOR │ Stopping workers.
   DIRECTOR │ See you!
```

### Comparing `stepup_reprep-1.1.2/tests/cases/pdflatex_input/main.sh` & `stepup_reprep-1.2.0/tests/cases/convert_weasyprint/main.sh`

 * *Files 20% similar despite different names*

```diff
@@ -17,30 +17,26 @@
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
 EOD
 
 # Reproducibility test
-rm paper.aux paper.log generated.tex
-mv paper.pdf paper1.pdf
+mv doc.pdf doc1.pdf
 python3 - << EOD
 from stepup.core.interact import *
-from stepup.reprep.make_manifest import write_manifest
-watch_delete("paper.pdf")
-watch_delete("generated.tex")
+from stepup.reprep.make_inventory import write_inventory
+watch_delete("doc.pdf")
 run()
 join()
-write_manifest("reproducibility_manifest.txt", ["paper.pdf", "paper1.pdf"])
+write_inventory("reproducibility_inventory.txt", ["doc.pdf", "doc1.pdf"])
 EOD
 
 # Wait for background processes, if any.
 wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f paper.pdf ]] || exit -1
-[[ -f paper.log ]] || exit -1
-[[ -f paper.aux ]] || exit -1
-[[ -f paper1.pdf ]] || exit -1
-[[ -f reproducibility_manifest.txt ]] || exit -1
-reprep-check-manifest paper.MANIFEST.txt
+[[ -f doc.html ]] || exit -1
+[[ -f doc.pdf ]] || exit -1
+[[ -f doc1.pdf ]] || exit -1
+[[ -f reproducibility_inventory.txt ]] || exit -1
```

### Comparing `stepup_reprep-1.1.2/tests/cases/pdflatex_input/smile.pdf` & `stepup_reprep-1.2.0/tests/cases/pdflatex_input/smile.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/raster_pdf/expected_graph.txt` & `stepup_reprep-1.2.0/tests/cases/raster_pdf/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/raster_pdf/expected_stdout.txt` & `stepup_reprep-1.2.0/tests/cases/raster_pdf/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/raster_pdf/main.sh` & `stepup_reprep-1.2.0/tests/cases/raster_pdf/main.sh`

 * *Files 18% similar despite different names*

```diff
@@ -19,23 +19,23 @@
 graph("current_graph")
 EOD
 
 # Reproducibility test
 mv rastered/smile.pdf rastered/smile1.pdf
 python3 - << EOD
 from stepup.core.interact import *
-from stepup.reprep.make_manifest import write_manifest
+from stepup.reprep.make_inventory import write_inventory
 watch_delete("rastered/smile.pdf")
 run()
 join()
-write_manifest("reproducibility_manifest.txt", ["rastered/smile.pdf", "rastered/smile1.pdf"])
+write_inventory("reproducibility_inventory.txt", ["rastered/smile.pdf", "rastered/smile1.pdf"])
 EOD
 
 # Wait for background processes, if any.
 wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f smile.pdf ]] || exit -1
 [[ -f rastered/smile.pdf ]] || exit -1
 [[ -f rastered/smile1.pdf ]] || exit -1
-[[ -f reproducibility_manifest.txt ]] || exit -1
+[[ -f reproducibility_inventory.txt ]] || exit -1
```

### Comparing `stepup_reprep-1.1.2/tests/cases/raster_pdf/smile.pdf` & `stepup_reprep-1.2.0/tests/cases/raster_pdf/smile.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/render_relpath/expected_graph.txt` & `stepup_reprep-1.2.0/tests/cases/render_relpath/expected_graph.txt`

 * *Files 8% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 file:public/
                 path = public/
                state = BUILT
           created by   step:mkdir -p public/
             consumes   file:./
             consumes   step:mkdir -p public/
-            supplies   file:public/main.MANIFEST.txt
+            supplies   file:public/main-inventory.txt
             supplies   file:public/main.aux
             supplies   file:public/main.log
             supplies   file:public/main.pdf
             supplies   file:public/main.tex
             supplies   file:public/preamble.inc.tex
             supplies   step:cp -aT static/preamble.inc.tex public/preamble.inc.tex
             supplies   step:python -m stepup.reprep.latex main.tex --run-bibtex  # wd=public/
@@ -180,25 +180,25 @@
   consumes (amended) = file:public/preamble.inc.tex
   supplies (amended) = file:public/main.log
    env_var (amended) = REPREP_LATEX
           created by   step:./plan.py  # wd=static/
             consumes   file:public/
             consumes   file:public/main.tex
             consumes   file:public/preamble.inc.tex
-             creates   file:public/main.MANIFEST.txt
+             creates   file:public/main-inventory.txt
              creates   file:public/main.aux
              creates   file:public/main.log
              creates   file:public/main.pdf
-            supplies   file:public/main.MANIFEST.txt
+            supplies   file:public/main-inventory.txt
             supplies   file:public/main.aux
             supplies   file:public/main.log
             supplies   file:public/main.pdf
 
-file:public/main.MANIFEST.txt
-                path = public/main.MANIFEST.txt
+file:public/main-inventory.txt
+                path = public/main-inventory.txt
                state = BUILT
           created by   step:python -m stepup.reprep.latex main.tex --run-bibtex  # wd=public/
             consumes   file:public/
             consumes   step:python -m stepup.reprep.latex main.tex --run-bibtex  # wd=public/
 
 file:public/main.aux
                 path = public/main.aux
```

### Comparing `stepup_reprep-1.1.2/tests/cases/tile_pdf/expected_graph.txt` & `stepup_reprep-1.2.0/tests/cases/tile_pdf/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/tile_pdf/expected_stdout.txt` & `stepup_reprep-1.2.0/tests/cases/tile_pdf/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/tile_pdf/hexagon.svg` & `stepup_reprep-1.2.0/tests/cases/tile_pdf/hexagon.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/tile_pdf/horizontal.svg` & `stepup_reprep-1.2.0/tests/cases/tile_pdf/horizontal.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/tile_pdf/main.sh` & `stepup_reprep-1.2.0/tests/cases/tile_pdf/main.sh`

 * *Files 10% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 graph("current_graph")
 EOD
 
 # Reproducibility test
 mv figure.pdf figure1.pdf
 python3 - << EOD
 from stepup.core.interact import *
-from stepup.reprep.make_manifest import write_manifest
+from stepup.reprep.make_inventory import write_inventory
 watch_delete("figure.pdf")
 run()
 join()
-write_manifest("reproducibility_manifest.txt", ["figure.pdf", "figure1.pdf"])
+write_inventory("reproducibility_inventory.txt", ["figure.pdf", "figure1.pdf"])
 EOD
 
 # Wait for background processes, if any.
 wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
@@ -47,8 +47,8 @@
 [[ -f square.pdf ]] || exit -1
 [[ -f pentagon.pdf ]] || exit -1
 [[ -f hexagon.pdf ]] || exit -1
 [[ -f vertical.pdf ]] || exit -1
 [[ -f horizontal.pdf ]] || exit -1
 [[ -f figure.pdf ]] || exit -1
 [[ -f figure1.pdf ]] || exit -1
-[[ -f reproducibility_manifest.txt ]] || exit -1
+[[ -f reproducibility_inventory.txt ]] || exit -1
```

### Comparing `stepup_reprep-1.1.2/tests/cases/tile_pdf/pentagon.svg` & `stepup_reprep-1.2.0/tests/cases/tile_pdf/pentagon.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/tile_pdf/square.svg` & `stepup_reprep-1.2.0/tests/cases/tile_pdf/square.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/tile_pdf/tile.py` & `stepup_reprep-1.2.0/tests/cases/tile_pdf/tile.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/tile_pdf/triangle.svg` & `stepup_reprep-1.2.0/tests/cases/tile_pdf/triangle.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/tile_pdf/vera.ttf` & `stepup_reprep-1.2.0/tests/cases/tile_pdf/vera.ttf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/tile_pdf/vertical.svg` & `stepup_reprep-1.2.0/tests/cases/tile_pdf/vertical.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/xelatex_input/expected_graph.txt` & `stepup_reprep-1.2.0/tests/cases/xelatex_input/expected_graph.txt`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
             consumes   file:./
             supplies   step:./plan.py
 
 file:./
                 path = ./
                state = STATIC
           created by   root:
-            supplies   file:paper.MANIFEST.txt
+            supplies   file:paper-inventory.txt
             supplies   file:paper.aux
             supplies   file:paper.log
             supplies   file:paper.out
             supplies   file:paper.pdf
             supplies   file:paper.tex
             supplies   file:plan.py
             supplies   file:subdir/
@@ -79,27 +79,27 @@
                      = file:paper.out
    env_var (amended) = REPREP_LATEX
           created by   step:./plan.py
             consumes   file:./
             consumes   file:paper.tex
             consumes   file:subdir/code.txt
             consumes   file:subdir/generated.tex
-             creates   file:paper.MANIFEST.txt
+             creates   file:paper-inventory.txt
              creates   file:paper.aux
              creates   file:paper.log
              creates   file:paper.out
              creates   file:paper.pdf
-            supplies   file:paper.MANIFEST.txt
+            supplies   file:paper-inventory.txt
             supplies   file:paper.aux
             supplies   file:paper.log
             supplies   file:paper.out
             supplies   file:paper.pdf
 
-file:paper.MANIFEST.txt
-                path = paper.MANIFEST.txt
+file:paper-inventory.txt
+                path = paper-inventory.txt
                state = BUILT
           created by   step:python -m stepup.reprep.latex paper.tex --run-bibtex
             consumes   file:./
             consumes   step:python -m stepup.reprep.latex paper.tex --run-bibtex
 
 file:paper.aux
                 path = paper.aux
```

### Comparing `stepup_reprep-1.1.2/tests/cases/xelatex_input/expected_stdout.txt` & `stepup_reprep-1.2.0/tests/cases/xelatex_input/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/xelatex_input/main.sh` & `stepup_reprep-1.2.0/tests/cases/nup_pdf/main.sh`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
-export SOURCE_DATE_EPOCH="315532800"
-export REPREP_LATEX="xelatex"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
 
@@ -18,34 +16,26 @@
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
 EOD
 
 # Reproducibility test
-rm paper.aux
-rm paper.log
-rm subdir/generated.tex
-rm subdir/code.txt
-mv paper.pdf paper1.pdf
+mv dst.pdf dst1.pdf
 python3 - << EOD
 from stepup.core.interact import *
-from stepup.reprep.make_manifest import write_manifest
-watch_delete("paper.pdf")
-watch_delete("subdir/generated.tex")
-watch_delete("subdir/code.txt")
+from stepup.reprep.make_inventory import write_inventory
+watch_delete("dst.pdf")
 run()
 join()
-write_manifest("reproducibility_manifest.txt", ["paper.pdf", "paper1.pdf"])
+write_inventory("reproducibility_inventory.txt", ["dst.pdf", "dst1.pdf"])
 EOD
 
 # Wait for background processes, if any.
 wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f paper.pdf ]] || exit -1
-[[ -f paper.log ]] || exit -1
-[[ -f paper.aux ]] || exit -1
-[[ -f paper1.pdf ]] || exit -1
-[[ -f reproducibility_manifest.txt ]] || exit -1
-reprep-check-manifest paper.MANIFEST.txt
+[[ -f src.pdf ]] || exit -1
+[[ -f dst.pdf ]] || exit -1
+[[ -f dst1.pdf ]] || exit -1
+[[ -f reproducibility_inventory.txt ]] || exit -1
```

### Comparing `stepup_reprep-1.1.2/tests/cases/xelatex_input/smile.pdf` & `stepup_reprep-1.2.0/tests/cases/xelatex_input/smile.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/cases/zip_manifest/expected_stdout.txt` & `stepup_reprep-1.2.0/tests/cases/convert_markdown/expected_stdout.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,16 @@
   DIRECTOR │ Launched worker 0
      PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
-     START │ echo hello > built.txt
-   SUCCESS │ echo hello > built.txt
-     START │ reprep-make-manifest static.txt built.txt -o MANIFEST.txt
-   SUCCESS │ reprep-make-manifest static.txt built.txt -o MANIFEST.txt
-     START │ python -m stepup.reprep.zip_manifest MANIFEST.txt upload.zip
-   SUCCESS │ python -m stepup.reprep.zip_manifest MANIFEST.txt upload.zip
+     START │ python -m stepup.reprep.convert_markdown demo.md demo.html --katex --katex-macros=macros.tex
+   SUCCESS │ python -m stepup.reprep.convert_markdown demo.md demo.html --katex --katex-macros=macros.tex
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
-   DELETED │ built.txt
-   DELETED │ upload.zip
+   DELETED │ demo.html
      PHASE │ run
-     START │ echo hello > built.txt
-   SUCCESS │ echo hello > built.txt
-      SKIP │ reprep-make-manifest static.txt built.txt -o MANIFEST.txt
-     START │ python -m stepup.reprep.zip_manifest MANIFEST.txt upload.zip
-   SUCCESS │ python -m stepup.reprep.zip_manifest MANIFEST.txt upload.zip
+     START │ python -m stepup.reprep.convert_markdown demo.md demo.html --katex --katex-macros=macros.tex
+   SUCCESS │ python -m stepup.reprep.convert_markdown demo.md demo.html --katex --katex-macros=macros.tex
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
   DIRECTOR │ Stopping workers.
   DIRECTOR │ See you!
```

### Comparing `stepup_reprep-1.1.2/tests/conftest.py` & `stepup_reprep-1.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/reprep_common.py` & `stepup_reprep-1.2.0/tests/reprep_common.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/test_bibtex_log.py` & `stepup_reprep-1.2.0/tests/test_bibtex_log.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/test_cases.py` & `stepup_reprep-1.2.0/tests/test_cases.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,21 +38,19 @@
         "add_notes_pdf",
         "check_hrefs_html",
         "check_hrefs_md",
         "convert_markdown",
         "convert_weasyprint",
         "latex_flat",
         "latex_flat_subdir",
-        "make_manifest_in",
-        "make_manifest_in_sub",
-        "make_manifest_list",
+        "make_inventory_list",
         "nup_pdf",
         "raster_pdf",
         "render_basic",
-        "zip_manifest",
+        "zip_inventory",
     ],
 )
 @pytest.mark.asyncio
 async def test_example(tmpdir, name: str):
     await run_example(Path("tests/cases") / name, tmpdir, OVERWRITE_EXPECTED)
```

### Comparing `stepup_reprep-1.1.2/tests/test_latex_deps.py` & `stepup_reprep-1.2.0/tests/test_latex_deps.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/test_latex_flat.py` & `stepup_reprep-1.2.0/tests/test_latex_flat.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/test_latex_log.py` & `stepup_reprep-1.2.0/tests/test_latex_log.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.2/tests/test_zip.py` & `stepup_reprep-1.2.0/tests/test_zip.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,47 +13,47 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
-"""Unit tests for stepup.reprep.zip_manifest."""
+"""Unit tests for stepup.reprep.zip_inventory."""
 
 import contextlib
 import zipfile
 
-from stepup.reprep.make_manifest import write_manifest
-from stepup.reprep.zip_manifest import zip_manifest
+from stepup.reprep.make_inventory import write_inventory
+from stepup.reprep.zip_inventory import zip_inventory
 
 
 def test_simple_chdir(path_tmp):
     with contextlib.chdir(path_tmp):
         with open("a.txt", "w") as fh:
             fh.write("Aaa")
         with open("b.txt", "w") as fh:
             fh.write("Bbb")
-        write_manifest("MANIFEST.txt", ["a.txt", "b.txt"])
-        zip_manifest("MANIFEST.txt", "test.zip")
+        write_inventory("inventory.txt", ["a.txt", "b.txt"])
+        zip_inventory("inventory.txt", "test.zip")
         contents = {}
         with zipfile.ZipFile("test.zip", "r") as fz:
             for name in fz.namelist():
                 contents[name] = fz.read(name).decode("utf-8")
         assert contents["a.txt"] == "Aaa"
         assert contents["b.txt"] == "Bbb"
-        assert "MANIFEST.txt" in contents
+        assert "inventory.txt" in contents
 
 
 def test_simple(path_tmp):
     with open(path_tmp / "a.txt", "w") as fh:
         fh.write("Aaa")
     with open(path_tmp / "b.txt", "w") as fh:
         fh.write("Bbb")
-    write_manifest(path_tmp / "MANIFEST.txt", [path_tmp / "a.txt", path_tmp / "b.txt"])
-    zip_manifest(path_tmp / "MANIFEST.txt", path_tmp / "test.zip")
+    write_inventory(path_tmp / "inventory.txt", [path_tmp / "a.txt", path_tmp / "b.txt"])
+    zip_inventory(path_tmp / "inventory.txt")
     contents = {}
-    with zipfile.ZipFile(path_tmp / "test.zip", "r") as fz:
+    with zipfile.ZipFile(path_tmp / "inventory.zip", "r") as fz:
         for name in fz.namelist():
             contents[name] = fz.read(name).decode("utf-8")
     assert contents["a.txt"] == "Aaa"
     assert contents["b.txt"] == "Bbb"
-    assert "MANIFEST.txt" in contents
+    assert "inventory.txt" in contents
```

