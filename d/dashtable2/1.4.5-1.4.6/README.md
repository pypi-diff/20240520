# Comparing `tmp/dashtable2-1.4.5.tar.gz` & `tmp/dashtable2-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dashtable2-1.4.5.tar", last modified: Thu May 16 19:08:28 2024, max compression
+gzip compressed data, was "dashtable2-1.4.6.tar", last modified: Mon May 20 16:12:28 2024, max compression
```

## Comparing `dashtable2-1.4.5.tar` & `dashtable2-1.4.6.tar`

### file list

```diff
@@ -1,97 +1,92 @@
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-16 19:08:28.504299 dashtable2-1.4.5/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1068 2024-05-16 18:55:09.000000 dashtable2-1.4.5/LICENSE.txt
--rw-r--r--   0 pasa      (1000) pasa      (1000)     2035 2024-05-16 19:08:28.504299 dashtable2-1.4.5/PKG-INFO
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1715 2024-05-16 18:55:09.000000 dashtable2-1.4.5/README.rst
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-16 19:08:28.494299 dashtable2-1.4.5/dashtable/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      418 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/__init__.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-16 19:08:28.496299 dashtable2-1.4.5/dashtable/dashutils/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      632 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/dashutils/__init__.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1134 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/dashutils/add_cushions.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      760 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/dashutils/center_line.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     2283 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/dashutils/check_span.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      938 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/dashutils/check_table.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      366 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/dashutils/ensure_table_strings.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      254 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/dashutils/get_longest_line_length.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      507 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/dashutils/get_span.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      741 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/dashutils/get_span_char_height.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      750 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/dashutils/get_span_char_width.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      827 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/dashutils/get_span_column_count.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      813 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/dashutils/get_span_row_count.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      547 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/dashutils/make_empty_table.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      798 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/dashutils/make_span.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      436 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/dashutils/multis_2_mono.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-16 19:08:28.496299 dashtable2-1.4.5/dashtable/data2md/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)       29 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/data2md/__init__.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1886 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/data2md/data2md.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      546 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/data2md/get_column_width.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-16 19:08:28.497299 dashtable2-1.4.5/dashtable/data2rst/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)       31 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/data2rst/__init__.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-16 19:08:28.498299 dashtable2-1.4.5/dashtable/data2rst/cell/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      334 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/data2rst/cell/__init__.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     3643 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/data2rst/cell/cell.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1291 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/data2rst/cell/center_cell_text.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      254 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/data2rst/cell/get_longest_line_length.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     2208 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/data2rst/cell/get_merge_direction.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      203 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/data2rst/cell/is_only.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1910 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/data2rst/cell/merge_cells.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1796 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/data2rst/cell/v_center_cell_text.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     3571 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/data2rst/data2rst.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     2123 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/data2rst/get_output_column_widths.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1574 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/data2rst/get_output_row_heights.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1921 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/data2rst/make_cell.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1497 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/data2rst/merge_all_cells.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      937 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/data2rst/table_cells_2_spans.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-16 19:08:28.499299 dashtable2-1.4.5/dashtable/data2simplerst/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)       73 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/data2simplerst/__init__.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     4606 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/data2simplerst/data2simplerst.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      463 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/data2simplerst/row_includes_spans.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)      135 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/exceptions.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-16 19:08:28.499299 dashtable2-1.4.5/dashtable/grid2data/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)       33 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/grid2data/__init__.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     3471 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/grid2data/grid2data.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-16 19:08:28.500299 dashtable2-1.4.5/dashtable/html2data/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)       33 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/html2data/__init__.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1630 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/html2data/extract_spans.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     2693 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/html2data/extract_table.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      483 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/html2data/find_unassigned_table_cell.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1058 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/html2data/get_html_column_count.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      454 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/html2data/get_html_row_count.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      586 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/html2data/headers_present.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1089 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/html2data/html2data.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-16 19:08:28.501299 dashtable2-1.4.5/dashtable/html2data/restructify/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)       37 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/html2data/restructify/__init__.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1768 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/html2data/restructify/add_links.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-16 19:08:28.503299 dashtable2-1.4.5/dashtable/html2data/restructify/converters/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      619 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/html2data/restructify/converters/__init__.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      350 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/html2data/restructify/converters/convert_a.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      167 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/html2data/restructify/converters/convert_b.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      486 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/html2data/restructify/converters/convert_blockquote.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      105 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/html2data/restructify/converters/convert_br.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)       94 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/html2data/restructify/converters/convert_cite.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      312 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/html2data/restructify/converters/convert_dd.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      442 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/html2data/restructify/converters/convert_div.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      129 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/html2data/restructify/converters/convert_em.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      155 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/html2data/restructify/converters/convert_h1.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      160 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/html2data/restructify/converters/convert_h2.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      167 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/html2data/restructify/converters/convert_h3.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      151 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/html2data/restructify/converters/convert_i.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      288 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/html2data/restructify/converters/convert_img.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1201 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/html2data/restructify/converters/convert_li.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      368 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/html2data/restructify/converters/convert_p.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      272 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/html2data/restructify/converters/convert_strong.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)       94 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/html2data/restructify/converters/convert_tt.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      771 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/html2data/restructify/process_tag.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1126 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/html2data/restructify/restructify.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1658 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/html2md.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     2577 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/html2rst.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-16 19:08:28.503299 dashtable2-1.4.5/dashtable/simple2data/
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)       37 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/simple2data/__init__.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)     3650 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/simple2data/simple2data.py
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      512 2024-05-16 18:55:09.000000 dashtable2-1.4.5/dashtable/simple2data/truncate_empty_lines.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-16 19:08:28.504299 dashtable2-1.4.5/dashtable2.egg-info/
--rw-r--r--   0 pasa      (1000) pasa      (1000)     2035 2024-05-16 19:08:28.000000 dashtable2-1.4.5/dashtable2.egg-info/PKG-INFO
--rw-r--r--   0 pasa      (1000) pasa      (1000)     3371 2024-05-16 19:08:28.000000 dashtable2-1.4.5/dashtable2.egg-info/SOURCES.txt
--rw-r--r--   0 pasa      (1000) pasa      (1000)        1 2024-05-16 19:08:28.000000 dashtable2-1.4.5/dashtable2.egg-info/dependency_links.txt
--rw-r--r--   0 pasa      (1000) pasa      (1000)       10 2024-05-16 19:08:28.000000 dashtable2-1.4.5/dashtable2.egg-info/top_level.txt
--rw-r--r--   0 pasa      (1000) pasa      (1000)       38 2024-05-16 19:08:28.505299 dashtable2-1.4.5/setup.cfg
--rwxr-xr-x   0 pasa      (1000) pasa      (1000)      869 2024-05-16 19:03:26.000000 dashtable2-1.4.5/setup.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 16:12:28.496844 dashtable2-1.4.6/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1068 2024-05-20 13:11:43.000000 dashtable2-1.4.6/LICENSE.txt
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     1067 2024-05-20 16:12:28.496844 dashtable2-1.4.6/PKG-INFO
+-rw-r--r--   0 pasa      (1000) pasa      (1000)      480 2024-05-20 13:40:39.000000 dashtable2-1.4.6/README.md
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 16:12:28.482844 dashtable2-1.4.6/dashtable/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      418 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/__init__.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 16:12:28.484844 dashtable2-1.4.6/dashtable/dashutils/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      441 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/dashutils/__init__.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1134 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/dashutils/add_cushions.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      760 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/dashutils/center_line.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     3239 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/dashutils/checks.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      326 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/dashutils/ensure_table_strings.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      547 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/dashutils/make_empty_table.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      798 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/dashutils/make_span.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      436 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/dashutils/multis_2_mono.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     3789 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/dashutils/spans.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 16:12:28.484844 dashtable2-1.4.6/dashtable/data2md/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)       29 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2md/__init__.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1886 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2md/data2md.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      546 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2md/get_column_width.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 16:12:28.486844 dashtable2-1.4.6/dashtable/data2rst/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)       31 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2rst/__init__.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 16:12:28.487844 dashtable2-1.4.6/dashtable/data2rst/cell/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      334 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2rst/cell/__init__.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     3643 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2rst/cell/cell.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1291 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2rst/cell/center_cell_text.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      254 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2rst/cell/get_longest_line_length.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     2208 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2rst/cell/get_merge_direction.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      203 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2rst/cell/is_only.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1910 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2rst/cell/merge_cells.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1796 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2rst/cell/v_center_cell_text.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     3661 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2rst/data2rst.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     2085 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2rst/get_output_column_widths.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1558 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2rst/get_output_row_heights.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1867 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2rst/make_cell.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1497 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2rst/merge_all_cells.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      937 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2rst/table_cells_2_spans.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 16:12:28.488844 dashtable2-1.4.6/dashtable/data2simplerst/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)       73 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2simplerst/__init__.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     4528 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2simplerst/data2simplerst.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      463 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/data2simplerst/row_includes_spans.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)      135 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/exceptions.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 16:12:28.489844 dashtable2-1.4.6/dashtable/grid2data/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)       33 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/grid2data/__init__.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     3471 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/grid2data/grid2data.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 16:12:28.490844 dashtable2-1.4.6/dashtable/html2data/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)       33 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/__init__.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1630 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/extract_spans.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     2693 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/extract_table.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      483 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/find_unassigned_table_cell.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1058 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/get_html_column_count.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      454 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/get_html_row_count.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      586 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/headers_present.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1089 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/html2data.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 16:12:28.491844 dashtable2-1.4.6/dashtable/html2data/restructify/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)       37 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/__init__.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1768 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/add_links.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 16:12:28.495844 dashtable2-1.4.6/dashtable/html2data/restructify/converters/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      619 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/__init__.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      350 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_a.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      167 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_b.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      486 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_blockquote.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      105 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_br.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)       94 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_cite.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      312 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_dd.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      442 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_div.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      129 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_em.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      155 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_h1.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      160 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_h2.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      167 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_h3.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      151 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_i.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      288 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_img.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1201 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_li.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      368 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_p.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      272 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_strong.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)       94 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_tt.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      771 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/process_tag.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1126 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2data/restructify/restructify.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1658 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2md.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     2571 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/html2rst.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 16:12:28.495844 dashtable2-1.4.6/dashtable/simple2data/
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)       37 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/simple2data/__init__.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     3651 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/simple2data/simple2data.py
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)      512 2024-05-20 13:11:43.000000 dashtable2-1.4.6/dashtable/simple2data/truncate_empty_lines.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-05-20 16:12:28.496844 dashtable2-1.4.6/dashtable2.egg-info/
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     1067 2024-05-20 16:12:28.000000 dashtable2-1.4.6/dashtable2.egg-info/PKG-INFO
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     3140 2024-05-20 16:12:28.000000 dashtable2-1.4.6/dashtable2.egg-info/SOURCES.txt
+-rw-r--r--   0 pasa      (1000) pasa      (1000)        1 2024-05-20 16:12:28.000000 dashtable2-1.4.6/dashtable2.egg-info/dependency_links.txt
+-rw-r--r--   0 pasa      (1000) pasa      (1000)       37 2024-05-20 16:12:28.000000 dashtable2-1.4.6/dashtable2.egg-info/requires.txt
+-rw-r--r--   0 pasa      (1000) pasa      (1000)       10 2024-05-20 16:12:28.000000 dashtable2-1.4.6/dashtable2.egg-info/top_level.txt
+-rw-r--r--   0 pasa      (1000) pasa      (1000)       38 2024-05-20 16:12:28.497844 dashtable2-1.4.6/setup.cfg
+-rwxr-xr-x   0 pasa      (1000) pasa      (1000)     1437 2024-05-20 15:48:35.000000 dashtable2-1.4.6/setup.py
```

### Comparing `dashtable2-1.4.5/LICENSE.txt` & `dashtable2-1.4.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.5/dashtable/dashutils/add_cushions.py` & `dashtable2-1.4.6/dashtable/dashutils/add_cushions.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.5/dashtable/dashutils/center_line.py` & `dashtable2-1.4.6/dashtable/dashutils/center_line.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.5/dashtable/dashutils/get_span_char_height.py` & `dashtable2-1.4.6/dashtable/dashutils/make_empty_table.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,24 @@
-from .get_span_row_count import get_span_row_count
-
-
-def get_span_char_height(span, row_heights):
+def make_empty_table(row_count, column_count):
     """
-    Get the height of a span in the number of newlines it fills.
+    Make an empty table
 
     Parameters
     ----------
-    span : list of list of int
-        A list of [row, column] pairs that make up the span
-    row_heights : list of int
-        A list of the number of newlines for each row in the table
+    row_count : int
+        The number of rows in the new table
+    column_count : int
+        The number of columns in the new table
 
     Returns
     -------
-    total_height : int
-        The height of the span in number of newlines
+    table : list of lists of str
+        Each cell will be an empty str ('')
     """
