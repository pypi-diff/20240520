# Comparing `tmp/wildberries_api_client-0.1.8.tar.gz` & `tmp/wildberries_api_client-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wildberries_api_client-0.1.8.tar", max compression
+gzip compressed data, was "wildberries_api_client-0.1.9.tar", max compression
```

## Comparing `wildberries_api_client-0.1.8.tar` & `wildberries_api_client-0.1.9.tar`

### file list

```diff
@@ -1,608 +1,608 @@
--rw-r--r--   0        0        0     1444 2024-03-12 21:20:37.432731 wildberries_api_client-0.1.8/README.md
--rw-r--r--   0        0        0      475 2024-04-09 11:48:48.325002 wildberries_api_client-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      389 2024-04-09 11:39:23.883372 wildberries_api_client-0.1.8/wildberries_api_client/__init__.py
--rw-r--r--   0        0        0    25798 2024-04-09 11:39:23.883372 wildberries_api_client-0.1.8/wildberries_api_client/_api_client.py
--rw-r--r--   0        0        0     8108 2024-04-09 11:39:23.883372 wildberries_api_client-0.1.8/wildberries_api_client/_configuration.py
--rw-r--r--   0        0        0    86041 2024-04-09 11:41:22.607984 wildberries_api_client-0.1.8/wildberries_api_client/_swagger_doc/swagger_analytics.yaml
--rw-r--r--   0        0        0   123720 2024-04-09 11:41:14.591943 wildberries_api_client-0.1.8/wildberries_api_client/_swagger_doc/swagger_content.yaml
--rw-r--r--   0        0        0   102691 2024-04-09 11:41:26.612005 wildberries_api_client-0.1.8/wildberries_api_client/_swagger_doc/swagger_feedbacks_questions.yaml
--rw-r--r--   0        0        0   119801 2024-04-09 11:41:20.603974 wildberries_api_client-0.1.8/wildberries_api_client/_swagger_doc/swagger_marketplace.yaml
--rw-r--r--   0        0        0    51073 2024-04-09 11:41:24.607995 wildberries_api_client-0.1.8/wildberries_api_client/_swagger_doc/swagger_prices.yaml
--rw-r--r--   0        0        0   197419 2024-04-09 11:41:18.599964 wildberries_api_client-0.1.8/wildberries_api_client/_swagger_doc/swagger_promotion.yaml
--rw-r--r--   0        0        0    10791 2024-04-09 11:41:16.591953 wildberries_api_client-0.1.8/wildberries_api_client/_swagger_doc/swagger_recommendations.yaml
--rw-r--r--   0        0        0    52604 2024-04-09 11:41:30.624026 wildberries_api_client-0.1.8/wildberries_api_client/_swagger_doc/swagger_statistics.yaml
--rw-r--r--   0        0        0    12940 2024-04-09 11:41:28.616016 wildberries_api_client-0.1.8/wildberries_api_client/_swagger_doc/swagger_tariffs.yaml
--rw-r--r--   0        0        0     1178 2024-04-09 11:39:23.887372 wildberries_api_client-0.1.8/wildberries_api_client/_swagger_doc/transliterate_script.py
--rw-r--r--   0        0        0     9476 2024-04-09 11:42:25.112307 wildberries_api_client-0.1.8/wildberries_api_client/analytics/__init__.py
--rw-r--r--   0        0        0      562 2024-04-09 11:42:25.116307 wildberries_api_client-0.1.8/wildberries_api_client/analytics/api/__init__.py
--rw-r--r--   0        0        0    17124 2024-04-09 11:42:24.960307 wildberries_api_client-0.1.8/wildberries_api_client/analytics/api/othety_pouderhaniam_api.py
--rw-r--r--   0        0        0     6117 2024-04-09 11:42:24.992307 wildberries_api_client-0.1.8/wildberries_api_client/analytics/api/platnaa_priemka_api.py
--rw-r--r--   0        0        0    14564 2024-04-09 11:42:25.020307 wildberries_api_client-0.1.8/wildberries_api_client/analytics/api/platnoe_hranenie_api.py
--rw-r--r--   0        0        0     7077 2024-04-09 11:42:25.048307 wildberries_api_client-0.1.8/wildberries_api_client/analytics/api/tovary_s_obazatelnoi_markirovkoi_api.py
--rw-r--r--   0        0        0    19640 2024-04-09 11:42:25.076307 wildberries_api_client-0.1.8/wildberries_api_client/analytics/api/voronka_prodah_api.py
--rw-r--r--   0        0        0    25741 2024-04-09 11:42:25.156308 wildberries_api_client-0.1.8/wildberries_api_client/analytics/api_client.py
--rw-r--r--   0        0        0     8849 2024-04-09 11:42:25.108307 wildberries_api_client-0.1.8/wildberries_api_client/analytics/configuration.py
--rw-r--r--   0        0        0     8813 2024-04-09 11:42:25.116307 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/__init__.py
--rw-r--r--   0        0        0     3721 2024-04-09 11:42:23.520299 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/create_task_response.py
--rw-r--r--   0        0        0     3847 2024-04-09 11:42:23.608300 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/create_task_response_data.py
--rw-r--r--   0        0        0     4443 2024-04-09 11:42:23.680300 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/error_internal_response.py
--rw-r--r--   0        0        0     3767 2024-04-09 11:42:23.732300 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/error_response.py
--rw-r--r--   0        0        0     4465 2024-04-09 11:42:23.772300 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/excise_report_request.py
--rw-r--r--   0        0        0     3829 2024-04-09 11:42:23.816301 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/excise_report_response.py
--rw-r--r--   0        0        0     3699 2024-04-09 11:42:23.852301 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/get_tasks_response.py
--rw-r--r--   0        0        0     4725 2024-04-09 11:42:23.888301 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/get_tasks_response_data.py
--rw-r--r--   0        0        0     3774 2024-04-09 11:42:23.924301 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/inline_response200.py
--rw-r--r--   0        0        0     3808 2024-04-09 11:42:23.952301 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/inline_response2001.py
--rw-r--r--   0        0        0     6885 2024-04-09 11:42:23.972301 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/inline_response2001_details.py
--rw-r--r--   0        0        0     3785 2024-04-09 11:42:23.992302 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/inline_response2002.py
--rw-r--r--   0        0        0     7598 2024-04-09 11:42:24.020302 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/inline_response2002_report.py
--rw-r--r--   0        0        0     3785 2024-04-09 11:42:24.040302 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/inline_response2003.py
--rw-r--r--   0        0        0    14955 2024-04-09 11:42:24.056302 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/inline_response2003_report.py
--rw-r--r--   0        0        0     8737 2024-04-09 11:42:24.076302 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/inline_response200_report.py
--rw-r--r--   0        0        0     3714 2024-04-09 11:42:24.092302 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/inline_response400.py
--rw-r--r--   0        0        0     3809 2024-04-09 11:42:24.112302 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/models_excise_report_response.py
--rw-r--r--   0        0        0     3113 2024-04-09 11:42:24.128302 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/models_excise_report_response_data.py
--rw-r--r--   0        0        0    13833 2024-04-09 11:42:24.144302 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/models_excise_report_response_data_inner.py
--rw-r--r--   0        0        0     7018 2024-04-09 11:42:24.160302 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_history_request.py
--rw-r--r--   0        0        0     4609 2024-04-09 11:42:24.176303 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_history_request_period.py
--rw-r--r--   0        0        0     6522 2024-04-09 11:42:24.192303 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_history_response.py
--rw-r--r--   0        0        0     6401 2024-04-09 11:42:24.208303 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_history_response_data.py
--rw-r--r--   0        0        0    13438 2024-04-09 11:42:24.224303 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_history_response_history.py
--rw-r--r--   0        0        0     9560 2024-04-09 11:42:24.240303 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_request.py
--rw-r--r--   0        0        0     4655 2024-04-09 11:42:24.256303 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_request_order_by.py
--rw-r--r--   0        0        0     4519 2024-04-09 11:42:24.272303 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_request_period.py
--rw-r--r--   0        0        0     6343 2024-04-09 11:42:24.288303 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_response.py
--rw-r--r--   0        0        0     5487 2024-04-09 11:42:24.304303 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_response_data.py
--rw-r--r--   0        0        0     8807 2024-04-09 11:42:24.320303 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_response_data_cards.py
--rw-r--r--   0        0        0     4563 2024-04-09 11:42:24.336303 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_response_data_object.py
--rw-r--r--   0        0        0     6280 2024-04-09 11:42:24.352303 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_response_data_statistics.py
--rw-r--r--   0        0        0    16504 2024-04-09 11:42:24.368303 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_response_data_statistics_period_comparison.py
--rw-r--r--   0        0        0     7233 2024-04-09 11:42:24.384303 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_response_data_statistics_period_comparison_conversions.py
--rw-r--r--   0        0        0    16256 2024-04-09 11:42:24.400304 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_response_data_statistics_previous_period.py
--rw-r--r--   0        0        0     7201 2024-04-09 11:42:24.416304 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_response_data_statistics_previous_period_conversions.py
--rw-r--r--   0        0        0    16244 2024-04-09 11:42:24.432304 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_response_data_statistics_selected_period.py
--rw-r--r--   0        0        0     7201 2024-04-09 11:42:24.448304 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_response_data_statistics_selected_period_conversions.py
--rw-r--r--   0        0        0     5009 2024-04-09 11:42:24.464304 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_response_data_stocks.py
--rw-r--r--   0        0        0     4523 2024-04-09 11:42:24.476304 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_response_data_tags.py
--rw-r--r--   0        0        0     8716 2024-04-09 11:42:24.496304 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_history_request.py
--rw-r--r--   0        0        0     4621 2024-04-09 11:42:24.512304 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_history_request_period.py
--rw-r--r--   0        0        0     6545 2024-04-09 11:42:24.528304 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_history_response.py
--rw-r--r--   0        0        0     6371 2024-04-09 11:42:24.544304 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_history_response_data.py
--rw-r--r--   0        0        0    13422 2024-04-09 11:42:24.564304 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_history_response_history.py
--rw-r--r--   0        0        0     4611 2024-04-09 11:42:24.588305 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_history_response_object.py
--rw-r--r--   0        0        0     4559 2024-04-09 11:42:24.608305 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_history_response_tag.py
--rw-r--r--   0        0        0     8867 2024-04-09 11:42:24.624305 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_request.py
--rw-r--r--   0        0        0     4635 2024-04-09 11:42:24.640305 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_request_order_by.py
--rw-r--r--   0        0        0     4531 2024-04-09 11:42:24.656305 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_request_period.py
--rw-r--r--   0        0        0     6366 2024-04-09 11:42:24.668305 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_response.py
--rw-r--r--   0        0        0     5529 2024-04-09 11:42:24.684305 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_response_data.py
--rw-r--r--   0        0        0     6413 2024-04-09 11:42:24.696305 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_response_data_groups.py
--rw-r--r--   0        0        0     4575 2024-04-09 11:42:24.716305 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_response_data_object.py
--rw-r--r--   0        0        0     6305 2024-04-09 11:42:24.728305 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_response_data_statistics.py
--rw-r--r--   0        0        0    16557 2024-04-09 11:42:24.744305 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_response_data_statistics_period_comparison.py
--rw-r--r--   0        0        0     7249 2024-04-09 11:42:24.760306 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_response_data_statistics_period_comparison_conversions.py
--rw-r--r--   0        0        0    16305 2024-04-09 11:42:24.772306 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_response_data_statistics_previous_period.py
--rw-r--r--   0        0        0     7235 2024-04-09 11:42:24.788306 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_response_data_statistics_previous_period_conversions.py
--rw-r--r--   0        0        0    16278 2024-04-09 11:42:24.804306 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_response_data_statistics_selected_period.py
--rw-r--r--   0        0        0     6121 2024-04-09 11:42:24.816306 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/response_error.py
--rw-r--r--   0        0        0     4725 2024-04-09 11:42:24.832306 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/response_error_additional_errors.py
--rw-r--r--   0        0        0     3069 2024-04-09 11:42:24.848306 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/response_paid_storage.py
--rw-r--r--   0        0        0    19791 2024-04-09 11:42:24.864306 wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/response_paid_storage_inner.py
--rw-r--r--   0        0        0    13621 2024-04-09 11:42:25.168308 wildberries_api_client-0.1.8/wildberries_api_client/analytics/rest.py
--rw-r--r--   0        0        0    11511 2024-04-09 11:42:13.856249 wildberries_api_client-0.1.8/wildberries_api_client/content/__init__.py
--rw-r--r--   0        0        0      521 2024-04-09 11:42:13.860249 wildberries_api_client-0.1.8/wildberries_api_client/content/api/__init__.py
--rw-r--r--   0        0        0    37657 2024-04-09 11:42:13.556248 wildberries_api_client-0.1.8/wildberries_api_client/content/api/konfigurator_api.py
--rw-r--r--   0        0        0    17179 2024-04-09 11:42:13.608248 wildberries_api_client-0.1.8/wildberries_api_client/content/api/korzina_api.py
--rw-r--r--   0        0        0    25230 2024-04-09 11:42:13.660248 wildberries_api_client-0.1.8/wildberries_api_client/content/api/mediafaily_api.py
--rw-r--r--   0        0        0    16680 2024-04-09 11:42:13.708248 wildberries_api_client-0.1.8/wildberries_api_client/content/api/prosmotr_api.py
--rw-r--r--   0        0        0    20617 2024-04-09 11:42:13.756249 wildberries_api_client-0.1.8/wildberries_api_client/content/api/tegi_api.py
--rw-r--r--   0        0        0    25314 2024-04-09 11:42:13.804249 wildberries_api_client-0.1.8/wildberries_api_client/content/api/zagruzka_api.py
--rw-r--r--   0        0        0    25668 2024-04-09 11:42:13.908249 wildberries_api_client-0.1.8/wildberries_api_client/content/api_client.py
--rw-r--r--   0        0        0     8782 2024-04-09 11:42:13.856249 wildberries_api_client-0.1.8/wildberries_api_client/content/configuration.py
--rw-r--r--   0        0        0    10893 2024-04-09 11:42:13.860249 wildberries_api_client-0.1.8/wildberries_api_client/content/models/__init__.py
--rw-r--r--   0        0        0     3717 2024-04-09 11:42:11.316236 wildberries_api_client-0.1.8/wildberries_api_client/content/models/cards_list_body.py
--rw-r--r--   0        0        0     2988 2024-04-09 11:42:11.388236 wildberries_api_client-0.1.8/wildberries_api_client/content/models/cards_move_nm_body.py
--rw-r--r--   0        0        0     3731 2024-04-09 11:42:11.444237 wildberries_api_client-0.1.8/wildberries_api_client/content/models/cards_recover_body.py
--rw-r--r--   0        0        0     3728 2024-04-09 11:42:11.484237 wildberries_api_client-0.1.8/wildberries_api_client/content/models/cards_trash_body.py
--rw-r--r--   0        0        0     9773 2024-04-09 11:42:11.540237 wildberries_api_client-0.1.8/wildberries_api_client/content/models/cards_update_body.py
--rw-r--r--   0        0        0     4892 2024-04-09 11:42:11.584237 wildberries_api_client-0.1.8/wildberries_api_client/content/models/cards_upload_body.py
--rw-r--r--   0        0        0     4657 2024-04-09 11:42:11.624238 wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2cardsupdate_characteristics.py
--rw-r--r--   0        0        0     5265 2024-04-09 11:42:11.648238 wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2cardsupdate_dimensions.py
--rw-r--r--   0        0        0     6395 2024-04-09 11:42:11.676238 wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2cardsupdate_sizes.py
--rw-r--r--   0        0        0     4840 2024-04-09 11:42:11.704238 wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2cardsupload_characteristics.py
--rw-r--r--   0        0        0     5265 2024-04-09 11:42:11.728238 wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2cardsupload_dimensions.py
--rw-r--r--   0        0        0     6170 2024-04-09 11:42:11.752238 wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2cardsupload_sizes.py
--rw-r--r--   0        0        0     9429 2024-04-09 11:42:11.780238 wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2cardsupload_variants.py
--rw-r--r--   0        0        0     9603 2024-04-09 11:42:11.804239 wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2cardsuploadadd_cards_to_add.py
--rw-r--r--   0        0        0     4691 2024-04-09 11:42:11.832239 wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2cardsuploadadd_characteristics.py
--rw-r--r--   0        0        0     6120 2024-04-09 11:42:11.856239 wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2cardsuploadadd_sizes.py
--rw-r--r--   0        0        0     5339 2024-04-09 11:42:11.880239 wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2getcardslist_settings.py
--rw-r--r--   0        0        0     3851 2024-04-09 11:42:11.904239 wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2getcardslist_settings_cursor.py
--rw-r--r--   0        0        0     9813 2024-04-09 11:42:11.928239 wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2getcardslist_settings_filter.py
--rw-r--r--   0        0        0     4032 2024-04-09 11:42:11.960239 wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2getcardslist_settings_sort.py
--rw-r--r--   0        0        0     5364 2024-04-09 11:42:11.988239 wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2getcardstrash_settings.py
--rw-r--r--   0        0        0     3857 2024-04-09 11:42:12.012240 wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2getcardstrash_settings_cursor.py
--rw-r--r--   0        0        0     4026 2024-04-09 11:42:12.040240 wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2getcardstrash_settings_filter.py
--rw-r--r--   0        0        0     4024 2024-04-09 11:42:12.064240 wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2getcardstrash_settings_sort.py
--rw-r--r--   0        0        0     3741 2024-04-09 11:42:12.092240 wildberries_api_client-0.1.8/wildberries_api_client/content/models/delete_trash_body.py
--rw-r--r--   0        0        0     6137 2024-04-09 11:42:12.136240 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response200.py
--rw-r--r--   0        0        0     4465 2024-04-09 11:42:12.172240 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2001.py
--rw-r--r--   0        0        0     6181 2024-04-09 11:42:12.200241 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response20010.py
--rw-r--r--   0        0        0     6199 2024-04-09 11:42:12.224241 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response20011.py
--rw-r--r--   0        0        0     4524 2024-04-09 11:42:12.244241 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response20011_data.py
--rw-r--r--   0        0        0     6081 2024-04-09 11:42:12.264241 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response20012.py
--rw-r--r--   0        0        0     6062 2024-04-09 11:42:12.280241 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response20013.py
--rw-r--r--   0        0        0     6113 2024-04-09 11:42:12.304241 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response20014.py
--rw-r--r--   0        0        0     5087 2024-04-09 11:42:12.320241 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response20014_data.py
--rw-r--r--   0        0        0     3004 2024-04-09 11:42:12.340241 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response20015.py
--rw-r--r--   0        0        0     3004 2024-04-09 11:42:12.356241 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response20016.py
--rw-r--r--   0        0        0     6071 2024-04-09 11:42:12.372242 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response20017.py
--rw-r--r--   0        0        0     4511 2024-04-09 11:42:12.388242 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response20018.py
--rw-r--r--   0        0        0    10453 2024-04-09 11:42:12.408242 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response20018_cards.py
--rw-r--r--   0        0        0     5055 2024-04-09 11:42:12.424242 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response20018_characteristics.py
--rw-r--r--   0        0        0     5071 2024-04-09 11:42:12.444242 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response20018_cursor.py
--rw-r--r--   0        0        0     5077 2024-04-09 11:42:12.464242 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response20018_dimensions.py
--rw-r--r--   0        0        0     6065 2024-04-09 11:42:12.480242 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response20018_sizes.py
--rw-r--r--   0        0        0    15931 2024-04-09 11:42:12.496242 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2001_cards.py
--rw-r--r--   0        0        0     5406 2024-04-09 11:42:12.512242 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2001_characteristics.py
--rw-r--r--   0        0        0     5463 2024-04-09 11:42:12.532242 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2001_cursor.py
--rw-r--r--   0        0        0     5233 2024-04-09 11:42:12.548242 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2001_dimensions.py
--rw-r--r--   0        0        0     5236 2024-04-09 11:42:12.564242 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2001_photos.py
--rw-r--r--   0        0        0     6167 2024-04-09 11:42:12.584243 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2001_sizes.py
--rw-r--r--   0        0        0     5623 2024-04-09 11:42:12.600243 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2001_tags.py
--rw-r--r--   0        0        0     6114 2024-04-09 11:42:12.616243 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2002.py
--rw-r--r--   0        0        0     7180 2024-04-09 11:42:12.632243 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2002_data.py
--rw-r--r--   0        0        0     6090 2024-04-09 11:42:12.648243 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2003.py
--rw-r--r--   0        0        0     4734 2024-04-09 11:42:12.660243 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2003_data.py
--rw-r--r--   0        0        0     6124 2024-04-09 11:42:12.676243 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2004.py
--rw-r--r--   0        0        0     5219 2024-04-09 11:42:12.692243 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2004_data.py
--rw-r--r--   0        0        0     6210 2024-04-09 11:42:12.708243 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2005.py
--rw-r--r--   0        0        0     7209 2024-04-09 11:42:12.760244 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2005_data.py
--rw-r--r--   0        0        0     6176 2024-04-09 11:42:12.784244 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2006.py
--rw-r--r--   0        0        0    10713 2024-04-09 11:42:12.808244 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2006_data.py
--rw-r--r--   0        0        0     6108 2024-04-09 11:42:12.828244 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2007.py
--rw-r--r--   0        0        0     4577 2024-04-09 11:42:12.844244 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2007_data.py
--rw-r--r--   0        0        0     6157 2024-04-09 11:42:12.860244 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2008.py
--rw-r--r--   0        0        0     6108 2024-04-09 11:42:12.876244 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2009.py
--rw-r--r--   0        0        0     4543 2024-04-09 11:42:12.888244 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2009_data.py
--rw-r--r--   0        0        0     2996 2024-04-09 11:42:12.904244 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response400.py
--rw-r--r--   0        0        0     3000 2024-04-09 11:42:12.920244 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response4001.py
--rw-r--r--   0        0        0     3000 2024-04-09 11:42:12.940245 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response4002.py
--rw-r--r--   0        0        0     3000 2024-04-09 11:42:12.952244 wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response4003.py
--rw-r--r--   0        0        0     3679 2024-04-09 11:42:12.968245 wildberries_api_client-0.1.8/wildberries_api_client/content/models/media_file_body.py
--rw-r--r--   0        0        0     3687 2024-04-09 11:42:12.980245 wildberries_api_client-0.1.8/wildberries_api_client/content/models/media_file_body1.py
--rw-r--r--   0        0        0     4459 2024-04-09 11:42:12.996245 wildberries_api_client-0.1.8/wildberries_api_client/content/models/media_save_body.py
--rw-r--r--   0        0        0     4601 2024-04-09 11:42:13.012245 wildberries_api_client-0.1.8/wildberries_api_client/content/models/media_save_body1.py
--rw-r--r--   0        0        0     4905 2024-04-09 11:42:13.024245 wildberries_api_client-0.1.8/wildberries_api_client/content/models/nomenclature_link_body.py
--rw-r--r--   0        0        0     3008 2024-04-09 11:42:13.040245 wildberries_api_client-0.1.8/wildberries_api_client/content/models/one_ofcards_move_nm_body.py
--rw-r--r--   0        0        0     3024 2024-04-09 11:42:13.052245 wildberries_api_client-0.1.8/wildberries_api_client/content/models/one_ofinline_response20015.py
--rw-r--r--   0        0        0     3024 2024-04-09 11:42:13.068245 wildberries_api_client-0.1.8/wildberries_api_client/content/models/one_ofinline_response20016.py
--rw-r--r--   0        0        0     3016 2024-04-09 11:42:13.080245 wildberries_api_client-0.1.8/wildberries_api_client/content/models/one_ofinline_response400.py
--rw-r--r--   0        0        0     3020 2024-04-09 11:42:13.100245 wildberries_api_client-0.1.8/wildberries_api_client/content/models/one_ofinline_response4001.py
--rw-r--r--   0        0        0     3020 2024-04-09 11:42:13.116245 wildberries_api_client-0.1.8/wildberries_api_client/content/models/one_ofinline_response4002.py
--rw-r--r--   0        0        0     3020 2024-04-09 11:42:13.128245 wildberries_api_client-0.1.8/wildberries_api_client/content/models/one_ofinline_response4003.py
--rw-r--r--   0        0        0     3084 2024-04-09 11:42:13.144245 wildberries_api_client-0.1.8/wildberries_api_client/content/models/one_ofresponse_card_create_additional_errors.py
--rw-r--r--   0        0        0     4932 2024-04-09 11:42:13.156246 wildberries_api_client-0.1.8/wildberries_api_client/content/models/request_move_nms_imt_conn.py
--rw-r--r--   0        0        0     3945 2024-04-09 11:42:13.172246 wildberries_api_client-0.1.8/wildberries_api_client/content/models/request_move_nms_imt_disconn.py
--rw-r--r--   0        0        0     6256 2024-04-09 11:42:13.184246 wildberries_api_client-0.1.8/wildberries_api_client/content/models/response_body_content_error400.py
--rw-r--r--   0        0        0     4056 2024-04-09 11:42:13.200246 wildberries_api_client-0.1.8/wildberries_api_client/content/models/response_body_content_error400_additional_errors.py
--rw-r--r--   0        0        0     6222 2024-04-09 11:42:13.216246 wildberries_api_client-0.1.8/wildberries_api_client/content/models/response_body_content_error403.py
--rw-r--r--   0        0        0     6150 2024-04-09 11:42:13.228246 wildberries_api_client-0.1.8/wildberries_api_client/content/models/response_card_create.py
--rw-r--r--   0        0        0     6118 2024-04-09 11:42:13.244246 wildberries_api_client-0.1.8/wildberries_api_client/content/models/response_content_error1.py
--rw-r--r--   0        0        0     3771 2024-04-09 11:42:13.264246 wildberries_api_client-0.1.8/wildberries_api_client/content/models/response_content_error1_additional_errors.py
--rw-r--r--   0        0        0     6118 2024-04-09 11:42:13.280246 wildberries_api_client-0.1.8/wildberries_api_client/content/models/response_content_error4.py
--rw-r--r--   0        0        0     3891 2024-04-09 11:42:13.292246 wildberries_api_client-0.1.8/wildberries_api_client/content/models/response_content_error4_additional_errors.py
--rw-r--r--   0        0        0     6118 2024-04-09 11:42:13.308246 wildberries_api_client-0.1.8/wildberries_api_client/content/models/response_content_error5.py
--rw-r--r--   0        0        0     3790 2024-04-09 11:42:13.324247 wildberries_api_client-0.1.8/wildberries_api_client/content/models/response_content_error5_additional_errors.py
--rw-r--r--   0        0        0     6102 2024-04-09 11:42:13.336246 wildberries_api_client-0.1.8/wildberries_api_client/content/models/response_content_error6.py
--rw-r--r--   0        0        0     3643 2024-04-09 11:42:13.352247 wildberries_api_client-0.1.8/wildberries_api_client/content/models/response_incorrect_date.py
--rw-r--r--   0        0        0     4238 2024-04-09 11:42:13.368247 wildberries_api_client-0.1.8/wildberries_api_client/content/models/tag_id_body.py
--rw-r--r--   0        0        0     4653 2024-04-09 11:42:13.380247 wildberries_api_client-0.1.8/wildberries_api_client/content/models/upload_add_body.py
--rw-r--r--   0        0        0     3849 2024-04-09 11:42:13.396247 wildberries_api_client-0.1.8/wildberries_api_client/content/models/v2_barcodes_body.py
--rw-r--r--   0        0        0     4782 2024-04-09 11:42:13.416247 wildberries_api_client-0.1.8/wildberries_api_client/content/models/v2_tag_body.py
--rw-r--r--   0        0        0    13556 2024-04-09 11:42:13.924250 wildberries_api_client-0.1.8/wildberries_api_client/content/rest.py
--rw-r--r--   0        0        0     8626 2024-04-09 11:42:29.552330 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/__init__.py
--rw-r--r--   0        0        0      373 2024-04-09 11:42:29.556330 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/api/__init__.py
--rw-r--r--   0        0        0    15796 2024-04-09 11:42:29.516330 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/api/hablony_dla_voprosov_i_otzyvov_api.py
--rw-r--r--   0        0        0    55850 2024-04-09 11:42:29.432330 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/api/otzyvy_api.py
--rw-r--r--   0        0        0    34196 2024-04-09 11:42:29.480330 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/api/voprosy_api.py
--rw-r--r--   0        0        0    25259 2024-04-09 11:42:29.596331 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/api_client.py
--rw-r--r--   0        0        0     8337 2024-04-09 11:42:29.552330 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/configuration.py
--rw-r--r--   0        0        0     8132 2024-04-09 11:42:29.556330 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/__init__.py
--rw-r--r--   0        0        0     3311 2024-04-09 11:42:27.936322 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/apiv1questions_answer.py
--rw-r--r--   0        0        0     5632 2024-04-09 11:42:27.992322 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response200.py
--rw-r--r--   0        0        0     5655 2024-04-09 11:42:28.036322 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2001.py
--rw-r--r--   0        0        0     5696 2024-04-09 11:42:28.084323 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20010.py
--rw-r--r--   0        0        0     4348 2024-04-09 11:42:28.124323 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20010_data.py
--rw-r--r--   0        0        0     5696 2024-04-09 11:42:28.152323 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20011.py
--rw-r--r--   0        0        0     4419 2024-04-09 11:42:28.176323 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20011_data.py
--rw-r--r--   0        0        0     5678 2024-04-09 11:42:28.196323 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20012.py
--rw-r--r--   0        0        0     5201 2024-04-09 11:42:28.216323 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20012_data.py
--rw-r--r--   0        0        0     5678 2024-04-09 11:42:28.252323 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20013.py
--rw-r--r--   0        0        0     4606 2024-04-09 11:42:28.280324 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20013_data.py
--rw-r--r--   0        0        0     7197 2024-04-09 11:42:28.300324 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20013_data_feedback_valuations.py
--rw-r--r--   0        0        0     5221 2024-04-09 11:42:28.320324 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20013_data_product_valuations.py
--rw-r--r--   0        0        0     5678 2024-04-09 11:42:28.340324 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20014.py
--rw-r--r--   0        0        0     4870 2024-04-09 11:42:28.364324 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20014_data.py
--rw-r--r--   0        0        0     5678 2024-04-09 11:42:28.384324 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20015.py
--rw-r--r--   0        0        0     3321 2024-04-09 11:42:28.404324 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20015_data.py
--rw-r--r--   0        0        0     5678 2024-04-09 11:42:28.420324 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20016.py
--rw-r--r--   0        0        0     4324 2024-04-09 11:42:28.436324 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20016_data.py
--rw-r--r--   0        0        0     5700 2024-04-09 11:42:28.456325 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20017.py
--rw-r--r--   0        0        0     5678 2024-04-09 11:42:28.476325 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20018.py
--rw-r--r--   0        0        0    21542 2024-04-09 11:42:28.496325 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20018_data.py
--rw-r--r--   0        0        0     4353 2024-04-09 11:42:28.520325 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20018_data_answer.py
--rw-r--r--   0        0        0     4345 2024-04-09 11:42:28.536325 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20018_data_photo_links.py
--rw-r--r--   0        0        0     8682 2024-04-09 11:42:28.556325 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20018_data_product_details.py
--rw-r--r--   0        0        0     5197 2024-04-09 11:42:28.572325 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20018_data_video.py
--rw-r--r--   0        0        0     2547 2024-04-09 11:42:28.592325 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20019.py
--rw-r--r--   0        0        0     4627 2024-04-09 11:42:28.608325 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2001_data.py
--rw-r--r--   0        0        0     5655 2024-04-09 11:42:28.624325 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2002.py
--rw-r--r--   0        0        0     2547 2024-04-09 11:42:28.644326 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20020.py
--rw-r--r--   0        0        0     2547 2024-04-09 11:42:28.660326 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20021.py
--rw-r--r--   0        0        0     3445 2024-04-09 11:42:28.676326 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2002_data.py
--rw-r--r--   0        0        0     6789 2024-04-09 11:42:28.692326 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2002_data_products.py
--rw-r--r--   0        0        0     5655 2024-04-09 11:42:28.708326 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2003.py
--rw-r--r--   0        0        0     5346 2024-04-09 11:42:28.724326 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2003_data.py
--rw-r--r--   0        0        0     5085 2024-04-09 11:42:28.740326 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2003_data_answer.py
--rw-r--r--   0        0        0     7875 2024-04-09 11:42:28.764326 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2003_data_product_details.py
--rw-r--r--   0        0        0     8745 2024-04-09 11:42:28.788326 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2003_data_questions.py
--rw-r--r--   0        0        0     5607 2024-04-09 11:42:28.808326 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2004.py
--rw-r--r--   0        0        0     5655 2024-04-09 11:42:28.824326 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2005.py
--rw-r--r--   0        0        0     4854 2024-04-09 11:42:28.836326 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2005_data.py
--rw-r--r--   0        0        0     5682 2024-04-09 11:42:28.852327 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2006.py
--rw-r--r--   0        0        0     5655 2024-04-09 11:42:28.868327 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2007.py
--rw-r--r--   0        0        0     8463 2024-04-09 11:42:28.884327 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2007_data.py
--rw-r--r--   0        0        0     5655 2024-04-09 11:42:28.904327 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2008.py
--rw-r--r--   0        0        0     5451 2024-04-09 11:42:28.916327 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2008_data.py
--rw-r--r--   0        0        0     5673 2024-04-09 11:42:28.932327 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2009.py
--rw-r--r--   0        0        0     4249 2024-04-09 11:42:28.948327 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2009_data.py
--rw-r--r--   0        0        0     4618 2024-04-09 11:42:28.960327 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response200_data.py
--rw-r--r--   0        0        0     2567 2024-04-09 11:42:28.976327 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/one_ofinline_response20019.py
--rw-r--r--   0        0        0     2567 2024-04-09 11:42:28.992327 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/one_ofinline_response20020.py
--rw-r--r--   0        0        0     2567 2024-04-09 11:42:29.004327 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/one_ofinline_response20021.py
--rw-r--r--   0        0        0     2551 2024-04-09 11:42:29.020327 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/one_ofv1_feedbacks_body.py
--rw-r--r--   0        0        0     2551 2024-04-09 11:42:29.040328 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/one_ofv1_questions_body.py
--rw-r--r--   0        0        0     3343 2024-04-09 11:42:29.052328 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/order_return_body.py
--rw-r--r--   0        0        0     5521 2024-04-09 11:42:29.068328 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/patch_del_resp_ok.py
--rw-r--r--   0        0        0     5563 2024-04-09 11:42:29.080328 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/post_template_ok.py
--rw-r--r--   0        0        0     3190 2024-04-09 11:42:29.096328 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/post_template_ok_data.py
--rw-r--r--   0        0        0     8888 2024-04-09 11:42:29.108328 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/product_rating.py
--rw-r--r--   0        0        0     5485 2024-04-09 11:42:29.124328 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/response200.py
--rw-r--r--   0        0        0     3299 2024-04-09 11:42:29.140328 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/response200_data.py
--rw-r--r--   0        0        0     4638 2024-04-09 11:42:29.156328 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/response200_data_templates.py
--rw-r--r--   0        0        0     5667 2024-04-09 11:42:29.172328 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/response_error_template.py
--rw-r--r--   0        0        0     2535 2024-04-09 11:42:29.184328 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/response_feadback.py
--rw-r--r--   0        0        0    21349 2024-04-09 11:42:29.200328 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/response_feadback_inner.py
--rw-r--r--   0        0        0     6351 2024-04-09 11:42:29.216328 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/responsefeedback_err.py
--rw-r--r--   0        0        0     2531 2024-04-09 11:42:29.228329 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/v1_feedbacks_body.py
--rw-r--r--   0        0        0     2531 2024-04-09 11:42:29.244329 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/v1_questions_body.py
--rw-r--r--   0        0        0     5169 2024-04-09 11:42:29.256329 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/v1_templates_body.py
--rw-r--r--   0        0        0     3461 2024-04-09 11:42:29.276329 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/v1_templates_body1.py
--rw-r--r--   0        0        0     5039 2024-04-09 11:42:29.300329 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/v1_templates_body2.py
--rw-r--r--   0        0        0    13099 2024-04-09 11:42:29.608331 wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/rest.py
--rw-r--r--   0        0        0     6029 2024-04-09 11:42:19.532278 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/__init__.py
--rw-r--r--   0        0        0      478 2024-04-09 11:42:19.536279 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/api/__init__.py
--rw-r--r--   0        0        0    14672 2024-04-09 11:42:19.364278 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/api/ostatki_api.py
--rw-r--r--   0        0        0    65043 2024-04-09 11:42:19.404278 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/api/postavki_api.py
--rw-r--r--   0        0        0    19880 2024-04-09 11:42:19.436278 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/api/propuska_api.py
--rw-r--r--   0        0        0    62159 2024-04-09 11:42:19.464278 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/api/sborohnye_zadania_api.py
--rw-r--r--   0        0        0    19721 2024-04-09 11:42:19.496278 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/api/sklady_api.py
--rw-r--r--   0        0        0    25162 2024-04-09 11:42:19.584279 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/api_client.py
--rw-r--r--   0        0        0     8264 2024-04-09 11:42:19.528278 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/configuration.py
--rw-r--r--   0        0        0     5446 2024-04-09 11:42:19.532278 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/__init__.py
--rw-r--r--   0        0        0     3936 2024-04-09 11:42:17.968270 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/apiv3stockswarehouse_id_stocks.py
--rw-r--r--   0        0        0     4408 2024-04-09 11:42:18.024271 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/error.py
--rw-r--r--   0        0        0     3248 2024-04-09 11:42:18.064271 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response200.py
--rw-r--r--   0        0        0     3745 2024-04-09 11:42:18.096271 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response2001.py
--rw-r--r--   0        0        0     3164 2024-04-09 11:42:18.128271 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response20010.py
--rw-r--r--   0        0        0     3210 2024-04-09 11:42:18.160272 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response20011.py
--rw-r--r--   0        0        0     3209 2024-04-09 11:42:18.192272 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response20012.py
--rw-r--r--   0        0        0     3900 2024-04-09 11:42:18.220272 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response20012_stocks.py
--rw-r--r--   0        0        0     3198 2024-04-09 11:42:18.256272 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response2002.py
--rw-r--r--   0        0        0     5728 2024-04-09 11:42:18.292272 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response2002_orders.py
--rw-r--r--   0        0        0     3272 2024-04-09 11:42:18.324272 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response2003.py
--rw-r--r--   0        0        0     4146 2024-04-09 11:42:18.348272 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response2003_orders.py
--rw-r--r--   0        0        0     3244 2024-04-09 11:42:18.372273 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response2004.py
--rw-r--r--   0        0        0     6566 2024-04-09 11:42:18.392273 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response2004_stickers.py
--rw-r--r--   0        0        0     3080 2024-04-09 11:42:18.420273 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response2005.py
--rw-r--r--   0        0        0     3244 2024-04-09 11:42:18.440273 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response2006.py
--rw-r--r--   0        0        0     4117 2024-04-09 11:42:18.464273 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response2006_stickers.py
--rw-r--r--   0        0        0     3864 2024-04-09 11:42:18.480273 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response2007.py
--rw-r--r--   0        0        0     3159 2024-04-09 11:42:18.500273 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response2008.py
--rw-r--r--   0        0        0     4080 2024-04-09 11:42:18.520273 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response2009.py
--rw-r--r--   0        0        0     3119 2024-04-09 11:42:18.540273 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response201.py
--rw-r--r--   0        0        0     3300 2024-04-09 11:42:18.560274 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response2011.py
--rw-r--r--   0        0        0     3119 2024-04-09 11:42:18.576274 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response2012.py
--rw-r--r--   0        0        0     3123 2024-04-09 11:42:18.596274 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response2013.py
--rw-r--r--   0        0        0     4868 2024-04-09 11:42:18.620274 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/meta.py
--rw-r--r--   0        0        0     3166 2024-04-09 11:42:18.640274 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/meta_gtin_body.py
--rw-r--r--   0        0        0     3166 2024-04-09 11:42:18.664274 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/meta_imei_body.py
--rw-r--r--   0        0        0     3289 2024-04-09 11:42:18.688274 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/meta_sgtin_body.py
--rw-r--r--   0        0        0     3135 2024-04-09 11:42:18.704274 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/meta_uin_body.py
--rw-r--r--   0        0        0     9113 2024-04-09 11:42:18.724274 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/model_pass.py
--rw-r--r--   0        0        0     2422 2024-04-09 11:42:18.744274 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/next.py
--rw-r--r--   0        0        0     9869 2024-04-09 11:42:18.764274 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/office.py
--rw-r--r--   0        0        0    18457 2024-04-09 11:42:18.784275 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/order.py
--rw-r--r--   0        0        0     9435 2024-04-09 11:42:18.808275 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/order_address.py
--rw-r--r--   0        0        0    19005 2024-04-09 11:42:18.832275 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/order_new.py
--rw-r--r--   0        0        0     3696 2024-04-09 11:42:18.856275 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/order_user.py
--rw-r--r--   0        0        0     3325 2024-04-09 11:42:18.876275 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/orders_externalstickers_body.py
--rw-r--r--   0        0        0     3330 2024-04-09 11:42:18.892275 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/orders_status_body.py
--rw-r--r--   0        0        0     3261 2024-04-09 11:42:18.908275 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/orders_stickers_body.py
--rw-r--r--   0        0        0     4339 2024-04-09 11:42:18.924275 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/pass_office.py
--rw-r--r--   0        0        0     6762 2024-04-09 11:42:18.940276 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/passes_pass_id_body.py
--rw-r--r--   0        0        0     3439 2024-04-09 11:42:18.956276 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/stocks_warehouse_id_body.py
--rw-r--r--   0        0        0     3203 2024-04-09 11:42:18.976276 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/stocks_warehouse_id_body1.py
--rw-r--r--   0        0        0     3203 2024-04-09 11:42:18.992276 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/stocks_warehouse_id_body2.py
--rw-r--r--   0        0        0     8073 2024-04-09 11:42:19.008276 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/supply.py
--rw-r--r--   0        0        0     3348 2024-04-09 11:42:19.024276 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/supply_id_trbx_body.py
--rw-r--r--   0        0        0     3389 2024-04-09 11:42:19.040276 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/supply_id_trbx_body1.py
--rw-r--r--   0        0        0    16008 2024-04-09 11:42:19.056276 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/supply_order.py
--rw-r--r--   0        0        0     3772 2024-04-09 11:42:19.072276 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/supply_trbx.py
--rw-r--r--   0        0        0     3960 2024-04-09 11:42:19.088276 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/trbx_stickers.py
--rw-r--r--   0        0        0     3403 2024-04-09 11:42:19.108276 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/trbx_stickers_body.py
--rw-r--r--   0        0        0     3398 2024-04-09 11:42:19.124276 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/trbx_trbx_id_body.py
--rw-r--r--   0        0        0     6666 2024-04-09 11:42:19.140277 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/v3_passes_body.py
--rw-r--r--   0        0        0     3133 2024-04-09 11:42:19.156277 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/v3_supplies_body.py
--rw-r--r--   0        0        0     4078 2024-04-09 11:42:19.172277 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/v3_warehouses_body.py
--rw-r--r--   0        0        0     7263 2024-04-09 11:42:19.192277 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/warehouse.py
--rw-r--r--   0        0        0     4208 2024-04-09 11:42:19.216277 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/warehouses_warehouse_id_body.py
--rw-r--r--   0        0        0    13034 2024-04-09 11:42:19.604279 wildberries_api_client-0.1.8/wildberries_api_client/marketplace/rest.py
--rw-r--r--   0        0        0     4686 2024-04-09 11:42:16.632264 wildberries_api_client-0.1.8/wildberries_api_client/prices/__init__.py
--rw-r--r--   0        0        0      507 2024-04-09 11:42:16.636263 wildberries_api_client-0.1.8/wildberries_api_client/prices/api/__init__.py
--rw-r--r--   0        0        0     8081 2024-04-09 11:42:16.596263 wildberries_api_client-0.1.8/wildberries_api_client/prices/api/ceny_api.py
--rw-r--r--   0        0        0    18723 2024-04-09 11:42:16.492263 wildberries_api_client-0.1.8/wildberries_api_client/prices/api/promokody_i_skidki_api.py
--rw-r--r--   0        0        0    18101 2024-04-09 11:42:16.528263 wildberries_api_client-0.1.8/wildberries_api_client/prices/api/sostoania_zagruzok_api.py
--rw-r--r--   0        0        0    10585 2024-04-09 11:42:16.552263 wildberries_api_client-0.1.8/wildberries_api_client/prices/api/spiski_tovarov_api.py
--rw-r--r--   0        0        0     9042 2024-04-09 11:42:16.576263 wildberries_api_client-0.1.8/wildberries_api_client/prices/api/ustanovka_cen_i_skidok_api.py
--rw-r--r--   0        0        0    25157 2024-04-09 11:42:16.680264 wildberries_api_client-0.1.8/wildberries_api_client/prices/api_client.py
--rw-r--r--   0        0        0     8274 2024-04-09 11:42:16.628264 wildberries_api_client-0.1.8/wildberries_api_client/prices/configuration.py
--rw-r--r--   0        0        0     4084 2024-04-09 11:42:16.636263 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/__init__.py
--rw-r--r--   0        0        0     2441 2024-04-09 11:42:15.080255 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/date1.py
--rw-r--r--   0        0        0     4819 2024-04-09 11:42:15.132256 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/good.py
--rw-r--r--   0        0        0     9567 2024-04-09 11:42:15.192256 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/good_buffer_history.py
--rw-r--r--   0        0        0    10043 2024-04-09 11:42:15.240256 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/good_history.py
--rw-r--r--   0        0        0     2461 2024-04-09 11:42:15.284257 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/good_status.py
--rw-r--r--   0        0        0     2485 2024-04-09 11:42:15.332257 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/good_status_buffer.py
--rw-r--r--   0        0        0     2441 2024-04-09 11:42:15.372257 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/goods.py
--rw-r--r--   0        0        0     7505 2024-04-09 11:42:15.412257 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/goods_list.py
--rw-r--r--   0        0        0     5681 2024-04-09 11:42:15.448257 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/goods_list_sizes.py
--rw-r--r--   0        0        0     5343 2024-04-09 11:42:15.500258 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response200.py
--rw-r--r--   0        0        0     3149 2024-04-09 11:42:15.544258 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response2001.py
--rw-r--r--   0        0        0     4237 2024-04-09 11:42:15.580258 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response2001_data.py
--rw-r--r--   0        0        0     4643 2024-04-09 11:42:15.612258 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response2002.py
--rw-r--r--   0        0        0     4631 2024-04-09 11:42:15.648258 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response2003.py
--rw-r--r--   0        0        0     4235 2024-04-09 11:42:15.688259 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response2003_data.py
--rw-r--r--   0        0        0     3149 2024-04-09 11:42:15.720259 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response2004.py
--rw-r--r--   0        0        0     3365 2024-04-09 11:42:15.752259 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response2004_data.py
--rw-r--r--   0        0        0     4631 2024-04-09 11:42:15.784259 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response2005.py
--rw-r--r--   0        0        0     3350 2024-04-09 11:42:15.816259 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response2005_data.py
--rw-r--r--   0        0        0     2493 2024-04-09 11:42:15.856259 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response2006.py
--rw-r--r--   0        0        0     5385 2024-04-09 11:42:15.888260 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response2007.py
--rw-r--r--   0        0        0     3297 2024-04-09 11:42:15.920260 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response2008.py
--rw-r--r--   0        0        0     4429 2024-04-09 11:42:15.952260 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response400.py
--rw-r--r--   0        0        0     2493 2024-04-09 11:42:15.980260 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response4001.py
--rw-r--r--   0        0        0     4429 2024-04-09 11:42:16.016260 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response401.py
--rw-r--r--   0        0        0     4429 2024-04-09 11:42:16.044260 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response4_xx.py
--rw-r--r--   0        0        0     4429 2024-04-09 11:42:16.064261 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response5_xx.py
--rw-r--r--   0        0        0     2457 2024-04-09 11:42:16.084261 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/model_date.py
--rw-r--r--   0        0        0     2513 2024-04-09 11:42:16.104261 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/one_ofinline_response2006.py
--rw-r--r--   0        0        0     2513 2024-04-09 11:42:16.124261 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/one_ofinline_response4001.py
--rw-r--r--   0        0        0     3793 2024-04-09 11:42:16.148261 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/response_error.py
--rw-r--r--   0        0        0    10201 2024-04-09 11:42:16.180261 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/size_good.py
--rw-r--r--   0        0        0     5458 2024-04-09 11:42:16.200261 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/size_good_req.py
--rw-r--r--   0        0        0     2473 2024-04-09 11:42:16.220261 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/size_goods_body.py
--rw-r--r--   0        0        0     3195 2024-04-09 11:42:16.236261 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/successful.py
--rw-r--r--   0        0        0     7572 2024-04-09 11:42:16.256261 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/supplier_task_metadata.py
--rw-r--r--   0        0        0     7832 2024-04-09 11:42:16.272262 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/supplier_task_metadata_buffer.py
--rw-r--r--   0        0        0     4707 2024-04-09 11:42:16.292262 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/task_already_exists_error.py
--rw-r--r--   0        0        0     4191 2024-04-09 11:42:16.312262 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/task_already_exists_error_data.py
--rw-r--r--   0        0        0     4498 2024-04-09 11:42:16.332262 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/task_created.py
--rw-r--r--   0        0        0     4059 2024-04-09 11:42:16.352262 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/task_created_data.py
--rw-r--r--   0        0        0     2461 2024-04-09 11:42:16.368262 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/task_status.py
--rw-r--r--   0        0        0     2485 2024-04-09 11:42:16.384262 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/task_status_buffer.py
--rw-r--r--   0        0        0     3834 2024-04-09 11:42:16.400262 wildberries_api_client-0.1.8/wildberries_api_client/prices/models/v1_prices_body.py
--rw-r--r--   0        0        0    13049 2024-04-09 11:42:16.692264 wildberries_api_client-0.1.8/wildberries_api_client/prices/rest.py
--rw-r--r--   0        0        0    12883 2024-04-09 11:42:09.904229 wildberries_api_client-0.1.8/wildberries_api_client/promotion/__init__.py
--rw-r--r--   0        0        0     1365 2024-04-09 11:42:09.908229 wildberries_api_client-0.1.8/wildberries_api_client/promotion/api/__init__.py
--rw-r--r--   0        0        0    13079 2024-04-09 11:42:09.568227 wildberries_api_client-0.1.8/wildberries_api_client/promotion/api/aktivnost_kampanii_api.py
--rw-r--r--   0        0        0    15473 2024-04-09 11:42:09.600227 wildberries_api_client-0.1.8/wildberries_api_client/promotion/api/aktivnost_mediakampanii_api.py
--rw-r--r--   0        0        0    23976 2024-04-09 11:42:09.628227 wildberries_api_client-0.1.8/wildberries_api_client/promotion/api/finansy_api.py
--rw-r--r--   0        0        0    14233 2024-04-09 11:42:09.652227 wildberries_api_client-0.1.8/wildberries_api_client/promotion/api/media_api.py
--rw-r--r--   0        0        0    23292 2024-04-09 11:42:09.680228 wildberries_api_client-0.1.8/wildberries_api_client/promotion/api/prodvihenie_api.py
--rw-r--r--   0        0        0    20016 2024-04-09 11:42:09.704228 wildberries_api_client-0.1.8/wildberries_api_client/promotion/api/slovari_api.py
--rw-r--r--   0        0        0    25550 2024-04-09 11:42:09.728228 wildberries_api_client-0.1.8/wildberries_api_client/promotion/api/statistika_api.py
--rw-r--r--   0        0        0     4846 2024-04-09 11:42:09.756228 wildberries_api_client-0.1.8/wildberries_api_client/promotion/api/statistika_mediakampanii_api.py
--rw-r--r--   0        0        0    16840 2024-04-09 11:42:09.776228 wildberries_api_client-0.1.8/wildberries_api_client/promotion/api/stavki_api.py
--rw-r--r--   0        0        0     5206 2024-04-09 11:42:09.800228 wildberries_api_client-0.1.8/wildberries_api_client/promotion/api/stavki_mediakampanii_api.py
--rw-r--r--   0        0        0     4584 2024-04-09 11:42:09.824228 wildberries_api_client-0.1.8/wildberries_api_client/promotion/api/upravlenie_obhimi_parametrami_kampanii_api.py
--rw-r--r--   0        0        0    19421 2024-04-09 11:42:09.844228 wildberries_api_client-0.1.8/wildberries_api_client/promotion/api/upravlenie_parametrami_avtomatiheskih_kampanii_api.py
--rw-r--r--   0        0        0    37598 2024-04-09 11:42:09.868229 wildberries_api_client-0.1.8/wildberries_api_client/promotion/api/upravlenie_parametrami_kampanii_v_poiske_ipoisk_katalog_api.py
--rw-r--r--   0        0        0    25364 2024-04-09 11:42:09.952229 wildberries_api_client-0.1.8/wildberries_api_client/promotion/api_client.py
--rw-r--r--   0        0        0     8472 2024-04-09 11:42:09.900229 wildberries_api_client-0.1.8/wildberries_api_client/promotion/configuration.py
--rw-r--r--   0        0        0    11417 2024-04-09 11:42:09.908229 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/__init__.py
--rw-r--r--   0        0        0     4262 2024-04-09 11:42:06.812213 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/advert_pause_body.py
--rw-r--r--   0        0        0     4252 2024-04-09 11:42:06.884213 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/advert_start_body.py
--rw-r--r--   0        0        0     4246 2024-04-09 11:42:06.944213 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/advert_stop_body.py
--rw-r--r--   0        0        0     3992 2024-04-09 11:42:07.008214 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/advv0allcpm_cpm.py
--rw-r--r--   0        0        0     4140 2024-04-09 11:42:07.052214 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/advv1searchsupplierproducts_kind.py
--rw-r--r--   0        0        0     4192 2024-04-09 11:42:07.096214 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/advv1searchsupplierproducts_subject.py
--rw-r--r--   0        0        0     5080 2024-04-09 11:42:07.144214 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/auto_active_body.py
--rw-r--r--   0        0        0     3495 2024-04-09 11:42:07.184215 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/auto_setexcluded_body.py
--rw-r--r--   0        0        0     4174 2024-04-09 11:42:07.224215 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/auto_updatenm_body.py
--rw-r--r--   0        0        0     2664 2024-04-09 11:42:07.264215 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/booster_stats.py
--rw-r--r--   0        0        0     4987 2024-04-09 11:42:07.308215 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/booster_stats_inner.py
--rw-r--r--   0        0        0     5277 2024-04-09 11:42:07.352216 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/budget_deposit_body.py
--rw-r--r--   0        0        0     5021 2024-04-09 11:42:07.396216 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/cpm_change_body.py
--rw-r--r--   0        0        0     2660 2024-04-09 11:42:07.436216 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/daily_stats1.py
--rw-r--r--   0        0        0     4273 2024-04-09 11:42:07.472216 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/daily_stats1_inner.py
--rw-r--r--   0        0        0     2660 2024-04-09 11:42:07.508216 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/daily_stats2.py
--rw-r--r--   0        0        0     4273 2024-04-09 11:42:07.544216 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/daily_stats2_inner.py
--rw-r--r--   0        0        0     2632 2024-04-09 11:42:07.580217 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/days.py
--rw-r--r--   0        0        0    11005 2024-04-09 11:42:07.616217 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/days_inner.py
--rw-r--r--   0        0        0     3504 2024-04-09 11:42:07.644217 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response200.py
--rw-r--r--   0        0        0     2688 2024-04-09 11:42:07.688217 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response2001.py
--rw-r--r--   0        0        0     9674 2024-04-09 11:42:07.724218 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20010.py
--rw-r--r--   0        0        0     7763 2024-04-09 11:42:07.748218 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20011.py
--rw-r--r--   0        0        0     4132 2024-04-09 11:42:07.772218 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20012.py
--rw-r--r--   0        0        0     4092 2024-04-09 11:42:07.800218 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20013.py
--rw-r--r--   0        0        0     4062 2024-04-09 11:42:07.824218 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20014.py
--rw-r--r--   0        0        0     4779 2024-04-09 11:42:07.848218 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20015.py
--rw-r--r--   0        0        0     4850 2024-04-09 11:42:07.868218 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20016.py
--rw-r--r--   0        0        0     2692 2024-04-09 11:42:07.884218 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20017.py
--rw-r--r--   0        0        0     6539 2024-04-09 11:42:07.904218 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20018.py
--rw-r--r--   0        0        0     4644 2024-04-09 11:42:07.924219 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20019.py
--rw-r--r--   0        0        0     5289 2024-04-09 11:42:07.944218 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20019_clusters.py
--rw-r--r--   0        0        0     4144 2024-04-09 11:42:07.968219 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response2002.py
--rw-r--r--   0        0        0     4259 2024-04-09 11:42:07.984219 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20020.py
--rw-r--r--   0        0        0     6405 2024-04-09 11:42:08.000219 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20020_stat.py
--rw-r--r--   0        0        0     4745 2024-04-09 11:42:08.020219 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20021.py
--rw-r--r--   0        0        0    12800 2024-04-09 11:42:08.036219 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20021_stat.py
--rw-r--r--   0        0        0     7628 2024-04-09 11:42:08.056219 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20021_words.py
--rw-r--r--   0        0        0     4334 2024-04-09 11:42:08.072219 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20021_words_keywords.py
--rw-r--r--   0        0        0     6850 2024-04-09 11:42:08.092219 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20022.py
--rw-r--r--   0        0        0     5652 2024-04-09 11:42:08.116220 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20022_catalog.py
--rw-r--r--   0        0        0     4896 2024-04-09 11:42:08.148220 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20022_dates.py
--rw-r--r--   0        0        0     5632 2024-04-09 11:42:08.176220 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20022_search.py
--rw-r--r--   0        0        0     4860 2024-04-09 11:42:08.204220 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20023.py
--rw-r--r--   0        0        0     6153 2024-04-09 11:42:08.220220 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20024.py
--rw-r--r--   0        0        0     6199 2024-04-09 11:42:08.236220 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response2002_adverts.py
--rw-r--r--   0        0        0     9246 2024-04-09 11:42:08.252220 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response2003.py
--rw-r--r--   0        0        0    10116 2024-04-09 11:42:08.272220 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response2004.py
--rw-r--r--   0        0        0     9967 2024-04-09 11:42:08.288221 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response2004_extended.py
--rw-r--r--   0        0        0    24213 2024-04-09 11:42:08.304221 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response2004_items.py
--rw-r--r--   0        0        0     4117 2024-04-09 11:42:08.328221 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response2004_show_hours.py
--rw-r--r--   0        0        0     4040 2024-04-09 11:42:08.344221 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response2005.py
--rw-r--r--   0        0        0     4147 2024-04-09 11:42:08.360221 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response2006.py
--rw-r--r--   0        0        0     4767 2024-04-09 11:42:08.376221 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response2007.py
--rw-r--r--   0        0        0     4903 2024-04-09 11:42:08.392221 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response2008.py
--rw-r--r--   0        0        0     2688 2024-04-09 11:42:08.408221 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response2009.py
--rw-r--r--   0        0        0     4447 2024-04-09 11:42:08.424221 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response200_advert_list.py
--rw-r--r--   0        0        0     5806 2024-04-09 11:42:08.440221 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response200_adverts.py
--rw-r--r--   0        0        0     3299 2024-04-09 11:42:08.456221 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response400.py
--rw-r--r--   0        0        0     2708 2024-04-09 11:42:08.476221 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/one_ofinline_response2001.py
--rw-r--r--   0        0        0     2712 2024-04-09 11:42:08.492221 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/one_ofinline_response20017.py
--rw-r--r--   0        0        0     2708 2024-04-09 11:42:08.508221 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/one_ofinline_response2009.py
--rw-r--r--   0        0        0     2680 2024-04-09 11:42:08.528222 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/one_ofv1_stats_body.py
--rw-r--r--   0        0        0     2696 2024-04-09 11:42:08.544222 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/one_ofv2_fullstats_body.py
--rw-r--r--   0        0        0     2700 2024-04-09 11:42:08.560222 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/request_with_campaign_id.py
--rw-r--r--   0        0        0     3379 2024-04-09 11:42:08.576222 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/request_with_campaign_id_inner.py
--rw-r--r--   0        0        0     2676 2024-04-09 11:42:08.588222 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/request_with_date.py
--rw-r--r--   0        0        0     4117 2024-04-09 11:42:08.604222 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/request_with_date_inner.py
--rw-r--r--   0        0        0     2692 2024-04-09 11:42:08.620222 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/request_with_interval.py
--rw-r--r--   0        0        0     4233 2024-04-09 11:42:08.640222 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/request_with_interval_inner.py
--rw-r--r--   0        0        0     3864 2024-04-09 11:42:08.656222 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response429.py
--rw-r--r--   0        0        0     3299 2024-04-09 11:42:08.672222 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_adv_error1.py
--rw-r--r--   0        0        0     4613 2024-04-09 11:42:08.688223 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_advert401.py
--rw-r--r--   0        0        0    12997 2024-04-09 11:42:08.704223 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_info_advert.py
--rw-r--r--   0        0        0     4174 2024-04-09 11:42:08.720223 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_info_advert_intervals.py
--rw-r--r--   0        0        0     4327 2024-04-09 11:42:08.740223 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_info_advert_nms.py
--rw-r--r--   0        0        0    11475 2024-04-09 11:42:08.756223 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_info_advert_params.py
--rw-r--r--   0        0        0    11745 2024-04-09 11:42:08.772223 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_info_advert_type8.py
--rw-r--r--   0        0        0     8667 2024-04-09 11:42:08.788223 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_info_advert_type8_auto_params.py
--rw-r--r--   0        0        0     5480 2024-04-09 11:42:08.816223 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_info_advert_type8_auto_params_active.py
--rw-r--r--   0        0        0     4242 2024-04-09 11:42:08.844223 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_info_advert_type8_auto_params_menus.py
--rw-r--r--   0        0        0     4192 2024-04-09 11:42:08.872223 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_info_advert_type8_auto_params_nm_cpm.py
--rw-r--r--   0        0        0     4226 2024-04-09 11:42:08.904224 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_info_advert_type8_auto_params_sets.py
--rw-r--r--   0        0        0     4262 2024-04-09 11:42:08.920224 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_info_advert_type8_auto_params_subject.py
--rw-r--r--   0        0        0    11793 2024-04-09 11:42:08.936224 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_info_advert_type9.py
--rw-r--r--   0        0        0     4152 2024-04-09 11:42:08.964224 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_info_advert_type9_menus.py
--rw-r--r--   0        0        0     4234 2024-04-09 11:42:08.980224 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_info_advert_type9_subject.py
--rw-r--r--   0        0        0     6863 2024-04-09 11:42:08.996224 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_info_advert_type9_united_params.py
--rw-r--r--   0        0        0     2680 2024-04-09 11:42:09.016224 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_with_date.py
--rw-r--r--   0        0        0    14243 2024-04-09 11:42:09.032224 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_with_date_inner.py
--rw-r--r--   0        0        0     2696 2024-04-09 11:42:09.052224 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_with_interval.py
--rw-r--r--   0        0        0    14963 2024-04-09 11:42:09.072224 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_with_interval_inner.py
--rw-r--r--   0        0        0     3407 2024-04-09 11:42:09.092224 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_with_return.py
--rw-r--r--   0        0        0     4625 2024-04-09 11:42:09.108225 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/seacat_savead_body.py
--rw-r--r--   0        0        0     3511 2024-04-09 11:42:09.124225 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/search_setexcluded_body.py
--rw-r--r--   0        0        0     3455 2024-04-09 11:42:09.140225 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/search_setphrase_body.py
--rw-r--r--   0        0        0     3435 2024-04-09 11:42:09.160225 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/search_setplus_body.py
--rw-r--r--   0        0        0     3455 2024-04-09 11:42:09.176225 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/search_setstrong_body.py
--rw-r--r--   0        0        0     3310 2024-04-09 11:42:09.192225 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/stat.py
--rw-r--r--   0        0        0     4080 2024-04-09 11:42:09.208225 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/stat_date.py
--rw-r--r--   0        0        0     4082 2024-04-09 11:42:09.224225 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/stat_interval.py
--rw-r--r--   0        0        0     4124 2024-04-09 11:42:09.240225 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/stat_interval_interval.py
--rw-r--r--   0        0        0     2640 2024-04-09 11:42:09.256225 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/stats1.py
--rw-r--r--   0        0        0     5604 2024-04-09 11:42:09.272225 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/stats1_inner.py
--rw-r--r--   0        0        0     2640 2024-04-09 11:42:09.288226 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/stats2.py
--rw-r--r--   0        0        0     7078 2024-04-09 11:42:09.304226 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/stats2_inner.py
--rw-r--r--   0        0        0    18349 2024-04-09 11:42:09.324226 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/stats_blok1.py
--rw-r--r--   0        0        0    18349 2024-04-09 11:42:09.340226 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/stats_blok2.py
--rw-r--r--   0        0        0     3803 2024-04-09 11:42:09.356226 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/v0_allcpm_body.py
--rw-r--r--   0        0        0     8090 2024-04-09 11:42:09.372226 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/v0_cpm_body.py
--rw-r--r--   0        0        0     4356 2024-04-09 11:42:09.396226 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/v0_rename_body.py
--rw-r--r--   0        0        0     9588 2024-04-09 11:42:09.412226 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/v1_savead_body.py
--rw-r--r--   0        0        0     2660 2024-04-09 11:42:09.428226 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/v1_stats_body.py
--rw-r--r--   0        0        0     2676 2024-04-09 11:42:09.444226 wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/v2_fullstats_body.py
--rw-r--r--   0        0        0    13244 2024-04-09 11:42:09.968229 wildberries_api_client-0.1.8/wildberries_api_client/promotion/rest.py
--rw-r--r--   0        0        0     1101 2024-04-09 11:42:26.556315 wildberries_api_client-0.1.8/wildberries_api_client/recommendations/__init__.py
--rw-r--r--   0        0        0      175 2024-04-09 11:42:26.560315 wildberries_api_client-0.1.8/wildberries_api_client/recommendations/api/__init__.py
--rw-r--r--   0        0        0    19295 2024-04-09 11:42:26.476314 wildberries_api_client-0.1.8/wildberries_api_client/recommendations/api/rekomendacii_api.py
--rw-r--r--   0        0        0    25179 2024-04-09 11:42:26.664315 wildberries_api_client-0.1.8/wildberries_api_client/recommendations/api_client.py
--rw-r--r--   0        0        0     8269 2024-04-09 11:42:26.552315 wildberries_api_client-0.1.8/wildberries_api_client/recommendations/configuration.py
--rw-r--r--   0        0        0      813 2024-04-09 11:42:26.560315 wildberries_api_client-0.1.8/wildberries_api_client/recommendations/models/__init__.py
--rw-r--r--   0        0        0     3142 2024-04-09 11:42:26.176313 wildberries_api_client-0.1.8/wildberries_api_client/recommendations/models/inline_response200.py
--rw-r--r--   0        0        0     3917 2024-04-09 11:42:26.228313 wildberries_api_client-0.1.8/wildberries_api_client/recommendations/models/inline_response200_data.py
--rw-r--r--   0        0        0     4136 2024-04-09 11:42:26.284313 wildberries_api_client-0.1.8/wildberries_api_client/recommendations/models/v1_del_body.py
--rw-r--r--   0        0        0     4124 2024-04-09 11:42:26.332314 wildberries_api_client-0.1.8/wildberries_api_client/recommendations/models/v1_ins_body.py
--rw-r--r--   0        0        0     4078 2024-04-09 11:42:26.380314 wildberries_api_client-0.1.8/wildberries_api_client/recommendations/models/v1_set_body.py
--rw-r--r--   0        0        0    13035 2024-04-09 11:42:26.688315 wildberries_api_client-0.1.8/wildberries_api_client/recommendations/rest.py
--rw-r--r--   0        0        0      662 2024-04-09 11:39:23.915372 wildberries_api_client-0.1.8/wildberries_api_client/setup.py
--rw-r--r--   0        0        0     3273 2024-04-09 11:42:22.020291 wildberries_api_client-0.1.8/wildberries_api_client/statistics/__init__.py
--rw-r--r--   0        0        0      264 2024-04-09 11:42:22.024291 wildberries_api_client-0.1.8/wildberries_api_client/statistics/api/__init__.py
--rw-r--r--   0        0        0    13880 2024-04-09 11:42:21.932291 wildberries_api_client-0.1.8/wildberries_api_client/statistics/api/otlohennaa_generacia_api.py
--rw-r--r--   0        0        0    30740 2024-04-09 11:42:21.964291 wildberries_api_client-0.1.8/wildberries_api_client/statistics/api/statistika_api.py
--rw-r--r--   0        0        0    25099 2024-04-09 11:42:22.076292 wildberries_api_client-0.1.8/wildberries_api_client/statistics/api_client.py
--rw-r--r--   0        0        0     8204 2024-04-09 11:42:22.016291 wildberries_api_client-0.1.8/wildberries_api_client/statistics/configuration.py
--rw-r--r--   0        0        0     2906 2024-04-09 11:42:22.020291 wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/__init__.py
--rw-r--r--   0        0        0     2805 2024-04-09 11:42:20.904286 wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/create_task_request.py
--rw-r--r--   0        0        0     4298 2024-04-09 11:42:20.972286 wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/create_task_request_paid_storage.py
--rw-r--r--   0        0        0     6013 2024-04-09 11:42:21.028286 wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/create_task_request_paid_storage_params.py
--rw-r--r--   0        0        0     3075 2024-04-09 11:42:21.080286 wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/create_task_response.py
--rw-r--r--   0        0        0     3203 2024-04-09 11:42:21.144287 wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/create_task_response_data.py
--rw-r--r--   0        0        0    58735 2024-04-09 11:42:21.208287 wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/detail_report_item.py
--rw-r--r--   0        0        0     3101 2024-04-09 11:42:21.260287 wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/download_request.py
--rw-r--r--   0        0        0     3121 2024-04-09 11:42:21.304288 wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/error_response.py
--rw-r--r--   0        0        0     3058 2024-04-09 11:42:21.356288 wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/get_tasks_request.py
--rw-r--r--   0        0        0     3053 2024-04-09 11:42:21.404288 wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/get_tasks_response.py
--rw-r--r--   0        0        0     3163 2024-04-09 11:42:21.448288 wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/get_tasks_response_bytes_error.py
--rw-r--r--   0        0        0     3248 2024-04-09 11:42:21.484289 wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/get_tasks_response_bytes_error_data.py
--rw-r--r--   0        0        0     4672 2024-04-09 11:42:21.520289 wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/get_tasks_response_bytes_error_data_tasks.py
--rw-r--r--   0        0        0     4077 2024-04-09 11:42:21.548289 wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/get_tasks_response_data.py
--rw-r--r--   0        0        0    13118 2024-04-09 11:42:21.576289 wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/incomes_item.py
--rw-r--r--   0        0        0     2415 2024-04-09 11:42:21.600289 wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/inline_response200.py
--rw-r--r--   0        0        0     2415 2024-04-09 11:42:21.624289 wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/inline_response429.py
--rw-r--r--   0        0        0     2435 2024-04-09 11:42:21.644289 wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/one_of_create_task_request.py
--rw-r--r--   0        0        0     2435 2024-04-09 11:42:21.668290 wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/one_ofinline_response200.py
--rw-r--r--   0        0        0     2435 2024-04-09 11:42:21.688289 wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/one_ofinline_response429.py
--rw-r--r--   0        0        0    25075 2024-04-09 11:42:21.712290 wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/orders_item.py
--rw-r--r--   0        0        0     3595 2024-04-09 11:42:21.732290 wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/response429.py
--rw-r--r--   0        0        0     3116 2024-04-09 11:42:21.752290 wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/response_error_statistics.py
--rw-r--r--   0        0        0     2423 2024-04-09 11:42:21.772290 wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/response_paid_storage.py
--rw-r--r--   0        0        0    18065 2024-04-09 11:42:21.792290 wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/response_paid_storage_inner.py
--rw-r--r--   0        0        0    25876 2024-04-09 11:42:21.820290 wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/sales_item.py
--rw-r--r--   0        0        0    16906 2024-04-09 11:42:21.844290 wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/stocks_item.py
--rw-r--r--   0        0        0    12975 2024-04-09 11:42:22.088292 wildberries_api_client-0.1.8/wildberries_api_client/statistics/rest.py
--rw-r--r--   0        0        0     2009 2024-04-09 11:42:31.340340 wildberries_api_client-0.1.8/wildberries_api_client/tariffs/__init__.py
--rw-r--r--   0        0        0      288 2024-04-09 11:42:31.344339 wildberries_api_client-0.1.8/wildberries_api_client/tariffs/api/__init__.py
--rw-r--r--   0        0        0     9355 2024-04-09 11:42:31.204339 wildberries_api_client-0.1.8/wildberries_api_client/tariffs/api/koefficienty_skladov_api.py
--rw-r--r--   0        0        0     5002 2024-04-09 11:42:31.268339 wildberries_api_client-0.1.8/wildberries_api_client/tariffs/api/stoimost_vozvrata_prodavcu_api.py
--rw-r--r--   0        0        0    25158 2024-04-09 11:42:31.416340 wildberries_api_client-0.1.8/wildberries_api_client/tariffs/api_client.py
--rw-r--r--   0        0        0     8304 2024-04-09 11:42:31.336340 wildberries_api_client-0.1.8/wildberries_api_client/tariffs/configuration.py
--rw-r--r--   0        0        0     1624 2024-04-09 11:42:31.344339 wildberries_api_client-0.1.8/wildberries_api_client/tariffs/models/__init__.py
--rw-r--r--   0        0        0     3233 2024-04-09 11:42:30.648336 wildberries_api_client-0.1.8/wildberries_api_client/tariffs/models/models_return_tariffs_response.py
--rw-r--r--   0        0        0     3200 2024-04-09 11:42:30.716336 wildberries_api_client-0.1.8/wildberries_api_client/tariffs/models/models_tariffs_box_response.py
--rw-r--r--   0        0        0     3233 2024-04-09 11:42:30.768337 wildberries_api_client-0.1.8/wildberries_api_client/tariffs/models/models_tariffs_pallet_response.py
--rw-r--r--   0        0        0     8745 2024-04-09 11:42:30.816337 wildberries_api_client-0.1.8/wildberries_api_client/tariffs/models/models_warehouse_box_rates.py
--rw-r--r--   0        0        0     9358 2024-04-09 11:42:30.872337 wildberries_api_client-0.1.8/wildberries_api_client/tariffs/models/models_warehouse_pallet_rates.py
--rw-r--r--   0        0        0    18800 2024-04-09 11:42:30.916337 wildberries_api_client-0.1.8/wildberries_api_client/tariffs/models/models_warehouse_return_rates.py
--rw-r--r--   0        0        0     6115 2024-04-09 11:42:30.952337 wildberries_api_client-0.1.8/wildberries_api_client/tariffs/models/models_warehouses_box_rates.py
--rw-r--r--   0        0        0     6248 2024-04-09 11:42:31.000338 wildberries_api_client-0.1.8/wildberries_api_client/tariffs/models/models_warehouses_pallet_rates.py
--rw-r--r--   0        0        0     8020 2024-04-09 11:42:31.032338 wildberries_api_client-0.1.8/wildberries_api_client/tariffs/models/models_warehouses_return_rates.py
--rw-r--r--   0        0        0     3265 2024-04-09 11:42:31.060338 wildberries_api_client-0.1.8/wildberries_api_client/tariffs/models/return_tariffs_response.py
--rw-r--r--   0        0        0     3232 2024-04-09 11:42:31.092338 wildberries_api_client-0.1.8/wildberries_api_client/tariffs/models/tariffs_box_response.py
--rw-r--r--   0        0        0     3265 2024-04-09 11:42:31.128338 wildberries_api_client-0.1.8/wildberries_api_client/tariffs/models/tariffs_pallet_response.py
--rw-r--r--   0        0        0    13046 2024-04-09 11:42:31.440340 wildberries_api_client-0.1.8/wildberries_api_client/tariffs/rest.py
--rw-r--r--   0        0        0     2205 1970-01-01 00:00:00.000000 wildberries_api_client-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1444 2024-03-12 21:20:37.432731 wildberries_api_client-0.1.9/README.md
+-rw-r--r--   0        0        0      475 2024-05-20 07:36:45.775474 wildberries_api_client-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      389 2024-04-09 11:39:23.883372 wildberries_api_client-0.1.9/wildberries_api_client/__init__.py
+-rw-r--r--   0        0        0    25798 2024-04-09 11:39:23.883372 wildberries_api_client-0.1.9/wildberries_api_client/_api_client.py
+-rw-r--r--   0        0        0     8108 2024-04-09 11:39:23.883372 wildberries_api_client-0.1.9/wildberries_api_client/_configuration.py
+-rw-r--r--   0        0        0    86041 2024-04-09 11:41:22.607984 wildberries_api_client-0.1.9/wildberries_api_client/_swagger_doc/swagger_analytics.yaml
+-rw-r--r--   0        0        0   123720 2024-04-09 11:41:14.591943 wildberries_api_client-0.1.9/wildberries_api_client/_swagger_doc/swagger_content.yaml
+-rw-r--r--   0        0        0   102691 2024-04-09 11:41:26.612005 wildberries_api_client-0.1.9/wildberries_api_client/_swagger_doc/swagger_feedbacks_questions.yaml
+-rw-r--r--   0        0        0   119801 2024-04-09 11:41:20.603974 wildberries_api_client-0.1.9/wildberries_api_client/_swagger_doc/swagger_marketplace.yaml
+-rw-r--r--   0        0        0    51073 2024-04-09 11:41:24.607995 wildberries_api_client-0.1.9/wildberries_api_client/_swagger_doc/swagger_prices.yaml
+-rw-r--r--   0        0        0   197419 2024-04-09 11:41:18.599964 wildberries_api_client-0.1.9/wildberries_api_client/_swagger_doc/swagger_promotion.yaml
+-rw-r--r--   0        0        0    10791 2024-04-09 11:41:16.591953 wildberries_api_client-0.1.9/wildberries_api_client/_swagger_doc/swagger_recommendations.yaml
+-rw-r--r--   0        0        0    52604 2024-04-09 11:41:30.624026 wildberries_api_client-0.1.9/wildberries_api_client/_swagger_doc/swagger_statistics.yaml
+-rw-r--r--   0        0        0    12940 2024-04-09 11:41:28.616016 wildberries_api_client-0.1.9/wildberries_api_client/_swagger_doc/swagger_tariffs.yaml
+-rw-r--r--   0        0        0     1178 2024-04-09 11:39:23.887372 wildberries_api_client-0.1.9/wildberries_api_client/_swagger_doc/transliterate_script.py
+-rw-r--r--   0        0        0     9476 2024-04-09 11:42:25.112307 wildberries_api_client-0.1.9/wildberries_api_client/analytics/__init__.py
+-rw-r--r--   0        0        0      562 2024-04-09 11:42:25.116307 wildberries_api_client-0.1.9/wildberries_api_client/analytics/api/__init__.py
+-rw-r--r--   0        0        0    17124 2024-04-09 11:42:24.960307 wildberries_api_client-0.1.9/wildberries_api_client/analytics/api/othety_pouderhaniam_api.py
+-rw-r--r--   0        0        0     6117 2024-04-09 11:42:24.992307 wildberries_api_client-0.1.9/wildberries_api_client/analytics/api/platnaa_priemka_api.py
+-rw-r--r--   0        0        0    14564 2024-04-09 11:42:25.020307 wildberries_api_client-0.1.9/wildberries_api_client/analytics/api/platnoe_hranenie_api.py
+-rw-r--r--   0        0        0     7077 2024-04-09 11:42:25.048307 wildberries_api_client-0.1.9/wildberries_api_client/analytics/api/tovary_s_obazatelnoi_markirovkoi_api.py
+-rw-r--r--   0        0        0    19640 2024-04-09 11:42:25.076307 wildberries_api_client-0.1.9/wildberries_api_client/analytics/api/voronka_prodah_api.py
+-rw-r--r--   0        0        0    25741 2024-04-09 11:42:25.156308 wildberries_api_client-0.1.9/wildberries_api_client/analytics/api_client.py
+-rw-r--r--   0        0        0     8849 2024-04-09 11:42:25.108307 wildberries_api_client-0.1.9/wildberries_api_client/analytics/configuration.py
+-rw-r--r--   0        0        0     8813 2024-04-09 11:42:25.116307 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/__init__.py
+-rw-r--r--   0        0        0     3721 2024-04-09 11:42:23.520299 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/create_task_response.py
+-rw-r--r--   0        0        0     3847 2024-04-09 11:42:23.608300 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/create_task_response_data.py
+-rw-r--r--   0        0        0     4443 2024-04-09 11:42:23.680300 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/error_internal_response.py
+-rw-r--r--   0        0        0     3767 2024-04-09 11:42:23.732300 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/error_response.py
+-rw-r--r--   0        0        0     4465 2024-04-09 11:42:23.772300 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/excise_report_request.py
+-rw-r--r--   0        0        0     3829 2024-04-09 11:42:23.816301 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/excise_report_response.py
+-rw-r--r--   0        0        0     3699 2024-04-09 11:42:23.852301 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/get_tasks_response.py
+-rw-r--r--   0        0        0     4725 2024-04-09 11:42:23.888301 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/get_tasks_response_data.py
+-rw-r--r--   0        0        0     3774 2024-04-09 11:42:23.924301 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/inline_response200.py
+-rw-r--r--   0        0        0     3808 2024-04-09 11:42:23.952301 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/inline_response2001.py
+-rw-r--r--   0        0        0     6885 2024-04-09 11:42:23.972301 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/inline_response2001_details.py
+-rw-r--r--   0        0        0     3785 2024-04-09 11:42:23.992302 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/inline_response2002.py
+-rw-r--r--   0        0        0     7598 2024-04-09 11:42:24.020302 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/inline_response2002_report.py
+-rw-r--r--   0        0        0     3785 2024-04-09 11:42:24.040302 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/inline_response2003.py
+-rw-r--r--   0        0        0    14955 2024-04-09 11:42:24.056302 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/inline_response2003_report.py
+-rw-r--r--   0        0        0     8737 2024-04-09 11:42:24.076302 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/inline_response200_report.py
+-rw-r--r--   0        0        0     3714 2024-04-09 11:42:24.092302 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/inline_response400.py
+-rw-r--r--   0        0        0     3809 2024-04-09 11:42:24.112302 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/models_excise_report_response.py
+-rw-r--r--   0        0        0     3113 2024-04-09 11:42:24.128302 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/models_excise_report_response_data.py
+-rw-r--r--   0        0        0    13833 2024-04-09 11:42:24.144302 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/models_excise_report_response_data_inner.py
+-rw-r--r--   0        0        0     7018 2024-04-09 11:42:24.160302 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_history_request.py
+-rw-r--r--   0        0        0     4609 2024-04-09 11:42:24.176303 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_history_request_period.py
+-rw-r--r--   0        0        0     6522 2024-04-09 11:42:24.192303 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_history_response.py
+-rw-r--r--   0        0        0     6401 2024-04-09 11:42:24.208303 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_history_response_data.py
+-rw-r--r--   0        0        0    13438 2024-04-09 11:42:24.224303 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_history_response_history.py
+-rw-r--r--   0        0        0     9560 2024-04-09 11:42:24.240303 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_request.py
+-rw-r--r--   0        0        0     4655 2024-04-09 11:42:24.256303 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_request_order_by.py
+-rw-r--r--   0        0        0     4519 2024-04-09 11:42:24.272303 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_request_period.py
+-rw-r--r--   0        0        0     6343 2024-04-09 11:42:24.288303 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_response.py
+-rw-r--r--   0        0        0     5487 2024-04-09 11:42:24.304303 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_response_data.py
+-rw-r--r--   0        0        0     8807 2024-04-09 11:42:24.320303 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_response_data_cards.py
+-rw-r--r--   0        0        0     4563 2024-04-09 11:42:24.336303 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_response_data_object.py
+-rw-r--r--   0        0        0     6280 2024-04-09 11:42:24.352303 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_response_data_statistics.py
+-rw-r--r--   0        0        0    16504 2024-04-09 11:42:24.368303 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_response_data_statistics_period_comparison.py
+-rw-r--r--   0        0        0     7233 2024-04-09 11:42:24.384303 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_response_data_statistics_period_comparison_conversions.py
+-rw-r--r--   0        0        0    16256 2024-04-09 11:42:24.400304 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_response_data_statistics_previous_period.py
+-rw-r--r--   0        0        0     7201 2024-04-09 11:42:24.416304 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_response_data_statistics_previous_period_conversions.py
+-rw-r--r--   0        0        0    16244 2024-04-09 11:42:24.432304 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_response_data_statistics_selected_period.py
+-rw-r--r--   0        0        0     7201 2024-04-09 11:42:24.448304 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_response_data_statistics_selected_period_conversions.py
+-rw-r--r--   0        0        0     5009 2024-04-09 11:42:24.464304 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_response_data_stocks.py
+-rw-r--r--   0        0        0     4523 2024-04-09 11:42:24.476304 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_response_data_tags.py
+-rw-r--r--   0        0        0     8716 2024-04-09 11:42:24.496304 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_history_request.py
+-rw-r--r--   0        0        0     4621 2024-04-09 11:42:24.512304 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_history_request_period.py
+-rw-r--r--   0        0        0     6545 2024-04-09 11:42:24.528304 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_history_response.py
+-rw-r--r--   0        0        0     6371 2024-04-09 11:42:24.544304 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_history_response_data.py
+-rw-r--r--   0        0        0    13422 2024-04-09 11:42:24.564304 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_history_response_history.py
+-rw-r--r--   0        0        0     4611 2024-04-09 11:42:24.588305 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_history_response_object.py
+-rw-r--r--   0        0        0     4559 2024-04-09 11:42:24.608305 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_history_response_tag.py
+-rw-r--r--   0        0        0     8867 2024-04-09 11:42:24.624305 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_request.py
+-rw-r--r--   0        0        0     4635 2024-04-09 11:42:24.640305 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_request_order_by.py
+-rw-r--r--   0        0        0     4531 2024-04-09 11:42:24.656305 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_request_period.py
+-rw-r--r--   0        0        0     6366 2024-04-09 11:42:24.668305 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_response.py
+-rw-r--r--   0        0        0     5529 2024-04-09 11:42:24.684305 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_response_data.py
+-rw-r--r--   0        0        0     6413 2024-04-09 11:42:24.696305 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_response_data_groups.py
+-rw-r--r--   0        0        0     4575 2024-04-09 11:42:24.716305 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_response_data_object.py
+-rw-r--r--   0        0        0     6305 2024-04-09 11:42:24.728305 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_response_data_statistics.py
+-rw-r--r--   0        0        0    16557 2024-04-09 11:42:24.744305 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_response_data_statistics_period_comparison.py
+-rw-r--r--   0        0        0     7249 2024-04-09 11:42:24.760306 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_response_data_statistics_period_comparison_conversions.py
+-rw-r--r--   0        0        0    16305 2024-04-09 11:42:24.772306 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_response_data_statistics_previous_period.py
+-rw-r--r--   0        0        0     7235 2024-04-09 11:42:24.788306 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_response_data_statistics_previous_period_conversions.py
+-rw-r--r--   0        0        0    16278 2024-04-09 11:42:24.804306 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_response_data_statistics_selected_period.py
+-rw-r--r--   0        0        0     6121 2024-04-09 11:42:24.816306 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/response_error.py
+-rw-r--r--   0        0        0     4725 2024-04-09 11:42:24.832306 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/response_error_additional_errors.py
+-rw-r--r--   0        0        0     3069 2024-04-09 11:42:24.848306 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/response_paid_storage.py
+-rw-r--r--   0        0        0    19791 2024-04-09 11:42:24.864306 wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/response_paid_storage_inner.py
+-rw-r--r--   0        0        0    13621 2024-04-09 11:42:25.168308 wildberries_api_client-0.1.9/wildberries_api_client/analytics/rest.py
+-rw-r--r--   0        0        0    11511 2024-04-09 11:42:13.856249 wildberries_api_client-0.1.9/wildberries_api_client/content/__init__.py
+-rw-r--r--   0        0        0      521 2024-04-09 11:42:13.860249 wildberries_api_client-0.1.9/wildberries_api_client/content/api/__init__.py
+-rw-r--r--   0        0        0    37657 2024-04-09 11:42:13.556248 wildberries_api_client-0.1.9/wildberries_api_client/content/api/konfigurator_api.py
+-rw-r--r--   0        0        0    17179 2024-04-09 11:42:13.608248 wildberries_api_client-0.1.9/wildberries_api_client/content/api/korzina_api.py
+-rw-r--r--   0        0        0    25230 2024-04-09 11:42:13.660248 wildberries_api_client-0.1.9/wildberries_api_client/content/api/mediafaily_api.py
+-rw-r--r--   0        0        0    16680 2024-04-09 11:42:13.708248 wildberries_api_client-0.1.9/wildberries_api_client/content/api/prosmotr_api.py
+-rw-r--r--   0        0        0    20617 2024-04-09 11:42:13.756249 wildberries_api_client-0.1.9/wildberries_api_client/content/api/tegi_api.py
+-rw-r--r--   0        0        0    25314 2024-04-09 11:42:13.804249 wildberries_api_client-0.1.9/wildberries_api_client/content/api/zagruzka_api.py
+-rw-r--r--   0        0        0    25668 2024-04-09 11:42:13.908249 wildberries_api_client-0.1.9/wildberries_api_client/content/api_client.py
+-rw-r--r--   0        0        0     8782 2024-04-09 11:42:13.856249 wildberries_api_client-0.1.9/wildberries_api_client/content/configuration.py
+-rw-r--r--   0        0        0    10893 2024-04-09 11:42:13.860249 wildberries_api_client-0.1.9/wildberries_api_client/content/models/__init__.py
+-rw-r--r--   0        0        0     3717 2024-04-09 11:42:11.316236 wildberries_api_client-0.1.9/wildberries_api_client/content/models/cards_list_body.py
+-rw-r--r--   0        0        0     2988 2024-04-09 11:42:11.388236 wildberries_api_client-0.1.9/wildberries_api_client/content/models/cards_move_nm_body.py
+-rw-r--r--   0        0        0     3731 2024-04-09 11:42:11.444237 wildberries_api_client-0.1.9/wildberries_api_client/content/models/cards_recover_body.py
+-rw-r--r--   0        0        0     3728 2024-04-09 11:42:11.484237 wildberries_api_client-0.1.9/wildberries_api_client/content/models/cards_trash_body.py
+-rw-r--r--   0        0        0     9773 2024-04-09 11:42:11.540237 wildberries_api_client-0.1.9/wildberries_api_client/content/models/cards_update_body.py
+-rw-r--r--   0        0        0     4892 2024-04-09 11:42:11.584237 wildberries_api_client-0.1.9/wildberries_api_client/content/models/cards_upload_body.py
+-rw-r--r--   0        0        0     4657 2024-04-09 11:42:11.624238 wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2cardsupdate_characteristics.py
+-rw-r--r--   0        0        0     5265 2024-04-09 11:42:11.648238 wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2cardsupdate_dimensions.py
+-rw-r--r--   0        0        0     6395 2024-04-09 11:42:11.676238 wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2cardsupdate_sizes.py
+-rw-r--r--   0        0        0     4840 2024-04-09 11:42:11.704238 wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2cardsupload_characteristics.py
+-rw-r--r--   0        0        0     5265 2024-04-09 11:42:11.728238 wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2cardsupload_dimensions.py
+-rw-r--r--   0        0        0     6170 2024-04-09 11:42:11.752238 wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2cardsupload_sizes.py
+-rw-r--r--   0        0        0     9429 2024-04-09 11:42:11.780238 wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2cardsupload_variants.py
+-rw-r--r--   0        0        0     9603 2024-04-09 11:42:11.804239 wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2cardsuploadadd_cards_to_add.py
+-rw-r--r--   0        0        0     4691 2024-04-09 11:42:11.832239 wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2cardsuploadadd_characteristics.py
+-rw-r--r--   0        0        0     6120 2024-04-09 11:42:11.856239 wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2cardsuploadadd_sizes.py
+-rw-r--r--   0        0        0     5339 2024-04-09 11:42:11.880239 wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2getcardslist_settings.py
+-rw-r--r--   0        0        0     3851 2024-04-09 11:42:11.904239 wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2getcardslist_settings_cursor.py
+-rw-r--r--   0        0        0     9813 2024-04-09 11:42:11.928239 wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2getcardslist_settings_filter.py
+-rw-r--r--   0        0        0     4032 2024-04-09 11:42:11.960239 wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2getcardslist_settings_sort.py
+-rw-r--r--   0        0        0     5364 2024-04-09 11:42:11.988239 wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2getcardstrash_settings.py
+-rw-r--r--   0        0        0     3857 2024-04-09 11:42:12.012240 wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2getcardstrash_settings_cursor.py
+-rw-r--r--   0        0        0     4026 2024-04-09 11:42:12.040240 wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2getcardstrash_settings_filter.py
+-rw-r--r--   0        0        0     4024 2024-04-09 11:42:12.064240 wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2getcardstrash_settings_sort.py
+-rw-r--r--   0        0        0     3741 2024-04-09 11:42:12.092240 wildberries_api_client-0.1.9/wildberries_api_client/content/models/delete_trash_body.py
+-rw-r--r--   0        0        0     6137 2024-04-09 11:42:12.136240 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response200.py
+-rw-r--r--   0        0        0     4465 2024-04-09 11:42:12.172240 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2001.py
+-rw-r--r--   0        0        0     6181 2024-04-09 11:42:12.200241 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response20010.py
+-rw-r--r--   0        0        0     6199 2024-04-09 11:42:12.224241 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response20011.py
+-rw-r--r--   0        0        0     4524 2024-04-09 11:42:12.244241 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response20011_data.py
+-rw-r--r--   0        0        0     6081 2024-04-09 11:42:12.264241 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response20012.py
+-rw-r--r--   0        0        0     6062 2024-04-09 11:42:12.280241 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response20013.py
+-rw-r--r--   0        0        0     6113 2024-04-09 11:42:12.304241 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response20014.py
+-rw-r--r--   0        0        0     5087 2024-04-09 11:42:12.320241 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response20014_data.py
+-rw-r--r--   0        0        0     3004 2024-04-09 11:42:12.340241 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response20015.py
+-rw-r--r--   0        0        0     3004 2024-04-09 11:42:12.356241 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response20016.py
+-rw-r--r--   0        0        0     6071 2024-04-09 11:42:12.372242 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response20017.py
+-rw-r--r--   0        0        0     4511 2024-04-09 11:42:12.388242 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response20018.py
+-rw-r--r--   0        0        0    10453 2024-04-09 11:42:12.408242 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response20018_cards.py
+-rw-r--r--   0        0        0     5055 2024-04-09 11:42:12.424242 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response20018_characteristics.py
+-rw-r--r--   0        0        0     5071 2024-04-09 11:42:12.444242 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response20018_cursor.py
+-rw-r--r--   0        0        0     5077 2024-04-09 11:42:12.464242 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response20018_dimensions.py
+-rw-r--r--   0        0        0     6065 2024-04-09 11:42:12.480242 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response20018_sizes.py
+-rw-r--r--   0        0        0    15931 2024-04-09 11:42:12.496242 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2001_cards.py
+-rw-r--r--   0        0        0     5406 2024-04-09 11:42:12.512242 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2001_characteristics.py
+-rw-r--r--   0        0        0     5463 2024-04-09 11:42:12.532242 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2001_cursor.py
+-rw-r--r--   0        0        0     5233 2024-04-09 11:42:12.548242 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2001_dimensions.py
+-rw-r--r--   0        0        0     5236 2024-04-09 11:42:12.564242 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2001_photos.py
+-rw-r--r--   0        0        0     6167 2024-04-09 11:42:12.584243 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2001_sizes.py
+-rw-r--r--   0        0        0     5623 2024-04-09 11:42:12.600243 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2001_tags.py
+-rw-r--r--   0        0        0     6114 2024-04-09 11:42:12.616243 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2002.py
+-rw-r--r--   0        0        0     7180 2024-04-09 11:42:12.632243 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2002_data.py
+-rw-r--r--   0        0        0     6090 2024-04-09 11:42:12.648243 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2003.py
+-rw-r--r--   0        0        0     4734 2024-04-09 11:42:12.660243 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2003_data.py
+-rw-r--r--   0        0        0     6124 2024-04-09 11:42:12.676243 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2004.py
+-rw-r--r--   0        0        0     5219 2024-04-09 11:42:12.692243 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2004_data.py
+-rw-r--r--   0        0        0     6210 2024-04-09 11:42:12.708243 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2005.py
+-rw-r--r--   0        0        0     7209 2024-04-09 11:42:12.760244 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2005_data.py
+-rw-r--r--   0        0        0     6176 2024-04-09 11:42:12.784244 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2006.py
+-rw-r--r--   0        0        0    10713 2024-04-09 11:42:12.808244 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2006_data.py
+-rw-r--r--   0        0        0     6108 2024-04-09 11:42:12.828244 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2007.py
+-rw-r--r--   0        0        0     4577 2024-04-09 11:42:12.844244 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2007_data.py
+-rw-r--r--   0        0        0     6157 2024-04-09 11:42:12.860244 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2008.py
+-rw-r--r--   0        0        0     6108 2024-04-09 11:42:12.876244 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2009.py
+-rw-r--r--   0        0        0     4543 2024-04-09 11:42:12.888244 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2009_data.py
+-rw-r--r--   0        0        0     2996 2024-04-09 11:42:12.904244 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response400.py
+-rw-r--r--   0        0        0     3000 2024-04-09 11:42:12.920244 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response4001.py
+-rw-r--r--   0        0        0     3000 2024-04-09 11:42:12.940245 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response4002.py
+-rw-r--r--   0        0        0     3000 2024-04-09 11:42:12.952244 wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response4003.py
+-rw-r--r--   0        0        0     3679 2024-04-09 11:42:12.968245 wildberries_api_client-0.1.9/wildberries_api_client/content/models/media_file_body.py
+-rw-r--r--   0        0        0     3687 2024-04-09 11:42:12.980245 wildberries_api_client-0.1.9/wildberries_api_client/content/models/media_file_body1.py
+-rw-r--r--   0        0        0     4459 2024-04-09 11:42:12.996245 wildberries_api_client-0.1.9/wildberries_api_client/content/models/media_save_body.py
+-rw-r--r--   0        0        0     4601 2024-04-09 11:42:13.012245 wildberries_api_client-0.1.9/wildberries_api_client/content/models/media_save_body1.py
+-rw-r--r--   0        0        0     4905 2024-04-09 11:42:13.024245 wildberries_api_client-0.1.9/wildberries_api_client/content/models/nomenclature_link_body.py
+-rw-r--r--   0        0        0     3008 2024-04-09 11:42:13.040245 wildberries_api_client-0.1.9/wildberries_api_client/content/models/one_ofcards_move_nm_body.py
+-rw-r--r--   0        0        0     3024 2024-04-09 11:42:13.052245 wildberries_api_client-0.1.9/wildberries_api_client/content/models/one_ofinline_response20015.py
+-rw-r--r--   0        0        0     3024 2024-04-09 11:42:13.068245 wildberries_api_client-0.1.9/wildberries_api_client/content/models/one_ofinline_response20016.py
+-rw-r--r--   0        0        0     3016 2024-04-09 11:42:13.080245 wildberries_api_client-0.1.9/wildberries_api_client/content/models/one_ofinline_response400.py
+-rw-r--r--   0        0        0     3020 2024-04-09 11:42:13.100245 wildberries_api_client-0.1.9/wildberries_api_client/content/models/one_ofinline_response4001.py
+-rw-r--r--   0        0        0     3020 2024-04-09 11:42:13.116245 wildberries_api_client-0.1.9/wildberries_api_client/content/models/one_ofinline_response4002.py
+-rw-r--r--   0        0        0     3020 2024-04-09 11:42:13.128245 wildberries_api_client-0.1.9/wildberries_api_client/content/models/one_ofinline_response4003.py
+-rw-r--r--   0        0        0     3084 2024-04-09 11:42:13.144245 wildberries_api_client-0.1.9/wildberries_api_client/content/models/one_ofresponse_card_create_additional_errors.py
+-rw-r--r--   0        0        0     4932 2024-04-09 11:42:13.156246 wildberries_api_client-0.1.9/wildberries_api_client/content/models/request_move_nms_imt_conn.py
+-rw-r--r--   0        0        0     3945 2024-04-09 11:42:13.172246 wildberries_api_client-0.1.9/wildberries_api_client/content/models/request_move_nms_imt_disconn.py
+-rw-r--r--   0        0        0     6256 2024-04-09 11:42:13.184246 wildberries_api_client-0.1.9/wildberries_api_client/content/models/response_body_content_error400.py
+-rw-r--r--   0        0        0     4056 2024-04-09 11:42:13.200246 wildberries_api_client-0.1.9/wildberries_api_client/content/models/response_body_content_error400_additional_errors.py
+-rw-r--r--   0        0        0     6222 2024-04-09 11:42:13.216246 wildberries_api_client-0.1.9/wildberries_api_client/content/models/response_body_content_error403.py
+-rw-r--r--   0        0        0     6150 2024-04-09 11:42:13.228246 wildberries_api_client-0.1.9/wildberries_api_client/content/models/response_card_create.py
+-rw-r--r--   0        0        0     6118 2024-04-09 11:42:13.244246 wildberries_api_client-0.1.9/wildberries_api_client/content/models/response_content_error1.py
+-rw-r--r--   0        0        0     3771 2024-04-09 11:42:13.264246 wildberries_api_client-0.1.9/wildberries_api_client/content/models/response_content_error1_additional_errors.py
+-rw-r--r--   0        0        0     6118 2024-04-09 11:42:13.280246 wildberries_api_client-0.1.9/wildberries_api_client/content/models/response_content_error4.py
+-rw-r--r--   0        0        0     3891 2024-04-09 11:42:13.292246 wildberries_api_client-0.1.9/wildberries_api_client/content/models/response_content_error4_additional_errors.py
+-rw-r--r--   0        0        0     6118 2024-04-09 11:42:13.308246 wildberries_api_client-0.1.9/wildberries_api_client/content/models/response_content_error5.py
+-rw-r--r--   0        0        0     3790 2024-04-09 11:42:13.324247 wildberries_api_client-0.1.9/wildberries_api_client/content/models/response_content_error5_additional_errors.py
+-rw-r--r--   0        0        0     6102 2024-04-09 11:42:13.336246 wildberries_api_client-0.1.9/wildberries_api_client/content/models/response_content_error6.py
+-rw-r--r--   0        0        0     3643 2024-04-09 11:42:13.352247 wildberries_api_client-0.1.9/wildberries_api_client/content/models/response_incorrect_date.py
+-rw-r--r--   0        0        0     4238 2024-04-09 11:42:13.368247 wildberries_api_client-0.1.9/wildberries_api_client/content/models/tag_id_body.py
+-rw-r--r--   0        0        0     4653 2024-04-09 11:42:13.380247 wildberries_api_client-0.1.9/wildberries_api_client/content/models/upload_add_body.py
+-rw-r--r--   0        0        0     3849 2024-04-09 11:42:13.396247 wildberries_api_client-0.1.9/wildberries_api_client/content/models/v2_barcodes_body.py
+-rw-r--r--   0        0        0     4782 2024-04-09 11:42:13.416247 wildberries_api_client-0.1.9/wildberries_api_client/content/models/v2_tag_body.py
+-rw-r--r--   0        0        0    13556 2024-04-09 11:42:13.924250 wildberries_api_client-0.1.9/wildberries_api_client/content/rest.py
+-rw-r--r--   0        0        0     8626 2024-04-09 11:42:29.552330 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/__init__.py
+-rw-r--r--   0        0        0      373 2024-04-09 11:42:29.556330 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/api/__init__.py
+-rw-r--r--   0        0        0    15796 2024-04-09 11:42:29.516330 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/api/hablony_dla_voprosov_i_otzyvov_api.py
+-rw-r--r--   0        0        0    55850 2024-04-09 11:42:29.432330 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/api/otzyvy_api.py
+-rw-r--r--   0        0        0    34196 2024-04-09 11:42:29.480330 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/api/voprosy_api.py
+-rw-r--r--   0        0        0    25259 2024-04-09 11:42:29.596331 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/api_client.py
+-rw-r--r--   0        0        0     8337 2024-04-09 11:42:29.552330 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/configuration.py
+-rw-r--r--   0        0        0     8132 2024-04-09 11:42:29.556330 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/__init__.py
+-rw-r--r--   0        0        0     3311 2024-04-09 11:42:27.936322 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/apiv1questions_answer.py
+-rw-r--r--   0        0        0     5632 2024-04-09 11:42:27.992322 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response200.py
+-rw-r--r--   0        0        0     5655 2024-04-09 11:42:28.036322 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2001.py
+-rw-r--r--   0        0        0     5696 2024-04-09 11:42:28.084323 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20010.py
+-rw-r--r--   0        0        0     4348 2024-04-09 11:42:28.124323 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20010_data.py
+-rw-r--r--   0        0        0     5696 2024-04-09 11:42:28.152323 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20011.py
+-rw-r--r--   0        0        0     4419 2024-04-09 11:42:28.176323 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20011_data.py
+-rw-r--r--   0        0        0     5678 2024-04-09 11:42:28.196323 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20012.py
+-rw-r--r--   0        0        0     5201 2024-04-09 11:42:28.216323 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20012_data.py
+-rw-r--r--   0        0        0     5678 2024-04-09 11:42:28.252323 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20013.py
+-rw-r--r--   0        0        0     4606 2024-04-09 11:42:28.280324 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20013_data.py
+-rw-r--r--   0        0        0     7197 2024-04-09 11:42:28.300324 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20013_data_feedback_valuations.py
+-rw-r--r--   0        0        0     5221 2024-04-09 11:42:28.320324 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20013_data_product_valuations.py
+-rw-r--r--   0        0        0     5678 2024-04-09 11:42:28.340324 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20014.py
+-rw-r--r--   0        0        0     4870 2024-04-09 11:42:28.364324 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20014_data.py
+-rw-r--r--   0        0        0     5678 2024-04-09 11:42:28.384324 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20015.py
+-rw-r--r--   0        0        0     3321 2024-04-09 11:42:28.404324 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20015_data.py
+-rw-r--r--   0        0        0     5678 2024-04-09 11:42:28.420324 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20016.py
+-rw-r--r--   0        0        0     4324 2024-04-09 11:42:28.436324 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20016_data.py
+-rw-r--r--   0        0        0     5700 2024-04-09 11:42:28.456325 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20017.py
+-rw-r--r--   0        0        0     5678 2024-04-09 11:42:28.476325 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20018.py
+-rw-r--r--   0        0        0    21542 2024-05-20 07:36:28.331383 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20018_data.py
+-rw-r--r--   0        0        0     4353 2024-04-09 11:42:28.520325 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20018_data_answer.py
+-rw-r--r--   0        0        0     4345 2024-04-09 11:42:28.536325 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20018_data_photo_links.py
+-rw-r--r--   0        0        0     8682 2024-04-09 11:42:28.556325 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20018_data_product_details.py
+-rw-r--r--   0        0        0     5197 2024-04-09 11:42:28.572325 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20018_data_video.py
+-rw-r--r--   0        0        0     2547 2024-04-09 11:42:28.592325 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20019.py
+-rw-r--r--   0        0        0     4627 2024-04-09 11:42:28.608325 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2001_data.py
+-rw-r--r--   0        0        0     5655 2024-04-09 11:42:28.624325 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2002.py
+-rw-r--r--   0        0        0     2547 2024-04-09 11:42:28.644326 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20020.py
+-rw-r--r--   0        0        0     2547 2024-04-09 11:42:28.660326 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20021.py
+-rw-r--r--   0        0        0     3445 2024-04-09 11:42:28.676326 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2002_data.py
+-rw-r--r--   0        0        0     6789 2024-04-09 11:42:28.692326 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2002_data_products.py
+-rw-r--r--   0        0        0     5655 2024-04-09 11:42:28.708326 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2003.py
+-rw-r--r--   0        0        0     5346 2024-04-09 11:42:28.724326 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2003_data.py
+-rw-r--r--   0        0        0     5085 2024-04-09 11:42:28.740326 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2003_data_answer.py
+-rw-r--r--   0        0        0     7875 2024-04-09 11:42:28.764326 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2003_data_product_details.py
+-rw-r--r--   0        0        0     8745 2024-04-09 11:42:28.788326 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2003_data_questions.py
+-rw-r--r--   0        0        0     5607 2024-04-09 11:42:28.808326 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2004.py
+-rw-r--r--   0        0        0     5655 2024-04-09 11:42:28.824326 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2005.py
+-rw-r--r--   0        0        0     4854 2024-04-09 11:42:28.836326 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2005_data.py
+-rw-r--r--   0        0        0     5682 2024-04-09 11:42:28.852327 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2006.py
+-rw-r--r--   0        0        0     5655 2024-04-09 11:42:28.868327 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2007.py
+-rw-r--r--   0        0        0     8463 2024-04-09 11:42:28.884327 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2007_data.py
+-rw-r--r--   0        0        0     5655 2024-04-09 11:42:28.904327 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2008.py
+-rw-r--r--   0        0        0     5451 2024-04-09 11:42:28.916327 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2008_data.py
+-rw-r--r--   0        0        0     5673 2024-04-09 11:42:28.932327 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2009.py
+-rw-r--r--   0        0        0     4249 2024-04-09 11:42:28.948327 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2009_data.py
+-rw-r--r--   0        0        0     4618 2024-04-09 11:42:28.960327 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response200_data.py
+-rw-r--r--   0        0        0     2567 2024-04-09 11:42:28.976327 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/one_ofinline_response20019.py
+-rw-r--r--   0        0        0     2567 2024-04-09 11:42:28.992327 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/one_ofinline_response20020.py
+-rw-r--r--   0        0        0     2567 2024-04-09 11:42:29.004327 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/one_ofinline_response20021.py
+-rw-r--r--   0        0        0     2551 2024-04-09 11:42:29.020327 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/one_ofv1_feedbacks_body.py
+-rw-r--r--   0        0        0     2551 2024-04-09 11:42:29.040328 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/one_ofv1_questions_body.py
+-rw-r--r--   0        0        0     3343 2024-04-09 11:42:29.052328 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/order_return_body.py
+-rw-r--r--   0        0        0     5521 2024-04-09 11:42:29.068328 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/patch_del_resp_ok.py
+-rw-r--r--   0        0        0     5563 2024-04-09 11:42:29.080328 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/post_template_ok.py
+-rw-r--r--   0        0        0     3190 2024-04-09 11:42:29.096328 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/post_template_ok_data.py
+-rw-r--r--   0        0        0     8888 2024-04-09 11:42:29.108328 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/product_rating.py
+-rw-r--r--   0        0        0     5485 2024-04-09 11:42:29.124328 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/response200.py
+-rw-r--r--   0        0        0     3299 2024-04-09 11:42:29.140328 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/response200_data.py
+-rw-r--r--   0        0        0     4638 2024-04-09 11:42:29.156328 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/response200_data_templates.py
+-rw-r--r--   0        0        0     5667 2024-04-09 11:42:29.172328 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/response_error_template.py
+-rw-r--r--   0        0        0     2535 2024-04-09 11:42:29.184328 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/response_feadback.py
+-rw-r--r--   0        0        0    21349 2024-04-09 11:42:29.200328 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/response_feadback_inner.py
+-rw-r--r--   0        0        0     6351 2024-04-09 11:42:29.216328 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/responsefeedback_err.py
+-rw-r--r--   0        0        0     2531 2024-04-09 11:42:29.228329 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/v1_feedbacks_body.py
+-rw-r--r--   0        0        0     2531 2024-04-09 11:42:29.244329 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/v1_questions_body.py
+-rw-r--r--   0        0        0     5169 2024-04-09 11:42:29.256329 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/v1_templates_body.py
+-rw-r--r--   0        0        0     3461 2024-04-09 11:42:29.276329 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/v1_templates_body1.py
+-rw-r--r--   0        0        0     5039 2024-04-09 11:42:29.300329 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/v1_templates_body2.py
+-rw-r--r--   0        0        0    13099 2024-04-09 11:42:29.608331 wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/rest.py
+-rw-r--r--   0        0        0     6029 2024-04-09 11:42:19.532278 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/__init__.py
+-rw-r--r--   0        0        0      478 2024-04-09 11:42:19.536279 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/api/__init__.py
+-rw-r--r--   0        0        0    14672 2024-04-09 11:42:19.364278 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/api/ostatki_api.py
+-rw-r--r--   0        0        0    65043 2024-04-09 11:42:19.404278 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/api/postavki_api.py
+-rw-r--r--   0        0        0    19880 2024-04-09 11:42:19.436278 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/api/propuska_api.py
+-rw-r--r--   0        0        0    62159 2024-04-09 11:42:19.464278 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/api/sborohnye_zadania_api.py
+-rw-r--r--   0        0        0    19721 2024-04-09 11:42:19.496278 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/api/sklady_api.py
+-rw-r--r--   0        0        0    25162 2024-04-09 11:42:19.584279 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/api_client.py
+-rw-r--r--   0        0        0     8264 2024-04-09 11:42:19.528278 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/configuration.py
+-rw-r--r--   0        0        0     5446 2024-04-09 11:42:19.532278 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/__init__.py
+-rw-r--r--   0        0        0     3936 2024-04-09 11:42:17.968270 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/apiv3stockswarehouse_id_stocks.py
+-rw-r--r--   0        0        0     4408 2024-04-09 11:42:18.024271 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/error.py
+-rw-r--r--   0        0        0     3248 2024-04-09 11:42:18.064271 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response200.py
+-rw-r--r--   0        0        0     3745 2024-04-09 11:42:18.096271 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response2001.py
+-rw-r--r--   0        0        0     3164 2024-04-09 11:42:18.128271 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response20010.py
+-rw-r--r--   0        0        0     3210 2024-04-09 11:42:18.160272 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response20011.py
+-rw-r--r--   0        0        0     3209 2024-04-09 11:42:18.192272 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response20012.py
+-rw-r--r--   0        0        0     3900 2024-04-09 11:42:18.220272 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response20012_stocks.py
+-rw-r--r--   0        0        0     3198 2024-04-09 11:42:18.256272 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response2002.py
+-rw-r--r--   0        0        0     5728 2024-04-09 11:42:18.292272 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response2002_orders.py
+-rw-r--r--   0        0        0     3272 2024-04-09 11:42:18.324272 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response2003.py
+-rw-r--r--   0        0        0     4146 2024-04-09 11:42:18.348272 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response2003_orders.py
+-rw-r--r--   0        0        0     3244 2024-04-09 11:42:18.372273 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response2004.py
+-rw-r--r--   0        0        0     6566 2024-04-09 11:42:18.392273 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response2004_stickers.py
+-rw-r--r--   0        0        0     3080 2024-04-09 11:42:18.420273 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response2005.py
+-rw-r--r--   0        0        0     3244 2024-04-09 11:42:18.440273 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response2006.py
+-rw-r--r--   0        0        0     4117 2024-04-09 11:42:18.464273 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response2006_stickers.py
+-rw-r--r--   0        0        0     3864 2024-04-09 11:42:18.480273 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response2007.py
+-rw-r--r--   0        0        0     3159 2024-04-09 11:42:18.500273 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response2008.py
+-rw-r--r--   0        0        0     4080 2024-04-09 11:42:18.520273 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response2009.py
+-rw-r--r--   0        0        0     3119 2024-04-09 11:42:18.540273 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response201.py
+-rw-r--r--   0        0        0     3300 2024-04-09 11:42:18.560274 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response2011.py
+-rw-r--r--   0        0        0     3119 2024-04-09 11:42:18.576274 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response2012.py
+-rw-r--r--   0        0        0     3123 2024-04-09 11:42:18.596274 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response2013.py
+-rw-r--r--   0        0        0     4868 2024-04-09 11:42:18.620274 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/meta.py
+-rw-r--r--   0        0        0     3166 2024-04-09 11:42:18.640274 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/meta_gtin_body.py
+-rw-r--r--   0        0        0     3166 2024-04-09 11:42:18.664274 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/meta_imei_body.py
+-rw-r--r--   0        0        0     3289 2024-04-09 11:42:18.688274 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/meta_sgtin_body.py
+-rw-r--r--   0        0        0     3135 2024-04-09 11:42:18.704274 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/meta_uin_body.py
+-rw-r--r--   0        0        0     9113 2024-04-09 11:42:18.724274 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/model_pass.py
+-rw-r--r--   0        0        0     2422 2024-04-09 11:42:18.744274 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/next.py
+-rw-r--r--   0        0        0     9869 2024-04-09 11:42:18.764274 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/office.py
+-rw-r--r--   0        0        0    18457 2024-04-09 11:42:18.784275 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/order.py
+-rw-r--r--   0        0        0     9435 2024-04-09 11:42:18.808275 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/order_address.py
+-rw-r--r--   0        0        0    19005 2024-04-09 11:42:18.832275 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/order_new.py
+-rw-r--r--   0        0        0     3696 2024-04-09 11:42:18.856275 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/order_user.py
+-rw-r--r--   0        0        0     3325 2024-04-09 11:42:18.876275 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/orders_externalstickers_body.py
+-rw-r--r--   0        0        0     3330 2024-04-09 11:42:18.892275 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/orders_status_body.py
+-rw-r--r--   0        0        0     3261 2024-04-09 11:42:18.908275 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/orders_stickers_body.py
+-rw-r--r--   0        0        0     4339 2024-04-09 11:42:18.924275 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/pass_office.py
+-rw-r--r--   0        0        0     6762 2024-04-09 11:42:18.940276 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/passes_pass_id_body.py
+-rw-r--r--   0        0        0     3439 2024-04-09 11:42:18.956276 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/stocks_warehouse_id_body.py
+-rw-r--r--   0        0        0     3203 2024-04-09 11:42:18.976276 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/stocks_warehouse_id_body1.py
+-rw-r--r--   0        0        0     3203 2024-04-09 11:42:18.992276 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/stocks_warehouse_id_body2.py
+-rw-r--r--   0        0        0     8073 2024-04-09 11:42:19.008276 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/supply.py
+-rw-r--r--   0        0        0     3348 2024-04-09 11:42:19.024276 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/supply_id_trbx_body.py
+-rw-r--r--   0        0        0     3389 2024-04-09 11:42:19.040276 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/supply_id_trbx_body1.py
+-rw-r--r--   0        0        0    16008 2024-04-09 11:42:19.056276 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/supply_order.py
+-rw-r--r--   0        0        0     3772 2024-04-09 11:42:19.072276 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/supply_trbx.py
+-rw-r--r--   0        0        0     3960 2024-04-09 11:42:19.088276 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/trbx_stickers.py
+-rw-r--r--   0        0        0     3403 2024-04-09 11:42:19.108276 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/trbx_stickers_body.py
+-rw-r--r--   0        0        0     3398 2024-04-09 11:42:19.124276 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/trbx_trbx_id_body.py
+-rw-r--r--   0        0        0     6666 2024-04-09 11:42:19.140277 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/v3_passes_body.py
+-rw-r--r--   0        0        0     3133 2024-04-09 11:42:19.156277 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/v3_supplies_body.py
+-rw-r--r--   0        0        0     4078 2024-04-09 11:42:19.172277 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/v3_warehouses_body.py
+-rw-r--r--   0        0        0     7263 2024-04-09 11:42:19.192277 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/warehouse.py
+-rw-r--r--   0        0        0     4208 2024-04-09 11:42:19.216277 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/warehouses_warehouse_id_body.py
+-rw-r--r--   0        0        0    13034 2024-04-09 11:42:19.604279 wildberries_api_client-0.1.9/wildberries_api_client/marketplace/rest.py
+-rw-r--r--   0        0        0     4686 2024-04-09 11:42:16.632264 wildberries_api_client-0.1.9/wildberries_api_client/prices/__init__.py
+-rw-r--r--   0        0        0      507 2024-04-09 11:42:16.636263 wildberries_api_client-0.1.9/wildberries_api_client/prices/api/__init__.py
+-rw-r--r--   0        0        0     8081 2024-04-09 11:42:16.596263 wildberries_api_client-0.1.9/wildberries_api_client/prices/api/ceny_api.py
+-rw-r--r--   0        0        0    18723 2024-04-09 11:42:16.492263 wildberries_api_client-0.1.9/wildberries_api_client/prices/api/promokody_i_skidki_api.py
+-rw-r--r--   0        0        0    18101 2024-04-09 11:42:16.528263 wildberries_api_client-0.1.9/wildberries_api_client/prices/api/sostoania_zagruzok_api.py
+-rw-r--r--   0        0        0    10585 2024-04-09 11:42:16.552263 wildberries_api_client-0.1.9/wildberries_api_client/prices/api/spiski_tovarov_api.py
+-rw-r--r--   0        0        0     9042 2024-04-09 11:42:16.576263 wildberries_api_client-0.1.9/wildberries_api_client/prices/api/ustanovka_cen_i_skidok_api.py
+-rw-r--r--   0        0        0    25157 2024-04-09 11:42:16.680264 wildberries_api_client-0.1.9/wildberries_api_client/prices/api_client.py
+-rw-r--r--   0        0        0     8274 2024-04-09 11:42:16.628264 wildberries_api_client-0.1.9/wildberries_api_client/prices/configuration.py
+-rw-r--r--   0        0        0     4084 2024-04-09 11:42:16.636263 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/__init__.py
+-rw-r--r--   0        0        0     2441 2024-04-09 11:42:15.080255 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/date1.py
+-rw-r--r--   0        0        0     4819 2024-04-09 11:42:15.132256 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/good.py
+-rw-r--r--   0        0        0     9567 2024-04-09 11:42:15.192256 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/good_buffer_history.py
+-rw-r--r--   0        0        0    10043 2024-04-09 11:42:15.240256 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/good_history.py
+-rw-r--r--   0        0        0     2461 2024-04-09 11:42:15.284257 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/good_status.py
+-rw-r--r--   0        0        0     2485 2024-04-09 11:42:15.332257 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/good_status_buffer.py
+-rw-r--r--   0        0        0     2441 2024-04-09 11:42:15.372257 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/goods.py
+-rw-r--r--   0        0        0     7505 2024-04-09 11:42:15.412257 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/goods_list.py
+-rw-r--r--   0        0        0     5681 2024-04-09 11:42:15.448257 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/goods_list_sizes.py
+-rw-r--r--   0        0        0     5343 2024-04-09 11:42:15.500258 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response200.py
+-rw-r--r--   0        0        0     3149 2024-04-09 11:42:15.544258 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response2001.py
+-rw-r--r--   0        0        0     4237 2024-04-09 11:42:15.580258 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response2001_data.py
+-rw-r--r--   0        0        0     4643 2024-04-09 11:42:15.612258 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response2002.py
+-rw-r--r--   0        0        0     4631 2024-04-09 11:42:15.648258 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response2003.py
+-rw-r--r--   0        0        0     4235 2024-04-09 11:42:15.688259 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response2003_data.py
+-rw-r--r--   0        0        0     3149 2024-04-09 11:42:15.720259 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response2004.py
+-rw-r--r--   0        0        0     3365 2024-04-09 11:42:15.752259 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response2004_data.py
+-rw-r--r--   0        0        0     4631 2024-04-09 11:42:15.784259 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response2005.py
+-rw-r--r--   0        0        0     3350 2024-04-09 11:42:15.816259 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response2005_data.py
+-rw-r--r--   0        0        0     2493 2024-04-09 11:42:15.856259 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response2006.py
+-rw-r--r--   0        0        0     5385 2024-04-09 11:42:15.888260 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response2007.py
+-rw-r--r--   0        0        0     3297 2024-04-09 11:42:15.920260 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response2008.py
+-rw-r--r--   0        0        0     4429 2024-04-09 11:42:15.952260 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response400.py
+-rw-r--r--   0        0        0     2493 2024-04-09 11:42:15.980260 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response4001.py
+-rw-r--r--   0        0        0     4429 2024-04-09 11:42:16.016260 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response401.py
+-rw-r--r--   0        0        0     4429 2024-04-09 11:42:16.044260 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response4_xx.py
+-rw-r--r--   0        0        0     4429 2024-04-09 11:42:16.064261 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response5_xx.py
+-rw-r--r--   0        0        0     2457 2024-04-09 11:42:16.084261 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/model_date.py
+-rw-r--r--   0        0        0     2513 2024-04-09 11:42:16.104261 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/one_ofinline_response2006.py
+-rw-r--r--   0        0        0     2513 2024-04-09 11:42:16.124261 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/one_ofinline_response4001.py
+-rw-r--r--   0        0        0     3793 2024-04-09 11:42:16.148261 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/response_error.py
+-rw-r--r--   0        0        0    10201 2024-04-09 11:42:16.180261 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/size_good.py
+-rw-r--r--   0        0        0     5458 2024-04-09 11:42:16.200261 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/size_good_req.py
+-rw-r--r--   0        0        0     2473 2024-04-09 11:42:16.220261 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/size_goods_body.py
+-rw-r--r--   0        0        0     3195 2024-04-09 11:42:16.236261 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/successful.py
+-rw-r--r--   0        0        0     7572 2024-04-09 11:42:16.256261 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/supplier_task_metadata.py
+-rw-r--r--   0        0        0     7832 2024-04-09 11:42:16.272262 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/supplier_task_metadata_buffer.py
+-rw-r--r--   0        0        0     4707 2024-04-09 11:42:16.292262 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/task_already_exists_error.py
+-rw-r--r--   0        0        0     4191 2024-04-09 11:42:16.312262 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/task_already_exists_error_data.py
+-rw-r--r--   0        0        0     4498 2024-04-09 11:42:16.332262 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/task_created.py
+-rw-r--r--   0        0        0     4059 2024-04-09 11:42:16.352262 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/task_created_data.py
+-rw-r--r--   0        0        0     2461 2024-04-09 11:42:16.368262 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/task_status.py
+-rw-r--r--   0        0        0     2485 2024-04-09 11:42:16.384262 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/task_status_buffer.py
+-rw-r--r--   0        0        0     3834 2024-04-09 11:42:16.400262 wildberries_api_client-0.1.9/wildberries_api_client/prices/models/v1_prices_body.py
+-rw-r--r--   0        0        0    13049 2024-04-09 11:42:16.692264 wildberries_api_client-0.1.9/wildberries_api_client/prices/rest.py
+-rw-r--r--   0        0        0    12883 2024-04-09 11:42:09.904229 wildberries_api_client-0.1.9/wildberries_api_client/promotion/__init__.py
+-rw-r--r--   0        0        0     1365 2024-04-09 11:42:09.908229 wildberries_api_client-0.1.9/wildberries_api_client/promotion/api/__init__.py
+-rw-r--r--   0        0        0    13079 2024-04-09 11:42:09.568227 wildberries_api_client-0.1.9/wildberries_api_client/promotion/api/aktivnost_kampanii_api.py
+-rw-r--r--   0        0        0    15473 2024-04-09 11:42:09.600227 wildberries_api_client-0.1.9/wildberries_api_client/promotion/api/aktivnost_mediakampanii_api.py
+-rw-r--r--   0        0        0    23976 2024-04-09 11:42:09.628227 wildberries_api_client-0.1.9/wildberries_api_client/promotion/api/finansy_api.py
+-rw-r--r--   0        0        0    14233 2024-04-09 11:42:09.652227 wildberries_api_client-0.1.9/wildberries_api_client/promotion/api/media_api.py
+-rw-r--r--   0        0        0    23292 2024-04-09 11:42:09.680228 wildberries_api_client-0.1.9/wildberries_api_client/promotion/api/prodvihenie_api.py
+-rw-r--r--   0        0        0    20016 2024-04-09 11:42:09.704228 wildberries_api_client-0.1.9/wildberries_api_client/promotion/api/slovari_api.py
+-rw-r--r--   0        0        0    25550 2024-04-09 11:42:09.728228 wildberries_api_client-0.1.9/wildberries_api_client/promotion/api/statistika_api.py
+-rw-r--r--   0        0        0     4846 2024-04-09 11:42:09.756228 wildberries_api_client-0.1.9/wildberries_api_client/promotion/api/statistika_mediakampanii_api.py
+-rw-r--r--   0        0        0    16840 2024-04-09 11:42:09.776228 wildberries_api_client-0.1.9/wildberries_api_client/promotion/api/stavki_api.py
+-rw-r--r--   0        0        0     5206 2024-04-09 11:42:09.800228 wildberries_api_client-0.1.9/wildberries_api_client/promotion/api/stavki_mediakampanii_api.py
+-rw-r--r--   0        0        0     4584 2024-04-09 11:42:09.824228 wildberries_api_client-0.1.9/wildberries_api_client/promotion/api/upravlenie_obhimi_parametrami_kampanii_api.py
+-rw-r--r--   0        0        0    19421 2024-04-09 11:42:09.844228 wildberries_api_client-0.1.9/wildberries_api_client/promotion/api/upravlenie_parametrami_avtomatiheskih_kampanii_api.py
+-rw-r--r--   0        0        0    37598 2024-04-09 11:42:09.868229 wildberries_api_client-0.1.9/wildberries_api_client/promotion/api/upravlenie_parametrami_kampanii_v_poiske_ipoisk_katalog_api.py
+-rw-r--r--   0        0        0    25364 2024-04-09 11:42:09.952229 wildberries_api_client-0.1.9/wildberries_api_client/promotion/api_client.py
+-rw-r--r--   0        0        0     8472 2024-04-09 11:42:09.900229 wildberries_api_client-0.1.9/wildberries_api_client/promotion/configuration.py
+-rw-r--r--   0        0        0    11417 2024-04-09 11:42:09.908229 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/__init__.py
+-rw-r--r--   0        0        0     4262 2024-04-09 11:42:06.812213 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/advert_pause_body.py
+-rw-r--r--   0        0        0     4252 2024-04-09 11:42:06.884213 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/advert_start_body.py
+-rw-r--r--   0        0        0     4246 2024-04-09 11:42:06.944213 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/advert_stop_body.py
+-rw-r--r--   0        0        0     3992 2024-04-09 11:42:07.008214 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/advv0allcpm_cpm.py
+-rw-r--r--   0        0        0     4140 2024-04-09 11:42:07.052214 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/advv1searchsupplierproducts_kind.py
+-rw-r--r--   0        0        0     4192 2024-04-09 11:42:07.096214 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/advv1searchsupplierproducts_subject.py
+-rw-r--r--   0        0        0     5080 2024-04-09 11:42:07.144214 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/auto_active_body.py
+-rw-r--r--   0        0        0     3495 2024-04-09 11:42:07.184215 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/auto_setexcluded_body.py
+-rw-r--r--   0        0        0     4174 2024-04-09 11:42:07.224215 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/auto_updatenm_body.py
+-rw-r--r--   0        0        0     2664 2024-04-09 11:42:07.264215 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/booster_stats.py
+-rw-r--r--   0        0        0     4987 2024-04-09 11:42:07.308215 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/booster_stats_inner.py
+-rw-r--r--   0        0        0     5277 2024-04-09 11:42:07.352216 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/budget_deposit_body.py
+-rw-r--r--   0        0        0     5021 2024-04-09 11:42:07.396216 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/cpm_change_body.py
+-rw-r--r--   0        0        0     2660 2024-04-09 11:42:07.436216 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/daily_stats1.py
+-rw-r--r--   0        0        0     4273 2024-04-09 11:42:07.472216 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/daily_stats1_inner.py
+-rw-r--r--   0        0        0     2660 2024-04-09 11:42:07.508216 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/daily_stats2.py
+-rw-r--r--   0        0        0     4273 2024-04-09 11:42:07.544216 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/daily_stats2_inner.py
+-rw-r--r--   0        0        0     2632 2024-04-09 11:42:07.580217 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/days.py
+-rw-r--r--   0        0        0    11005 2024-04-09 11:42:07.616217 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/days_inner.py
+-rw-r--r--   0        0        0     3504 2024-04-09 11:42:07.644217 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response200.py
+-rw-r--r--   0        0        0     2688 2024-04-09 11:42:07.688217 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response2001.py
+-rw-r--r--   0        0        0     9674 2024-04-09 11:42:07.724218 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20010.py
+-rw-r--r--   0        0        0     7763 2024-04-09 11:42:07.748218 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20011.py
+-rw-r--r--   0        0        0     4132 2024-04-09 11:42:07.772218 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20012.py
+-rw-r--r--   0        0        0     4092 2024-04-09 11:42:07.800218 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20013.py
+-rw-r--r--   0        0        0     4062 2024-04-09 11:42:07.824218 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20014.py
+-rw-r--r--   0        0        0     4779 2024-04-09 11:42:07.848218 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20015.py
+-rw-r--r--   0        0        0     4850 2024-04-09 11:42:07.868218 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20016.py
+-rw-r--r--   0        0        0     2692 2024-04-09 11:42:07.884218 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20017.py
+-rw-r--r--   0        0        0     6539 2024-04-09 11:42:07.904218 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20018.py
+-rw-r--r--   0        0        0     4644 2024-04-09 11:42:07.924219 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20019.py
+-rw-r--r--   0        0        0     5289 2024-04-09 11:42:07.944218 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20019_clusters.py
+-rw-r--r--   0        0        0     4144 2024-04-09 11:42:07.968219 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response2002.py
+-rw-r--r--   0        0        0     4259 2024-04-09 11:42:07.984219 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20020.py
+-rw-r--r--   0        0        0     6405 2024-04-09 11:42:08.000219 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20020_stat.py
+-rw-r--r--   0        0        0     4745 2024-04-09 11:42:08.020219 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20021.py
+-rw-r--r--   0        0        0    12800 2024-04-09 11:42:08.036219 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20021_stat.py
+-rw-r--r--   0        0        0     7628 2024-04-09 11:42:08.056219 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20021_words.py
+-rw-r--r--   0        0        0     4334 2024-04-09 11:42:08.072219 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20021_words_keywords.py
+-rw-r--r--   0        0        0     6850 2024-04-09 11:42:08.092219 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20022.py
+-rw-r--r--   0        0        0     5652 2024-04-09 11:42:08.116220 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20022_catalog.py
+-rw-r--r--   0        0        0     4896 2024-04-09 11:42:08.148220 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20022_dates.py
+-rw-r--r--   0        0        0     5632 2024-04-09 11:42:08.176220 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20022_search.py
+-rw-r--r--   0        0        0     4860 2024-04-09 11:42:08.204220 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20023.py
+-rw-r--r--   0        0        0     6153 2024-04-09 11:42:08.220220 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20024.py
+-rw-r--r--   0        0        0     6199 2024-04-09 11:42:08.236220 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response2002_adverts.py
+-rw-r--r--   0        0        0     9246 2024-04-09 11:42:08.252220 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response2003.py
+-rw-r--r--   0        0        0    10116 2024-04-09 11:42:08.272220 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response2004.py
+-rw-r--r--   0        0        0     9967 2024-04-09 11:42:08.288221 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response2004_extended.py
+-rw-r--r--   0        0        0    24213 2024-04-09 11:42:08.304221 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response2004_items.py
+-rw-r--r--   0        0        0     4117 2024-04-09 11:42:08.328221 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response2004_show_hours.py
+-rw-r--r--   0        0        0     4040 2024-04-09 11:42:08.344221 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response2005.py
+-rw-r--r--   0        0        0     4147 2024-04-09 11:42:08.360221 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response2006.py
+-rw-r--r--   0        0        0     4767 2024-04-09 11:42:08.376221 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response2007.py
+-rw-r--r--   0        0        0     4903 2024-04-09 11:42:08.392221 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response2008.py
+-rw-r--r--   0        0        0     2688 2024-04-09 11:42:08.408221 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response2009.py
+-rw-r--r--   0        0        0     4447 2024-04-09 11:42:08.424221 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response200_advert_list.py
+-rw-r--r--   0        0        0     5806 2024-04-09 11:42:08.440221 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response200_adverts.py
+-rw-r--r--   0        0        0     3299 2024-04-09 11:42:08.456221 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response400.py
+-rw-r--r--   0        0        0     2708 2024-04-09 11:42:08.476221 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/one_ofinline_response2001.py
+-rw-r--r--   0        0        0     2712 2024-04-09 11:42:08.492221 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/one_ofinline_response20017.py
+-rw-r--r--   0        0        0     2708 2024-04-09 11:42:08.508221 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/one_ofinline_response2009.py
+-rw-r--r--   0        0        0     2680 2024-04-09 11:42:08.528222 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/one_ofv1_stats_body.py
+-rw-r--r--   0        0        0     2696 2024-04-09 11:42:08.544222 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/one_ofv2_fullstats_body.py
+-rw-r--r--   0        0        0     2700 2024-04-09 11:42:08.560222 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/request_with_campaign_id.py
+-rw-r--r--   0        0        0     3379 2024-04-09 11:42:08.576222 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/request_with_campaign_id_inner.py
+-rw-r--r--   0        0        0     2676 2024-04-09 11:42:08.588222 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/request_with_date.py
+-rw-r--r--   0        0        0     4117 2024-04-09 11:42:08.604222 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/request_with_date_inner.py
+-rw-r--r--   0        0        0     2692 2024-04-09 11:42:08.620222 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/request_with_interval.py
+-rw-r--r--   0        0        0     4233 2024-04-09 11:42:08.640222 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/request_with_interval_inner.py
+-rw-r--r--   0        0        0     3864 2024-04-09 11:42:08.656222 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response429.py
+-rw-r--r--   0        0        0     3299 2024-04-09 11:42:08.672222 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_adv_error1.py
+-rw-r--r--   0        0        0     4613 2024-04-09 11:42:08.688223 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_advert401.py
+-rw-r--r--   0        0        0    12997 2024-04-09 11:42:08.704223 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_info_advert.py
+-rw-r--r--   0        0        0     4174 2024-04-09 11:42:08.720223 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_info_advert_intervals.py
+-rw-r--r--   0        0        0     4327 2024-04-09 11:42:08.740223 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_info_advert_nms.py
+-rw-r--r--   0        0        0    11475 2024-04-09 11:42:08.756223 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_info_advert_params.py
+-rw-r--r--   0        0        0    11745 2024-04-09 11:42:08.772223 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_info_advert_type8.py
+-rw-r--r--   0        0        0     8667 2024-04-09 11:42:08.788223 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_info_advert_type8_auto_params.py
+-rw-r--r--   0        0        0     5480 2024-04-09 11:42:08.816223 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_info_advert_type8_auto_params_active.py
+-rw-r--r--   0        0        0     4242 2024-04-09 11:42:08.844223 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_info_advert_type8_auto_params_menus.py
+-rw-r--r--   0        0        0     4192 2024-04-09 11:42:08.872223 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_info_advert_type8_auto_params_nm_cpm.py
+-rw-r--r--   0        0        0     4226 2024-04-09 11:42:08.904224 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_info_advert_type8_auto_params_sets.py
+-rw-r--r--   0        0        0     4262 2024-04-09 11:42:08.920224 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_info_advert_type8_auto_params_subject.py
+-rw-r--r--   0        0        0    11793 2024-04-09 11:42:08.936224 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_info_advert_type9.py
+-rw-r--r--   0        0        0     4152 2024-04-09 11:42:08.964224 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_info_advert_type9_menus.py
+-rw-r--r--   0        0        0     4234 2024-04-09 11:42:08.980224 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_info_advert_type9_subject.py
+-rw-r--r--   0        0        0     6863 2024-04-09 11:42:08.996224 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_info_advert_type9_united_params.py
+-rw-r--r--   0        0        0     2680 2024-04-09 11:42:09.016224 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_with_date.py
+-rw-r--r--   0        0        0    14243 2024-04-09 11:42:09.032224 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_with_date_inner.py
+-rw-r--r--   0        0        0     2696 2024-04-09 11:42:09.052224 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_with_interval.py
+-rw-r--r--   0        0        0    14963 2024-04-09 11:42:09.072224 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_with_interval_inner.py
+-rw-r--r--   0        0        0     3407 2024-04-09 11:42:09.092224 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_with_return.py
+-rw-r--r--   0        0        0     4625 2024-04-09 11:42:09.108225 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/seacat_savead_body.py
+-rw-r--r--   0        0        0     3511 2024-04-09 11:42:09.124225 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/search_setexcluded_body.py
+-rw-r--r--   0        0        0     3455 2024-04-09 11:42:09.140225 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/search_setphrase_body.py
+-rw-r--r--   0        0        0     3435 2024-04-09 11:42:09.160225 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/search_setplus_body.py
+-rw-r--r--   0        0        0     3455 2024-04-09 11:42:09.176225 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/search_setstrong_body.py
+-rw-r--r--   0        0        0     3310 2024-04-09 11:42:09.192225 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/stat.py
+-rw-r--r--   0        0        0     4080 2024-04-09 11:42:09.208225 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/stat_date.py
+-rw-r--r--   0        0        0     4082 2024-04-09 11:42:09.224225 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/stat_interval.py
+-rw-r--r--   0        0        0     4124 2024-04-09 11:42:09.240225 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/stat_interval_interval.py
+-rw-r--r--   0        0        0     2640 2024-04-09 11:42:09.256225 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/stats1.py
+-rw-r--r--   0        0        0     5604 2024-04-09 11:42:09.272225 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/stats1_inner.py
+-rw-r--r--   0        0        0     2640 2024-04-09 11:42:09.288226 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/stats2.py
+-rw-r--r--   0        0        0     7078 2024-04-09 11:42:09.304226 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/stats2_inner.py
+-rw-r--r--   0        0        0    18349 2024-04-09 11:42:09.324226 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/stats_blok1.py
+-rw-r--r--   0        0        0    18349 2024-04-09 11:42:09.340226 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/stats_blok2.py
+-rw-r--r--   0        0        0     3803 2024-04-09 11:42:09.356226 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/v0_allcpm_body.py
+-rw-r--r--   0        0        0     8090 2024-04-09 11:42:09.372226 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/v0_cpm_body.py
+-rw-r--r--   0        0        0     4356 2024-04-09 11:42:09.396226 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/v0_rename_body.py
+-rw-r--r--   0        0        0     9588 2024-04-09 11:42:09.412226 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/v1_savead_body.py
+-rw-r--r--   0        0        0     2660 2024-04-09 11:42:09.428226 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/v1_stats_body.py
+-rw-r--r--   0        0        0     2676 2024-04-09 11:42:09.444226 wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/v2_fullstats_body.py
+-rw-r--r--   0        0        0    13244 2024-04-09 11:42:09.968229 wildberries_api_client-0.1.9/wildberries_api_client/promotion/rest.py
+-rw-r--r--   0        0        0     1101 2024-04-09 11:42:26.556315 wildberries_api_client-0.1.9/wildberries_api_client/recommendations/__init__.py
+-rw-r--r--   0        0        0      175 2024-04-09 11:42:26.560315 wildberries_api_client-0.1.9/wildberries_api_client/recommendations/api/__init__.py
+-rw-r--r--   0        0        0    19295 2024-04-09 11:42:26.476314 wildberries_api_client-0.1.9/wildberries_api_client/recommendations/api/rekomendacii_api.py
+-rw-r--r--   0        0        0    25179 2024-04-09 11:42:26.664315 wildberries_api_client-0.1.9/wildberries_api_client/recommendations/api_client.py
+-rw-r--r--   0        0        0     8269 2024-04-09 11:42:26.552315 wildberries_api_client-0.1.9/wildberries_api_client/recommendations/configuration.py
+-rw-r--r--   0        0        0      813 2024-04-09 11:42:26.560315 wildberries_api_client-0.1.9/wildberries_api_client/recommendations/models/__init__.py
+-rw-r--r--   0        0        0     3142 2024-04-09 11:42:26.176313 wildberries_api_client-0.1.9/wildberries_api_client/recommendations/models/inline_response200.py
+-rw-r--r--   0        0        0     3917 2024-04-09 11:42:26.228313 wildberries_api_client-0.1.9/wildberries_api_client/recommendations/models/inline_response200_data.py
+-rw-r--r--   0        0        0     4136 2024-04-09 11:42:26.284313 wildberries_api_client-0.1.9/wildberries_api_client/recommendations/models/v1_del_body.py
+-rw-r--r--   0        0        0     4124 2024-04-09 11:42:26.332314 wildberries_api_client-0.1.9/wildberries_api_client/recommendations/models/v1_ins_body.py
+-rw-r--r--   0        0        0     4078 2024-04-09 11:42:26.380314 wildberries_api_client-0.1.9/wildberries_api_client/recommendations/models/v1_set_body.py
+-rw-r--r--   0        0        0    13035 2024-04-09 11:42:26.688315 wildberries_api_client-0.1.9/wildberries_api_client/recommendations/rest.py
+-rw-r--r--   0        0        0      662 2024-04-09 11:39:23.915372 wildberries_api_client-0.1.9/wildberries_api_client/setup.py
+-rw-r--r--   0        0        0     3273 2024-04-09 11:42:22.020291 wildberries_api_client-0.1.9/wildberries_api_client/statistics/__init__.py
+-rw-r--r--   0        0        0      264 2024-04-09 11:42:22.024291 wildberries_api_client-0.1.9/wildberries_api_client/statistics/api/__init__.py
+-rw-r--r--   0        0        0    13880 2024-04-09 11:42:21.932291 wildberries_api_client-0.1.9/wildberries_api_client/statistics/api/otlohennaa_generacia_api.py
+-rw-r--r--   0        0        0    30740 2024-04-09 11:42:21.964291 wildberries_api_client-0.1.9/wildberries_api_client/statistics/api/statistika_api.py
+-rw-r--r--   0        0        0    25099 2024-04-09 11:42:22.076292 wildberries_api_client-0.1.9/wildberries_api_client/statistics/api_client.py
+-rw-r--r--   0        0        0     8204 2024-04-09 11:42:22.016291 wildberries_api_client-0.1.9/wildberries_api_client/statistics/configuration.py
+-rw-r--r--   0        0        0     2906 2024-04-09 11:42:22.020291 wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/__init__.py
+-rw-r--r--   0        0        0     2805 2024-04-09 11:42:20.904286 wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/create_task_request.py
+-rw-r--r--   0        0        0     4298 2024-04-09 11:42:20.972286 wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/create_task_request_paid_storage.py
+-rw-r--r--   0        0        0     6013 2024-04-09 11:42:21.028286 wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/create_task_request_paid_storage_params.py
+-rw-r--r--   0        0        0     3075 2024-04-09 11:42:21.080286 wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/create_task_response.py
+-rw-r--r--   0        0        0     3203 2024-04-09 11:42:21.144287 wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/create_task_response_data.py
+-rw-r--r--   0        0        0    58735 2024-04-09 11:42:21.208287 wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/detail_report_item.py
+-rw-r--r--   0        0        0     3101 2024-04-09 11:42:21.260287 wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/download_request.py
+-rw-r--r--   0        0        0     3121 2024-04-09 11:42:21.304288 wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/error_response.py
+-rw-r--r--   0        0        0     3058 2024-04-09 11:42:21.356288 wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/get_tasks_request.py
+-rw-r--r--   0        0        0     3053 2024-04-09 11:42:21.404288 wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/get_tasks_response.py
+-rw-r--r--   0        0        0     3163 2024-04-09 11:42:21.448288 wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/get_tasks_response_bytes_error.py
+-rw-r--r--   0        0        0     3248 2024-04-09 11:42:21.484289 wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/get_tasks_response_bytes_error_data.py
+-rw-r--r--   0        0        0     4672 2024-04-09 11:42:21.520289 wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/get_tasks_response_bytes_error_data_tasks.py
+-rw-r--r--   0        0        0     4077 2024-04-09 11:42:21.548289 wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/get_tasks_response_data.py
+-rw-r--r--   0        0        0    13118 2024-04-09 11:42:21.576289 wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/incomes_item.py
+-rw-r--r--   0        0        0     2415 2024-04-09 11:42:21.600289 wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/inline_response200.py
+-rw-r--r--   0        0        0     2415 2024-04-09 11:42:21.624289 wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/inline_response429.py
+-rw-r--r--   0        0        0     2435 2024-04-09 11:42:21.644289 wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/one_of_create_task_request.py
+-rw-r--r--   0        0        0     2435 2024-04-09 11:42:21.668290 wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/one_ofinline_response200.py
+-rw-r--r--   0        0        0     2435 2024-04-09 11:42:21.688289 wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/one_ofinline_response429.py
+-rw-r--r--   0        0        0    25075 2024-04-09 11:42:21.712290 wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/orders_item.py
+-rw-r--r--   0        0        0     3595 2024-04-09 11:42:21.732290 wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/response429.py
+-rw-r--r--   0        0        0     3116 2024-04-09 11:42:21.752290 wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/response_error_statistics.py
+-rw-r--r--   0        0        0     2423 2024-04-09 11:42:21.772290 wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/response_paid_storage.py
+-rw-r--r--   0        0        0    18065 2024-04-09 11:42:21.792290 wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/response_paid_storage_inner.py
+-rw-r--r--   0        0        0    25876 2024-04-09 11:42:21.820290 wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/sales_item.py
+-rw-r--r--   0        0        0    16906 2024-04-09 11:42:21.844290 wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/stocks_item.py
+-rw-r--r--   0        0        0    12975 2024-04-09 11:42:22.088292 wildberries_api_client-0.1.9/wildberries_api_client/statistics/rest.py
+-rw-r--r--   0        0        0     2009 2024-04-09 11:42:31.340340 wildberries_api_client-0.1.9/wildberries_api_client/tariffs/__init__.py
+-rw-r--r--   0        0        0      288 2024-04-09 11:42:31.344339 wildberries_api_client-0.1.9/wildberries_api_client/tariffs/api/__init__.py
+-rw-r--r--   0        0        0     9355 2024-04-09 11:42:31.204339 wildberries_api_client-0.1.9/wildberries_api_client/tariffs/api/koefficienty_skladov_api.py
+-rw-r--r--   0        0        0     5002 2024-04-09 11:42:31.268339 wildberries_api_client-0.1.9/wildberries_api_client/tariffs/api/stoimost_vozvrata_prodavcu_api.py
+-rw-r--r--   0        0        0    25158 2024-04-09 11:42:31.416340 wildberries_api_client-0.1.9/wildberries_api_client/tariffs/api_client.py
+-rw-r--r--   0        0        0     8304 2024-04-09 11:42:31.336340 wildberries_api_client-0.1.9/wildberries_api_client/tariffs/configuration.py
+-rw-r--r--   0        0        0     1624 2024-04-09 11:42:31.344339 wildberries_api_client-0.1.9/wildberries_api_client/tariffs/models/__init__.py
+-rw-r--r--   0        0        0     3233 2024-04-09 11:42:30.648336 wildberries_api_client-0.1.9/wildberries_api_client/tariffs/models/models_return_tariffs_response.py
+-rw-r--r--   0        0        0     3200 2024-04-09 11:42:30.716336 wildberries_api_client-0.1.9/wildberries_api_client/tariffs/models/models_tariffs_box_response.py
+-rw-r--r--   0        0        0     3233 2024-04-09 11:42:30.768337 wildberries_api_client-0.1.9/wildberries_api_client/tariffs/models/models_tariffs_pallet_response.py
+-rw-r--r--   0        0        0     8745 2024-04-09 11:42:30.816337 wildberries_api_client-0.1.9/wildberries_api_client/tariffs/models/models_warehouse_box_rates.py
+-rw-r--r--   0        0        0     9358 2024-04-09 11:42:30.872337 wildberries_api_client-0.1.9/wildberries_api_client/tariffs/models/models_warehouse_pallet_rates.py
+-rw-r--r--   0        0        0    18800 2024-04-09 11:42:30.916337 wildberries_api_client-0.1.9/wildberries_api_client/tariffs/models/models_warehouse_return_rates.py
+-rw-r--r--   0        0        0     6115 2024-04-09 11:42:30.952337 wildberries_api_client-0.1.9/wildberries_api_client/tariffs/models/models_warehouses_box_rates.py
+-rw-r--r--   0        0        0     6248 2024-04-09 11:42:31.000338 wildberries_api_client-0.1.9/wildberries_api_client/tariffs/models/models_warehouses_pallet_rates.py
+-rw-r--r--   0        0        0     8020 2024-04-09 11:42:31.032338 wildberries_api_client-0.1.9/wildberries_api_client/tariffs/models/models_warehouses_return_rates.py
+-rw-r--r--   0        0        0     3265 2024-04-09 11:42:31.060338 wildberries_api_client-0.1.9/wildberries_api_client/tariffs/models/return_tariffs_response.py
+-rw-r--r--   0        0        0     3232 2024-04-09 11:42:31.092338 wildberries_api_client-0.1.9/wildberries_api_client/tariffs/models/tariffs_box_response.py
+-rw-r--r--   0        0        0     3265 2024-04-09 11:42:31.128338 wildberries_api_client-0.1.9/wildberries_api_client/tariffs/models/tariffs_pallet_response.py
+-rw-r--r--   0        0        0    13046 2024-04-09 11:42:31.440340 wildberries_api_client-0.1.9/wildberries_api_client/tariffs/rest.py
+-rw-r--r--   0        0        0     2205 1970-01-01 00:00:00.000000 wildberries_api_client-0.1.9/PKG-INFO
```

### Comparing `wildberries_api_client-0.1.8/README.md` & `wildberries_api_client-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/_api_client.py` & `wildberries_api_client-0.1.9/wildberries_api_client/_api_client.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/_configuration.py` & `wildberries_api_client-0.1.9/wildberries_api_client/_configuration.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/_swagger_doc/swagger_analytics.yaml` & `wildberries_api_client-0.1.9/wildberries_api_client/_swagger_doc/swagger_analytics.yaml`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/_swagger_doc/swagger_content.yaml` & `wildberries_api_client-0.1.9/wildberries_api_client/_swagger_doc/swagger_content.yaml`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/_swagger_doc/swagger_feedbacks_questions.yaml` & `wildberries_api_client-0.1.9/wildberries_api_client/_swagger_doc/swagger_feedbacks_questions.yaml`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/_swagger_doc/swagger_marketplace.yaml` & `wildberries_api_client-0.1.9/wildberries_api_client/_swagger_doc/swagger_marketplace.yaml`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/_swagger_doc/swagger_prices.yaml` & `wildberries_api_client-0.1.9/wildberries_api_client/_swagger_doc/swagger_prices.yaml`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/_swagger_doc/swagger_promotion.yaml` & `wildberries_api_client-0.1.9/wildberries_api_client/_swagger_doc/swagger_promotion.yaml`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/_swagger_doc/swagger_recommendations.yaml` & `wildberries_api_client-0.1.9/wildberries_api_client/_swagger_doc/swagger_recommendations.yaml`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/_swagger_doc/swagger_statistics.yaml` & `wildberries_api_client-0.1.9/wildberries_api_client/_swagger_doc/swagger_statistics.yaml`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/_swagger_doc/swagger_tariffs.yaml` & `wildberries_api_client-0.1.9/wildberries_api_client/_swagger_doc/swagger_tariffs.yaml`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/_swagger_doc/transliterate_script.py` & `wildberries_api_client-0.1.9/wildberries_api_client/_swagger_doc/transliterate_script.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/__init__.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/api/__init__.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/api/__init__.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/api/othety_pouderhaniam_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/api/othety_pouderhaniam_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/api/platnaa_priemka_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/api/platnaa_priemka_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/api/platnoe_hranenie_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/api/platnoe_hranenie_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/api/tovary_s_obazatelnoi_markirovkoi_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/api/tovary_s_obazatelnoi_markirovkoi_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/api/voronka_prodah_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/api/voronka_prodah_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/api_client.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/api_client.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/configuration.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/configuration.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/__init__.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/__init__.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/create_task_response.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/create_task_response.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/create_task_response_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/create_task_response_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/error_internal_response.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/error_internal_response.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/error_response.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/error_response.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/excise_report_request.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/excise_report_request.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/excise_report_response.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/excise_report_response.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/get_tasks_response.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/get_tasks_response.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/get_tasks_response_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/get_tasks_response_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/inline_response200.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/inline_response200.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/inline_response2001.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/inline_response2001.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/inline_response2001_details.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/inline_response2001_details.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/inline_response2002.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/inline_response2002.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/inline_response2002_report.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/inline_response2002_report.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/inline_response2003.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/inline_response2003.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/inline_response2003_report.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/inline_response2003_report.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/inline_response200_report.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/inline_response200_report.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/inline_response400.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/inline_response400.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/models_excise_report_response.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/models_excise_report_response.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/models_excise_report_response_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/models_excise_report_response_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/models_excise_report_response_data_inner.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/models_excise_report_response_data_inner.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_history_request.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_history_request.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_history_request_period.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_history_request_period.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_history_response.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_history_response.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_history_response_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_history_response_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_history_response_history.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_history_response_history.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_request.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_request.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_request_order_by.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_request_order_by.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_request_period.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_request_period.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_response.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_response.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_response_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_response_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_response_data_cards.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_response_data_cards.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_response_data_object.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_response_data_object.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_response_data_statistics.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_response_data_statistics.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_response_data_statistics_period_comparison.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_response_data_statistics_period_comparison.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_response_data_statistics_period_comparison_conversions.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_response_data_statistics_period_comparison_conversions.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_response_data_statistics_previous_period.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_response_data_statistics_previous_period.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_response_data_statistics_previous_period_conversions.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_response_data_statistics_previous_period_conversions.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_response_data_statistics_selected_period.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_response_data_statistics_selected_period.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_response_data_statistics_selected_period_conversions.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_response_data_statistics_selected_period_conversions.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_response_data_stocks.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_response_data_stocks.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_detail_response_data_tags.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_detail_response_data_tags.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_history_request.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_history_request.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_history_request_period.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_history_request_period.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_history_response.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_history_response.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_history_response_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_history_response_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_history_response_history.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_history_response_history.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_history_response_object.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_history_response_object.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_history_response_tag.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_history_response_tag.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_request.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_request.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_request_order_by.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_request_order_by.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_request_period.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_request_period.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_response.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_response.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_response_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_response_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_response_data_groups.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_response_data_groups.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_response_data_object.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_response_data_object.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_response_data_statistics.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_response_data_statistics.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_response_data_statistics_period_comparison.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_response_data_statistics_period_comparison.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_response_data_statistics_period_comparison_conversions.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_response_data_statistics_period_comparison_conversions.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_response_data_statistics_previous_period.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_response_data_statistics_previous_period.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_response_data_statistics_previous_period_conversions.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_response_data_statistics_previous_period_conversions.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/nm_report_grouped_response_data_statistics_selected_period.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/nm_report_grouped_response_data_statistics_selected_period.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/response_error.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/response_error.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/response_error_additional_errors.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/response_error_additional_errors.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/response_paid_storage.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/response_paid_storage.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/models/response_paid_storage_inner.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/models/response_paid_storage_inner.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/analytics/rest.py` & `wildberries_api_client-0.1.9/wildberries_api_client/analytics/rest.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/__init__.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/__init__.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/api/__init__.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/api/__init__.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/api/konfigurator_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/api/konfigurator_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/api/korzina_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/api/korzina_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/api/mediafaily_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/api/mediafaily_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/api/prosmotr_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/api/prosmotr_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/api/tegi_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/api/tegi_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/api/zagruzka_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/api/zagruzka_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/api_client.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/api_client.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/configuration.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/configuration.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/__init__.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/__init__.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/cards_list_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/cards_list_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/cards_move_nm_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/cards_move_nm_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/cards_recover_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/cards_recover_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/cards_trash_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/cards_trash_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/cards_update_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/cards_update_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/cards_upload_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/cards_upload_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2cardsupdate_characteristics.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2cardsupdate_characteristics.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2cardsupdate_dimensions.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2cardsupdate_dimensions.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2cardsupdate_sizes.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2cardsupdate_sizes.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2cardsupload_characteristics.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2cardsupload_characteristics.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2cardsupload_dimensions.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2cardsupload_dimensions.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2cardsupload_sizes.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2cardsupload_sizes.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2cardsupload_variants.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2cardsupload_variants.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2cardsuploadadd_cards_to_add.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2cardsuploadadd_cards_to_add.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2cardsuploadadd_characteristics.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2cardsuploadadd_characteristics.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2cardsuploadadd_sizes.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2cardsuploadadd_sizes.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2getcardslist_settings.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2getcardslist_settings.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2getcardslist_settings_cursor.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2getcardslist_settings_cursor.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2getcardslist_settings_filter.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2getcardslist_settings_filter.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2getcardslist_settings_sort.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2getcardslist_settings_sort.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2getcardstrash_settings.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2getcardstrash_settings.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2getcardstrash_settings_cursor.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2getcardstrash_settings_cursor.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2getcardstrash_settings_filter.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2getcardstrash_settings_filter.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/contentv2getcardstrash_settings_sort.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/contentv2getcardstrash_settings_sort.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/delete_trash_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/delete_trash_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response200.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response200.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2001.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2001.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response20010.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response20010.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response20011.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response20011.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response20011_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response20011_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response20012.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response20012.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response20013.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response20013.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response20014.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response20014.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response20014_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response20014_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response20015.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response20015.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response20016.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response20016.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response20017.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response20017.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response20018.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response20018.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response20018_cards.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response20018_cards.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response20018_characteristics.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response20018_characteristics.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response20018_cursor.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response20018_cursor.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response20018_dimensions.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response20018_dimensions.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response20018_sizes.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response20018_sizes.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2001_cards.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2001_cards.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2001_characteristics.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2001_characteristics.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2001_cursor.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2001_cursor.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2001_dimensions.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2001_dimensions.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2001_photos.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2001_photos.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2001_sizes.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2001_sizes.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2001_tags.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2001_tags.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2002.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2002.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2002_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2002_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2003.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2003.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2003_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2003_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2004.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2004.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2004_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2004_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2005.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2005.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2005_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2005_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2006.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2006.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2006_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2006_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2007.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2007.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2007_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2007_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2008.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2008.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2009.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2009.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response2009_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response2009_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response400.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response400.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response4001.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response4001.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response4002.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response4002.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/inline_response4003.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/inline_response4003.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/media_file_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/media_file_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/media_file_body1.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/media_file_body1.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/media_save_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/media_save_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/media_save_body1.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/media_save_body1.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/nomenclature_link_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/nomenclature_link_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/one_ofcards_move_nm_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/one_ofcards_move_nm_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/one_ofinline_response20015.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/one_ofinline_response20015.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/one_ofinline_response20016.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/one_ofinline_response20016.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/one_ofinline_response400.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/one_ofinline_response400.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/one_ofinline_response4001.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/one_ofinline_response4001.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/one_ofinline_response4002.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/one_ofinline_response4002.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/one_ofinline_response4003.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/one_ofinline_response4003.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/one_ofresponse_card_create_additional_errors.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/one_ofresponse_card_create_additional_errors.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/request_move_nms_imt_conn.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/request_move_nms_imt_conn.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/request_move_nms_imt_disconn.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/request_move_nms_imt_disconn.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/response_body_content_error400.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/response_body_content_error400.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/response_body_content_error400_additional_errors.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/response_body_content_error400_additional_errors.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/response_body_content_error403.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/response_body_content_error403.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/response_card_create.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/response_card_create.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/response_content_error1.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/response_content_error1.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/response_content_error1_additional_errors.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/response_content_error1_additional_errors.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/response_content_error4.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/response_content_error4.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/response_content_error4_additional_errors.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/response_content_error4_additional_errors.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/response_content_error5.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/response_content_error5.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/response_content_error5_additional_errors.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/response_content_error5_additional_errors.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/response_content_error6.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/response_content_error6.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/response_incorrect_date.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/response_incorrect_date.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/tag_id_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/tag_id_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/upload_add_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/upload_add_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/v2_barcodes_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/v2_barcodes_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/models/v2_tag_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/models/v2_tag_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/content/rest.py` & `wildberries_api_client-0.1.9/wildberries_api_client/content/rest.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/__init__.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/__init__.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/api/hablony_dla_voprosov_i_otzyvov_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/api/hablony_dla_voprosov_i_otzyvov_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/api/otzyvy_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/api/otzyvy_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/api/voprosy_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/api/voprosy_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/api_client.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/api_client.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/configuration.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/configuration.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/__init__.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/__init__.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/apiv1questions_answer.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/apiv1questions_answer.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response200.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response200.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2001.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2001.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20010.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20010.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20010_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20010_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20011.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20011.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20011_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20011_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20012.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20012.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20012_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20012_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20013.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20013.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20013_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20013_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20013_data_feedback_valuations.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20013_data_feedback_valuations.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20013_data_product_valuations.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20013_data_product_valuations.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20014.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20014.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20014_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20014_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20015.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20015.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20015_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20015_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20016.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20016.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20016_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20016_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20017.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20017.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20018.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20018.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20018_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20018_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'id': 'int',
+        'id': 'str',
         'user_name': 'str',
         'matching_size': 'str',
         'text': 'str',
         'product_valuation': 'int',
         'created_date': 'datetime',
         'state': 'str',
         'answer': 'InlineResponse20018DataAnswer',
```

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20018_data_answer.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20018_data_answer.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20018_data_photo_links.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20018_data_photo_links.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20018_data_product_details.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20018_data_product_details.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20018_data_video.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20018_data_video.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20019.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20019.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2001_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2001_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2002.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2002.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20020.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20020.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response20021.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response20021.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2002_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2002_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2002_data_products.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2002_data_products.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2003.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2003.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2003_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2003_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2003_data_answer.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2003_data_answer.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2003_data_product_details.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2003_data_product_details.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2003_data_questions.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2003_data_questions.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2004.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2004.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2005.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2005.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2005_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2005_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2006.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2006.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2007.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2007.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2007_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2007_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2008.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2008.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2008_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2008_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2009.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2009.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response2009_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response2009_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/inline_response200_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/inline_response200_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/one_ofinline_response20019.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/one_ofinline_response20019.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/one_ofinline_response20020.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/one_ofinline_response20020.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/one_ofinline_response20021.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/one_ofinline_response20021.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/one_ofv1_feedbacks_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/one_ofv1_feedbacks_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/one_ofv1_questions_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/one_ofv1_questions_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/order_return_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/order_return_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/patch_del_resp_ok.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/patch_del_resp_ok.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/post_template_ok.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/post_template_ok.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/post_template_ok_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/post_template_ok_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/product_rating.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/product_rating.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/response200.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/response200.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/response200_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/response200_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/response200_data_templates.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/response200_data_templates.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/response_error_template.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/response_error_template.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/response_feadback.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/response_feadback.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/response_feadback_inner.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/response_feadback_inner.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/responsefeedback_err.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/responsefeedback_err.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/v1_feedbacks_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/v1_feedbacks_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/v1_questions_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/v1_questions_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/v1_templates_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/v1_templates_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/v1_templates_body1.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/v1_templates_body1.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/models/v1_templates_body2.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/models/v1_templates_body2.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/feedbacks_questions/rest.py` & `wildberries_api_client-0.1.9/wildberries_api_client/feedbacks_questions/rest.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/__init__.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/__init__.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/api/ostatki_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/api/ostatki_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/api/postavki_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/api/postavki_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/api/propuska_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/api/propuska_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/api/sborohnye_zadania_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/api/sborohnye_zadania_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/api/sklady_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/api/sklady_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/api_client.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/api_client.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/configuration.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/configuration.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/__init__.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/__init__.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/apiv3stockswarehouse_id_stocks.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/apiv3stockswarehouse_id_stocks.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/error.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/error.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response200.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response200.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response2001.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response2001.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response20010.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response20010.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response20011.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response20011.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response20012.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response20012.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response20012_stocks.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response20012_stocks.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response2002.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response2002.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response2002_orders.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response2002_orders.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response2003.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response2003.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response2003_orders.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response2003_orders.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response2004.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response2004.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response2004_stickers.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response2004_stickers.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response2005.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response2005.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response2006.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response2006.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response2006_stickers.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response2006_stickers.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response2007.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response2007.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response2008.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response2008.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response2009.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response2009.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response201.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response201.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response2011.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response2011.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response2012.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response2012.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/inline_response2013.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/inline_response2013.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/meta.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/meta.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/meta_gtin_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/meta_gtin_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/meta_imei_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/meta_imei_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/meta_sgtin_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/meta_sgtin_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/meta_uin_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/meta_uin_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/model_pass.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/model_pass.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/next.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/next.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/office.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/office.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/order.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/order.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/order_address.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/order_address.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/order_new.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/order_new.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/order_user.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/order_user.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/orders_externalstickers_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/orders_externalstickers_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/orders_status_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/orders_status_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/orders_stickers_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/orders_stickers_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/pass_office.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/pass_office.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/passes_pass_id_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/passes_pass_id_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/stocks_warehouse_id_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/stocks_warehouse_id_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/stocks_warehouse_id_body1.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/stocks_warehouse_id_body1.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/stocks_warehouse_id_body2.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/stocks_warehouse_id_body2.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/supply.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/supply.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/supply_id_trbx_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/supply_id_trbx_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/supply_id_trbx_body1.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/supply_id_trbx_body1.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/supply_order.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/supply_order.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/supply_trbx.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/supply_trbx.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/trbx_stickers.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/trbx_stickers.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/trbx_stickers_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/trbx_stickers_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/trbx_trbx_id_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/trbx_trbx_id_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/v3_passes_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/v3_passes_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/v3_supplies_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/v3_supplies_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/v3_warehouses_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/v3_warehouses_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/warehouse.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/warehouse.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/models/warehouses_warehouse_id_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/models/warehouses_warehouse_id_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/marketplace/rest.py` & `wildberries_api_client-0.1.9/wildberries_api_client/marketplace/rest.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/__init__.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/__init__.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/api/ceny_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/api/ceny_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/api/promokody_i_skidki_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/api/promokody_i_skidki_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/api/sostoania_zagruzok_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/api/sostoania_zagruzok_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/api/spiski_tovarov_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/api/spiski_tovarov_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/api/ustanovka_cen_i_skidok_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/api/ustanovka_cen_i_skidok_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/api_client.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/api_client.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/configuration.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/configuration.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/__init__.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/__init__.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/date1.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/date1.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/good.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/good.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/good_buffer_history.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/good_buffer_history.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/good_history.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/good_history.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/good_status.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/good_status.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/good_status_buffer.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/good_status_buffer.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/goods.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/goods.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/goods_list.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/goods_list.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/goods_list_sizes.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/goods_list_sizes.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response200.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response200.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response2001.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response2001.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response2001_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response2001_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response2002.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response2002.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response2003.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response2003.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response2003_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response2003_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response2004.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response2004.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response2004_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response2004_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response2005.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response2005.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response2005_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response2005_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response2006.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response2006.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response2007.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response2007.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response2008.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response2008.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response400.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response400.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response4001.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response4001.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response401.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response401.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response4_xx.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response4_xx.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/inline_response5_xx.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/inline_response5_xx.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/model_date.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/model_date.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/one_ofinline_response2006.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/one_ofinline_response2006.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/one_ofinline_response4001.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/one_ofinline_response4001.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/response_error.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/response_error.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/size_good.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/size_good.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/size_good_req.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/size_good_req.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/size_goods_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/size_goods_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/successful.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/successful.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/supplier_task_metadata.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/supplier_task_metadata.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/supplier_task_metadata_buffer.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/supplier_task_metadata_buffer.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/task_already_exists_error.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/task_already_exists_error.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/task_already_exists_error_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/task_already_exists_error_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/task_created.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/task_created.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/task_created_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/task_created_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/task_status.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/task_status.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/task_status_buffer.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/task_status_buffer.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/models/v1_prices_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/models/v1_prices_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/prices/rest.py` & `wildberries_api_client-0.1.9/wildberries_api_client/prices/rest.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/__init__.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/__init__.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/api/__init__.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/api/__init__.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/api/aktivnost_kampanii_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/api/aktivnost_kampanii_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/api/aktivnost_mediakampanii_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/api/aktivnost_mediakampanii_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/api/finansy_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/api/finansy_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/api/media_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/api/media_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/api/prodvihenie_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/api/prodvihenie_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/api/slovari_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/api/slovari_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/api/statistika_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/api/statistika_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/api/statistika_mediakampanii_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/api/statistika_mediakampanii_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/api/stavki_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/api/stavki_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/api/stavki_mediakampanii_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/api/stavki_mediakampanii_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/api/upravlenie_obhimi_parametrami_kampanii_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/api/upravlenie_obhimi_parametrami_kampanii_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/api/upravlenie_parametrami_avtomatiheskih_kampanii_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/api/upravlenie_parametrami_avtomatiheskih_kampanii_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/api/upravlenie_parametrami_kampanii_v_poiske_ipoisk_katalog_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/api/upravlenie_parametrami_kampanii_v_poiske_ipoisk_katalog_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/api_client.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/api_client.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/configuration.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/configuration.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/__init__.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/__init__.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/advert_pause_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/advert_pause_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/advert_start_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/advert_start_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/advert_stop_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/advert_stop_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/advv0allcpm_cpm.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/advv0allcpm_cpm.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/advv1searchsupplierproducts_kind.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/advv1searchsupplierproducts_kind.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/advv1searchsupplierproducts_subject.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/advv1searchsupplierproducts_subject.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/auto_active_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/auto_active_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/auto_setexcluded_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/auto_setexcluded_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/auto_updatenm_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/auto_updatenm_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/booster_stats.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/booster_stats.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/booster_stats_inner.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/booster_stats_inner.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/budget_deposit_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/budget_deposit_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/cpm_change_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/cpm_change_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/daily_stats1.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/daily_stats1.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/daily_stats1_inner.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/daily_stats1_inner.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/daily_stats2.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/daily_stats2.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/daily_stats2_inner.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/daily_stats2_inner.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/days.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/days.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/days_inner.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/days_inner.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response200.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response200.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response2001.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response2001.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20010.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20010.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20011.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20011.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20012.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20012.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20013.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20013.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20014.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20014.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20015.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20015.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20016.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20016.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20017.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20017.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20018.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20018.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20019.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20019.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20019_clusters.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20019_clusters.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response2002.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response2002.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20020.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20020.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20020_stat.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20020_stat.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20021.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20021.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20021_stat.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20021_stat.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20021_words.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20021_words.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20021_words_keywords.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20021_words_keywords.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20022.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20022.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20022_catalog.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20022_catalog.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20022_dates.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20022_dates.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20022_search.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20022_search.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20023.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20023.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response20024.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response20024.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response2002_adverts.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response2002_adverts.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response2003.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response2003.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response2004.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response2004.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response2004_extended.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response2004_extended.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response2004_items.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response2004_items.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response2004_show_hours.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response2004_show_hours.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response2005.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response2005.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response2006.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response2006.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response2007.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response2007.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response2008.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response2008.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response2009.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response2009.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response200_advert_list.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response200_advert_list.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response200_adverts.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response200_adverts.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/inline_response400.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/inline_response400.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/one_ofinline_response2001.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/one_ofinline_response2001.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/one_ofinline_response20017.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/one_ofinline_response20017.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/one_ofinline_response2009.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/one_ofinline_response2009.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/one_ofv1_stats_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/one_ofv1_stats_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/one_ofv2_fullstats_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/one_ofv2_fullstats_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/request_with_campaign_id.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/request_with_campaign_id.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/request_with_campaign_id_inner.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/request_with_campaign_id_inner.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/request_with_date.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/request_with_date.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/request_with_date_inner.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/request_with_date_inner.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/request_with_interval.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/request_with_interval.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/request_with_interval_inner.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/request_with_interval_inner.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response429.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response429.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_adv_error1.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_adv_error1.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_advert401.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_advert401.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_info_advert.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_info_advert.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_info_advert_intervals.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_info_advert_intervals.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_info_advert_nms.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_info_advert_nms.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_info_advert_params.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_info_advert_params.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_info_advert_type8.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_info_advert_type8.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_info_advert_type8_auto_params.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_info_advert_type8_auto_params.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_info_advert_type8_auto_params_active.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_info_advert_type8_auto_params_active.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_info_advert_type8_auto_params_menus.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_info_advert_type8_auto_params_menus.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_info_advert_type8_auto_params_nm_cpm.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_info_advert_type8_auto_params_nm_cpm.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_info_advert_type8_auto_params_sets.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_info_advert_type8_auto_params_sets.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_info_advert_type8_auto_params_subject.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_info_advert_type8_auto_params_subject.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_info_advert_type9.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_info_advert_type9.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_info_advert_type9_menus.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_info_advert_type9_menus.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_info_advert_type9_subject.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_info_advert_type9_subject.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_info_advert_type9_united_params.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_info_advert_type9_united_params.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_with_date.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_with_date.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_with_date_inner.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_with_date_inner.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_with_interval.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_with_interval.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_with_interval_inner.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_with_interval_inner.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/response_with_return.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/response_with_return.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/seacat_savead_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/seacat_savead_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/search_setexcluded_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/search_setexcluded_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/search_setphrase_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/search_setphrase_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/search_setplus_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/search_setplus_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/search_setstrong_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/search_setstrong_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/stat.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/stat.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/stat_date.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/stat_date.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/stat_interval.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/stat_interval.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/stat_interval_interval.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/stat_interval_interval.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/stats1.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/stats1.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/stats1_inner.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/stats1_inner.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/stats2.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/stats2.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/stats2_inner.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/stats2_inner.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/stats_blok1.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/stats_blok1.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/stats_blok2.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/stats_blok2.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/v0_allcpm_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/v0_allcpm_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/v0_cpm_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/v0_cpm_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/v0_rename_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/v0_rename_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/v1_savead_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/v1_savead_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/v1_stats_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/v1_stats_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/models/v2_fullstats_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/models/v2_fullstats_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/promotion/rest.py` & `wildberries_api_client-0.1.9/wildberries_api_client/promotion/rest.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/recommendations/__init__.py` & `wildberries_api_client-0.1.9/wildberries_api_client/recommendations/__init__.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/recommendations/api/rekomendacii_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/recommendations/api/rekomendacii_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/recommendations/api_client.py` & `wildberries_api_client-0.1.9/wildberries_api_client/recommendations/api_client.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/recommendations/configuration.py` & `wildberries_api_client-0.1.9/wildberries_api_client/recommendations/configuration.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/recommendations/models/__init__.py` & `wildberries_api_client-0.1.9/wildberries_api_client/recommendations/models/__init__.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/recommendations/models/inline_response200.py` & `wildberries_api_client-0.1.9/wildberries_api_client/recommendations/models/inline_response200.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/recommendations/models/inline_response200_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/recommendations/models/inline_response200_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/recommendations/models/v1_del_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/recommendations/models/v1_del_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/recommendations/models/v1_ins_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/recommendations/models/v1_ins_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/recommendations/models/v1_set_body.py` & `wildberries_api_client-0.1.9/wildberries_api_client/recommendations/models/v1_set_body.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/recommendations/rest.py` & `wildberries_api_client-0.1.9/wildberries_api_client/recommendations/rest.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/setup.py` & `wildberries_api_client-0.1.9/wildberries_api_client/setup.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/statistics/__init__.py` & `wildberries_api_client-0.1.9/wildberries_api_client/statistics/__init__.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/statistics/api/otlohennaa_generacia_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/statistics/api/otlohennaa_generacia_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/statistics/api/statistika_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/statistics/api/statistika_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/statistics/api_client.py` & `wildberries_api_client-0.1.9/wildberries_api_client/statistics/api_client.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/statistics/configuration.py` & `wildberries_api_client-0.1.9/wildberries_api_client/statistics/configuration.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/__init__.py` & `wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/__init__.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/create_task_request.py` & `wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/create_task_request.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/create_task_request_paid_storage.py` & `wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/create_task_request_paid_storage.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/create_task_request_paid_storage_params.py` & `wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/create_task_request_paid_storage_params.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/create_task_response.py` & `wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/create_task_response.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/create_task_response_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/create_task_response_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/detail_report_item.py` & `wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/detail_report_item.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/download_request.py` & `wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/download_request.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/error_response.py` & `wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/error_response.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/get_tasks_request.py` & `wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/get_tasks_request.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/get_tasks_response.py` & `wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/get_tasks_response.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/get_tasks_response_bytes_error.py` & `wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/get_tasks_response_bytes_error.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/get_tasks_response_bytes_error_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/get_tasks_response_bytes_error_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/get_tasks_response_bytes_error_data_tasks.py` & `wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/get_tasks_response_bytes_error_data_tasks.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/get_tasks_response_data.py` & `wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/get_tasks_response_data.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/incomes_item.py` & `wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/incomes_item.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/inline_response200.py` & `wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/inline_response200.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/inline_response429.py` & `wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/inline_response429.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/one_of_create_task_request.py` & `wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/one_of_create_task_request.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/one_ofinline_response200.py` & `wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/one_ofinline_response200.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/one_ofinline_response429.py` & `wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/one_ofinline_response429.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/orders_item.py` & `wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/orders_item.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/response429.py` & `wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/response429.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/response_error_statistics.py` & `wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/response_error_statistics.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/response_paid_storage.py` & `wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/response_paid_storage.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/response_paid_storage_inner.py` & `wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/response_paid_storage_inner.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/sales_item.py` & `wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/sales_item.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/statistics/models/stocks_item.py` & `wildberries_api_client-0.1.9/wildberries_api_client/statistics/models/stocks_item.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/statistics/rest.py` & `wildberries_api_client-0.1.9/wildberries_api_client/statistics/rest.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/tariffs/__init__.py` & `wildberries_api_client-0.1.9/wildberries_api_client/tariffs/__init__.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/tariffs/api/koefficienty_skladov_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/tariffs/api/koefficienty_skladov_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/tariffs/api/stoimost_vozvrata_prodavcu_api.py` & `wildberries_api_client-0.1.9/wildberries_api_client/tariffs/api/stoimost_vozvrata_prodavcu_api.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/tariffs/api_client.py` & `wildberries_api_client-0.1.9/wildberries_api_client/tariffs/api_client.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/tariffs/configuration.py` & `wildberries_api_client-0.1.9/wildberries_api_client/tariffs/configuration.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/tariffs/models/__init__.py` & `wildberries_api_client-0.1.9/wildberries_api_client/tariffs/models/__init__.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/tariffs/models/models_return_tariffs_response.py` & `wildberries_api_client-0.1.9/wildberries_api_client/tariffs/models/models_return_tariffs_response.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/tariffs/models/models_tariffs_box_response.py` & `wildberries_api_client-0.1.9/wildberries_api_client/tariffs/models/models_tariffs_box_response.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/tariffs/models/models_tariffs_pallet_response.py` & `wildberries_api_client-0.1.9/wildberries_api_client/tariffs/models/models_tariffs_pallet_response.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/tariffs/models/models_warehouse_box_rates.py` & `wildberries_api_client-0.1.9/wildberries_api_client/tariffs/models/models_warehouse_box_rates.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/tariffs/models/models_warehouse_pallet_rates.py` & `wildberries_api_client-0.1.9/wildberries_api_client/tariffs/models/models_warehouse_pallet_rates.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/tariffs/models/models_warehouse_return_rates.py` & `wildberries_api_client-0.1.9/wildberries_api_client/tariffs/models/models_warehouse_return_rates.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/tariffs/models/models_warehouses_box_rates.py` & `wildberries_api_client-0.1.9/wildberries_api_client/tariffs/models/models_warehouses_box_rates.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/tariffs/models/models_warehouses_pallet_rates.py` & `wildberries_api_client-0.1.9/wildberries_api_client/tariffs/models/models_warehouses_pallet_rates.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/tariffs/models/models_warehouses_return_rates.py` & `wildberries_api_client-0.1.9/wildberries_api_client/tariffs/models/models_warehouses_return_rates.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/tariffs/models/return_tariffs_response.py` & `wildberries_api_client-0.1.9/wildberries_api_client/tariffs/models/return_tariffs_response.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/tariffs/models/tariffs_box_response.py` & `wildberries_api_client-0.1.9/wildberries_api_client/tariffs/models/tariffs_box_response.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/tariffs/models/tariffs_pallet_response.py` & `wildberries_api_client-0.1.9/wildberries_api_client/tariffs/models/tariffs_pallet_response.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/wildberries_api_client/tariffs/rest.py` & `wildberries_api_client-0.1.9/wildberries_api_client/tariffs/rest.py`

 * *Files identical despite different names*

### Comparing `wildberries_api_client-0.1.8/PKG-INFO` & `wildberries_api_client-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wildberries-api-client
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 License: MIT
 Author: letby
 Author-email: fvahit2@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

