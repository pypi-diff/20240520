# Comparing `tmp/dashtable2-1.4.6.tar.gz` & `tmp/dashtable2-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dashtable2-1.4.6.tar", last modified: Mon May 20 16:12:28 2024, max compression
+gzip compressed data, was "dashtable2-1.4.7.tar", last modified: Mon May 20 18:22:56 2024, max compression
```

## Comparing `dashtable2-1.4.6.tar` & `dashtable2-1.4.7.tar`

### file list

```diff
@@ -1,92 +1,91 @@
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 16:12:28.496844 dashtable2-1.4.6/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1068 2024-05-20 13:11:43.000000 dashtable2-1.4.6/LICENSE.txt
--rw-r--r--   0 pasa      (1000) pasa      (1000)     1067 2024-05-20 16:12:28.496844 dashtable2-1.4.6/PKG-INFO
--rw-r--r--   0 pasa      (1000) pasa      (1000)      480 2024-05-20 13:40:39.000000 dashtable2-1.4.6/README.md
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 16:12:28.482844 dashtable2-1.4.6/dashtable/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      418 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/__init__.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 16:12:28.484844 dashtable2-1.4.6/dashtable/dashutils/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      441 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/dashutils/__init__.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1134 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/dashutils/add_cushions.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      760 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/dashutils/center_line.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)     3239 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/dashutils/checks.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      326 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/dashutils/ensure_table_strings.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      547 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/dashutils/make_empty_table.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      798 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/dashutils/make_span.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      436 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/dashutils/multis_2_mono.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)     3789 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/dashutils/spans.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 16:12:28.484844 dashtable2-1.4.6/dashtable/data2md/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)       29 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2md/__init__.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1886 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2md/data2md.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      546 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2md/get_column_width.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 16:12:28.486844 dashtable2-1.4.6/dashtable/data2rst/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)       31 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2rst/__init__.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 16:12:28.487844 dashtable2-1.4.6/dashtable/data2rst/cell/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      334 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2rst/cell/__init__.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     3643 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2rst/cell/cell.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1291 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2rst/cell/center_cell_text.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      254 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2rst/cell/get_longest_line_length.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     2208 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2rst/cell/get_merge_direction.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      203 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2rst/cell/is_only.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1910 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2rst/cell/merge_cells.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1796 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2rst/cell/v_center_cell_text.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     3661 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2rst/data2rst.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     2085 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2rst/get_output_column_widths.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1558 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2rst/get_output_row_heights.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1867 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2rst/make_cell.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1497 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2rst/merge_all_cells.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      937 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2rst/table_cells_2_spans.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 16:12:28.488844 dashtable2-1.4.6/dashtable/data2simplerst/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)       73 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2simplerst/__init__.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     4528 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2simplerst/data2simplerst.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      463 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2simplerst/row_includes_spans.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)      135 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/exceptions.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 16:12:28.489844 dashtable2-1.4.6/dashtable/grid2data/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)       33 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/grid2data/__init__.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     3471 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/grid2data/grid2data.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 16:12:28.490844 dashtable2-1.4.6/dashtable/html2data/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)       33 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/__init__.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1630 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/extract_spans.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     2693 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/extract_table.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      483 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/find_unassigned_table_cell.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1058 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/get_html_column_count.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      454 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/get_html_row_count.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      586 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/headers_present.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1089 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/html2data.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 16:12:28.491844 dashtable2-1.4.6/dashtable/html2data/restructify/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)       37 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/__init__.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1768 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/add_links.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 16:12:28.495844 dashtable2-1.4.6/dashtable/html2data/restructify/converters/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      619 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/__init__.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      350 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_a.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      167 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_b.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      486 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_blockquote.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      105 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_br.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)       94 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_cite.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      312 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_dd.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      442 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_div.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      129 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_em.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      155 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_h1.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      160 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_h2.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      167 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_h3.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      151 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_i.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      288 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_img.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1201 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_li.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      368 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_p.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      272 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_strong.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)       94 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_tt.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      771 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/process_tag.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1126 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/restructify.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1658 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2md.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     2571 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2rst.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 16:12:28.495844 dashtable2-1.4.6/dashtable/simple2data/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)       37 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/simple2data/__init__.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     3651 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/simple2data/simple2data.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      512 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/simple2data/truncate_empty_lines.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 16:12:28.496844 dashtable2-1.4.6/dashtable2.egg-info/
--rw-r--r--   0 pasa      (1000) pasa      (1000)     1067 2024-05-20 16:12:28.000000 dashtable2-1.4.6/dashtable2.egg-info/PKG-INFO
--rw-r--r--   0 pasa      (1000) pasa      (1000)     3140 2024-05-20 16:12:28.000000 dashtable2-1.4.6/dashtable2.egg-info/SOURCES.txt
--rw-r--r--   0 pasa      (1000) pasa      (1000)        1 2024-05-20 16:12:28.000000 dashtable2-1.4.6/dashtable2.egg-info/dependency_links.txt
--rw-r--r--   0 pasa      (1000) pasa      (1000)       37 2024-05-20 16:12:28.000000 dashtable2-1.4.6/dashtable2.egg-info/requires.txt
--rw-r--r--   0 pasa      (1000) pasa      (1000)       10 2024-05-20 16:12:28.000000 dashtable2-1.4.6/dashtable2.egg-info/top_level.txt
--rw-r--r--   0 pasa      (1000) pasa      (1000)       38 2024-05-20 16:12:28.497844 dashtable2-1.4.6/setup.cfg
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1437 2024-05-20 15:48:35.000000 dashtable2-1.4.6/setup.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 18:22:56.127946 dashtable2-1.4.7/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1068 2024-05-20 13:11:43.000000 dashtable2-1.4.7/LICENSE.txt
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     1107 2024-05-20 18:22:56.127946 dashtable2-1.4.7/PKG-INFO
+-rw-r--r--   0 pasa      (1000) pasa      (1000)      480 2024-05-20 13:40:39.000000 dashtable2-1.4.7/README.md
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 18:22:56.117946 dashtable2-1.4.7/dashtable/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      418 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/__init__.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 18:22:56.119946 dashtable2-1.4.7/dashtable/dashutils/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      441 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/dashutils/__init__.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1134 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/dashutils/add_cushions.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      760 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/dashutils/center_line.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     3239 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/dashutils/checks.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      326 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/dashutils/ensure_table_strings.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      547 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/dashutils/make_empty_table.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      798 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/dashutils/make_span.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      436 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/dashutils/multis_2_mono.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     3789 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/dashutils/spans.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 18:22:56.119946 dashtable2-1.4.7/dashtable/data2md/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)       29 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/data2md/__init__.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1886 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/data2md/data2md.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      546 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/data2md/get_column_width.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 18:22:56.120946 dashtable2-1.4.7/dashtable/data2rst/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)       31 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/data2rst/__init__.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 18:22:56.121946 dashtable2-1.4.7/dashtable/data2rst/cell/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      296 2024-05-20 18:22:16.000000 dashtable2-1.4.7/dashtable/data2rst/cell/__init__.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     3643 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/data2rst/cell/cell.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1291 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/data2rst/cell/center_cell_text.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      254 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/data2rst/cell/get_longest_line_length.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      203 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/data2rst/cell/is_only.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     4914 2024-05-20 18:22:16.000000 dashtable2-1.4.7/dashtable/data2rst/cell/merge.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1796 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/data2rst/cell/v_center_cell_text.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     3661 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/data2rst/data2rst.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     2085 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/data2rst/get_output_column_widths.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1558 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/data2rst/get_output_row_heights.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1867 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/data2rst/make_cell.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1501 2024-05-20 18:22:16.000000 dashtable2-1.4.7/dashtable/data2rst/merge_all_cells.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      937 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/data2rst/table_cells_2_spans.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 18:22:56.121946 dashtable2-1.4.7/dashtable/data2simplerst/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)       73 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/data2simplerst/__init__.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     4528 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/data2simplerst/data2simplerst.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      463 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/data2simplerst/row_includes_spans.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)      135 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/exceptions.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 18:22:56.121946 dashtable2-1.4.7/dashtable/grid2data/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)       33 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/grid2data/__init__.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     3471 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/grid2data/grid2data.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 18:22:56.122946 dashtable2-1.4.7/dashtable/html2data/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)       33 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/html2data/__init__.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1630 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/html2data/extract_spans.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     2693 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/html2data/extract_table.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      483 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/html2data/find_unassigned_table_cell.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1058 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/html2data/get_html_column_count.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      454 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/html2data/get_html_row_count.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      586 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/html2data/headers_present.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1089 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/html2data/html2data.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 18:22:56.123946 dashtable2-1.4.7/dashtable/html2data/restructify/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)       37 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/html2data/restructify/__init__.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1768 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/html2data/restructify/add_links.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 18:22:56.125946 dashtable2-1.4.7/dashtable/html2data/restructify/converters/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      619 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/html2data/restructify/converters/__init__.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      350 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/html2data/restructify/converters/convert_a.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      167 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/html2data/restructify/converters/convert_b.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      486 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/html2data/restructify/converters/convert_blockquote.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      105 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/html2data/restructify/converters/convert_br.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)       94 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/html2data/restructify/converters/convert_cite.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      312 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/html2data/restructify/converters/convert_dd.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      442 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/html2data/restructify/converters/convert_div.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      129 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/html2data/restructify/converters/convert_em.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      155 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/html2data/restructify/converters/convert_h1.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      160 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/html2data/restructify/converters/convert_h2.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      167 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/html2data/restructify/converters/convert_h3.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      151 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/html2data/restructify/converters/convert_i.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      288 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/html2data/restructify/converters/convert_img.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1201 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/html2data/restructify/converters/convert_li.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      368 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/html2data/restructify/converters/convert_p.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      272 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/html2data/restructify/converters/convert_strong.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)       94 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/html2data/restructify/converters/convert_tt.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      771 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/html2data/restructify/process_tag.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1126 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/html2data/restructify/restructify.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1658 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/html2md.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     2571 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/html2rst.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 18:22:56.126946 dashtable2-1.4.7/dashtable/simple2data/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)       37 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/simple2data/__init__.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     3651 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/simple2data/simple2data.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      512 2024-05-20 13:11:43.000000 dashtable2-1.4.7/dashtable/simple2data/truncate_empty_lines.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 18:22:56.126946 dashtable2-1.4.7/dashtable2.egg-info/
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     1107 2024-05-20 18:22:56.000000 dashtable2-1.4.7/dashtable2.egg-info/PKG-INFO
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     3087 2024-05-20 18:22:56.000000 dashtable2-1.4.7/dashtable2.egg-info/SOURCES.txt
+-rw-r--r--   0 pasa      (1000) pasa      (1000)        1 2024-05-20 18:22:56.000000 dashtable2-1.4.7/dashtable2.egg-info/dependency_links.txt
+-rw-r--r--   0 pasa      (1000) pasa      (1000)       37 2024-05-20 18:22:56.000000 dashtable2-1.4.7/dashtable2.egg-info/requires.txt
+-rw-r--r--   0 pasa      (1000) pasa      (1000)       10 2024-05-20 18:22:56.000000 dashtable2-1.4.7/dashtable2.egg-info/top_level.txt
+-rw-r--r--   0 pasa      (1000) pasa      (1000)       38 2024-05-20 18:22:56.127946 dashtable2-1.4.7/setup.cfg
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1488 2024-05-20 16:14:28.000000 dashtable2-1.4.7/setup.py
```

### Comparing `dashtable2-1.4.6/LICENSE.txt` & `dashtable2-1.4.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.6/PKG-INFO` & `dashtable2-1.4.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: dashtable2
-Version: 1.4.6
+Version: 1.4.7
 Summary: A library for converting a HTML tables into ASCII tables, rowspan and colspan allowed!
 Home-page: https://github.com/PasaOpasen/dashtable2
 Author: doakey3 & gustavklopp & pasaopasen
 Author-email: qtckpuhdsa@gmail.com
 License: MIT
 Keywords: text table,conversion,documentation
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
 # DashTable2
 
 [![PyPI
 version](https://badge.fury.io/py/dashtable2.svg)](https://pypi.org/project/dashtable2/)
```

### Comparing `dashtable2-1.4.6/dashtable/dashutils/add_cushions.py` & `dashtable2-1.4.7/dashtable/dashutils/add_cushions.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.6/dashtable/dashutils/center_line.py` & `dashtable2-1.4.7/dashtable/dashutils/center_line.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.6/dashtable/dashutils/checks.py` & `dashtable2-1.4.7/dashtable/dashutils/checks.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.6/dashtable/dashutils/make_empty_table.py` & `dashtable2-1.4.7/dashtable/dashutils/make_empty_table.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.6/dashtable/dashutils/make_span.py` & `dashtable2-1.4.7/dashtable/dashutils/make_span.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.6/dashtable/dashutils/spans.py` & `dashtable2-1.4.7/dashtable/dashutils/spans.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.6/dashtable/data2md/data2md.py` & `dashtable2-1.4.7/dashtable/data2md/data2md.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.6/dashtable/data2md/get_column_width.py` & `dashtable2-1.4.7/dashtable/data2md/get_column_width.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.6/dashtable/data2rst/cell/cell.py` & `dashtable2-1.4.7/dashtable/data2rst/cell/cell.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.6/dashtable/data2rst/cell/center_cell_text.py` & `dashtable2-1.4.7/dashtable/data2rst/cell/center_cell_text.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.6/dashtable/data2rst/cell/v_center_cell_text.py` & `dashtable2-1.4.7/dashtable/data2rst/cell/v_center_cell_text.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.6/dashtable/data2rst/data2rst.py` & `dashtable2-1.4.7/dashtable/data2rst/data2rst.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.6/dashtable/data2rst/get_output_column_widths.py` & `dashtable2-1.4.7/dashtable/data2rst/get_output_column_widths.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.6/dashtable/data2rst/get_output_row_heights.py` & `dashtable2-1.4.7/dashtable/data2rst/get_output_row_heights.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.6/dashtable/data2rst/make_cell.py` & `dashtable2-1.4.7/dashtable/data2rst/make_cell.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.6/dashtable/data2rst/merge_all_cells.py` & `dashtable2-1.4.7/dashtable/data2rst/merge_all_cells.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,20 +29,20 @@
         count = 0
 
         while count < len(cells):
             cell1 = cells[current]
             cell2 = cells[count]
 
             merge_direction = get_merge_direction(cell1, cell2)
-            if merge_direction == "NONE":
+            if merge_direction is None:
 
                 if checked[current, count]:  # already checked
                     if checked.all():  # if all combinations checked -- raise infinite loop error
                         from ..exceptions import NonMergableException
-                        raise NonMergableException('current cells cannot be merged due to too heavy structure')
+                        raise NonMergableException('current cells cannot be merged due to too complicated structure')
 
                 checked[current, count] = True
                 count += 1
             else:
                 merge_cells(cell1, cell2, merge_direction)
 
                 if current > count:
```

### Comparing `dashtable2-1.4.6/dashtable/data2rst/table_cells_2_spans.py` & `dashtable2-1.4.7/dashtable/data2rst/table_cells_2_spans.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.6/dashtable/data2simplerst/data2simplerst.py` & `dashtable2-1.4.7/dashtable/data2simplerst/data2simplerst.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.6/dashtable/grid2data/grid2data.py` & `dashtable2-1.4.7/dashtable/grid2data/grid2data.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.6/dashtable/html2data/extract_spans.py` & `dashtable2-1.4.7/dashtable/html2data/extract_spans.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.6/dashtable/html2data/extract_table.py` & `dashtable2-1.4.7/dashtable/html2data/extract_table.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.6/dashtable/html2data/get_html_column_count.py` & `dashtable2-1.4.7/dashtable/html2data/get_html_column_count.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.6/dashtable/html2data/headers_present.py` & `dashtable2-1.4.7/dashtable/html2data/headers_present.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.6/dashtable/html2data/html2data.py` & `dashtable2-1.4.7/dashtable/html2data/html2data.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.6/dashtable/html2data/restructify/add_links.py` & `dashtable2-1.4.7/dashtable/html2data/restructify/add_links.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.6/dashtable/html2data/restructify/converters/__init__.py` & `dashtable2-1.4.7/dashtable/html2data/restructify/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_li.py` & `dashtable2-1.4.7/dashtable/html2data/restructify/converters/convert_li.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.6/dashtable/html2data/restructify/process_tag.py` & `dashtable2-1.4.7/dashtable/html2data/restructify/process_tag.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.6/dashtable/html2data/restructify/restructify.py` & `dashtable2-1.4.7/dashtable/html2data/restructify/restructify.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.6/dashtable/html2md.py` & `dashtable2-1.4.7/dashtable/html2md.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.6/dashtable/html2rst.py` & `dashtable2-1.4.7/dashtable/html2rst.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.6/dashtable/simple2data/simple2data.py` & `dashtable2-1.4.7/dashtable/simple2data/simple2data.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.6/dashtable/simple2data/truncate_empty_lines.py` & `dashtable2-1.4.7/dashtable/simple2data/truncate_empty_lines.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.6/dashtable2.egg-info/PKG-INFO` & `dashtable2-1.4.7/dashtable2.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: dashtable2
-Version: 1.4.6
+Version: 1.4.7
 Summary: A library for converting a HTML tables into ASCII tables, rowspan and colspan allowed!
 Home-page: https://github.com/PasaOpasen/dashtable2
 Author: doakey3 & gustavklopp & pasaopasen
 Author-email: qtckpuhdsa@gmail.com
 License: MIT
 Keywords: text table,conversion,documentation
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
 # DashTable2
 
 [![PyPI
 version](https://badge.fury.io/py/dashtable2.svg)](https://pypi.org/project/dashtable2/)
```

### Comparing `dashtable2-1.4.6/dashtable2.egg-info/SOURCES.txt` & `dashtable2-1.4.7/dashtable2.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,16 @@
 dashtable/data2rst/make_cell.py
 dashtable/data2rst/merge_all_cells.py
 dashtable/data2rst/table_cells_2_spans.py
 dashtable/data2rst/cell/__init__.py
 dashtable/data2rst/cell/cell.py
 dashtable/data2rst/cell/center_cell_text.py
 dashtable/data2rst/cell/get_longest_line_length.py
-dashtable/data2rst/cell/get_merge_direction.py
 dashtable/data2rst/cell/is_only.py
-dashtable/data2rst/cell/merge_cells.py
+dashtable/data2rst/cell/merge.py
 dashtable/data2rst/cell/v_center_cell_text.py
 dashtable/data2simplerst/__init__.py
 dashtable/data2simplerst/data2simplerst.py
 dashtable/data2simplerst/row_includes_spans.py
 dashtable/grid2data/__init__.py
 dashtable/grid2data/grid2data.py
 dashtable/html2data/__init__.py
```

### Comparing `dashtable2-1.4.6/setup.py` & `dashtable2-1.4.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         'dashtable.html2data.restructify',
         'dashtable.html2data.restructify.converters'
     ],
     version=Path('version.txt').read_text(encoding='utf-8').strip(),
 
     description='A library for converting a HTML tables into ASCII tables, rowspan and colspan allowed!',
     long_description=open('README.md').read(),
+    long_description_content_type="text/markdown",
 
     author='doakey3 & gustavklopp & pasaopasen',
     author_email='qtckpuhdsa@gmail.com',
     url='https://github.com/PasaOpasen/dashtable2',
     license='MIT',
     keywords=[
         'text table', 'conversion', 'documentation'
```