-    start_row = span[0][0]
-    row_count = get_span_row_count(span)
-    total_height = 0
-
-    for i in range(start_row, start_row + row_count):
-        total_height += row_heights[i]
-    total_height += row_count - 1
-
-    return total_height
+    table = []
+    while row_count > 0:
+        row = []
+        for column in range(column_count):
+            row.append('')
+        table.append(row)
+        row_count -= 1
+    return table
```

### Comparing `dashtable2-1.4.5/dashtable/dashutils/get_span_char_width.py` & `dashtable2-1.4.6/dashtable/data2md/get_column_width.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,24 @@
-from .get_span_column_count import get_span_column_count
-
-
-def get_span_char_width(span, column_widths):
+def get_column_width(column, table):
     """
-    Sum the widths of the columns that make up the span, plus the extra.
+    Get the character width of a column in a table
 
     Parameters
     ----------
-    span : list of lists of int
-        list of [row, column] pairs that make up the span
-    column_widths : list of int
-        The widths of the columns that make up the table
+    column : int
+        The column index analyze
+    table : list of lists of str
+        The table of rows of strings. For this to be accurate, each
+        string must only be 1 line long.
 
     Returns
     -------
-    total_width : int
-        The total width of the span
+        width : int
     """
+    width = 3
 
-    start_column = span[0][1]
-    column_count = get_span_column_count(span)
-    total_width = 0
-
-    for i in range(start_column, start_column + column_count):
-        total_width += column_widths[i]
-
-    total_width += column_count - 1
+    for row in range(len(table)):
+        cell_width = len(table[row][column])
+        if cell_width > width:
+            width = cell_width
 
