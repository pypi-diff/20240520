# Comparing `tmp/aspose-words-cloud-24.4.0.tar.gz` & `tmp/aspose-words-cloud-24.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aspose-words-cloud-24.4.0.tar", last modified: Mon Apr 15 11:03:23 2024, max compression
+gzip compressed data, was "dist/aspose-words-cloud-24.5.0.tar", last modified: Mon May 20 06:04:38 2024, max compression
```

## Comparing `aspose-words-cloud-24.4.0.tar` & `aspose-words-cloud-24.5.0.tar`

### file list

```diff
@@ -1,699 +1,699 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 11:03:23.000000 aspose-words-cloud-24.4.0/
--rw-r--r--   0 root         (0) root         (0)     1075 2024-04-15 11:02:11.000000 aspose-words-cloud-24.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    14928 2024-04-15 11:02:11.000000 aspose-words-cloud-24.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 11:03:23.000000 aspose-words-cloud-24.4.0/test/
--rw-r--r--   0 root         (0) root         (0)     3484 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/test/base_test_context.py
--rw-r--r--   0 root         (0) root         (0)     9634 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/test/test_batch.py
--rw-r--r--   0 root         (0) root         (0)     3318 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/test/test_examples.py
--rw-r--r--   0 root         (0) root         (0)     3273 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2598 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/test/test_url_encode.py
--rw-r--r--   0 root         (0) root         (0)     2597 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/test/test_doc_with_password.py
--rw-r--r--   0 root         (0) root         (0)     4054 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/test/test_readme.py
--rw-r--r--   0 root         (0) root         (0)    16164 2024-04-15 11:03:23.000000 aspose-words-cloud-24.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2228 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 11:03:22.000000 aspose-words-cloud-24.4.0/asposewordscloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 11:03:22.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/
--rw-r--r--   0 root         (0) root         (0)    11797 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/document.py
--rw-r--r--   0 root         (0) root         (0)     5933 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/style_apply.py
--rw-r--r--   0 root         (0) root         (0)    49569 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/jpeg_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     7129 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/custom_xml_parts_response.py
--rw-r--r--   0 root         (0) root         (0)     6803 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/paragraph_insert.py
--rw-r--r--   0 root         (0) root         (0)     6666 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/list_response.py
--rw-r--r--   0 root         (0) root         (0)     9739 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/csv_data_load_options.py
--rw-r--r--   0 root         (0) root         (0)    49428 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/bmp_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)    25105 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/word_ml_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     7035 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/custom_xml_part_response.py
--rw-r--r--   0 root         (0) root         (0)     6992 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/list_levels.py
--rw-r--r--   0 root         (0) root         (0)     6803 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/bookmarks_response.py
--rw-r--r--   0 root         (0) root         (0)     7265 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/office_math_objects_response.py
--rw-r--r--   0 root         (0) root         (0)     6777 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/lists_response.py
--rw-r--r--   0 root         (0) root         (0)    16546 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/drawing_object_insert.py
--rw-r--r--   0 root         (0) root         (0)     6756 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/form_field_collection.py
--rw-r--r--   0 root         (0) root         (0)     7155 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/office_math_object_response.py
--rw-r--r--   0 root         (0) root         (0)     6775 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/fields_response.py
--rw-r--r--   0 root         (0) root         (0)     7938 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/image_entry_list.py
--rw-r--r--   0 root         (0) root         (0)    28467 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/dot_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     9313 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/document_entry.py
--rw-r--r--   0 root         (0) root         (0)    25420 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/style.py
--rw-r--r--   0 root         (0) root         (0)     7205 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/field_link.py
--rw-r--r--   0 root         (0) root         (0)    28769 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/dotx_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)    54561 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/tiff_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6675 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/save_response.py
--rw-r--r--   0 root         (0) root         (0)     6616 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/run_response.py
--rw-r--r--   0 root         (0) root         (0)     6713 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/table_cell_response.py
--rw-r--r--   0 root         (0) root         (0)    79147 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/epub_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     7056 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/paragraph_list_format_response.py
--rw-r--r--   0 root         (0) root         (0)     6947 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/xml_data_load_options.py
--rw-r--r--   0 root         (0) root         (0)     9687 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/footnote_update.py
--rw-r--r--   0 root         (0) root         (0)    28915 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/ott_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     7504 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/table_cell.py
--rw-r--r--   0 root         (0) root         (0)     6895 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/office_math_objects_collection.py
--rw-r--r--   0 root         (0) root         (0)     6868 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/hyperlinks_response.py
--rw-r--r--   0 root         (0) root         (0)     7054 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/bookmarks_outline_level_data.py
--rw-r--r--   0 root         (0) root         (0)    14588 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/drawing_object_update.py
--rw-r--r--   0 root         (0) root         (0)    40123 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/structured_document_tag_update.py
--rw-r--r--   0 root         (0) root         (0)     7502 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/paragraph.py
--rw-r--r--   0 root         (0) root         (0)     6887 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/footnotes_response.py
--rw-r--r--   0 root         (0) root         (0)     7997 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/split_document_result.py
--rw-r--r--   0 root         (0) root         (0)    22516 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/table_cell_format.py
--rw-r--r--   0 root         (0) root         (0)     7408 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/structured_document_tags_response.py
--rw-r--r--   0 root         (0) root         (0)     7157 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/paragraph_format_response.py
--rw-r--r--   0 root         (0) root         (0)     6980 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/section_page_setup_response.py
--rw-r--r--   0 root         (0) root         (0)     6787 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/hyperlink_response.py
--rw-r--r--   0 root         (0) root         (0)     8615 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/field.py
--rw-r--r--   0 root         (0) root         (0)    10083 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/header_footer.py
--rw-r--r--   0 root         (0) root         (0)     6968 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/tab_stops_response.py
--rw-r--r--   0 root         (0) root         (0)     6779 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/footnote_response.py
--rw-r--r--   0 root         (0) root         (0)     6679 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/document_response.py
--rw-r--r--   0 root         (0) root         (0)    42207 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/page_setup.py
--rw-r--r--   0 root         (0) root         (0)    28608 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/table_properties.py
--rw-r--r--   0 root         (0) root         (0)     6350 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/bookmark_data.py
--rw-r--r--   0 root         (0) root         (0)     6739 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/comment_response.py
--rw-r--r--   0 root         (0) root         (0)    31283 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/markdown_save_options_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 11:03:23.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/
--rw-r--r--   0 root         (0) root         (0)     1682 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_header_footer_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1662 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/delete_border_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1679 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_page_numbers_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1668 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_footnote_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1668 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_bookmark_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1644 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/save_as_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1674 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/compress_document_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1656 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_list_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1671 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/compare_document_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1659 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_field_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1653 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_run_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1696 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_section_page_setup_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1705 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/delete_paragraph_list_format_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1671 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/protect_document_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1659 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_table_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1659 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_style_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1696 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/delete_paragraph_tab_stop_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1724 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_or_update_paragraph_tab_stop_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1667 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_run_font_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1710 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/delete_all_paragraph_tab_stops_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1662 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_fields_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1673 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/replace_with_text_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1659 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/replace_text_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1670 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_table_row_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1671 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_watermark_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1687 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_custom_xml_part_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1682 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/reject_all_revisions_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1690 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_table_row_format_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1665 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_comment_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1711 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_structured_document_tag_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1685 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_drawing_object_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1659 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_field_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1673 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_form_field_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1691 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_paragraph_format_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1665 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/delete_borders_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1659 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/remove_range_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1668 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_bookmark_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1682 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/accept_all_revisions_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1668 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_footnote_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1687 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_custom_xml_part_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1705 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_paragraph_list_format_online_response.py
--rw-r--r--   0 root         (0) root         (0)     7285 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1665 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_comment_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1653 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_run_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1693 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_table_cell_format_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1658 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/save_as_tiff_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1656 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_list_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1659 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_style_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1677 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/unprotect_document_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1673 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_form_field_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1662 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_border_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1661 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/save_as_range_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1691 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_table_properties_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1665 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/split_document_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1671 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_paragraph_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1653 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/copy_style_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1711 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_structured_document_tag_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1673 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_list_level_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1671 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/delete_watermark_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1713 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/apply_style_to_document_element_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1673 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_table_cell_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1685 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_drawing_object_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1722 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/create_or_update_document_property_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1685 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_watermark_text_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1668 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/append_document_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1688 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_watermark_image_online_response.py
--rw-r--r--   0 root         (0) root         (0)    28769 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/docm_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)    34002 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/ps_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6907 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/comments_collection.py
--rw-r--r--   0 root         (0) root         (0)     6234 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/position_before_node.py
--rw-r--r--   0 root         (0) root         (0)    28769 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/dotm_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6736 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/bookmark_response.py
--rw-r--r--   0 root         (0) root         (0)     9637 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/tab_stop.py
--rw-r--r--   0 root         (0) root         (0)     6934 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/table_link_collection_response.py
--rw-r--r--   0 root         (0) root         (0)     6855 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/hyperlinks.py
--rw-r--r--   0 root         (0) root         (0)     6427 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/table_link.py
--rw-r--r--   0 root         (0) root         (0)     6354 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/xml_color.py
--rw-r--r--   0 root         (0) root         (0)     7442 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/custom_xml_part_update.py
--rw-r--r--   0 root         (0) root         (0)     6969 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/header_footer_response.py
--rw-r--r--   0 root         (0) root         (0)    39486 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/structured_document_tag.py
--rw-r--r--   0 root         (0) root         (0)     7986 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/protection_request_v2.py
--rw-r--r--   0 root         (0) root         (0)     6637 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/font_response.py
--rw-r--r--   0 root         (0) root         (0)     6823 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/paragraph_response.py
--rw-r--r--   0 root         (0) root         (0)     6988 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/structured_document_tag_collection.py
--rw-r--r--   0 root         (0) root         (0)     6674 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/field_response.py
--rw-r--r--   0 root         (0) root         (0)     5717 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/comment_link.py
--rw-r--r--   0 root         (0) root         (0)     9105 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/file_link.py
--rw-r--r--   0 root         (0) root         (0)     6414 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/node_link.py
--rw-r--r--   0 root         (0) root         (0)     7986 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/protection_data_response.py
--rw-r--r--   0 root         (0) root         (0)    41453 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/structured_document_tag_insert.py
--rw-r--r--   0 root         (0) root         (0)    16589 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/compare_options.py
--rw-r--r--   0 root         (0) root         (0)     7168 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/load_web_document_data.py
--rw-r--r--   0 root         (0) root         (0)     9800 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/style_update.py
--rw-r--r--   0 root         (0) root         (0)     5418 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/report_build_options.py
--rw-r--r--   0 root         (0) root         (0)     6634 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/range_text_response.py
--rw-r--r--   0 root         (0) root         (0)     7098 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/paragraph_link_collection_response.py
--rw-r--r--   0 root         (0) root         (0)    12417 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/report_engine_settings.py
--rw-r--r--   0 root         (0) root         (0)     6643 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/words_api_error_response.py
--rw-r--r--   0 root         (0) root         (0)     6734 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/footnote_collection.py
--rw-r--r--   0 root         (0) root         (0)     7438 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/style_insert.py
--rw-r--r--   0 root         (0) root         (0)     5773 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/custom_xml_part_link.py
--rw-r--r--   0 root         (0) root         (0)     8544 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/table.py
--rw-r--r--   0 root         (0) root         (0)     8266 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/table_row_insert.py
--rw-r--r--   0 root         (0) root         (0)     6974 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/modification_operation_result.py
--rw-r--r--   0 root         (0) root         (0)     7231 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/custom_xml_parts_collection.py
--rw-r--r--   0 root         (0) root         (0)    20654 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/form_field_checkbox.py
--rw-r--r--   0 root         (0) root         (0)     7016 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/section_link_collection_response.py
--rw-r--r--   0 root         (0) root         (0)     5980 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/range_document.py
--rw-r--r--   0 root         (0) root         (0)     6044 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/story_child_nodes.py
--rw-r--r--   0 root         (0) root         (0)     6837 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/drawing_object_collection.py
--rw-r--r--   0 root         (0) root         (0)     7174 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/paragraph_link.py
--rw-r--r--   0 root         (0) root         (0)     6967 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/split_document_response.py
--rw-r--r--   0 root         (0) root         (0)     6544 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/drawing_object_link.py
--rw-r--r--   0 root         (0) root         (0)     8721 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/downsample_options_data.py
--rw-r--r--   0 root         (0) root         (0)    10273 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/pdf_digital_signature_details_data.py
--rw-r--r--   0 root         (0) root         (0)     7058 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/drawing_objects_response.py
--rw-r--r--   0 root         (0) root         (0)    10255 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/table_row_format.py
--rw-r--r--   0 root         (0) root         (0)     8187 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/save_result.py
--rw-r--r--   0 root         (0) root         (0)     8736 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/tab_stop_insert.py
--rw-r--r--   0 root         (0) root         (0)    38040 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/open_xps_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6650 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/optimization_options.py
--rw-r--r--   0 root         (0) root         (0)    13045 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/office_math_object.py
--rw-r--r--   0 root         (0) root         (0)     6840 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/styles_response.py
--rw-r--r--   0 root         (0) root         (0)     6597 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/protection_data.py
--rw-r--r--   0 root         (0) root         (0)    29351 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/flat_opc_macro_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6990 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/position_inside_node.py
--rw-r--r--   0 root         (0) root         (0)     6249 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/image_entry.py
--rw-r--r--   0 root         (0) root         (0)    11982 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/comment.py
--rw-r--r--   0 root         (0) root         (0)     6684 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/compress_response.py
--rw-r--r--   0 root         (0) root         (0)    28919 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/odt_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6221 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/position_after_node.py
--rw-r--r--   0 root         (0) root         (0)     6651 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/list_update.py
--rw-r--r--   0 root         (0) root         (0)    19911 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/form_field_drop_down.py
--rw-r--r--   0 root         (0) root         (0)    17259 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/list_info.py
--rw-r--r--   0 root         (0) root         (0)     9385 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/classification_response.py
--rw-r--r--   0 root         (0) root         (0)     7070 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/table_cell_format_response.py
--rw-r--r--   0 root         (0) root         (0)    11154 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/compare_data.py
--rw-r--r--   0 root         (0) root         (0)    28756 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/rtf_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6910 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/watermark_text.py
--rw-r--r--   0 root         (0) root         (0)     8390 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/document_property.py
--rw-r--r--   0 root         (0) root         (0)     6326 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/info_additional_item.py
--rw-r--r--   0 root         (0) root         (0)     6695 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/borders_collection.py
--rw-r--r--   0 root         (0) root         (0)     6680 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/field_collection.py
--rw-r--r--   0 root         (0) root         (0)     6981 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/classification_result.py
--rw-r--r--   0 root         (0) root         (0)    77998 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/html_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)    37768 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/xaml_fixed_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     7184 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/paragraph_link_collection.py
--rw-r--r--   0 root         (0) root         (0)     6849 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/comments_response.py
--rw-r--r--   0 root         (0) root         (0)    39921 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/svg_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)    29570 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/flat_opc_template_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)    49428 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/gif_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6781 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/borders_response.py
--rw-r--r--   0 root         (0) root         (0)     7110 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/header_footers_response.py
--rw-r--r--   0 root         (0) root         (0)    49428 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/eps_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)    37639 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/xps_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)    22896 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/list_level.py
--rw-r--r--   0 root         (0) root         (0)     6686 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/run_insert.py
--rw-r--r--   0 root         (0) root         (0)    73921 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/pdf_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     5938 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/style_copy.py
--rw-r--r--   0 root         (0) root         (0)    18235 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/drawing_object.py
--rw-r--r--   0 root         (0) root         (0)     7027 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/revisions_modification_response.py
--rw-r--r--   0 root         (0) root         (0)     8299 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/info_response.py
--rw-r--r--   0 root         (0) root         (0)     7012 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/table_link_collection.py
--rw-r--r--   0 root         (0) root         (0)     6639 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/field_update.py
--rw-r--r--   0 root         (0) root         (0)     7249 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/list_insert.py
--rw-r--r--   0 root         (0) root         (0)    28983 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/flat_opc_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6715 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/style_response.py
--rw-r--r--   0 root         (0) root         (0)    49428 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/png_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     7086 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/bookmark.py
--rw-r--r--   0 root         (0) root         (0)    24177 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/form_field_text_input.py
--rw-r--r--   0 root         (0) root         (0)     6864 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/form_field_response.py
--rw-r--r--   0 root         (0) root         (0)     7147 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/user_information.py
--rw-r--r--   0 root         (0) root         (0)     7859 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/replace_text_response.py
--rw-r--r--   0 root         (0) root         (0)    10430 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/section.py
--rw-r--r--   0 root         (0) root         (0)    19089 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6695 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/runs_response.py
--rw-r--r--   0 root         (0) root         (0)     5710 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/run_update.py
--rw-r--r--   0 root         (0) root         (0)     8518 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/time_zone_info_data.py
--rw-r--r--   0 root         (0) root         (0)     7806 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/protection_request.py
--rw-r--r--   0 root         (0) root         (0)    16292 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/metafile_rendering_options_data.py
--rw-r--r--   0 root         (0) root         (0)    10866 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/replace_text_parameters.py
--rw-r--r--   0 root         (0) root         (0)     8039 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/search_response.py
--rw-r--r--   0 root         (0) root         (0)    11222 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/watermark_data_text.py
--rw-r--r--   0 root         (0) root         (0)     6989 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/search_results_collection.py
--rw-r--r--   0 root         (0) root         (0)     6865 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/drawing_object_response.py
--rw-r--r--   0 root         (0) root         (0)    19148 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/list_level_update.py
--rw-r--r--   0 root         (0) root         (0)     7090 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/document_property_response.py
--rw-r--r--   0 root         (0) root         (0)     8239 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/watermark_data_image.py
--rw-r--r--   0 root         (0) root         (0)     5515 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/file_reference.py
--rw-r--r--   0 root         (0) root         (0)     7976 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/table_insert.py
--rw-r--r--   0 root         (0) root         (0)    52315 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/html_fixed_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6977 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/replace_range.py
--rw-r--r--   0 root         (0) root         (0)     6535 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/runs.py
--rw-r--r--   0 root         (0) root         (0)     6666 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/files_upload_result.py
--rw-r--r--   0 root         (0) root         (0)    13389 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/outline_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6522 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/document_position.py
--rw-r--r--   0 root         (0) root         (0)    13119 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/border.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 11:03:22.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/
--rw-r--r--   0 root         (0) root         (0)     7446 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_paragraph_list_format_request.py
--rw-r--r--   0 root         (0) root         (0)     7338 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_page_numbers_request.py
--rw-r--r--   0 root         (0) root         (0)     7427 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/append_document_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5816 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_paragraphs_request.py
--rw-r--r--   0 root         (0) root         (0)     4865 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/copy_folder_request.py
--rw-r--r--   0 root         (0) root         (0)     7222 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_table_request.py
--rw-r--r--   0 root         (0) root         (0)     6331 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_drawing_object_by_index_request.py
--rw-r--r--   0 root         (0) root         (0)     6245 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_border_request.py
--rw-r--r--   0 root         (0) root         (0)     6553 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_office_math_objects_request.py
--rw-r--r--   0 root         (0) root         (0)     6414 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_table_row_request.py
--rw-r--r--   0 root         (0) root         (0)     5690 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/build_report_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5543 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_properties_request.py
--rw-r--r--   0 root         (0) root         (0)     5719 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_style_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7380 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_custom_xml_part_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7036 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_section_request.py
--rw-r--r--   0 root         (0) root         (0)     5239 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_comments_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6037 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_bookmark_by_name_request.py
--rw-r--r--   0 root         (0) root         (0)     6507 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_bookmarks_request.py
--rw-r--r--   0 root         (0) root         (0)     6378 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_comments_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5460 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_comments_request.py
--rw-r--r--   0 root         (0) root         (0)     7947 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_section_page_setup_request.py
--rw-r--r--   0 root         (0) root         (0)     5122 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/move_file_request.py
--rw-r--r--   0 root         (0) root         (0)     6994 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_header_footer_of_section_request.py
--rw-r--r--   0 root         (0) root         (0)     5990 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_comment_request.py
--rw-r--r--   0 root         (0) root         (0)     7149 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/build_report_request.py
--rw-r--r--   0 root         (0) root         (0)     5105 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/copy_file_request.py
--rw-r--r--   0 root         (0) root         (0)     5954 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_table_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5618 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_office_math_objects_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7230 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/split_document_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5994 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_form_field_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7432 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/save_as_range_request.py
--rw-r--r--   0 root         (0) root         (0)     7246 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_paragraph_request.py
--rw-r--r--   0 root         (0) root         (0)     5753 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_borders_request.py
--rw-r--r--   0 root         (0) root         (0)     8332 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_table_cell_format_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7164 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_custom_xml_part_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6275 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_office_math_object_request.py
--rw-r--r--   0 root         (0) root         (0)     7681 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/replace_with_text_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6350 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_statistics_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7307 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_structured_document_tag_request.py
--rw-r--r--   0 root         (0) root         (0)     6191 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_style_from_document_element_request.py
--rw-r--r--   0 root         (0) root         (0)     6483 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_table_row_format_request.py
--rw-r--r--   0 root         (0) root         (0)     6044 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/reject_all_revisions_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7597 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_table_cell_request.py
--rw-r--r--   0 root         (0) root         (0)     5679 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/execute_mail_merge_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7105 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_table_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6615 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_watermark_request.py
--rw-r--r--   0 root         (0) root         (0)     8057 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_form_field_request.py
--rw-r--r--   0 root         (0) root         (0)     6168 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_table_request.py
--rw-r--r--   0 root         (0) root         (0)     4376 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/load_web_document_request.py
--rw-r--r--   0 root         (0) root         (0)     7039 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_borders_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5511 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_hyperlinks_request.py
--rw-r--r--   0 root         (0) root         (0)     7522 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_table_request.py
--rw-r--r--   0 root         (0) root         (0)     7948 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_field_request.py
--rw-r--r--   0 root         (0) root         (0)     7986 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/create_or_update_document_property_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5784 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_tables_request.py
--rw-r--r--   0 root         (0) root         (0)     4359 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/classify_request.py
--rw-r--r--   0 root         (0) root         (0)     6049 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_paragraph_format_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5782 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_runs_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6044 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_paragraph_tab_stops_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7576 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_watermark_image_request.py
--rw-r--r--   0 root         (0) root         (0)     6714 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/protect_document_request.py
--rw-r--r--   0 root         (0) root         (0)     6414 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_custom_xml_parts_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5559 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_form_fields_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7278 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_list_request.py
--rw-r--r--   0 root         (0) root         (0)     6303 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_paragraph_list_format_request.py
--rw-r--r--   0 root         (0) root         (0)     8028 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_footnote_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7220 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/copy_style_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6089 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_paragraph_list_format_online_request.py
--rw-r--r--   0 root         (0) root         (0)     8134 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_drawing_object_request.py
--rw-r--r--   0 root         (0) root         (0)     6204 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_paragraph_request.py
--rw-r--r--   0 root         (0) root         (0)     6429 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_office_math_objects_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6665 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_all_paragraph_tab_stops_request.py
--rw-r--r--   0 root         (0) root         (0)     7030 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/render_math_object_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6980 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_document_property_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7259 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_comment_request.py
--rw-r--r--   0 root         (0) root         (0)     6855 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_all_paragraph_tab_stops_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5595 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_paragraphs_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7560 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_watermark_image_online_request.py
--rw-r--r--   0 root         (0) root         (0)     8022 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_form_field_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6348 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_with_format_request.py
--rw-r--r--   0 root         (0) root         (0)     7045 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/merge_with_next_request.py
--rw-r--r--   0 root         (0) root         (0)     6928 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/merge_with_next_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6258 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_paragraph_tab_stops_request.py
--rw-r--r--   0 root         (0) root         (0)     6037 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_custom_xml_part_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7604 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_paragraph_request.py
--rw-r--r--   0 root         (0) root         (0)     4351 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/create_document_request.py
--rw-r--r--   0 root         (0) root         (0)     5523 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_protection_request.py
--rw-r--r--   0 root         (0) root         (0)     7445 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_watermark_request.py
--rw-r--r--   0 root         (0) root         (0)     6378 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_header_footer_request.py
--rw-r--r--   0 root         (0) root         (0)     4321 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_folder_request.py
--rw-r--r--   0 root         (0) root         (0)     7522 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_or_update_paragraph_tab_stop_request.py
--rw-r--r--   0 root         (0) root         (0)     5436 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_lists_request.py
--rw-r--r--   0 root         (0) root         (0)     6984 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/render_table_online_request.py
--rw-r--r--   0 root         (0) root         (0)     8314 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_structured_document_tag_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5892 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_field_names_request.py
--rw-r--r--   0 root         (0) root         (0)     8089 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_table_properties_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7875 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_header_footer_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7340 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/replace_text_request.py
--rw-r--r--   0 root         (0) root         (0)     8224 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_paragraph_format_online_request.py
--rw-r--r--   0 root         (0) root         (0)     8295 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_table_row_format_request.py
--rw-r--r--   0 root         (0) root         (0)     5877 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/unprotect_document_request.py
--rw-r--r--   0 root         (0) root         (0)     7231 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_list_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7819 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_style_request.py
--rw-r--r--   0 root         (0) root         (0)     5215 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_lists_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6492 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_macros_request.py
--rw-r--r--   0 root         (0) root         (0)     8137 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_run_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7408 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_table_cell_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6276 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_table_row_format_online_request.py
--rw-r--r--   0 root         (0) root         (0)     1076 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/batch_request.py
--rw-r--r--   0 root         (0) root         (0)     7281 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_custom_xml_part_request.py
--rw-r--r--   0 root         (0) root         (0)     6927 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_bookmark_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7405 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_watermark_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7470 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_field_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7388 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_border_request.py
--rw-r--r--   0 root         (0) root         (0)     7252 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/render_drawing_object_request.py
--rw-r--r--   0 root         (0) root         (0)     7191 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/render_table_request.py
--rw-r--r--   0 root         (0) root         (0)     8272 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_table_row_format_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5776 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_section_online_request.py
--rw-r--r--   0 root         (0) root         (0)     8138 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_border_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5847 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_drawing_objects_request.py
--rw-r--r--   0 root         (0) root         (0)     7222 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_field_request.py
--rw-r--r--   0 root         (0) root         (0)     8176 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_border_request.py
--rw-r--r--   0 root         (0) root         (0)     6195 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_footnote_request.py
--rw-r--r--   0 root         (0) root         (0)     8272 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_list_level_request.py
--rw-r--r--   0 root         (0) root         (0)     6473 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_table_cell_request.py
--rw-r--r--   0 root         (0) root         (0)     7237 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/render_math_object_request.py
--rw-r--r--   0 root         (0) root         (0)     6168 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_field_request.py
--rw-r--r--   0 root         (0) root         (0)    11185 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/save_as_tiff_request.py
--rw-r--r--   0 root         (0) root         (0)     6899 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/optimize_document_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7352 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_table_row_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7462 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_table_row_request.py
--rw-r--r--   0 root         (0) root         (0)     3489 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_info_request.py
--rw-r--r--   0 root         (0) root         (0)     7919 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_section_page_setup_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7516 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_field_request.py
--rw-r--r--   0 root         (0) root         (0)     5322 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_properties_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7296 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_office_math_object_request.py
--rw-r--r--   0 root         (0) root         (0)     6579 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/render_page_request.py
--rw-r--r--   0 root         (0) root         (0)     6472 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/save_as_request.py
--rw-r--r--   0 root         (0) root         (0)     6649 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/compress_document_request.py
--rw-r--r--   0 root         (0) root         (0)     7219 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/render_paragraph_request.py
--rw-r--r--   0 root         (0) root         (0)     6612 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/compress_document_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6453 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_run_font_request.py
--rw-r--r--   0 root         (0) root         (0)     5979 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_fields_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6313 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_header_footers_request.py
--rw-r--r--   0 root         (0) root         (0)     4875 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/move_folder_request.py
--rw-r--r--   0 root         (0) root         (0)     5838 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_fields_request.py
--rw-r--r--   0 root         (0) root         (0)     8118 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_table_properties_request.py
--rw-r--r--   0 root         (0) root         (0)     5556 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_request.py
--rw-r--r--   0 root         (0) root         (0)     6793 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_fields_request.py
--rw-r--r--   0 root         (0) root         (0)     6538 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_custom_xml_parts_request.py
--rw-r--r--   0 root         (0) root         (0)     8059 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/apply_style_to_document_element_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5839 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_office_math_objects_request.py
--rw-r--r--   0 root         (0) root         (0)     5866 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_section_page_setup_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7038 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_comment_request.py
--rw-r--r--   0 root         (0) root         (0)     6087 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_structured_document_tag_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7729 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_list_request.py
--rw-r--r--   0 root         (0) root         (0)     4415 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/download_file_request.py
--rw-r--r--   0 root         (0) root         (0)     6372 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/render_page_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7243 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_bookmark_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7264 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_style_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7689 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_list_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7272 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/copy_style_request.py
--rw-r--r--   0 root         (0) root         (0)     5933 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_style_request.py
--rw-r--r--   0 root         (0) root         (0)     7474 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_run_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7157 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_drawing_object_online_request.py
--rw-r--r--   0 root         (0) root         (0)     8133 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_custom_xml_part_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7479 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_run_request.py
--rw-r--r--   0 root         (0) root         (0)     6266 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_table_cell_online_request.py
--rw-r--r--   0 root         (0) root         (0)     8064 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_footnote_request.py
--rw-r--r--   0 root         (0) root         (0)     5990 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_paragraph_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7844 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_bookmark_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7932 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_form_field_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6615 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/compare_document_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6121 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_hyperlink_by_index_request.py
--rw-r--r--   0 root         (0) root         (0)     7974 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_form_field_request.py
--rw-r--r--   0 root         (0) root         (0)     5954 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_field_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5860 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_structured_document_tags_request.py
--rw-r--r--   0 root         (0) root         (0)     7112 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/remove_range_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5769 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_footnotes_request.py
--rw-r--r--   0 root         (0) root         (0)     6893 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_borders_request.py
--rw-r--r--   0 root         (0) root         (0)     8227 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_paragraph_list_format_request.py
--rw-r--r--   0 root         (0) root         (0)     7280 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_headers_footers_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7465 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/append_document_request.py
--rw-r--r--   0 root         (0) root         (0)     7586 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_footnote_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6336 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_table_cell_format_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7629 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_footnote_request.py
--rw-r--r--   0 root         (0) root         (0)     5524 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_fields_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5911 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/accept_all_revisions_request.py
--rw-r--r--   0 root         (0) root         (0)     5247 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_bookmarks_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7418 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_custom_xml_part_request.py
--rw-r--r--   0 root         (0) root         (0)    34176 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6301 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_structured_document_tag_request.py
--rw-r--r--   0 root         (0) root         (0)     7286 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_bookmark_request.py
--rw-r--r--   0 root         (0) root         (0)     7123 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_footnote_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6263 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_table_properties_request.py
--rw-r--r--   0 root         (0) root         (0)     6368 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_macros_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6787 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_header_footer_of_section_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5632 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/search_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7393 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_watermark_text_request.py
--rw-r--r--   0 root         (0) root         (0)     5862 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_property_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6076 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_property_request.py
--rw-r--r--   0 root         (0) root         (0)     5468 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_bookmarks_request.py
--rw-r--r--   0 root         (0) root         (0)     7293 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/link_header_footers_to_previous_request.py
--rw-r--r--   0 root         (0) root         (0)     6209 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_run_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7780 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_style_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7282 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/replace_text_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5977 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_style_from_document_element_online_request.py
--rw-r--r--   0 root         (0) root         (0)    11138 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/save_as_tiff_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5626 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_drawing_objects_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7761 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_comment_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6080 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_section_page_setup_request.py
--rw-r--r--   0 root         (0) root         (0)     7179 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_office_math_object_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7122 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/copy_styles_from_template_request.py
--rw-r--r--   0 root         (0) root         (0)     6413 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/save_as_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7250 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_form_field_request.py
--rw-r--r--   0 root         (0) root         (0)     3422 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/reset_cache_request.py
--rw-r--r--   0 root         (0) root         (0)     6606 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_range_text_request.py
--rw-r--r--   0 root         (0) root         (0)     7907 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_header_footer_request.py
--rw-r--r--   0 root         (0) root         (0)     5776 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_comment_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7079 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_paragraph_tab_stop_request.py
--rw-r--r--   0 root         (0) root         (0)     5911 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/reject_all_revisions_request.py
--rw-r--r--   0 root         (0) root         (0)     5290 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_hyperlinks_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6921 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_section_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6967 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/remove_range_request.py
--rw-r--r--   0 root         (0) root         (0)     5639 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_structured_document_tags_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7909 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_field_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7486 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_table_row_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6251 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_custom_xml_part_request.py
--rw-r--r--   0 root         (0) root         (0)     7555 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_table_cell_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6392 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_range_text_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6117 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_drawing_object_by_index_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7038 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_section_request.py
--rw-r--r--   0 root         (0) root         (0)     5532 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_borders_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7365 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_watermark_text_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5302 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_protection_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7522 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_run_request.py
--rw-r--r--   0 root         (0) root         (0)     7990 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/create_or_update_document_property_request.py
--rw-r--r--   0 root         (0) root         (0)     8050 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/apply_style_to_document_element_request.py
--rw-r--r--   0 root         (0) root         (0)     5444 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_styles_request.py
--rw-r--r--   0 root         (0) root         (0)     7304 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_page_numbers_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5278 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_sections_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7522 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_header_footer_request.py
--rw-r--r--   0 root         (0) root         (0)     5981 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_footnote_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5823 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_bookmark_by_name_online_request.py
--rw-r--r--   0 root         (0) root         (0)     8164 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_custom_xml_part_request.py
--rw-r--r--   0 root         (0) root         (0)     8254 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_list_level_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6099 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_header_footers_online_request.py
--rw-r--r--   0 root         (0) root         (0)     4135 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/create_folder_request.py
--rw-r--r--   0 root         (0) root         (0)     8337 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_structured_document_tag_request.py
--rw-r--r--   0 root         (0) root         (0)     6073 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_drawing_object_ole_data_online_request.py
--rw-r--r--   0 root         (0) root         (0)     8567 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_drawing_object_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5846 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/search_request.py
--rw-r--r--   0 root         (0) root         (0)     8119 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_drawing_object_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7105 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_field_online_request.py
--rw-r--r--   0 root         (0) root         (0)     8354 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_table_cell_format_request.py
--rw-r--r--   0 root         (0) root         (0)     7857 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_structured_document_tag_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7798 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_comment_request.py
--rw-r--r--   0 root         (0) root         (0)     6765 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_watermark_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6571 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_statistics_request.py
--rw-r--r--   0 root         (0) root         (0)     7213 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/optimize_document_request.py
--rw-r--r--   0 root         (0) root         (0)     7274 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_drawing_object_request.py
--rw-r--r--   0 root         (0) root         (0)     6416 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_run_request.py
--rw-r--r--   0 root         (0) root         (0)     7611 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_paragraph_list_format_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5514 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_custom_xml_parts_request.py
--rw-r--r--   0 root         (0) root         (0)     7240 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_footnote_request.py
--rw-r--r--   0 root         (0) root         (0)     3823 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_available_fonts_request.py
--rw-r--r--   0 root         (0) root         (0)     7045 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/render_drawing_object_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7369 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_run_online_request.py
--rw-r--r--   0 root         (0) root         (0)      763 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/base_request_object.py
--rw-r--r--   0 root         (0) root         (0)     6031 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_border_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7133 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_form_field_online_request.py
--rw-r--r--   0 root         (0) root         (0)     4158 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_files_list_request.py
--rw-r--r--   0 root         (0) root         (0)     7190 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_structured_document_tag_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5878 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_list_request.py
--rw-r--r--   0 root         (0) root         (0)     7089 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/split_document_request.py
--rw-r--r--   0 root         (0) root         (0)     7264 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_paragraph_tab_stop_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5680 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_field_names_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7562 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_paragraph_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7880 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_bookmark_request.py
--rw-r--r--   0 root         (0) root         (0)     5982 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/classify_document_request.py
--rw-r--r--   0 root         (0) root         (0)     6049 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_table_properties_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7887 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_structured_document_tag_request.py
--rw-r--r--   0 root         (0) root         (0)     6738 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/convert_document_request.py
--rw-r--r--   0 root         (0) root         (0)     6246 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_run_font_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6655 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/compare_document_request.py
--rw-r--r--   0 root         (0) root         (0)     5907 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_hyperlink_by_index_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6543 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_table_cell_format_request.py
--rw-r--r--   0 root         (0) root         (0)     6263 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_paragraph_format_request.py
--rw-r--r--   0 root         (0) root         (0)     6921 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_comment_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7129 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_paragraph_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5223 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_styles_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5990 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_section_request.py
--rw-r--r--   0 root         (0) root         (0)     6208 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_form_field_request.py
--rw-r--r--   0 root         (0) root         (0)     8255 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_run_font_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6085 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_drawing_object_image_data_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7397 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_headers_footers_request.py
--rw-r--r--   0 root         (0) root         (0)     7310 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_style_request.py
--rw-r--r--   0 root         (0) root         (0)     8253 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_paragraph_format_request.py
--rw-r--r--   0 root         (0) root         (0)     6662 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/protect_document_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5780 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_form_fields_request.py
--rw-r--r--   0 root         (0) root         (0)     7476 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_table_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6207 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_table_row_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7518 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_table_cell_request.py
--rw-r--r--   0 root         (0) root         (0)     5665 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_list_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7044 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_bookmark_request.py
--rw-r--r--   0 root         (0) root         (0)     7757 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/execute_mail_merge_request.py
--rw-r--r--   0 root         (0) root         (0)     5745 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_fields_request.py
--rw-r--r--   0 root         (0) root         (0)     5778 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/classify_document_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5996 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_runs_request.py
--rw-r--r--   0 root         (0) root         (0)     8575 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_drawing_object_request.py
--rw-r--r--   0 root         (0) root         (0)     7540 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_border_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6502 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_comments_request.py
--rw-r--r--   0 root         (0) root         (0)     6061 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_office_math_object_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6383 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_bookmarks_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6287 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_drawing_object_ole_data_request.py
--rw-r--r--   0 root         (0) root         (0)     7387 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/save_as_range_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5293 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_custom_xml_parts_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7097 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_document_property_request.py
--rw-r--r--   0 root         (0) root         (0)     7215 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_comment_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6021 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/unprotect_document_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6299 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_drawing_object_image_data_request.py
--rw-r--r--   0 root         (0) root         (0)     7012 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/render_paragraph_online_request.py
--rw-r--r--   0 root         (0) root         (0)     8171 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_run_request.py
--rw-r--r--   0 root         (0) root         (0)     5005 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/upload_file_request.py
--rw-r--r--   0 root         (0) root         (0)     8279 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_run_font_request.py
--rw-r--r--   0 root         (0) root         (0)     8202 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_paragraph_list_format_online_request.py
--rw-r--r--   0 root         (0) root         (0)     3537 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_public_key_request.py
--rw-r--r--   0 root         (0) root         (0)     6164 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_header_footer_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6669 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_fields_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5563 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_tables_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7529 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_table_row_request.py
--rw-r--r--   0 root         (0) root         (0)     6044 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/accept_all_revisions_online_request.py
--rw-r--r--   0 root         (0) root         (0)     4347 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_file_request.py
--rw-r--r--   0 root         (0) root         (0)     5548 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_footnotes_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5499 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_sections_request.py
--rw-r--r--   0 root         (0) root         (0)     7714 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/replace_with_text_request.py
--rw-r--r--   0 root         (0) root         (0)     6919 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_section_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7534 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_or_update_paragraph_tab_stop_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7412 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_header_footer_online_request.py
--rw-r--r--   0 root         (0) root         (0)    29938 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/flat_opc_template_macro_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6771 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/document_properties.py
--rw-r--r--   0 root         (0) root         (0)     7519 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/list_format_update.py
--rw-r--r--   0 root         (0) root         (0)     5990 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/document_property_create_or_update.py
--rw-r--r--   0 root         (0) root         (0)    26592 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/xaml_flow_pack_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)    49428 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/emf_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     9800 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/shading.py
--rw-r--r--   0 root         (0) root         (0)     9200 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/words_api_link.py
--rw-r--r--   0 root         (0) root         (0)    45727 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/paragraph_format_update.py
--rw-r--r--   0 root         (0) root         (0)     7402 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/public_key_response.py
--rw-r--r--   0 root         (0) root         (0)     7897 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/error.py
--rw-r--r--   0 root         (0) root         (0)     8761 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/bookmark_insert.py
--rw-r--r--   0 root         (0) root         (0)     6904 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/field_names_response.py
--rw-r--r--   0 root         (0) root         (0)     7076 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/header_footer_link.py
--rw-r--r--   0 root         (0) root         (0)    28769 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/docx_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)    11215 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/comment_update.py
--rw-r--r--   0 root         (0) root         (0)     7752 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/stat_data_response.py
--rw-r--r--   0 root         (0) root         (0)     7060 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/run_link.py
--rw-r--r--   0 root         (0) root         (0)     6965 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/form_fields_response.py
--rw-r--r--   0 root         (0) root         (0)    46984 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/paragraph_format.py
--rw-r--r--   0 root         (0) root         (0)     6824 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/bookmarks.py
--rw-r--r--   0 root         (0) root         (0)     6699 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/lists.py
--rw-r--r--   0 root         (0) root         (0)     9502 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/list_format.py
--rw-r--r--   0 root         (0) root         (0)     7207 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/structured_document_tag_response.py
--rw-r--r--   0 root         (0) root         (0)     9687 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/footnote_insert.py
--rw-r--r--   0 root         (0) root         (0)     6659 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/table_response.py
--rw-r--r--   0 root         (0) root         (0)     6872 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/header_footer_link_collection.py
--rw-r--r--   0 root         (0) root         (0)     7351 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/custom_xml_part.py
--rw-r--r--   0 root         (0) root         (0)    36208 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/pcl_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     7627 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/field_insert.py
--rw-r--r--   0 root         (0) root         (0)     7112 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/preferred_width.py
--rw-r--r--   0 root         (0) root         (0)     6770 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/error_details.py
--rw-r--r--   0 root         (0) root         (0)    34299 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/text_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)    50578 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/font.py
--rw-r--r--   0 root         (0) root         (0)     6669 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/border_response.py
--rw-r--r--   0 root         (0) root         (0)     7198 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/document_properties_response.py
--rw-r--r--   0 root         (0) root         (0)     7215 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/table_cell_insert.py
--rw-r--r--   0 root         (0) root         (0)     7159 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/structured_document_tag_list_item.py
--rw-r--r--   0 root         (0) root         (0)     8288 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/font_info.py
--rw-r--r--   0 root         (0) root         (0)     6495 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/field_names.py
--rw-r--r--   0 root         (0) root         (0)     7098 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/section_link_collection.py
--rw-r--r--   0 root         (0) root         (0)     6458 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/footnote_link.py
--rw-r--r--   0 root         (0) root         (0)     9168 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/link.py
--rw-r--r--   0 root         (0) root         (0)     7442 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/custom_xml_part_insert.py
--rw-r--r--   0 root         (0) root         (0)     7019 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/table_row_format_response.py
--rw-r--r--   0 root         (0) root         (0)     8814 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/storage_file.py
--rw-r--r--   0 root         (0) root         (0)     7100 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/footnotes_stat_data.py
--rw-r--r--   0 root         (0) root         (0)     8522 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/table_row.py
--rw-r--r--   0 root         (0) root         (0)    20156 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/field_options.py
--rw-r--r--   0 root         (0) root         (0)    28471 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/doc_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     7234 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/hyperlink.py
--rw-r--r--   0 root         (0) root         (0)     5428 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/pdf_permissions.py
--rw-r--r--   0 root         (0) root         (0)     6673 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/table_row_response.py
--rw-r--r--   0 root         (0) root         (0)    10126 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/page_number.py
--rw-r--r--   0 root         (0) root         (0)     5859 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/files_list.py
--rw-r--r--   0 root         (0) root         (0)     6741 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/section_response.py
--rw-r--r--   0 root         (0) root         (0)     8814 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/api_error.py
--rw-r--r--   0 root         (0) root         (0)     6931 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/table_properties_response.py
--rw-r--r--   0 root         (0) root         (0)     9714 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/available_fonts_response.py
--rw-r--r--   0 root         (0) root         (0)     6862 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/search_result.py
--rw-r--r--   0 root         (0) root         (0)     9149 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/page_stat_data.py
--rw-r--r--   0 root         (0) root         (0)    26330 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/xaml_flow_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)    12132 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/json_data_load_options.py
--rw-r--r--   0 root         (0) root         (0)     6453 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/section_link.py
--rw-r--r--   0 root         (0) root         (0)     7481 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/compress_options.py
--rw-r--r--   0 root         (0) root         (0)    81316 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/mhtml_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6990 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/run.py
--rw-r--r--   0 root         (0) root         (0)     5754 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/words_response.py
--rw-r--r--   0 root         (0) root         (0)    11973 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/footnote.py
--rw-r--r--   0 root         (0) root         (0)     5728 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/link_element.py
--rw-r--r--   0 root         (0) root         (0)     8008 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/pdf_encryption_details_data.py
--rw-r--r--   0 root         (0) root         (0)    11215 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/comment_insert.py
--rw-r--r--   0 root         (0) root         (0)     6500 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/office_math_link.py
--rw-r--r--   0 root         (0) root         (0)     8634 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/document_entry_list.py
--rw-r--r--   0 root         (0) root         (0)    10474 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/models/document_stat_data.py
--rw-r--r--   0 root         (0) root         (0)    11506 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/rest.py
--rw-r--r--   0 root         (0) root         (0)    19297 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9423 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 11:03:22.000000 aspose-words-cloud-24.4.0/asposewordscloud/apis/
--rw-r--r--   0 root         (0) root         (0)  1410970 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/apis/words_api.py
--rw-r--r--   0 root         (0) root         (0)      140 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    50017 2024-04-15 11:02:12.000000 aspose-words-cloud-24.4.0/asposewordscloud/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 11:03:22.000000 aspose-words-cloud-24.4.0/aspose_words_cloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)    39677 2024-04-15 11:03:22.000000 aspose-words-cloud-24.4.0/aspose_words_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-15 11:03:21.000000 aspose-words-cloud-24.4.0/aspose_words_cloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 11:03:21.000000 aspose-words-cloud-24.4.0/aspose_words_cloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    16164 2024-04-15 11:03:21.000000 aspose-words-cloud-24.4.0/aspose_words_cloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 11:03:21.000000 aspose-words-cloud-24.4.0/aspose_words_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-15 11:03:23.000000 aspose-words-cloud-24.4.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 06:04:38.000000 aspose-words-cloud-24.5.0/
+-rw-r--r--   0 root         (0) root         (0)     1075 2024-05-20 06:03:22.000000 aspose-words-cloud-24.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    15162 2024-05-20 06:03:22.000000 aspose-words-cloud-24.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 06:04:38.000000 aspose-words-cloud-24.5.0/test/
+-rw-r--r--   0 root         (0) root         (0)     3484 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/test/base_test_context.py
+-rw-r--r--   0 root         (0) root         (0)     9634 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/test/test_batch.py
+-rw-r--r--   0 root         (0) root         (0)     3318 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/test/test_examples.py
+-rw-r--r--   0 root         (0) root         (0)     3273 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2598 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/test/test_url_encode.py
+-rw-r--r--   0 root         (0) root         (0)     2597 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/test/test_doc_with_password.py
+-rw-r--r--   0 root         (0) root         (0)     4054 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/test/test_readme.py
+-rw-r--r--   0 root         (0) root         (0)    16398 2024-05-20 06:04:38.000000 aspose-words-cloud-24.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2228 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 06:04:37.000000 aspose-words-cloud-24.5.0/asposewordscloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 06:04:37.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/
+-rw-r--r--   0 root         (0) root         (0)    11797 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/document.py
+-rw-r--r--   0 root         (0) root         (0)     5933 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/style_apply.py
+-rw-r--r--   0 root         (0) root         (0)    49569 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/jpeg_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     7129 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/custom_xml_parts_response.py
+-rw-r--r--   0 root         (0) root         (0)     6803 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/paragraph_insert.py
+-rw-r--r--   0 root         (0) root         (0)     6666 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/list_response.py
+-rw-r--r--   0 root         (0) root         (0)     9739 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/csv_data_load_options.py
+-rw-r--r--   0 root         (0) root         (0)    49428 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/bmp_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    25105 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/word_ml_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     7035 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/custom_xml_part_response.py
+-rw-r--r--   0 root         (0) root         (0)     6992 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/list_levels.py
+-rw-r--r--   0 root         (0) root         (0)     6803 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/bookmarks_response.py
+-rw-r--r--   0 root         (0) root         (0)     7265 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/office_math_objects_response.py
+-rw-r--r--   0 root         (0) root         (0)     6777 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/lists_response.py
+-rw-r--r--   0 root         (0) root         (0)    16546 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/drawing_object_insert.py
+-rw-r--r--   0 root         (0) root         (0)     6756 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/form_field_collection.py
+-rw-r--r--   0 root         (0) root         (0)     7155 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/office_math_object_response.py
+-rw-r--r--   0 root         (0) root         (0)     6775 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/fields_response.py
+-rw-r--r--   0 root         (0) root         (0)     7938 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/image_entry_list.py
+-rw-r--r--   0 root         (0) root         (0)    28467 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/dot_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     9313 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/document_entry.py
+-rw-r--r--   0 root         (0) root         (0)    25420 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/style.py
+-rw-r--r--   0 root         (0) root         (0)     7205 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/field_link.py
+-rw-r--r--   0 root         (0) root         (0)    28769 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/dotx_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    54561 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/tiff_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6675 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/save_response.py
+-rw-r--r--   0 root         (0) root         (0)     6616 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/run_response.py
+-rw-r--r--   0 root         (0) root         (0)     6713 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/table_cell_response.py
+-rw-r--r--   0 root         (0) root         (0)    79147 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/epub_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     7056 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/paragraph_list_format_response.py
+-rw-r--r--   0 root         (0) root         (0)     6947 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/xml_data_load_options.py
+-rw-r--r--   0 root         (0) root         (0)     9687 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/footnote_update.py
+-rw-r--r--   0 root         (0) root         (0)    28915 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/ott_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     7504 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/table_cell.py
+-rw-r--r--   0 root         (0) root         (0)     6895 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/office_math_objects_collection.py
+-rw-r--r--   0 root         (0) root         (0)     6868 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/hyperlinks_response.py
+-rw-r--r--   0 root         (0) root         (0)     7054 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/bookmarks_outline_level_data.py
+-rw-r--r--   0 root         (0) root         (0)    14588 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/drawing_object_update.py
+-rw-r--r--   0 root         (0) root         (0)    40123 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/structured_document_tag_update.py
+-rw-r--r--   0 root         (0) root         (0)     7502 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/paragraph.py
+-rw-r--r--   0 root         (0) root         (0)     6887 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/footnotes_response.py
+-rw-r--r--   0 root         (0) root         (0)     7997 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/split_document_result.py
+-rw-r--r--   0 root         (0) root         (0)    22516 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/table_cell_format.py
+-rw-r--r--   0 root         (0) root         (0)     7408 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/structured_document_tags_response.py
+-rw-r--r--   0 root         (0) root         (0)     7157 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/paragraph_format_response.py
+-rw-r--r--   0 root         (0) root         (0)     6980 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/section_page_setup_response.py
+-rw-r--r--   0 root         (0) root         (0)     6787 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/hyperlink_response.py
+-rw-r--r--   0 root         (0) root         (0)     8615 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/field.py
+-rw-r--r--   0 root         (0) root         (0)    10083 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/header_footer.py
+-rw-r--r--   0 root         (0) root         (0)     6968 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/tab_stops_response.py
+-rw-r--r--   0 root         (0) root         (0)     6779 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/footnote_response.py
+-rw-r--r--   0 root         (0) root         (0)     6679 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/document_response.py
+-rw-r--r--   0 root         (0) root         (0)    42207 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/page_setup.py
+-rw-r--r--   0 root         (0) root         (0)    28608 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/table_properties.py
+-rw-r--r--   0 root         (0) root         (0)     6350 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/bookmark_data.py
+-rw-r--r--   0 root         (0) root         (0)     6739 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/comment_response.py
+-rw-r--r--   0 root         (0) root         (0)    31283 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/markdown_save_options_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 06:04:38.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/
+-rw-r--r--   0 root         (0) root         (0)     1682 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_header_footer_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/delete_border_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_page_numbers_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_footnote_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_bookmark_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/save_as_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/compress_document_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1656 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_list_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1671 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/compare_document_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_field_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1653 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_run_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1696 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_section_page_setup_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1705 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/delete_paragraph_list_format_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1671 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/protect_document_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_table_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_style_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1696 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/delete_paragraph_tab_stop_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1724 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_or_update_paragraph_tab_stop_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1667 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_run_font_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/delete_all_paragraph_tab_stops_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_fields_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1673 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/replace_with_text_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/replace_text_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_table_row_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1671 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_watermark_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1687 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_custom_xml_part_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1682 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/reject_all_revisions_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1690 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_table_row_format_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1665 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_comment_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1711 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_structured_document_tag_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1685 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_drawing_object_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_field_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1673 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_form_field_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1691 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_paragraph_format_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1665 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/delete_borders_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/remove_range_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_bookmark_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1682 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/accept_all_revisions_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_footnote_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1687 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_custom_xml_part_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1705 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_paragraph_list_format_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     7285 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1665 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_comment_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1653 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_run_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1693 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_table_cell_format_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/save_as_tiff_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1656 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_list_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_style_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1677 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/unprotect_document_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1673 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_form_field_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_border_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1661 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/save_as_range_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1691 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_table_properties_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1665 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/split_document_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1671 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_paragraph_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1653 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/copy_style_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1711 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_structured_document_tag_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1673 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_list_level_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1671 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/delete_watermark_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1713 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/apply_style_to_document_element_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1673 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_table_cell_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1685 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_drawing_object_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1722 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/create_or_update_document_property_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1685 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_watermark_text_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/append_document_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1688 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_watermark_image_online_response.py
+-rw-r--r--   0 root         (0) root         (0)    28769 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/docm_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    34002 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/ps_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6907 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/comments_collection.py
+-rw-r--r--   0 root         (0) root         (0)     6234 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/position_before_node.py
+-rw-r--r--   0 root         (0) root         (0)    28769 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/dotm_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6736 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/bookmark_response.py
+-rw-r--r--   0 root         (0) root         (0)     9637 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/tab_stop.py
+-rw-r--r--   0 root         (0) root         (0)     6934 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/table_link_collection_response.py
+-rw-r--r--   0 root         (0) root         (0)     6855 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/hyperlinks.py
+-rw-r--r--   0 root         (0) root         (0)     6427 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/table_link.py
+-rw-r--r--   0 root         (0) root         (0)     6354 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/xml_color.py
+-rw-r--r--   0 root         (0) root         (0)     7442 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/custom_xml_part_update.py
+-rw-r--r--   0 root         (0) root         (0)     6969 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/header_footer_response.py
+-rw-r--r--   0 root         (0) root         (0)    39486 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/structured_document_tag.py
+-rw-r--r--   0 root         (0) root         (0)     7986 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/protection_request_v2.py
+-rw-r--r--   0 root         (0) root         (0)     6637 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/font_response.py
+-rw-r--r--   0 root         (0) root         (0)     6823 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/paragraph_response.py
+-rw-r--r--   0 root         (0) root         (0)     6988 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/structured_document_tag_collection.py
+-rw-r--r--   0 root         (0) root         (0)     6674 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/field_response.py
+-rw-r--r--   0 root         (0) root         (0)     5717 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/comment_link.py
+-rw-r--r--   0 root         (0) root         (0)     9105 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/file_link.py
+-rw-r--r--   0 root         (0) root         (0)     6414 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/node_link.py
+-rw-r--r--   0 root         (0) root         (0)     7986 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/protection_data_response.py
+-rw-r--r--   0 root         (0) root         (0)    41453 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/structured_document_tag_insert.py
+-rw-r--r--   0 root         (0) root         (0)    16589 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/compare_options.py
+-rw-r--r--   0 root         (0) root         (0)     7168 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/load_web_document_data.py
+-rw-r--r--   0 root         (0) root         (0)     9800 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/style_update.py
+-rw-r--r--   0 root         (0) root         (0)     5418 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/report_build_options.py
+-rw-r--r--   0 root         (0) root         (0)     6634 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/range_text_response.py
+-rw-r--r--   0 root         (0) root         (0)     7098 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/paragraph_link_collection_response.py
+-rw-r--r--   0 root         (0) root         (0)    12417 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/report_engine_settings.py
+-rw-r--r--   0 root         (0) root         (0)     6643 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/words_api_error_response.py
+-rw-r--r--   0 root         (0) root         (0)     6734 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/footnote_collection.py
+-rw-r--r--   0 root         (0) root         (0)     7438 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/style_insert.py
+-rw-r--r--   0 root         (0) root         (0)     5773 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/custom_xml_part_link.py
+-rw-r--r--   0 root         (0) root         (0)     8544 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/table.py
+-rw-r--r--   0 root         (0) root         (0)     8266 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/table_row_insert.py
+-rw-r--r--   0 root         (0) root         (0)     6974 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/modification_operation_result.py
+-rw-r--r--   0 root         (0) root         (0)     7231 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/custom_xml_parts_collection.py
+-rw-r--r--   0 root         (0) root         (0)    20654 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/form_field_checkbox.py
+-rw-r--r--   0 root         (0) root         (0)     7016 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/section_link_collection_response.py
+-rw-r--r--   0 root         (0) root         (0)     5980 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/range_document.py
+-rw-r--r--   0 root         (0) root         (0)     6044 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/story_child_nodes.py
+-rw-r--r--   0 root         (0) root         (0)     6837 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/drawing_object_collection.py
+-rw-r--r--   0 root         (0) root         (0)     7174 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/paragraph_link.py
+-rw-r--r--   0 root         (0) root         (0)     6967 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/split_document_response.py
+-rw-r--r--   0 root         (0) root         (0)     6544 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/drawing_object_link.py
+-rw-r--r--   0 root         (0) root         (0)     8721 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/downsample_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    10273 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/pdf_digital_signature_details_data.py
+-rw-r--r--   0 root         (0) root         (0)     7058 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/drawing_objects_response.py
+-rw-r--r--   0 root         (0) root         (0)    10255 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/table_row_format.py
+-rw-r--r--   0 root         (0) root         (0)     8187 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/save_result.py
+-rw-r--r--   0 root         (0) root         (0)     8736 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/tab_stop_insert.py
+-rw-r--r--   0 root         (0) root         (0)    38040 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/open_xps_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6650 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/optimization_options.py
+-rw-r--r--   0 root         (0) root         (0)    13045 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/office_math_object.py
+-rw-r--r--   0 root         (0) root         (0)     6840 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/styles_response.py
+-rw-r--r--   0 root         (0) root         (0)     6597 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/protection_data.py
+-rw-r--r--   0 root         (0) root         (0)    29351 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/flat_opc_macro_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6990 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/position_inside_node.py
+-rw-r--r--   0 root         (0) root         (0)     6249 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/image_entry.py
+-rw-r--r--   0 root         (0) root         (0)    11982 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/comment.py
+-rw-r--r--   0 root         (0) root         (0)     6684 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/compress_response.py
+-rw-r--r--   0 root         (0) root         (0)    28919 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/odt_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6221 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/position_after_node.py
+-rw-r--r--   0 root         (0) root         (0)     6651 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/list_update.py
+-rw-r--r--   0 root         (0) root         (0)    19911 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/form_field_drop_down.py
+-rw-r--r--   0 root         (0) root         (0)    17259 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/list_info.py
+-rw-r--r--   0 root         (0) root         (0)     9385 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/classification_response.py
+-rw-r--r--   0 root         (0) root         (0)     7070 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/table_cell_format_response.py
+-rw-r--r--   0 root         (0) root         (0)    11154 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/compare_data.py
+-rw-r--r--   0 root         (0) root         (0)    28756 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/rtf_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6910 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/watermark_text.py
+-rw-r--r--   0 root         (0) root         (0)     8390 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/document_property.py
+-rw-r--r--   0 root         (0) root         (0)     6326 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/info_additional_item.py
+-rw-r--r--   0 root         (0) root         (0)     6695 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/borders_collection.py
+-rw-r--r--   0 root         (0) root         (0)     6680 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/field_collection.py
+-rw-r--r--   0 root         (0) root         (0)     6981 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/classification_result.py
+-rw-r--r--   0 root         (0) root         (0)    77998 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/html_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    37768 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/xaml_fixed_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     7184 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/paragraph_link_collection.py
+-rw-r--r--   0 root         (0) root         (0)     6849 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/comments_response.py
+-rw-r--r--   0 root         (0) root         (0)    39921 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/svg_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    29570 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/flat_opc_template_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    49428 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/gif_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6781 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/borders_response.py
+-rw-r--r--   0 root         (0) root         (0)     7110 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/header_footers_response.py
+-rw-r--r--   0 root         (0) root         (0)    49428 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/eps_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    37639 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/xps_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    22896 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/list_level.py
+-rw-r--r--   0 root         (0) root         (0)     6686 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/run_insert.py
+-rw-r--r--   0 root         (0) root         (0)    73921 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/pdf_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     5938 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/style_copy.py
+-rw-r--r--   0 root         (0) root         (0)    18235 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/drawing_object.py
+-rw-r--r--   0 root         (0) root         (0)     7027 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/revisions_modification_response.py
+-rw-r--r--   0 root         (0) root         (0)     8299 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/info_response.py
+-rw-r--r--   0 root         (0) root         (0)     7012 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/table_link_collection.py
+-rw-r--r--   0 root         (0) root         (0)     6639 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/field_update.py
+-rw-r--r--   0 root         (0) root         (0)     7249 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/list_insert.py
+-rw-r--r--   0 root         (0) root         (0)    28983 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/flat_opc_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6715 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/style_response.py
+-rw-r--r--   0 root         (0) root         (0)    49428 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/png_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     7086 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/bookmark.py
+-rw-r--r--   0 root         (0) root         (0)    24177 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/form_field_text_input.py
+-rw-r--r--   0 root         (0) root         (0)     6864 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/form_field_response.py
+-rw-r--r--   0 root         (0) root         (0)     7147 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/user_information.py
+-rw-r--r--   0 root         (0) root         (0)     7859 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/replace_text_response.py
+-rw-r--r--   0 root         (0) root         (0)    10430 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/section.py
+-rw-r--r--   0 root         (0) root         (0)    19089 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6695 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/runs_response.py
+-rw-r--r--   0 root         (0) root         (0)     5710 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/run_update.py
+-rw-r--r--   0 root         (0) root         (0)     8518 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/time_zone_info_data.py
+-rw-r--r--   0 root         (0) root         (0)     7806 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/protection_request.py
+-rw-r--r--   0 root         (0) root         (0)    16292 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/metafile_rendering_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    10866 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/replace_text_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     8039 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/search_response.py
+-rw-r--r--   0 root         (0) root         (0)    11222 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/watermark_data_text.py
+-rw-r--r--   0 root         (0) root         (0)     6989 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/search_results_collection.py
+-rw-r--r--   0 root         (0) root         (0)     6865 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/drawing_object_response.py
+-rw-r--r--   0 root         (0) root         (0)    19148 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/list_level_update.py
+-rw-r--r--   0 root         (0) root         (0)     7090 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/document_property_response.py
+-rw-r--r--   0 root         (0) root         (0)     8239 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/watermark_data_image.py
+-rw-r--r--   0 root         (0) root         (0)     5515 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/file_reference.py
+-rw-r--r--   0 root         (0) root         (0)     7976 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/table_insert.py
+-rw-r--r--   0 root         (0) root         (0)    52315 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/html_fixed_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6977 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/replace_range.py
+-rw-r--r--   0 root         (0) root         (0)     6535 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/runs.py
+-rw-r--r--   0 root         (0) root         (0)     6666 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/files_upload_result.py
+-rw-r--r--   0 root         (0) root         (0)    13389 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/outline_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6522 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/document_position.py
+-rw-r--r--   0 root         (0) root         (0)    13119 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/border.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 06:04:38.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/
+-rw-r--r--   0 root         (0) root         (0)     7446 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_paragraph_list_format_request.py
+-rw-r--r--   0 root         (0) root         (0)     7338 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_page_numbers_request.py
+-rw-r--r--   0 root         (0) root         (0)     7427 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/append_document_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5816 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_paragraphs_request.py
+-rw-r--r--   0 root         (0) root         (0)     4865 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/copy_folder_request.py
+-rw-r--r--   0 root         (0) root         (0)     7222 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_table_request.py
+-rw-r--r--   0 root         (0) root         (0)     6331 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_drawing_object_by_index_request.py
+-rw-r--r--   0 root         (0) root         (0)     6245 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_border_request.py
+-rw-r--r--   0 root         (0) root         (0)     6553 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_office_math_objects_request.py
+-rw-r--r--   0 root         (0) root         (0)     6414 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_table_row_request.py
+-rw-r--r--   0 root         (0) root         (0)     5690 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/build_report_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5543 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_properties_request.py
+-rw-r--r--   0 root         (0) root         (0)     5719 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_style_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7380 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_custom_xml_part_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7036 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_section_request.py
+-rw-r--r--   0 root         (0) root         (0)     5239 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_comments_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6037 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_bookmark_by_name_request.py
+-rw-r--r--   0 root         (0) root         (0)     6507 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_bookmarks_request.py
+-rw-r--r--   0 root         (0) root         (0)     6378 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_comments_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5460 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_comments_request.py
+-rw-r--r--   0 root         (0) root         (0)     7947 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_section_page_setup_request.py
+-rw-r--r--   0 root         (0) root         (0)     5122 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/move_file_request.py
+-rw-r--r--   0 root         (0) root         (0)     6994 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_header_footer_of_section_request.py
+-rw-r--r--   0 root         (0) root         (0)     5990 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_comment_request.py
+-rw-r--r--   0 root         (0) root         (0)     7149 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/build_report_request.py
+-rw-r--r--   0 root         (0) root         (0)     5105 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/copy_file_request.py
+-rw-r--r--   0 root         (0) root         (0)     5954 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_table_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5618 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_office_math_objects_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7230 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/split_document_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5994 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_form_field_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7432 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/save_as_range_request.py
+-rw-r--r--   0 root         (0) root         (0)     7246 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_paragraph_request.py
+-rw-r--r--   0 root         (0) root         (0)     5753 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_borders_request.py
+-rw-r--r--   0 root         (0) root         (0)     8332 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_table_cell_format_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7164 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_custom_xml_part_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6275 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_office_math_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     7681 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/replace_with_text_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6350 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_statistics_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7307 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_structured_document_tag_request.py
+-rw-r--r--   0 root         (0) root         (0)     6191 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_style_from_document_element_request.py
+-rw-r--r--   0 root         (0) root         (0)     6483 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_table_row_format_request.py
+-rw-r--r--   0 root         (0) root         (0)     6044 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/reject_all_revisions_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7597 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_table_cell_request.py
+-rw-r--r--   0 root         (0) root         (0)     5679 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/execute_mail_merge_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7105 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_table_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6615 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_watermark_request.py
+-rw-r--r--   0 root         (0) root         (0)     8057 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_form_field_request.py
+-rw-r--r--   0 root         (0) root         (0)     6168 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_table_request.py
+-rw-r--r--   0 root         (0) root         (0)     4376 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/load_web_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     7039 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_borders_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5511 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_hyperlinks_request.py
+-rw-r--r--   0 root         (0) root         (0)     7522 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_table_request.py
+-rw-r--r--   0 root         (0) root         (0)     7948 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_field_request.py
+-rw-r--r--   0 root         (0) root         (0)     7986 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/create_or_update_document_property_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5784 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_tables_request.py
+-rw-r--r--   0 root         (0) root         (0)     4359 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/classify_request.py
+-rw-r--r--   0 root         (0) root         (0)     6049 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_paragraph_format_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5782 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_runs_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6044 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_paragraph_tab_stops_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7576 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_watermark_image_request.py
+-rw-r--r--   0 root         (0) root         (0)     6714 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/protect_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     6414 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_custom_xml_parts_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5559 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_form_fields_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7278 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_list_request.py
+-rw-r--r--   0 root         (0) root         (0)     6303 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_paragraph_list_format_request.py
+-rw-r--r--   0 root         (0) root         (0)     8028 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_footnote_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7220 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/copy_style_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6089 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_paragraph_list_format_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     8134 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_drawing_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     6204 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_paragraph_request.py
+-rw-r--r--   0 root         (0) root         (0)     6429 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_office_math_objects_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6665 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_all_paragraph_tab_stops_request.py
+-rw-r--r--   0 root         (0) root         (0)     7030 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/render_math_object_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6980 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_document_property_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7259 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_comment_request.py
+-rw-r--r--   0 root         (0) root         (0)     6855 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_all_paragraph_tab_stops_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5595 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_paragraphs_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7560 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_watermark_image_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     8022 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_form_field_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6348 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_with_format_request.py
+-rw-r--r--   0 root         (0) root         (0)     7045 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/merge_with_next_request.py
+-rw-r--r--   0 root         (0) root         (0)     6928 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/merge_with_next_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6258 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_paragraph_tab_stops_request.py
+-rw-r--r--   0 root         (0) root         (0)     6037 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_custom_xml_part_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7604 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_paragraph_request.py
+-rw-r--r--   0 root         (0) root         (0)     4351 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/create_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     5523 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_protection_request.py
+-rw-r--r--   0 root         (0) root         (0)     7445 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_watermark_request.py
+-rw-r--r--   0 root         (0) root         (0)     6378 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_header_footer_request.py
+-rw-r--r--   0 root         (0) root         (0)     4321 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_folder_request.py
+-rw-r--r--   0 root         (0) root         (0)     7522 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_or_update_paragraph_tab_stop_request.py
+-rw-r--r--   0 root         (0) root         (0)     5436 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_lists_request.py
+-rw-r--r--   0 root         (0) root         (0)     6984 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/render_table_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     8314 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_structured_document_tag_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5892 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_field_names_request.py
+-rw-r--r--   0 root         (0) root         (0)     8089 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_table_properties_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7875 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_header_footer_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7340 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/replace_text_request.py
+-rw-r--r--   0 root         (0) root         (0)     8224 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_paragraph_format_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     8295 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_table_row_format_request.py
+-rw-r--r--   0 root         (0) root         (0)     5877 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/unprotect_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     7231 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_list_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7819 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_style_request.py
+-rw-r--r--   0 root         (0) root         (0)     5215 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_lists_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6492 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_macros_request.py
+-rw-r--r--   0 root         (0) root         (0)     8137 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_run_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7408 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_table_cell_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6276 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_table_row_format_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     1076 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/batch_request.py
+-rw-r--r--   0 root         (0) root         (0)     7281 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_custom_xml_part_request.py
+-rw-r--r--   0 root         (0) root         (0)     6927 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_bookmark_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7405 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_watermark_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7470 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_field_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7388 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_border_request.py
+-rw-r--r--   0 root         (0) root         (0)     7252 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/render_drawing_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     7191 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/render_table_request.py
+-rw-r--r--   0 root         (0) root         (0)     8272 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_table_row_format_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5776 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_section_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     8138 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_border_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5847 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_drawing_objects_request.py
+-rw-r--r--   0 root         (0) root         (0)     7222 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_field_request.py
+-rw-r--r--   0 root         (0) root         (0)     8176 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_border_request.py
+-rw-r--r--   0 root         (0) root         (0)     6195 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_footnote_request.py
+-rw-r--r--   0 root         (0) root         (0)     8272 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_list_level_request.py
+-rw-r--r--   0 root         (0) root         (0)     6473 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_table_cell_request.py
+-rw-r--r--   0 root         (0) root         (0)     7237 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/render_math_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     6168 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_field_request.py
+-rw-r--r--   0 root         (0) root         (0)    11185 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/save_as_tiff_request.py
+-rw-r--r--   0 root         (0) root         (0)     6899 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/optimize_document_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7352 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_table_row_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7462 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_table_row_request.py
+-rw-r--r--   0 root         (0) root         (0)     3489 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_info_request.py
+-rw-r--r--   0 root         (0) root         (0)     7919 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_section_page_setup_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7516 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_field_request.py
+-rw-r--r--   0 root         (0) root         (0)     5322 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_properties_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7296 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_office_math_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     6579 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/render_page_request.py
+-rw-r--r--   0 root         (0) root         (0)     6472 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/save_as_request.py
+-rw-r--r--   0 root         (0) root         (0)     6649 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/compress_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     7219 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/render_paragraph_request.py
+-rw-r--r--   0 root         (0) root         (0)     6612 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/compress_document_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6453 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_run_font_request.py
+-rw-r--r--   0 root         (0) root         (0)     5979 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_fields_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6313 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_header_footers_request.py
+-rw-r--r--   0 root         (0) root         (0)     4875 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/move_folder_request.py
+-rw-r--r--   0 root         (0) root         (0)     5838 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_fields_request.py
+-rw-r--r--   0 root         (0) root         (0)     8118 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_table_properties_request.py
+-rw-r--r--   0 root         (0) root         (0)     5556 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     6793 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_fields_request.py
+-rw-r--r--   0 root         (0) root         (0)     6538 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_custom_xml_parts_request.py
+-rw-r--r--   0 root         (0) root         (0)     8059 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/apply_style_to_document_element_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5839 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_office_math_objects_request.py
+-rw-r--r--   0 root         (0) root         (0)     5866 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_section_page_setup_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7038 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_comment_request.py
+-rw-r--r--   0 root         (0) root         (0)     6087 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_structured_document_tag_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7729 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_list_request.py
+-rw-r--r--   0 root         (0) root         (0)     4415 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/download_file_request.py
+-rw-r--r--   0 root         (0) root         (0)     6372 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/render_page_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7243 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_bookmark_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7264 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_style_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7689 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_list_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7272 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/copy_style_request.py
+-rw-r--r--   0 root         (0) root         (0)     5933 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_style_request.py
+-rw-r--r--   0 root         (0) root         (0)     7474 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_run_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7157 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_drawing_object_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     8133 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_custom_xml_part_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7479 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_run_request.py
+-rw-r--r--   0 root         (0) root         (0)     6266 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_table_cell_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     8064 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_footnote_request.py
+-rw-r--r--   0 root         (0) root         (0)     5990 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_paragraph_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7844 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_bookmark_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7932 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_form_field_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6615 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/compare_document_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6121 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_hyperlink_by_index_request.py
+-rw-r--r--   0 root         (0) root         (0)     7974 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_form_field_request.py
+-rw-r--r--   0 root         (0) root         (0)     5954 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_field_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5860 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_structured_document_tags_request.py
+-rw-r--r--   0 root         (0) root         (0)     7112 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/remove_range_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5769 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_footnotes_request.py
+-rw-r--r--   0 root         (0) root         (0)     6893 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_borders_request.py
+-rw-r--r--   0 root         (0) root         (0)     8227 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_paragraph_list_format_request.py
+-rw-r--r--   0 root         (0) root         (0)     7280 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_headers_footers_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7465 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/append_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     7586 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_footnote_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6336 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_table_cell_format_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7629 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_footnote_request.py
+-rw-r--r--   0 root         (0) root         (0)     5524 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_fields_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5911 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/accept_all_revisions_request.py
+-rw-r--r--   0 root         (0) root         (0)     5247 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_bookmarks_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7418 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_custom_xml_part_request.py
+-rw-r--r--   0 root         (0) root         (0)    34176 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6301 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_structured_document_tag_request.py
+-rw-r--r--   0 root         (0) root         (0)     7286 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_bookmark_request.py
+-rw-r--r--   0 root         (0) root         (0)     7123 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_footnote_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6263 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_table_properties_request.py
+-rw-r--r--   0 root         (0) root         (0)     6368 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_macros_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6787 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_header_footer_of_section_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5632 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/search_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7393 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_watermark_text_request.py
+-rw-r--r--   0 root         (0) root         (0)     5862 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_property_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6076 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_property_request.py
+-rw-r--r--   0 root         (0) root         (0)     5468 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_bookmarks_request.py
+-rw-r--r--   0 root         (0) root         (0)     7293 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/link_header_footers_to_previous_request.py
+-rw-r--r--   0 root         (0) root         (0)     6209 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_run_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7780 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_style_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7282 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/replace_text_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5977 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_style_from_document_element_online_request.py
+-rw-r--r--   0 root         (0) root         (0)    11138 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/save_as_tiff_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5626 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_drawing_objects_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7761 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_comment_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6080 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_section_page_setup_request.py
+-rw-r--r--   0 root         (0) root         (0)     7179 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_office_math_object_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7122 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/copy_styles_from_template_request.py
+-rw-r--r--   0 root         (0) root         (0)     6413 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/save_as_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7250 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_form_field_request.py
+-rw-r--r--   0 root         (0) root         (0)     3422 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/reset_cache_request.py
+-rw-r--r--   0 root         (0) root         (0)     6606 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_range_text_request.py
+-rw-r--r--   0 root         (0) root         (0)     7907 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_header_footer_request.py
+-rw-r--r--   0 root         (0) root         (0)     5776 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_comment_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7079 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_paragraph_tab_stop_request.py
+-rw-r--r--   0 root         (0) root         (0)     5911 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/reject_all_revisions_request.py
+-rw-r--r--   0 root         (0) root         (0)     5290 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_hyperlinks_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6921 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_section_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6967 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/remove_range_request.py
+-rw-r--r--   0 root         (0) root         (0)     5639 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_structured_document_tags_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7909 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_field_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7486 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_table_row_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6251 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_custom_xml_part_request.py
+-rw-r--r--   0 root         (0) root         (0)     7555 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_table_cell_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6392 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_range_text_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6117 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_drawing_object_by_index_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7038 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_section_request.py
+-rw-r--r--   0 root         (0) root         (0)     5532 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_borders_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7365 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_watermark_text_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5302 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_protection_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7522 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_run_request.py
+-rw-r--r--   0 root         (0) root         (0)     7990 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/create_or_update_document_property_request.py
+-rw-r--r--   0 root         (0) root         (0)     8050 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/apply_style_to_document_element_request.py
+-rw-r--r--   0 root         (0) root         (0)     5444 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_styles_request.py
+-rw-r--r--   0 root         (0) root         (0)     7304 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_page_numbers_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5278 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_sections_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7522 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_header_footer_request.py
+-rw-r--r--   0 root         (0) root         (0)     5981 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_footnote_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5823 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_bookmark_by_name_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     8164 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_custom_xml_part_request.py
+-rw-r--r--   0 root         (0) root         (0)     8254 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_list_level_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6099 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_header_footers_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     4135 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/create_folder_request.py
+-rw-r--r--   0 root         (0) root         (0)     8337 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_structured_document_tag_request.py
+-rw-r--r--   0 root         (0) root         (0)     6073 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_drawing_object_ole_data_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     8567 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_drawing_object_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5846 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/search_request.py
+-rw-r--r--   0 root         (0) root         (0)     8119 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_drawing_object_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7105 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_field_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     8354 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_table_cell_format_request.py
+-rw-r--r--   0 root         (0) root         (0)     7857 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_structured_document_tag_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7798 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_comment_request.py
+-rw-r--r--   0 root         (0) root         (0)     6765 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_watermark_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6571 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_statistics_request.py
+-rw-r--r--   0 root         (0) root         (0)     7213 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/optimize_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     7274 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_drawing_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     6416 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_run_request.py
+-rw-r--r--   0 root         (0) root         (0)     7611 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_paragraph_list_format_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5514 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_custom_xml_parts_request.py
+-rw-r--r--   0 root         (0) root         (0)     7240 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_footnote_request.py
+-rw-r--r--   0 root         (0) root         (0)     3823 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_available_fonts_request.py
+-rw-r--r--   0 root         (0) root         (0)     7045 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/render_drawing_object_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7369 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_run_online_request.py
+-rw-r--r--   0 root         (0) root         (0)      763 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/base_request_object.py
+-rw-r--r--   0 root         (0) root         (0)     6031 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_border_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7133 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_form_field_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     4158 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_files_list_request.py
+-rw-r--r--   0 root         (0) root         (0)     7190 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_structured_document_tag_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5878 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_list_request.py
+-rw-r--r--   0 root         (0) root         (0)     7089 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/split_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     7264 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_paragraph_tab_stop_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5680 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_field_names_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7562 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_paragraph_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7880 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_bookmark_request.py
+-rw-r--r--   0 root         (0) root         (0)     5982 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/classify_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     6049 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_table_properties_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7887 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_structured_document_tag_request.py
+-rw-r--r--   0 root         (0) root         (0)     6738 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/convert_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     6246 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_run_font_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6655 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/compare_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     5907 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_hyperlink_by_index_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6543 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_table_cell_format_request.py
+-rw-r--r--   0 root         (0) root         (0)     6263 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_paragraph_format_request.py
+-rw-r--r--   0 root         (0) root         (0)     6921 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_comment_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7129 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_paragraph_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5223 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_styles_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5990 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_section_request.py
+-rw-r--r--   0 root         (0) root         (0)     6208 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_form_field_request.py
+-rw-r--r--   0 root         (0) root         (0)     8255 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_run_font_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6085 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_drawing_object_image_data_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7397 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_headers_footers_request.py
+-rw-r--r--   0 root         (0) root         (0)     7310 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_style_request.py
+-rw-r--r--   0 root         (0) root         (0)     8253 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_paragraph_format_request.py
+-rw-r--r--   0 root         (0) root         (0)     6662 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/protect_document_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5780 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_form_fields_request.py
+-rw-r--r--   0 root         (0) root         (0)     7476 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_table_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6207 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_table_row_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7518 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_table_cell_request.py
+-rw-r--r--   0 root         (0) root         (0)     5665 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_list_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7044 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_bookmark_request.py
+-rw-r--r--   0 root         (0) root         (0)     7757 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/execute_mail_merge_request.py
+-rw-r--r--   0 root         (0) root         (0)     5745 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_fields_request.py
+-rw-r--r--   0 root         (0) root         (0)     5778 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/classify_document_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5996 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_runs_request.py
+-rw-r--r--   0 root         (0) root         (0)     8575 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_drawing_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     7540 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_border_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6502 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_comments_request.py
+-rw-r--r--   0 root         (0) root         (0)     6061 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_office_math_object_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6383 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_bookmarks_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6287 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_drawing_object_ole_data_request.py
+-rw-r--r--   0 root         (0) root         (0)     7387 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/save_as_range_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5293 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_custom_xml_parts_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7097 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_document_property_request.py
+-rw-r--r--   0 root         (0) root         (0)     7215 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_comment_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6021 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/unprotect_document_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6299 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_drawing_object_image_data_request.py
+-rw-r--r--   0 root         (0) root         (0)     7012 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/render_paragraph_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     8171 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_run_request.py
+-rw-r--r--   0 root         (0) root         (0)     5005 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/upload_file_request.py
+-rw-r--r--   0 root         (0) root         (0)     8279 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_run_font_request.py
+-rw-r--r--   0 root         (0) root         (0)     8202 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_paragraph_list_format_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     3537 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_public_key_request.py
+-rw-r--r--   0 root         (0) root         (0)     6164 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_header_footer_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6669 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_fields_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5563 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_tables_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7529 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_table_row_request.py
+-rw-r--r--   0 root         (0) root         (0)     6044 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/accept_all_revisions_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     4347 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_file_request.py
+-rw-r--r--   0 root         (0) root         (0)     5548 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_footnotes_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5499 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_sections_request.py
+-rw-r--r--   0 root         (0) root         (0)     7714 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/replace_with_text_request.py
+-rw-r--r--   0 root         (0) root         (0)     6919 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_section_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7534 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_or_update_paragraph_tab_stop_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7412 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_header_footer_online_request.py
+-rw-r--r--   0 root         (0) root         (0)    29938 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/flat_opc_template_macro_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6771 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/document_properties.py
+-rw-r--r--   0 root         (0) root         (0)     7519 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/list_format_update.py
+-rw-r--r--   0 root         (0) root         (0)     5990 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/document_property_create_or_update.py
+-rw-r--r--   0 root         (0) root         (0)    26592 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/xaml_flow_pack_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    49428 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/emf_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     9800 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/shading.py
+-rw-r--r--   0 root         (0) root         (0)     9200 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/words_api_link.py
+-rw-r--r--   0 root         (0) root         (0)    45727 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/paragraph_format_update.py
+-rw-r--r--   0 root         (0) root         (0)     7402 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/public_key_response.py
+-rw-r--r--   0 root         (0) root         (0)     7897 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/error.py
+-rw-r--r--   0 root         (0) root         (0)     8761 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/bookmark_insert.py
+-rw-r--r--   0 root         (0) root         (0)     6904 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/field_names_response.py
+-rw-r--r--   0 root         (0) root         (0)     7076 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/header_footer_link.py
+-rw-r--r--   0 root         (0) root         (0)    28769 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/docx_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    11215 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/comment_update.py
+-rw-r--r--   0 root         (0) root         (0)     7752 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/stat_data_response.py
+-rw-r--r--   0 root         (0) root         (0)     7060 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/run_link.py
+-rw-r--r--   0 root         (0) root         (0)     6965 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/form_fields_response.py
+-rw-r--r--   0 root         (0) root         (0)    46984 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/paragraph_format.py
+-rw-r--r--   0 root         (0) root         (0)     6824 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/bookmarks.py
+-rw-r--r--   0 root         (0) root         (0)     6699 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/lists.py
+-rw-r--r--   0 root         (0) root         (0)     9502 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/list_format.py
+-rw-r--r--   0 root         (0) root         (0)     7207 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/structured_document_tag_response.py
+-rw-r--r--   0 root         (0) root         (0)     9687 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/footnote_insert.py
+-rw-r--r--   0 root         (0) root         (0)     6659 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/table_response.py
+-rw-r--r--   0 root         (0) root         (0)     6872 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/header_footer_link_collection.py
+-rw-r--r--   0 root         (0) root         (0)     7351 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/custom_xml_part.py
+-rw-r--r--   0 root         (0) root         (0)    36208 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/pcl_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     7627 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/field_insert.py
+-rw-r--r--   0 root         (0) root         (0)     7112 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/preferred_width.py
+-rw-r--r--   0 root         (0) root         (0)     6770 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/error_details.py
+-rw-r--r--   0 root         (0) root         (0)    34299 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/text_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    50578 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/font.py
+-rw-r--r--   0 root         (0) root         (0)     6669 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/border_response.py
+-rw-r--r--   0 root         (0) root         (0)     7198 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/document_properties_response.py
+-rw-r--r--   0 root         (0) root         (0)     7215 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/table_cell_insert.py
+-rw-r--r--   0 root         (0) root         (0)     7159 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/structured_document_tag_list_item.py
+-rw-r--r--   0 root         (0) root         (0)     8288 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/font_info.py
+-rw-r--r--   0 root         (0) root         (0)     6495 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/field_names.py
+-rw-r--r--   0 root         (0) root         (0)     7098 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/section_link_collection.py
+-rw-r--r--   0 root         (0) root         (0)     6458 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/footnote_link.py
+-rw-r--r--   0 root         (0) root         (0)     9168 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     7442 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/custom_xml_part_insert.py
+-rw-r--r--   0 root         (0) root         (0)     7019 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/table_row_format_response.py
+-rw-r--r--   0 root         (0) root         (0)     8814 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/storage_file.py
+-rw-r--r--   0 root         (0) root         (0)     7100 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/footnotes_stat_data.py
+-rw-r--r--   0 root         (0) root         (0)     8522 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/table_row.py
+-rw-r--r--   0 root         (0) root         (0)    20156 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/field_options.py
+-rw-r--r--   0 root         (0) root         (0)    28471 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/doc_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     7234 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/hyperlink.py
+-rw-r--r--   0 root         (0) root         (0)     5428 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/pdf_permissions.py
+-rw-r--r--   0 root         (0) root         (0)     6673 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/table_row_response.py
+-rw-r--r--   0 root         (0) root         (0)    10126 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/page_number.py
+-rw-r--r--   0 root         (0) root         (0)     5859 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/files_list.py
+-rw-r--r--   0 root         (0) root         (0)     6741 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/section_response.py
+-rw-r--r--   0 root         (0) root         (0)     8814 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/api_error.py
+-rw-r--r--   0 root         (0) root         (0)     6931 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/table_properties_response.py
+-rw-r--r--   0 root         (0) root         (0)     9714 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/available_fonts_response.py
+-rw-r--r--   0 root         (0) root         (0)     6862 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/search_result.py
+-rw-r--r--   0 root         (0) root         (0)     9149 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/page_stat_data.py
+-rw-r--r--   0 root         (0) root         (0)    26330 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/xaml_flow_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    12132 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/json_data_load_options.py
+-rw-r--r--   0 root         (0) root         (0)     6453 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/section_link.py
+-rw-r--r--   0 root         (0) root         (0)     7481 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/compress_options.py
+-rw-r--r--   0 root         (0) root         (0)    81316 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/mhtml_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6990 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/run.py
+-rw-r--r--   0 root         (0) root         (0)     5754 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/words_response.py
+-rw-r--r--   0 root         (0) root         (0)    11973 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/footnote.py
+-rw-r--r--   0 root         (0) root         (0)     5728 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/link_element.py
+-rw-r--r--   0 root         (0) root         (0)     8008 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/pdf_encryption_details_data.py
+-rw-r--r--   0 root         (0) root         (0)    11215 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/comment_insert.py
+-rw-r--r--   0 root         (0) root         (0)     6500 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/office_math_link.py
+-rw-r--r--   0 root         (0) root         (0)     8634 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/document_entry_list.py
+-rw-r--r--   0 root         (0) root         (0)    10474 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/models/document_stat_data.py
+-rw-r--r--   0 root         (0) root         (0)    11506 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/rest.py
+-rw-r--r--   0 root         (0) root         (0)    19297 2024-05-20 06:03:22.000000 aspose-words-cloud-24.5.0/asposewordscloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9423 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 06:04:37.000000 aspose-words-cloud-24.5.0/asposewordscloud/apis/
+-rw-r--r--   0 root         (0) root         (0)  1410970 2024-05-20 06:03:23.000000 aspose-words-cloud-24.5.0/asposewordscloud/apis/words_api.py
+-rw-r--r--   0 root         (0) root         (0)      140 2024-05-20 06:03:22.000000 aspose-words-cloud-24.5.0/asposewordscloud/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    50017 2024-05-20 06:03:22.000000 aspose-words-cloud-24.5.0/asposewordscloud/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 06:04:37.000000 aspose-words-cloud-24.5.0/aspose_words_cloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    39677 2024-05-20 06:04:36.000000 aspose-words-cloud-24.5.0/aspose_words_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-20 06:04:36.000000 aspose-words-cloud-24.5.0/aspose_words_cloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-20 06:04:36.000000 aspose-words-cloud-24.5.0/aspose_words_cloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    16398 2024-05-20 06:04:36.000000 aspose-words-cloud-24.5.0/aspose_words_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 06:04:36.000000 aspose-words-cloud-24.5.0/aspose_words_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 06:04:38.000000 aspose-words-cloud-24.5.0/setup.cfg
```

### Comparing `aspose-words-cloud-24.4.0/LICENSE` & `aspose-words-cloud-24.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/README.md` & `aspose-words-cloud-24.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 - Fetch web pages via URL and save in Microsoft Word file formats.
 - Get document information in JSON or XML representation.
 - [Fetch statistical data](https://docs.aspose.cloud/display/wordscloud/Get+Document+Statistics) of a document.
 - [Remove all macros](https://docs.aspose.cloud/display/wordscloud/Remove+all+Macros+from+Document) contained in a specific document.
 - [Convert a document to desired file format](https://docs.aspose.cloud/display/wordscloud/Convert+Document+to+Destination+Format+with+Detailed+Settings+and+Save+Result+to+Storage) along with detailed settings.
 - Convert an encrypted PDF document into Word document format.
 
+## Enhancements in Version 24.5
+
+- Added the support of multistorage operations. Saving a file as a result of an operation can be performed in a specific storage, when, used file path in the next format '@storage:path/to/file.doc'.
+
+
 ## Enhancements in Version 24.4
 
 - Added the 'MergeWithNext' method to merge a section with the next one.
 - Added the 'LockAspectRatio' propperty for DrawingObjectInsert and DrawingObjectUpdate methods.
 
 
 ## Enhancements in Version 24.3
```

### Comparing `aspose-words-cloud-24.4.0/test/base_test_context.py` & `aspose-words-cloud-24.5.0/test/base_test_context.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/test/test_batch.py` & `aspose-words-cloud-24.5.0/test/test_batch.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/test/test_examples.py` & `aspose-words-cloud-24.5.0/test/test_examples.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/test/__init__.py` & `aspose-words-cloud-24.5.0/test/__init__.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/test/test_url_encode.py` & `aspose-words-cloud-24.5.0/test/test_url_encode.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/test/test_doc_with_password.py` & `aspose-words-cloud-24.5.0/test/test_doc_with_password.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/test/test_readme.py` & `aspose-words-cloud-24.5.0/test/test_readme.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/PKG-INFO` & `aspose-words-cloud-24.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aspose-words-cloud
-Version: 24.4.0
+Version: 24.5.0
 Summary: Python Cloud SDK wraps Aspose.Words Cloud API so you could seamlessly integrate Microsoft Word file generation, manipulation, conversion & inspection features into your own python applications.
 Home-page: https://github.com/aspose-words-cloud/aspose-words-cloud-python
 Author: Yaroslaw Ekimov
 Author-email: yaroslaw.ekimov@aspose.com
 License: UNKNOWN
 Keywords: office,convert,word,pdf,docx,html,rtf,png,jpg,split,merge,edit,word to pdf,pdf to word,docx to pdf,pdf to docx,word to html,html to word,reporting,mailmerge,statistics,watermark,fields,generate,create,report,table,paragraph,images,text,generator,creator,maker
 Platform: UNKNOWN
@@ -34,14 +34,19 @@
 - Fetch web pages via URL and save in Microsoft Word file formats.
 - Get document information in JSON or XML representation.
 - [Fetch statistical data](https://docs.aspose.cloud/display/wordscloud/Get+Document+Statistics) of a document.
 - [Remove all macros](https://docs.aspose.cloud/display/wordscloud/Remove+all+Macros+from+Document) contained in a specific document.
 - [Convert a document to desired file format](https://docs.aspose.cloud/display/wordscloud/Convert+Document+to+Destination+Format+with+Detailed+Settings+and+Save+Result+to+Storage) along with detailed settings.
 - Convert an encrypted PDF document into Word document format.
 
+## Enhancements in Version 24.5
+
+- Added the support of multistorage operations. Saving a file as a result of an operation can be performed in a specific storage, when, used file path in the next format '@storage:path/to/file.doc'.
+
+
 ## Enhancements in Version 24.4
 
 - Added the 'MergeWithNext' method to merge a section with the next one.
 - Added the 'LockAspectRatio' propperty for DrawingObjectInsert and DrawingObjectUpdate methods.
 
 
 ## Enhancements in Version 24.3
```

### Comparing `aspose-words-cloud-24.4.0/setup.py` & `aspose-words-cloud-24.5.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # coding: utf-8
 
 """
     Aspose.Words for Cloud API Reference
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 24.4
+    OpenAPI spec version: 24.5
 
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "aspose-words-cloud"
-VERSION = "24.4.0"
+VERSION = "24.5.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/document.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/document.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/style_apply.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/style_apply.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/jpeg_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/jpeg_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/custom_xml_parts_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/custom_xml_parts_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/paragraph_insert.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/paragraph_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/list_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/list_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/csv_data_load_options.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/csv_data_load_options.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/bmp_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/bmp_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/word_ml_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/word_ml_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/custom_xml_part_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/custom_xml_part_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/list_levels.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/list_levels.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/bookmarks_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/bookmarks_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/office_math_objects_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/office_math_objects_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/lists_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/lists_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/drawing_object_insert.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/drawing_object_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/form_field_collection.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/form_field_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/office_math_object_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/office_math_object_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/fields_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/fields_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/image_entry_list.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/image_entry_list.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/dot_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/dot_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/document_entry.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/document_entry.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/style.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/style.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/field_link.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/field_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/dotx_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/dotx_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/tiff_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/tiff_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/save_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/save_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/run_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/run_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/table_cell_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/table_cell_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/epub_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/epub_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/paragraph_list_format_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/paragraph_list_format_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/xml_data_load_options.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/xml_data_load_options.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/footnote_update.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/footnote_update.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/ott_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/ott_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/table_cell.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/table_cell.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/office_math_objects_collection.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/office_math_objects_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/hyperlinks_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/hyperlinks_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/bookmarks_outline_level_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/bookmarks_outline_level_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/drawing_object_update.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/drawing_object_update.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/structured_document_tag_update.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/structured_document_tag_update.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/paragraph.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/paragraph.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/footnotes_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/footnotes_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/split_document_result.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/split_document_result.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/table_cell_format.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/table_cell_format.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/structured_document_tags_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/structured_document_tags_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/paragraph_format_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/paragraph_format_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/section_page_setup_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/section_page_setup_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/hyperlink_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/hyperlink_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/field.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/field.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/header_footer.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/header_footer.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/tab_stops_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/tab_stops_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/footnote_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/footnote_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/document_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/document_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/page_setup.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/page_setup.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/table_properties.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/table_properties.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/bookmark_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/bookmark_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/comment_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/comment_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/markdown_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/markdown_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_header_footer_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_header_footer_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/delete_border_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/delete_border_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_page_numbers_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_page_numbers_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_footnote_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_footnote_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_bookmark_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_bookmark_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/save_as_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/save_as_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/compress_document_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/compress_document_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_list_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_list_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/compare_document_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/compare_document_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_field_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_field_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_run_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_run_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_section_page_setup_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_section_page_setup_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/delete_paragraph_list_format_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/delete_paragraph_list_format_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/protect_document_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/protect_document_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_table_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_table_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_style_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_style_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/delete_paragraph_tab_stop_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/delete_paragraph_tab_stop_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_or_update_paragraph_tab_stop_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_or_update_paragraph_tab_stop_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_run_font_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_run_font_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/delete_all_paragraph_tab_stops_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/delete_all_paragraph_tab_stops_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_fields_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_fields_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/replace_with_text_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/replace_with_text_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/replace_text_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/replace_text_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_table_row_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_table_row_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_watermark_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_watermark_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_custom_xml_part_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_custom_xml_part_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/reject_all_revisions_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/reject_all_revisions_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_table_row_format_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_table_row_format_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_comment_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_comment_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_structured_document_tag_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_structured_document_tag_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_drawing_object_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_drawing_object_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_field_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_field_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_form_field_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_form_field_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_paragraph_format_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_paragraph_format_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/delete_borders_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/delete_borders_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/remove_range_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/remove_range_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_bookmark_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_bookmark_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/accept_all_revisions_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/accept_all_revisions_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_footnote_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_footnote_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_custom_xml_part_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_custom_xml_part_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_paragraph_list_format_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_paragraph_list_format_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/__init__.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_comment_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_comment_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_run_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_run_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_table_cell_format_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_table_cell_format_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/save_as_tiff_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/save_as_tiff_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_list_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_list_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_style_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_style_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/unprotect_document_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/unprotect_document_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_form_field_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_form_field_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_border_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_border_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/save_as_range_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/save_as_range_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_table_properties_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_table_properties_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/split_document_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/split_document_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_paragraph_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_paragraph_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/copy_style_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/copy_style_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_structured_document_tag_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_structured_document_tag_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_list_level_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_list_level_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/delete_watermark_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/delete_watermark_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/apply_style_to_document_element_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/apply_style_to_document_element_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_table_cell_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_table_cell_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/update_drawing_object_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/update_drawing_object_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/create_or_update_document_property_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/create_or_update_document_property_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_watermark_text_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_watermark_text_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/append_document_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/append_document_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/responses/insert_watermark_image_online_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/responses/insert_watermark_image_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/docm_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/docm_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/ps_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/ps_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/comments_collection.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/comments_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/position_before_node.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/position_before_node.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/dotm_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/dotm_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/bookmark_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/bookmark_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/tab_stop.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/tab_stop.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/table_link_collection_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/table_link_collection_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/hyperlinks.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/hyperlinks.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/table_link.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/table_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/xml_color.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/xml_color.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/custom_xml_part_update.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/custom_xml_part_update.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/header_footer_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/header_footer_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/structured_document_tag.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/structured_document_tag.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/protection_request_v2.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/protection_request_v2.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/font_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/font_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/paragraph_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/paragraph_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/structured_document_tag_collection.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/structured_document_tag_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/field_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/field_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/comment_link.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/comment_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/file_link.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/file_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/node_link.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/node_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/protection_data_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/protection_data_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/structured_document_tag_insert.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/structured_document_tag_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/compare_options.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/compare_options.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/load_web_document_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/load_web_document_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/style_update.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/style_update.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/report_build_options.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/report_build_options.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/range_text_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/range_text_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/paragraph_link_collection_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/paragraph_link_collection_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/report_engine_settings.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/report_engine_settings.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/words_api_error_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/words_api_error_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/footnote_collection.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/footnote_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/style_insert.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/style_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/custom_xml_part_link.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/custom_xml_part_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/table.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/table.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/table_row_insert.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/table_row_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/modification_operation_result.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/modification_operation_result.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/custom_xml_parts_collection.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/custom_xml_parts_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/form_field_checkbox.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/form_field_checkbox.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/section_link_collection_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/section_link_collection_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/range_document.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/range_document.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/story_child_nodes.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/story_child_nodes.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/drawing_object_collection.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/drawing_object_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/paragraph_link.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/paragraph_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/split_document_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/split_document_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/drawing_object_link.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/drawing_object_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/downsample_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/downsample_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/pdf_digital_signature_details_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/pdf_digital_signature_details_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/drawing_objects_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/drawing_objects_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/table_row_format.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/table_row_format.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/save_result.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/save_result.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/tab_stop_insert.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/tab_stop_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/open_xps_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/open_xps_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/optimization_options.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/optimization_options.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/office_math_object.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/office_math_object.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/styles_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/styles_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/protection_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/protection_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/flat_opc_macro_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/flat_opc_macro_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/position_inside_node.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/position_inside_node.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/image_entry.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/image_entry.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/comment.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/comment.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/compress_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/compress_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/odt_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/odt_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/position_after_node.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/position_after_node.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/list_update.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/list_update.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/form_field_drop_down.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/form_field_drop_down.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/list_info.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/list_info.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/classification_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/classification_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/table_cell_format_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/table_cell_format_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/compare_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/compare_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/rtf_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/rtf_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/watermark_text.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/watermark_text.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/document_property.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/document_property.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/info_additional_item.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/info_additional_item.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/borders_collection.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/borders_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/field_collection.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/field_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/classification_result.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/classification_result.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/html_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/html_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/xaml_fixed_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/xaml_fixed_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/paragraph_link_collection.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/paragraph_link_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/comments_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/comments_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/svg_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/svg_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/flat_opc_template_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/flat_opc_template_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/gif_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/gif_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/borders_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/borders_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/header_footers_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/header_footers_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/eps_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/eps_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/xps_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/xps_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/list_level.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/list_level.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/run_insert.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/run_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/pdf_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/pdf_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/style_copy.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/style_copy.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/drawing_object.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/drawing_object.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/revisions_modification_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/revisions_modification_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/info_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/info_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/table_link_collection.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/table_link_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/field_update.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/field_update.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/list_insert.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/list_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/flat_opc_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/flat_opc_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/style_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/style_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/png_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/png_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/bookmark.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/bookmark.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/form_field_text_input.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/form_field_text_input.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/form_field_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/form_field_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/user_information.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/user_information.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/replace_text_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/replace_text_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/section.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/section.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/__init__.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/runs_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/runs_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/run_update.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/run_update.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/time_zone_info_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/time_zone_info_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/protection_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/protection_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/metafile_rendering_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/metafile_rendering_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/replace_text_parameters.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/replace_text_parameters.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/search_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/search_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/watermark_data_text.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/watermark_data_text.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/search_results_collection.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/search_results_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/drawing_object_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/drawing_object_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/list_level_update.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/list_level_update.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/document_property_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/document_property_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/watermark_data_image.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/watermark_data_image.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/file_reference.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/file_reference.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/table_insert.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/table_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/html_fixed_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/html_fixed_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/replace_range.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/replace_range.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/runs.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/runs.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/files_upload_result.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/files_upload_result.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/outline_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/outline_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/document_position.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/document_position.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/border.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/border.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_paragraph_list_format_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_paragraph_list_format_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_page_numbers_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_page_numbers_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/append_document_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/append_document_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_paragraphs_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_paragraphs_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/copy_folder_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/copy_folder_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_table_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_table_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_drawing_object_by_index_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_drawing_object_by_index_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_border_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_border_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_office_math_objects_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_office_math_objects_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_table_row_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_table_row_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/build_report_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/build_report_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_properties_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_properties_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_style_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_style_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_custom_xml_part_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_custom_xml_part_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_section_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_section_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_comments_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_comments_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_bookmark_by_name_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_bookmark_by_name_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_bookmarks_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_bookmarks_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_comments_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_comments_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_comments_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_comments_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_section_page_setup_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_section_page_setup_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/move_file_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/move_file_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_header_footer_of_section_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_header_footer_of_section_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_comment_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_comment_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/build_report_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/build_report_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/copy_file_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/copy_file_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_table_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_table_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_office_math_objects_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_office_math_objects_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/split_document_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/split_document_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_form_field_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_form_field_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/save_as_range_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/save_as_range_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_paragraph_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_paragraph_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_borders_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_borders_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_table_cell_format_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_table_cell_format_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_custom_xml_part_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_custom_xml_part_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_office_math_object_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_office_math_object_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/replace_with_text_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/replace_with_text_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_statistics_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_statistics_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_structured_document_tag_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_structured_document_tag_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_style_from_document_element_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_style_from_document_element_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_table_row_format_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_table_row_format_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/reject_all_revisions_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/reject_all_revisions_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_table_cell_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_table_cell_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/execute_mail_merge_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/execute_mail_merge_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_table_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_table_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_watermark_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_watermark_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_form_field_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_form_field_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_table_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_table_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/load_web_document_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/load_web_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_borders_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_borders_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_hyperlinks_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_hyperlinks_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_table_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_table_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_field_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_field_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/create_or_update_document_property_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/create_or_update_document_property_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_tables_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_tables_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/classify_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/classify_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_paragraph_format_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_paragraph_format_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_runs_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_runs_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_paragraph_tab_stops_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_paragraph_tab_stops_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_watermark_image_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_watermark_image_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/protect_document_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/protect_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_custom_xml_parts_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_custom_xml_parts_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_form_fields_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_form_fields_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_list_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_list_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_paragraph_list_format_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_paragraph_list_format_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_footnote_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_footnote_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/copy_style_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/copy_style_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_paragraph_list_format_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_paragraph_list_format_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_drawing_object_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_drawing_object_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_paragraph_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_paragraph_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_office_math_objects_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_office_math_objects_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_all_paragraph_tab_stops_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_all_paragraph_tab_stops_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/render_math_object_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/render_math_object_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_document_property_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_document_property_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_comment_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_comment_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_all_paragraph_tab_stops_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_all_paragraph_tab_stops_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_paragraphs_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_paragraphs_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_watermark_image_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_watermark_image_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_form_field_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_form_field_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_with_format_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_with_format_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/merge_with_next_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/merge_with_next_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/merge_with_next_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/merge_with_next_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_paragraph_tab_stops_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_paragraph_tab_stops_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_custom_xml_part_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_custom_xml_part_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_paragraph_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_paragraph_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/create_document_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/create_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_protection_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_protection_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_watermark_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_watermark_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_header_footer_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_header_footer_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_folder_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_folder_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_or_update_paragraph_tab_stop_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_or_update_paragraph_tab_stop_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_lists_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_lists_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/render_table_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/render_table_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_structured_document_tag_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_structured_document_tag_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_field_names_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_field_names_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_table_properties_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_table_properties_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_header_footer_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_header_footer_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/replace_text_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/replace_text_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_paragraph_format_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_paragraph_format_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_table_row_format_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_table_row_format_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/unprotect_document_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/unprotect_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_list_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_list_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_style_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_style_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_lists_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_lists_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_macros_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_macros_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_run_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_run_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_table_cell_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_table_cell_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_table_row_format_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_table_row_format_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/batch_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/batch_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_custom_xml_part_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_custom_xml_part_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_bookmark_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_bookmark_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_watermark_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_watermark_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_field_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_field_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_border_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_border_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/render_drawing_object_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/render_drawing_object_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/render_table_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/render_table_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_table_row_format_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_table_row_format_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_section_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_section_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_border_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_border_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_drawing_objects_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_drawing_objects_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_field_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_field_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_border_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_border_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_footnote_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_footnote_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_list_level_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_list_level_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_table_cell_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_table_cell_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/render_math_object_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/render_math_object_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_field_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_field_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/save_as_tiff_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/save_as_tiff_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/optimize_document_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/optimize_document_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_table_row_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_table_row_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_table_row_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_table_row_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_info_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_info_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_section_page_setup_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_section_page_setup_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_field_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_field_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_properties_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_properties_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_office_math_object_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_office_math_object_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/render_page_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/render_page_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/save_as_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/save_as_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/compress_document_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/compress_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/render_paragraph_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/render_paragraph_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/compress_document_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/compress_document_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_run_font_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_run_font_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_fields_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_fields_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_header_footers_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_header_footers_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/move_folder_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/move_folder_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_fields_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_fields_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_table_properties_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_table_properties_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_fields_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_fields_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_custom_xml_parts_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_custom_xml_parts_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/apply_style_to_document_element_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/apply_style_to_document_element_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_office_math_objects_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_office_math_objects_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_section_page_setup_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_section_page_setup_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_comment_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_comment_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_structured_document_tag_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_structured_document_tag_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_list_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_list_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/download_file_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/download_file_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/render_page_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/render_page_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_bookmark_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_bookmark_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_style_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_style_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_list_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_list_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/copy_style_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/copy_style_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_style_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_style_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_run_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_run_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_drawing_object_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_drawing_object_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_custom_xml_part_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_custom_xml_part_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_run_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_run_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_table_cell_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_table_cell_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_footnote_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_footnote_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_paragraph_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_paragraph_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_bookmark_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_bookmark_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_form_field_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_form_field_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/compare_document_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/compare_document_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_hyperlink_by_index_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_hyperlink_by_index_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_form_field_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_form_field_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_field_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_field_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_structured_document_tags_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_structured_document_tags_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/remove_range_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/remove_range_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_footnotes_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_footnotes_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_borders_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_borders_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_paragraph_list_format_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_paragraph_list_format_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_headers_footers_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_headers_footers_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/append_document_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/append_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_footnote_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_footnote_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_table_cell_format_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_table_cell_format_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_footnote_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_footnote_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_fields_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_fields_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/accept_all_revisions_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/accept_all_revisions_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_bookmarks_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_bookmarks_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_custom_xml_part_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_custom_xml_part_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/__init__.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_structured_document_tag_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_structured_document_tag_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_bookmark_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_bookmark_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_footnote_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_footnote_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_table_properties_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_table_properties_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_macros_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_macros_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_header_footer_of_section_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_header_footer_of_section_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/search_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/search_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_watermark_text_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_watermark_text_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_property_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_property_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_property_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_property_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_bookmarks_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_bookmarks_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/link_header_footers_to_previous_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/link_header_footers_to_previous_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_run_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_run_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_style_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_style_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/replace_text_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/replace_text_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_style_from_document_element_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_style_from_document_element_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/save_as_tiff_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/save_as_tiff_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_drawing_objects_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_drawing_objects_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_comment_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_comment_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_section_page_setup_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_section_page_setup_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_office_math_object_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_office_math_object_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/copy_styles_from_template_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/copy_styles_from_template_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/save_as_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/save_as_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_form_field_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_form_field_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/reset_cache_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/reset_cache_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_range_text_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_range_text_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_header_footer_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_header_footer_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_comment_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_comment_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_paragraph_tab_stop_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_paragraph_tab_stop_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/reject_all_revisions_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/reject_all_revisions_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_hyperlinks_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_hyperlinks_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_section_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_section_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/remove_range_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/remove_range_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_structured_document_tags_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_structured_document_tags_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_field_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_field_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_table_row_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_table_row_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_custom_xml_part_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_custom_xml_part_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_table_cell_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_table_cell_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_range_text_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_range_text_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_drawing_object_by_index_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_drawing_object_by_index_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_section_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_section_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_borders_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_borders_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_watermark_text_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_watermark_text_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_protection_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_protection_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_run_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_run_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/create_or_update_document_property_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/create_or_update_document_property_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/apply_style_to_document_element_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/apply_style_to_document_element_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_styles_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_styles_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_page_numbers_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_page_numbers_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_sections_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_sections_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_header_footer_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_header_footer_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_footnote_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_footnote_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_bookmark_by_name_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_bookmark_by_name_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_custom_xml_part_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_custom_xml_part_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_list_level_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_list_level_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_header_footers_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_header_footers_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/create_folder_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/create_folder_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_structured_document_tag_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_structured_document_tag_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_drawing_object_ole_data_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_drawing_object_ole_data_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_drawing_object_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_drawing_object_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/search_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/search_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_drawing_object_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_drawing_object_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_field_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_field_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_table_cell_format_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_table_cell_format_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_structured_document_tag_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_structured_document_tag_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_comment_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_comment_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_watermark_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_watermark_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_statistics_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_statistics_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/optimize_document_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/optimize_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_drawing_object_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_drawing_object_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_run_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_run_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_paragraph_list_format_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_paragraph_list_format_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_custom_xml_parts_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_custom_xml_parts_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_footnote_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_footnote_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_available_fonts_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_available_fonts_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/render_drawing_object_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/render_drawing_object_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_run_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_run_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/base_request_object.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/base_request_object.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_border_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_border_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_form_field_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_form_field_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_files_list_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_files_list_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_structured_document_tag_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_structured_document_tag_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_list_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_list_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/split_document_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/split_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_paragraph_tab_stop_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_paragraph_tab_stop_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_field_names_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_field_names_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_paragraph_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_paragraph_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_bookmark_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_bookmark_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/classify_document_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/classify_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_table_properties_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_table_properties_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_structured_document_tag_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_structured_document_tag_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/convert_document_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/convert_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_run_font_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_run_font_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/compare_document_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/compare_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_hyperlink_by_index_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_hyperlink_by_index_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_table_cell_format_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_table_cell_format_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_paragraph_format_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_paragraph_format_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_comment_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_comment_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_paragraph_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_paragraph_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_styles_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_styles_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_section_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_section_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_form_field_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_form_field_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_run_font_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_run_font_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_drawing_object_image_data_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_drawing_object_image_data_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_headers_footers_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_headers_footers_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_style_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_style_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_paragraph_format_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_paragraph_format_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/protect_document_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/protect_document_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_form_fields_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_form_fields_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_table_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_table_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_table_row_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_table_row_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_table_cell_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_table_cell_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_list_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_list_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_bookmark_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_bookmark_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/execute_mail_merge_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/execute_mail_merge_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_fields_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_fields_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/classify_document_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/classify_document_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_runs_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_runs_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_drawing_object_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_drawing_object_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_border_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_border_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_comments_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_comments_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_office_math_object_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_office_math_object_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_bookmarks_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_bookmarks_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_drawing_object_ole_data_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_drawing_object_ole_data_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/save_as_range_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/save_as_range_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_custom_xml_parts_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_custom_xml_parts_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_document_property_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_document_property_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_comment_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_comment_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/unprotect_document_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/unprotect_document_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_document_drawing_object_image_data_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_document_drawing_object_image_data_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/render_paragraph_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/render_paragraph_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_run_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_run_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/upload_file_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/upload_file_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_run_font_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_run_font_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/update_paragraph_list_format_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/update_paragraph_list_format_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_public_key_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_public_key_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_header_footer_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_header_footer_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_fields_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_fields_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_tables_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_tables_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_table_row_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_table_row_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/accept_all_revisions_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/accept_all_revisions_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_file_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_file_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_footnotes_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_footnotes_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/get_sections_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/get_sections_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/replace_with_text_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/replace_with_text_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_section_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_section_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/insert_or_update_paragraph_tab_stop_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/insert_or_update_paragraph_tab_stop_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/requests/delete_header_footer_online_request.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/requests/delete_header_footer_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/flat_opc_template_macro_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/flat_opc_template_macro_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/document_properties.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/document_properties.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/list_format_update.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/list_format_update.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/document_property_create_or_update.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/document_property_create_or_update.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/xaml_flow_pack_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/xaml_flow_pack_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/emf_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/emf_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/shading.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/shading.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/words_api_link.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/words_api_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/paragraph_format_update.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/paragraph_format_update.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/public_key_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/public_key_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/error.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/error.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/bookmark_insert.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/bookmark_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/field_names_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/field_names_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/header_footer_link.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/header_footer_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/docx_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/docx_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/comment_update.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/comment_update.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/stat_data_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/stat_data_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/run_link.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/run_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/form_fields_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/form_fields_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/paragraph_format.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/paragraph_format.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/bookmarks.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/bookmarks.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/lists.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/lists.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/list_format.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/list_format.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/structured_document_tag_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/structured_document_tag_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/footnote_insert.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/footnote_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/table_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/table_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/header_footer_link_collection.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/header_footer_link_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/custom_xml_part.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/custom_xml_part.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/pcl_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/pcl_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/field_insert.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/field_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/preferred_width.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/preferred_width.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/error_details.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/error_details.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/text_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/text_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/font.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/font.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/border_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/border_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/document_properties_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/document_properties_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/table_cell_insert.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/table_cell_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/structured_document_tag_list_item.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/structured_document_tag_list_item.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/font_info.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/font_info.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/field_names.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/field_names.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/section_link_collection.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/section_link_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/footnote_link.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/footnote_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/link.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/custom_xml_part_insert.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/custom_xml_part_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/table_row_format_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/table_row_format_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/storage_file.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/storage_file.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/footnotes_stat_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/footnotes_stat_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/table_row.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/table_row.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/field_options.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/field_options.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/doc_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/doc_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/hyperlink.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/hyperlink.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/pdf_permissions.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/pdf_permissions.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/table_row_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/table_row_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/page_number.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/page_number.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/files_list.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/files_list.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/section_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/section_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/api_error.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/api_error.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/table_properties_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/table_properties_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/available_fonts_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/available_fonts_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/search_result.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/search_result.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/page_stat_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/page_stat_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/xaml_flow_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/xaml_flow_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/json_data_load_options.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/json_data_load_options.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/section_link.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/section_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/compress_options.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/compress_options.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/mhtml_save_options_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/mhtml_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/run.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/run.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/words_response.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/words_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/footnote.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/footnote.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/link_element.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/link_element.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/pdf_encryption_details_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/pdf_encryption_details_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/comment_insert.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/comment_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/office_math_link.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/office_math_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/document_entry_list.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/document_entry_list.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/models/document_stat_data.py` & `aspose-words-cloud-24.5.0/asposewordscloud/models/document_stat_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/rest.py` & `aspose-words-cloud-24.5.0/asposewordscloud/rest.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/__init__.py` & `aspose-words-cloud-24.5.0/asposewordscloud/__init__.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/configuration.py` & `aspose-words-cloud-24.5.0/asposewordscloud/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,10 +258,10 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 24.4\n"\
-               "SDK Package Version: 24.4".\
+               "Version of the API: 24.5\n"\
+               "SDK Package Version: 24.5".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/apis/words_api.py` & `aspose-words-cloud-24.5.0/asposewordscloud/apis/words_api.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/asposewordscloud/api_client.py` & `aspose-words-cloud-24.5.0/asposewordscloud/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -343,20 +343,20 @@
                  cookie=None):
         if configuration is None:
             configuration = Configuration()
         self.configuration = configuration
 
         self.pool = None
         self.rest_client = rest.RESTClientObject(configuration)
-        self.default_headers = {'x-aspose-client': 'python sdk', 'x-aspose-client-version': '24.4'}
+        self.default_headers = {'x-aspose-client': 'python sdk', 'x-aspose-client-version': '24.5'}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'python sdk 24.4'
+        self.user_agent = 'python sdk 24.5'
 
     def __del__(self):
         if not self.pool is None:
             self.pool.close()
             self.pool.join()
 
     @property
```

### Comparing `aspose-words-cloud-24.4.0/aspose_words_cloud.egg-info/SOURCES.txt` & `aspose-words-cloud-24.5.0/aspose_words_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-24.4.0/aspose_words_cloud.egg-info/PKG-INFO` & `aspose-words-cloud-24.5.0/aspose_words_cloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aspose-words-cloud
-Version: 24.4.0
+Version: 24.5.0
 Summary: Python Cloud SDK wraps Aspose.Words Cloud API so you could seamlessly integrate Microsoft Word file generation, manipulation, conversion & inspection features into your own python applications.
 Home-page: https://github.com/aspose-words-cloud/aspose-words-cloud-python
 Author: Yaroslaw Ekimov
 Author-email: yaroslaw.ekimov@aspose.com
 License: UNKNOWN
 Keywords: office,convert,word,pdf,docx,html,rtf,png,jpg,split,merge,edit,word to pdf,pdf to word,docx to pdf,pdf to docx,word to html,html to word,reporting,mailmerge,statistics,watermark,fields,generate,create,report,table,paragraph,images,text,generator,creator,maker
 Platform: UNKNOWN
@@ -34,14 +34,19 @@
 - Fetch web pages via URL and save in Microsoft Word file formats.
 - Get document information in JSON or XML representation.
 - [Fetch statistical data](https://docs.aspose.cloud/display/wordscloud/Get+Document+Statistics) of a document.
 - [Remove all macros](https://docs.aspose.cloud/display/wordscloud/Remove+all+Macros+from+Document) contained in a specific document.
 - [Convert a document to desired file format](https://docs.aspose.cloud/display/wordscloud/Convert+Document+to+Destination+Format+with+Detailed+Settings+and+Save+Result+to+Storage) along with detailed settings.
 - Convert an encrypted PDF document into Word document format.
 
+## Enhancements in Version 24.5
+
+- Added the support of multistorage operations. Saving a file as a result of an operation can be performed in a specific storage, when, used file path in the next format '@storage:path/to/file.doc'.
+
+
 ## Enhancements in Version 24.4
 
 - Added the 'MergeWithNext' method to merge a section with the next one.
 - Added the 'LockAspectRatio' propperty for DrawingObjectInsert and DrawingObjectUpdate methods.
 
 
 ## Enhancements in Version 24.3
```