-    return total_width
+    return width
```

### Comparing `dashtable2-1.4.5/dashtable/dashutils/make_span.py` & `dashtable2-1.4.6/dashtable/dashutils/make_span.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.5/dashtable/data2md/data2md.py` & `dashtable2-1.4.6/dashtable/data2md/data2md.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.5/dashtable/data2rst/cell/cell.py` & `dashtable2-1.4.6/dashtable/data2rst/cell/cell.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.5/dashtable/data2rst/cell/center_cell_text.py` & `dashtable2-1.4.6/dashtable/data2rst/cell/center_cell_text.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.5/dashtable/data2rst/cell/get_merge_direction.py` & `dashtable2-1.4.6/dashtable/data2rst/cell/get_merge_direction.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.5/dashtable/data2rst/cell/merge_cells.py` & `dashtable2-1.4.6/dashtable/data2rst/cell/merge_cells.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.5/dashtable/data2rst/cell/v_center_cell_text.py` & `dashtable2-1.4.6/dashtable/data2rst/cell/v_center_cell_text.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.5/dashtable/data2rst/data2rst.py` & `dashtable2-1.4.6/dashtable/data2rst/data2rst.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,34 @@
+
+from typing import List, Tuple, Sequence, Optional, Any
+
+import copy
+
 from .get_output_column_widths import get_output_column_widths
 from .get_output_row_heights import get_output_row_heights
 
 from ..dashutils import add_cushions
 from ..dashutils import ensure_table_strings
-from ..dashutils.check_table import check_table
-from ..dashutils.check_span import check_span
+from ..dashutils.checks import check_table, check_span
 
 from .make_cell import make_cell
 from .table_cells_2_spans import table_cells_2_spans
 from .merge_all_cells import merge_all_cells
 
 from .cell import center_cell_text
 from .cell import v_center_cell_text
 
-import copy
-
 
-def data2rst(table, spans=[[[0, 0]]], use_headers=True,
-             center_cells=False, center_headers=False):
+def data2rst(
+    table: List[List[Any]],
+    spans: Optional[Sequence[Sequence[Tuple[int, int]]]] = None,
+    use_headers: bool = True,
+    center_cells: bool = False,
+    center_headers: bool = False
+):
     """
     Convert a list of lists of str into a reStructuredText Grid Table
 
     Parameters
     ----------
     table : list of lists of str
     spans : list of lists of lists of int, optional
@@ -53,58 +60,59 @@
     ...     [ [3, 1], [4, 1] ],
     ...     [ [3, 2], [4, 2] ],
     ...     [ [2, 1], [2, 2] ],
     ... ]
     >>> table = [
     ...     ["Header 1", "Header 2", "Header 3"],
     ...     ["body row 1", "column 2", "column 3"],
-    ...     ["body row 2", "Cells may span columns", ""],
-    ...     ["body row 3", "Cells may span rows.", "- Cells\\n-contain\\n-blocks"],
+    ...     ["body row 2", "Cells may span columns.", ""],
+    ...     ["body row 3", "Cells may\\nspan rows.", "- Cells\\n- contain\\n- blocks."],
     ...     ["body row 4", "", ""],
     ... ]
-    >>> print(dashtable.data2rst(table, spans))
-    +------------+------------+-----------+
-    | Header 1   | Header 2   | Header 3  |
-    +============+============+===========+
-    | body row 1 | column 2   | column 3  |
-    +------------+------------+-----------+
-    | body row 2 | Cells may span columns.|
-    +------------+------------+-----------+
-    | body row 3 | Cells may  | - Cells   |
-    +------------+ span rows. | - contain |
-    | body row 4 |            | - blocks. |
-    +------------+------------+-----------+
+    >>> print(data2rst(table, spans))
+    +------------+-------------+-----------+
+    | Header 1   | Header 2    | Header 3  |
+    +============+=============+===========+
+    | body row 1 | column 2    | column 3  |
+    +------------+-------------+-----------+
+    | body row 2 | Cells may span columns. |
+    +------------+-------------+-----------+
+    | body row 3 | Cells may   | - Cells   |
+    +------------+ span rows.  | - contain |
+    | body row 4 |             | - blocks. |
+    +------------+-------------+-----------+
+
     """
 
     table = copy.deepcopy(table)
 
     table_ok = check_table(table)
     if not table_ok == "":
         return "ERROR: " + table_ok
 
-    if not spans == [[[0, 0]]]:
-        for span in spans:
-            span_ok = check_span(span, table)
-            if not span_ok == "":
-                return "ERROR: " + span_ok
+    spans = spans or []
+    for span in spans:
+        span_ok = check_span(span, table)
+        if not span_ok == "":
+            return "ERROR: " + span_ok
 
     table = ensure_table_strings(table)
     table = add_cushions(table)
 
     spans = table_cells_2_spans(table, spans)
 
     widths = get_output_column_widths(table, spans)
     heights = get_output_row_heights(table, spans)
 
     cells = []
     for span in spans:
         cell = make_cell(table, span, widths, heights, use_headers)
         cells.append(cell)
 
-    cells = list(sorted(cells))
+    cells = sorted(cells)
 
     if center_cells:
         for cell in cells:
             if not cell.is_header:
                 center_cell_text(cell)
                 v_center_cell_text(cell)
```

### Comparing `dashtable2-1.4.5/dashtable/data2rst/get_output_column_widths.py` & `dashtable2-1.4.6/dashtable/data2rst/get_output_column_widths.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from ..dashutils import get_span
-from ..dashutils import get_span_column_count
-from ..dashutils import get_longest_line_length
+
+from ..dashutils.spans import get_span, get_longest_line_length, get_span_column_count
+
 
 def get_output_column_widths(table, spans):
     """
     Gets the widths of the columns of the output table
 
     Parameters
     ----------
```

### Comparing `dashtable2-1.4.5/dashtable/data2rst/get_output_row_heights.py` & `dashtable2-1.4.6/dashtable/data2rst/get_output_row_heights.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from ..dashutils import get_span
-from ..dashutils import get_span_row_count
+
+from ..dashutils.spans import get_span, get_span_row_count
 
 
 def get_output_row_heights(table, spans):
     """
     Get the heights of the rows of the output table.
 
     Parameters
```

### Comparing `dashtable2-1.4.5/dashtable/data2rst/make_cell.py` & `dashtable2-1.4.6/dashtable/data2rst/make_cell.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-from ..dashutils import get_span_char_width
-from ..dashutils import get_span_char_height
-from ..dashutils import get_span_row_count
-from ..dashutils import get_span_column_count
+
+from ..dashutils.spans import get_span_char_width, get_span_char_height, get_span_column_count, get_span_row_count
 
 from .cell import Cell
 
 
-def make_cell(table, span, widths, heights, use_headers):
+def make_cell(table, span, widths, heights, use_headers) -> Cell:
     """
     Convert the contents of a span of the table to a grid table cell
 
     Parameters
     ----------
     table : list of lists of str
         The table of rows containg strings to convert to a grid table
```

### Comparing `dashtable2-1.4.5/dashtable/data2rst/merge_all_cells.py` & `dashtable2-1.4.6/dashtable/data2rst/merge_all_cells.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.5/dashtable/data2rst/table_cells_2_spans.py` & `dashtable2-1.4.6/dashtable/data2rst/table_cells_2_spans.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.5/dashtable/data2simplerst/data2simplerst.py` & `dashtable2-1.4.6/dashtable/data2simplerst/data2simplerst.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from ..dashutils import ensure_table_strings
-from ..dashutils.check_table import check_table
-from ..dashutils.check_span import check_span
+from ..dashutils.checks import check_table, check_span
 from ..dashutils.multis_2_mono import multis_2_mono
 from ..dashutils.center_line import center_line
-from ..dashutils.get_span_column_count import get_span_column_count
-from ..dashutils.get_span import get_span
+from ..dashutils.spans import get_span, get_span_column_count
 
 from .row_includes_spans import row_includes_spans
 
 import copy
 
+
 def data2simplerst(table, spans=[[[0, 0]]], use_headers=True, headers_row=0):
     """
     Convert table data to a simple rst table
 
     Parameters
     ----------
     table : list of lists of str
@@ -42,15 +41,15 @@
     ...     ["True", "False", "True"],
     ...     ["False", "True", "True"],
     ...     ["True", "True", "True"],
     ... ]
     >>> spans = [
     ...     [ [0, 0], [0, 1] ]
     ... ]
-    >>> print(data2simplerst(table, spans, headers_row=1))
+    >>> print(data2simplerst(table, spans, headers_row=1).strip())
     ======  =====  ======
        Inputs      Output
     -------------  ------
       A       B    A or B
     ======  =====  ======
     False   False  False
      True   False   True
```

### Comparing `dashtable2-1.4.5/dashtable/grid2data/grid2data.py` & `dashtable2-1.4.6/dashtable/grid2data/grid2data.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.5/dashtable/html2data/extract_spans.py` & `dashtable2-1.4.6/dashtable/html2data/extract_spans.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.5/dashtable/html2data/extract_table.py` & `dashtable2-1.4.6/dashtable/html2data/extract_table.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.5/dashtable/html2data/get_html_column_count.py` & `dashtable2-1.4.6/dashtable/html2data/get_html_column_count.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.5/dashtable/html2data/headers_present.py` & `dashtable2-1.4.6/dashtable/html2data/headers_present.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.5/dashtable/html2data/html2data.py` & `dashtable2-1.4.6/dashtable/html2data/html2data.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.5/dashtable/html2data/restructify/add_links.py` & `dashtable2-1.4.6/dashtable/html2data/restructify/add_links.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.5/dashtable/html2data/restructify/converters/__init__.py` & `dashtable2-1.4.6/dashtable/html2data/restructify/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.5/dashtable/html2data/restructify/converters/convert_li.py` & `dashtable2-1.4.6/dashtable/html2data/restructify/converters/convert_li.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.5/dashtable/html2data/restructify/process_tag.py` & `dashtable2-1.4.6/dashtable/html2data/restructify/process_tag.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.5/dashtable/html2data/restructify/restructify.py` & `dashtable2-1.4.6/dashtable/html2data/restructify/restructify.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.5/dashtable/html2md.py` & `dashtable2-1.4.6/dashtable/html2md.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.5/dashtable/html2rst.py` & `dashtable2-1.4.6/dashtable/html2rst.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,20 +60,20 @@
     ...             </ol>
     ...         </td>
     ...     </tr>
     ... </table>
     ... '''
     >>> import dashtable
     >>> print(dashtable.html2rst(html_text))
-    +---------------------+----------------+--------------+
-    | Header 1            | Header 2       | Header 3     |
-    +=====================+================+==============+
-    | This is a paragraph | -  List item 1 | #. Ordered 1 |
-    |                     | -  List item 2 | #. Ordered 2 |
-    +---------------------+----------------+--------------+
+    +---------------------+---------------+--------------+
+    | Header 1            | Header 2      | Header 3     |
+    +=====================+===============+==============+
+    | This is a paragraph | * List item 1 | 1. Ordered 1 |
+    |                     | * List item 2 | 2. Ordered 2 |
+    +---------------------+---------------+--------------+
 
     .. _BeautifulSoup: https://www.crummy.com/software/BeautifulSoup/
     """
 
     if os.path.isfile(html_string):
         file = open(html_string, 'r', encoding='utf-8')
         lines = file.readlines()
```

### Comparing `dashtable2-1.4.5/dashtable/simple2data/simple2data.py` & `dashtable2-1.4.6/dashtable/simple2data/simple2data.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     >>> from dashtable import simple2data
     >>> table, spans, use_headers, headers_row = simple2data(html_text)
     >>> from pprint import pprint
     >>> pprint(table)
     [['Inputs', 'Output', ''],
      ['A', 'B', 'A or B'],
      ['False', 'False', 'False'],
-     ['True, 'False', 'True'],
+     ['True', 'False', 'True'],
      ['False', 'True', 'True'],
      ['True', 'True', 'True']]
     >>> print(spans)
     [[[0, 0], [0, 1]]]
     >>> print(use_headers)
     True
     >>> print(headers_row)
```

### Comparing `dashtable2-1.4.5/dashtable/simple2data/truncate_empty_lines.py` & `dashtable2-1.4.6/dashtable/simple2data/truncate_empty_lines.py`

 * *Files identical despite different names*

### Comparing `dashtable2-1.4.5/dashtable2.egg-info/SOURCES.txt` & `dashtable2-1.4.6/dashtable2.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 LICENSE.txt
-README.rst
+README.md
 setup.py
 dashtable/__init__.py
 dashtable/exceptions.py
 dashtable/html2md.py
 dashtable/html2rst.py
 dashtable/dashutils/__init__.py
 dashtable/dashutils/add_cushions.py
 dashtable/dashutils/center_line.py
-dashtable/dashutils/check_span.py
-dashtable/dashutils/check_table.py
+dashtable/dashutils/checks.py
 dashtable/dashutils/ensure_table_strings.py
-dashtable/dashutils/get_longest_line_length.py
-dashtable/dashutils/get_span.py
-dashtable/dashutils/get_span_char_height.py
-dashtable/dashutils/get_span_char_width.py
-dashtable/dashutils/get_span_column_count.py
-dashtable/dashutils/get_span_row_count.py
 dashtable/dashutils/make_empty_table.py
 dashtable/dashutils/make_span.py
 dashtable/dashutils/multis_2_mono.py
+dashtable/dashutils/spans.py
 dashtable/data2md/__init__.py
 dashtable/data2md/data2md.py
 dashtable/data2md/get_column_width.py
 dashtable/data2rst/__init__.py
 dashtable/data2rst/data2rst.py
 dashtable/data2rst/get_output_column_widths.py
 dashtable/data2rst/get_output_row_heights.py
@@ -75,8 +69,9 @@
 dashtable/html2data/restructify/converters/convert_tt.py
 dashtable/simple2data/__init__.py
 dashtable/simple2data/simple2data.py
 dashtable/simple2data/truncate_empty_lines.py
 dashtable2.egg-info/PKG-INFO
 dashtable2.egg-info/SOURCES.txt
 dashtable2.egg-info/dependency_links.txt
+dashtable2.egg-info/requires.txt
 dashtable2.egg-info/top_level.txt
```

