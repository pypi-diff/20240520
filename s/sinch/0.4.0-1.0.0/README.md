# Comparing `tmp/sinch-0.4.0.tar.gz` & `tmp/sinch-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinch-0.4.0.tar", max compression
+gzip compressed data, was "sinch-1.0.0.tar", max compression
```

## Comparing `sinch-0.4.0.tar` & `sinch-1.0.0.tar`

### file list

```diff
@@ -1,202 +1,244 @@
--rw-r--r--   0        0        0    11357 2023-03-22 17:32:22.871176 sinch-0.4.0/LICENSE
--rw-r--r--   0        0        0     5263 2024-03-27 21:03:02.055866 sinch-0.4.0/README.md
--rw-r--r--   0        0        0     1068 2024-03-27 21:03:52.491467 sinch-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      297 2024-03-27 21:04:09.454890 sinch-0.4.0/sinch/__init__.py
--rw-r--r--   0        0        0        0 2023-03-22 17:32:23.035728 sinch-0.4.0/sinch/core/__init__.py
--rw-r--r--   0        0        0        0 2023-03-22 17:32:23.037629 sinch-0.4.0/sinch/core/adapters/__init__.py
--rw-r--r--   0        0        0     1999 2024-02-05 14:52:20.682400 sinch-0.4.0/sinch/core/adapters/asyncio_http_adapter.py
--rw-r--r--   0        0        0     1767 2024-02-05 14:52:20.683289 sinch-0.4.0/sinch/core/adapters/requests_http_transport.py
--rw-r--r--   0        0        0        0 2023-03-22 17:32:23.034141 sinch-0.4.0/sinch/core/clients/__init__.py
--rw-r--r--   0        0        0     1773 2024-03-27 21:03:02.057296 sinch-0.4.0/sinch/core/clients/sinch_client_async.py
--rw-r--r--   0        0        0     1112 2024-03-27 21:03:02.057496 sinch-0.4.0/sinch/core/clients/sinch_client_base.py
--rw-r--r--   0        0        0     4160 2024-03-26 14:14:39.190172 sinch-0.4.0/sinch/core/clients/sinch_client_configuration.py
--rw-r--r--   0        0        0     1697 2024-03-27 21:03:02.057690 sinch-0.4.0/sinch/core/clients/sinch_client_sync.py
--rw-r--r--   0        0        0      605 2024-02-05 14:52:20.688233 sinch-0.4.0/sinch/core/endpoint.py
--rw-r--r--   0        0        0      237 2024-02-05 14:52:20.689123 sinch-0.4.0/sinch/core/enums.py
--rw-r--r--   0        0        0      342 2024-02-05 14:52:20.689975 sinch-0.4.0/sinch/core/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-22 17:32:23.036538 sinch-0.4.0/sinch/core/models/__init__.py
--rw-r--r--   0        0        0      359 2024-03-19 22:35:35.576292 sinch-0.4.0/sinch/core/models/base_model.py
--rw-r--r--   0        0        0      196 2024-02-05 14:52:20.691349 sinch-0.4.0/sinch/core/models/http_request.py
--rw-r--r--   0        0        0      121 2023-03-22 17:32:23.036376 sinch-0.4.0/sinch/core/models/http_response.py
--rw-r--r--   0        0        0     4296 2024-02-05 14:52:20.691975 sinch-0.4.0/sinch/core/pagination.py
--rw-r--r--   0        0        0        0 2023-03-22 17:32:23.039761 sinch-0.4.0/sinch/core/ports/__init__.py
--rw-r--r--   0        0        0     5223 2024-02-05 14:52:20.693270 sinch-0.4.0/sinch/core/ports/http_transport.py
--rw-r--r--   0        0        0     1947 2024-02-02 10:49:49.714988 sinch-0.4.0/sinch/core/signature.py
--rw-r--r--   0        0        0     1868 2024-02-05 14:52:20.694048 sinch-0.4.0/sinch/core/token_manager.py
--rw-r--r--   0        0        0        0 2024-03-15 18:21:43.126059 sinch-0.4.0/sinch/domains/__init__.py
--rw-r--r--   0        0        0      797 2023-03-22 17:32:22.998271 sinch-0.4.0/sinch/domains/authentication/__init__.py
--rw-r--r--   0        0        0        0 2023-03-22 17:32:22.996552 sinch-0.4.0/sinch/domains/authentication/endpoints/__init__.py
--rw-r--r--   0        0        0     1346 2024-02-05 14:52:20.694827 sinch-0.4.0/sinch/domains/authentication/endpoints/oauth.py
--rw-r--r--   0        0        0      107 2023-03-22 17:32:22.999421 sinch-0.4.0/sinch/domains/authentication/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-22 17:32:22.998813 sinch-0.4.0/sinch/domains/authentication/models/__init__.py
--rw-r--r--   0        0        0      214 2023-03-22 17:32:22.999139 sinch-0.4.0/sinch/domains/authentication/models/authentication.py
--rw-r--r--   0        0        0    40613 2024-02-05 14:52:20.695759 sinch-0.4.0/sinch/domains/conversation/__init__.py
--rw-r--r--   0        0        0        0 2023-03-22 17:32:23.007641 sinch-0.4.0/sinch/domains/conversation/endpoints/__init__.py
--rw-r--r--   0        0        0        0 2023-03-22 17:32:23.005910 sinch-0.4.0/sinch/domains/conversation/endpoints/app/__init__.py
--rw-r--r--   0        0        0     1923 2024-02-05 14:52:20.696486 sinch-0.4.0/sinch/domains/conversation/endpoints/app/create_app.py
--rw-r--r--   0        0        0     1309 2024-02-05 14:52:20.697344 sinch-0.4.0/sinch/domains/conversation/endpoints/app/delete_app.py
--rw-r--r--   0        0        0     1844 2024-02-05 14:52:20.697985 sinch-0.4.0/sinch/domains/conversation/endpoints/app/get_app.py
--rw-r--r--   0        0        0     1851 2024-02-05 14:52:20.698513 sinch-0.4.0/sinch/domains/conversation/endpoints/app/list_apps.py
--rw-r--r--   0        0        0     2212 2024-02-05 14:52:20.699033 sinch-0.4.0/sinch/domains/conversation/endpoints/app/update_app.py
--rw-r--r--   0        0        0     1518 2024-02-05 14:52:20.699864 sinch-0.4.0/sinch/domains/conversation/endpoints/capability.py
--rw-r--r--   0        0        0        0 2023-03-22 17:32:23.002890 sinch-0.4.0/sinch/domains/conversation/endpoints/contact/__init__.py
--rw-r--r--   0        0        0     1793 2024-02-05 14:52:20.700683 sinch-0.4.0/sinch/domains/conversation/endpoints/contact/create_contact.py
--rw-r--r--   0        0        0     1194 2024-02-05 14:52:20.701291 sinch-0.4.0/sinch/domains/conversation/endpoints/contact/delete_contact.py
--rw-r--r--   0        0        0     1451 2024-02-05 14:52:20.702142 sinch-0.4.0/sinch/domains/conversation/endpoints/contact/get_channel_profile.py
--rw-r--r--   0        0        0     1721 2024-02-05 14:52:20.702759 sinch-0.4.0/sinch/domains/conversation/endpoints/contact/get_contact.py
--rw-r--r--   0        0        0     2054 2024-02-05 14:52:20.703414 sinch-0.4.0/sinch/domains/conversation/endpoints/contact/list_contact.py
--rw-r--r--   0        0        0     1416 2024-02-05 14:52:20.704012 sinch-0.4.0/sinch/domains/conversation/endpoints/contact/merge_contacts.py
--rw-r--r--   0        0        0     1406 2024-02-05 14:52:20.706455 sinch-0.4.0/sinch/domains/conversation/endpoints/contact/update_contact.py
--rw-r--r--   0        0        0        0 2023-03-22 17:32:23.015785 sinch-0.4.0/sinch/domains/conversation/endpoints/conversation/__init__.py
--rw-r--r--   0        0        0     1751 2024-02-05 14:52:20.707197 sinch-0.4.0/sinch/domains/conversation/endpoints/conversation/create_conversation.py
--rw-r--r--   0        0        0     1354 2024-02-05 14:52:20.707833 sinch-0.4.0/sinch/domains/conversation/endpoints/conversation/delete_conversation.py
--rw-r--r--   0        0        0     1735 2024-02-05 14:52:20.708378 sinch-0.4.0/sinch/domains/conversation/endpoints/conversation/get_conversation.py
--rw-r--r--   0        0        0     1469 2024-02-05 14:52:20.709050 sinch-0.4.0/sinch/domains/conversation/endpoints/conversation/inject_message_to_conversation.py
--rw-r--r--   0        0        0     2575 2024-02-05 14:52:20.710102 sinch-0.4.0/sinch/domains/conversation/endpoints/conversation/list_conversations.py
--rw-r--r--   0        0        0     1341 2024-02-05 14:52:20.711407 sinch-0.4.0/sinch/domains/conversation/endpoints/conversation/stop_conversation.py
--rw-r--r--   0        0        0     1882 2024-02-05 14:52:20.711934 sinch-0.4.0/sinch/domains/conversation/endpoints/conversation/update_conversation.py
--rw-r--r--   0        0        0      502 2023-03-22 17:32:23.010138 sinch-0.4.0/sinch/domains/conversation/endpoints/conversation_endpoint.py
--rw-r--r--   0        0        0     1414 2024-02-05 14:52:20.713236 sinch-0.4.0/sinch/domains/conversation/endpoints/events.py
--rw-r--r--   0        0        0        0 2023-03-22 17:32:23.009079 sinch-0.4.0/sinch/domains/conversation/endpoints/message/__init__.py
--rw-r--r--   0        0        0     1469 2024-02-05 14:52:20.714793 sinch-0.4.0/sinch/domains/conversation/endpoints/message/delete_message.py
--rw-r--r--   0        0        0     1986 2024-02-05 14:52:20.717035 sinch-0.4.0/sinch/domains/conversation/endpoints/message/get_message.py
--rw-r--r--   0        0        0     3150 2024-02-05 14:52:20.717636 sinch-0.4.0/sinch/domains/conversation/endpoints/message/list_message.py
--rw-r--r--   0        0        0     1395 2024-02-05 14:52:20.718772 sinch-0.4.0/sinch/domains/conversation/endpoints/message/send_message.py
--rw-r--r--   0        0        0     1654 2024-02-05 14:52:20.719387 sinch-0.4.0/sinch/domains/conversation/endpoints/opt_in.py
--rw-r--r--   0        0        0     1664 2024-02-05 14:52:20.720008 sinch-0.4.0/sinch/domains/conversation/endpoints/opt_out.py
--rw-r--r--   0        0        0        0 2023-03-22 17:32:23.011410 sinch-0.4.0/sinch/domains/conversation/endpoints/templates/__init__.py
--rw-r--r--   0        0        0     1721 2024-02-05 14:52:20.720641 sinch-0.4.0/sinch/domains/conversation/endpoints/templates/create_template.py
--rw-r--r--   0        0        0     1342 2024-02-05 14:52:20.721716 sinch-0.4.0/sinch/domains/conversation/endpoints/templates/delete_template.py
--rw-r--r--   0        0        0     1696 2024-02-05 14:52:20.722579 sinch-0.4.0/sinch/domains/conversation/endpoints/templates/get_template.py
--rw-r--r--   0        0        0     1748 2024-02-05 14:52:20.723099 sinch-0.4.0/sinch/domains/conversation/endpoints/templates/list_templates.py
--rw-r--r--   0        0        0     1836 2024-02-05 14:52:20.724017 sinch-0.4.0/sinch/domains/conversation/endpoints/templates/update_template.py
--rw-r--r--   0        0        0     1451 2024-02-05 14:52:20.724765 sinch-0.4.0/sinch/domains/conversation/endpoints/transcode.py
--rw-r--r--   0        0        0        0 2023-03-22 17:32:23.014523 sinch-0.4.0/sinch/domains/conversation/endpoints/webhooks/__init__.py
--rw-r--r--   0        0        0     1643 2024-02-05 14:52:20.725382 sinch-0.4.0/sinch/domains/conversation/endpoints/webhooks/create_webhook.py
--rw-r--r--   0        0        0     1308 2024-02-05 14:52:20.728621 sinch-0.4.0/sinch/domains/conversation/endpoints/webhooks/delete_webhook.py
--rw-r--r--   0        0        0     1612 2024-02-05 14:52:20.729731 sinch-0.4.0/sinch/domains/conversation/endpoints/webhooks/get_webhook.py
--rw-r--r--   0        0        0     1793 2024-02-05 14:52:20.730906 sinch-0.4.0/sinch/domains/conversation/endpoints/webhooks/list_webhooks.py
--rw-r--r--   0        0        0     1754 2024-02-05 14:52:20.731594 sinch-0.4.0/sinch/domains/conversation/endpoints/webhooks/update_webhook.py
--rw-r--r--   0        0        0      728 2023-03-22 17:32:23.000317 sinch-0.4.0/sinch/domains/conversation/enums.py
--rw-r--r--   0        0        0      105 2023-03-22 17:32:23.032595 sinch-0.4.0/sinch/domains/conversation/exceptions.py
--rw-r--r--   0        0        0     1843 2023-03-22 17:32:23.025158 sinch-0.4.0/sinch/domains/conversation/models/__init__.py
--rw-r--r--   0        0        0        0 2023-03-22 17:32:23.022203 sinch-0.4.0/sinch/domains/conversation/models/app/__init__.py
--rw-r--r--   0        0        0     1029 2023-03-22 17:32:23.022534 sinch-0.4.0/sinch/domains/conversation/models/app/requests.py
--rw-r--r--   0        0        0      606 2023-03-22 17:32:23.021990 sinch-0.4.0/sinch/domains/conversation/models/app/responses.py
--rw-r--r--   0        0        0        0 2023-03-22 17:32:23.023398 sinch-0.4.0/sinch/domains/conversation/models/capability/__init__.py
--rw-r--r--   0        0        0      231 2023-03-22 17:32:23.023720 sinch-0.4.0/sinch/domains/conversation/models/capability/requests.py
--rw-r--r--   0        0        0      218 2023-03-22 17:32:23.023214 sinch-0.4.0/sinch/domains/conversation/models/capability/responses.py
--rw-r--r--   0        0        0        0 2023-03-22 17:32:23.021092 sinch-0.4.0/sinch/domains/conversation/models/contact/__init__.py
--rw-r--r--   0        0        0     1418 2023-03-22 17:32:23.021408 sinch-0.4.0/sinch/domains/conversation/models/contact/requests.py
--rw-r--r--   0        0        0      852 2023-03-22 17:32:23.020912 sinch-0.4.0/sinch/domains/conversation/models/contact/responses.py
--rw-r--r--   0        0        0      292 2023-03-22 17:32:23.032015 sinch-0.4.0/sinch/domains/conversation/models/conversation/__init__.py
--rw-r--r--   0        0        0     1247 2023-03-22 17:32:23.032302 sinch-0.4.0/sinch/domains/conversation/models/conversation/requests.py
--rw-r--r--   0        0        0      782 2023-03-22 17:32:23.031696 sinch-0.4.0/sinch/domains/conversation/models/conversation/responses.py
--rw-r--r--   0        0        0        0 2023-03-22 17:32:23.030231 sinch-0.4.0/sinch/domains/conversation/models/event/__init__.py
--rw-r--r--   0        0        0      314 2023-03-22 17:32:23.030603 sinch-0.4.0/sinch/domains/conversation/models/event/requests.py
--rw-r--r--   0        0        0      197 2023-03-22 17:32:23.030043 sinch-0.4.0/sinch/domains/conversation/models/event/responses.py
--rw-r--r--   0        0        0        0 2023-03-22 17:32:23.026054 sinch-0.4.0/sinch/domains/conversation/models/message/__init__.py
--rw-r--r--   0        0        0     1060 2023-03-22 17:32:23.026459 sinch-0.4.0/sinch/domains/conversation/models/message/requests.py
--rw-r--r--   0        0        0      600 2023-03-22 17:32:23.025842 sinch-0.4.0/sinch/domains/conversation/models/message/responses.py
--rw-r--r--   0        0        0        0 2023-03-22 17:32:23.027339 sinch-0.4.0/sinch/domains/conversation/models/opt_in_opt_out/__init__.py
--rw-r--r--   0        0        0      458 2023-03-22 17:32:23.027648 sinch-0.4.0/sinch/domains/conversation/models/opt_in_opt_out/requests.py
--rw-r--r--   0        0        0      306 2023-03-22 17:32:23.027157 sinch-0.4.0/sinch/domains/conversation/models/opt_in_opt_out/responses.py
--rw-r--r--   0        0        0      291 2023-03-22 17:32:23.028553 sinch-0.4.0/sinch/domains/conversation/models/templates/__init__.py
--rw-r--r--   0        0        0      642 2023-03-22 17:32:23.029346 sinch-0.4.0/sinch/domains/conversation/models/templates/requests.py
--rw-r--r--   0        0        0      639 2023-03-22 17:32:23.028276 sinch-0.4.0/sinch/domains/conversation/models/templates/responses.py
--rw-r--r--   0        0        0        0 2023-03-22 17:32:23.024547 sinch-0.4.0/sinch/domains/conversation/models/transcoding/__init__.py
--rw-r--r--   0        0        0      260 2023-03-22 17:32:23.024870 sinch-0.4.0/sinch/domains/conversation/models/transcoding/requests.py
--rw-r--r--   0        0        0      192 2023-03-22 17:32:23.024366 sinch-0.4.0/sinch/domains/conversation/models/transcoding/responses.py
--rw-r--r--   0        0        0      276 2023-03-22 17:32:23.019781 sinch-0.4.0/sinch/domains/conversation/models/webhook/__init__.py
--rw-r--r--   0        0        0      740 2023-03-22 17:32:23.020120 sinch-0.4.0/sinch/domains/conversation/models/webhook/requests.py
--rw-r--r--   0        0        0      576 2023-03-22 17:32:23.019469 sinch-0.4.0/sinch/domains/conversation/models/webhook/responses.py
--rw-r--r--   0        0        0    12944 2024-02-05 14:52:20.733463 sinch-0.4.0/sinch/domains/numbers/__init__.py
--rw-r--r--   0        0        0        0 2023-03-22 17:32:22.970908 sinch-0.4.0/sinch/domains/numbers/endpoints/__init__.py
--rw-r--r--   0        0        0        0 2023-09-04 14:27:43.268520 sinch-0.4.0/sinch/domains/numbers/endpoints/active/__init__.py
--rw-r--r--   0        0        0     1990 2024-02-05 14:52:20.734796 sinch-0.4.0/sinch/domains/numbers/endpoints/active/get_number_configuration.py
--rw-r--r--   0        0        0     2921 2024-02-05 14:52:20.736614 sinch-0.4.0/sinch/domains/numbers/endpoints/active/list_active_numbers_for_project.py
--rw-r--r--   0        0        0     2009 2024-02-05 14:52:20.737576 sinch-0.4.0/sinch/domains/numbers/endpoints/active/release_number_from_project.py
--rw-r--r--   0        0        0     2133 2024-02-05 14:52:20.738402 sinch-0.4.0/sinch/domains/numbers/endpoints/active/update_number_configuration.py
--rw-r--r--   0        0        0        0 2023-09-04 14:27:43.269937 sinch-0.4.0/sinch/domains/numbers/endpoints/available/__init__.py
--rw-r--r--   0        0        0     1478 2024-02-05 14:52:20.739731 sinch-0.4.0/sinch/domains/numbers/endpoints/available/activate_number.py
--rw-r--r--   0        0        0     2604 2024-02-05 14:52:20.740632 sinch-0.4.0/sinch/domains/numbers/endpoints/available/list_available_numbers.py
--rw-r--r--   0        0        0     2867 2024-02-05 14:52:20.741488 sinch-0.4.0/sinch/domains/numbers/endpoints/available/rent_any_number.py
--rw-r--r--   0        0        0     1802 2024-02-05 14:52:20.742314 sinch-0.4.0/sinch/domains/numbers/endpoints/available/search_for_number.py
--rw-r--r--   0        0        0        0 2024-02-02 10:49:49.715757 sinch-0.4.0/sinch/domains/numbers/endpoints/callbacks/__init__.py
--rw-r--r--   0        0        0     1146 2024-02-05 14:52:20.743335 sinch-0.4.0/sinch/domains/numbers/endpoints/callbacks/get_configuration.py
--rw-r--r--   0        0        0     1440 2024-02-05 14:52:20.744589 sinch-0.4.0/sinch/domains/numbers/endpoints/callbacks/update_configuration.py
--rw-r--r--   0        0        0      482 2023-03-22 17:32:22.972748 sinch-0.4.0/sinch/domains/numbers/endpoints/numbers_endpoint.py
--rw-r--r--   0        0        0        0 2023-09-04 14:27:43.271177 sinch-0.4.0/sinch/domains/numbers/endpoints/regions/__init__.py
--rw-r--r--   0        0        0     1899 2024-02-05 14:52:20.747234 sinch-0.4.0/sinch/domains/numbers/endpoints/regions/list_available_regions.py
--rw-r--r--   0        0        0      186 2023-03-22 17:32:22.969507 sinch-0.4.0/sinch/domains/numbers/enums.py
--rw-r--r--   0        0        0      100 2023-03-22 17:32:22.975582 sinch-0.4.0/sinch/domains/numbers/exceptions.py
--rw-r--r--   0        0        0      916 2023-09-04 14:27:43.271965 sinch-0.4.0/sinch/domains/numbers/models/__init__.py
--rw-r--r--   0        0        0      500 2023-09-04 14:27:43.272197 sinch-0.4.0/sinch/domains/numbers/models/active/__init__.py
--rw-r--r--   0        0        0      711 2024-02-05 14:52:20.752181 sinch-0.4.0/sinch/domains/numbers/models/active/requests.py
--rw-r--r--   0        0        0      556 2023-09-04 14:27:43.272975 sinch-0.4.0/sinch/domains/numbers/models/active/responses.py
--rw-r--r--   0        0        0        0 2023-09-04 14:27:43.273170 sinch-0.4.0/sinch/domains/numbers/models/available/__init__.py
--rw-r--r--   0        0        0      776 2023-09-05 15:42:43.238636 sinch-0.4.0/sinch/domains/numbers/models/available/requests.py
--rw-r--r--   0        0        0      826 2023-09-05 15:42:43.239803 sinch-0.4.0/sinch/domains/numbers/models/available/responses.py
--rw-r--r--   0        0        0        0 2024-02-02 10:49:49.716920 sinch-0.4.0/sinch/domains/numbers/models/callbacks/__init__.py
--rw-r--r--   0        0        0      204 2024-02-02 10:49:49.717548 sinch-0.4.0/sinch/domains/numbers/models/callbacks/requests.py
--rw-r--r--   0        0        0      422 2024-02-02 10:49:49.717914 sinch-0.4.0/sinch/domains/numbers/models/callbacks/responses.py
--rw-r--r--   0        0        0      192 2023-09-04 14:27:43.274147 sinch-0.4.0/sinch/domains/numbers/models/regions/__init__.py
--rw-r--r--   0        0        0      223 2023-09-04 14:27:43.274387 sinch-0.4.0/sinch/domains/numbers/models/regions/requests.py
--rw-r--r--   0        0        0      272 2023-09-04 14:27:43.274643 sinch-0.4.0/sinch/domains/numbers/models/regions/responses.py
--rw-r--r--   0        0        0    22047 2024-02-05 14:52:20.753177 sinch-0.4.0/sinch/domains/sms/__init__.py
--rw-r--r--   0        0        0        0 2023-03-22 17:32:22.979555 sinch-0.4.0/sinch/domains/sms/endpoints/__init__.py
--rw-r--r--   0        0        0        0 2023-03-22 17:32:22.985941 sinch-0.4.0/sinch/domains/sms/endpoints/batches/__init__.py
--rw-r--r--   0        0        0     1785 2024-02-05 14:52:20.754161 sinch-0.4.0/sinch/domains/sms/endpoints/batches/cancel_batch.py
--rw-r--r--   0        0        0     1833 2024-02-05 14:52:20.754802 sinch-0.4.0/sinch/domains/sms/endpoints/batches/get_batch.py
--rw-r--r--   0        0        0     2119 2024-02-05 14:52:20.755323 sinch-0.4.0/sinch/domains/sms/endpoints/batches/list_batches.py
--rw-r--r--   0        0        0     1912 2024-02-05 14:52:20.756145 sinch-0.4.0/sinch/domains/sms/endpoints/batches/replace_batch.py
--rw-r--r--   0        0        0     1832 2024-02-05 14:52:20.757708 sinch-0.4.0/sinch/domains/sms/endpoints/batches/send_batch.py
--rw-r--r--   0        0        0     1746 2024-02-05 14:52:20.758398 sinch-0.4.0/sinch/domains/sms/endpoints/batches/send_batch_dry_run.py
--rw-r--r--   0        0        0     1355 2024-02-05 14:52:20.759101 sinch-0.4.0/sinch/domains/sms/endpoints/batches/send_delivery_feedback.py
--rw-r--r--   0        0        0     1966 2024-02-05 14:52:20.759556 sinch-0.4.0/sinch/domains/sms/endpoints/batches/update_batch.py
--rw-r--r--   0        0        0        0 2023-03-22 17:32:22.977507 sinch-0.4.0/sinch/domains/sms/endpoints/delivery_reports/__init__.py
--rw-r--r--   0        0        0     2445 2024-02-05 14:52:20.760105 sinch-0.4.0/sinch/domains/sms/endpoints/delivery_reports/get_all_delivery_reports_for_project.py
--rw-r--r--   0        0        0     1966 2024-02-05 14:52:20.760619 sinch-0.4.0/sinch/domains/sms/endpoints/delivery_reports/get_delivery_report_for_batch.py
--rw-r--r--   0        0        0     2030 2024-02-05 14:52:20.761246 sinch-0.4.0/sinch/domains/sms/endpoints/delivery_reports/get_delivery_report_for_number.py
--rw-r--r--   0        0        0        0 2023-03-22 17:32:22.980432 sinch-0.4.0/sinch/domains/sms/endpoints/groups/__init__.py
--rw-r--r--   0        0        0     1558 2024-02-05 14:52:20.761911 sinch-0.4.0/sinch/domains/sms/endpoints/groups/create_group.py
--rw-r--r--   0        0        0     1190 2024-02-05 14:52:20.762375 sinch-0.4.0/sinch/domains/sms/endpoints/groups/delete_group.py
--rw-r--r--   0        0        0     1524 2024-02-05 14:52:20.762844 sinch-0.4.0/sinch/domains/sms/endpoints/groups/get_group.py
--rw-r--r--   0        0        0     1307 2024-02-05 14:52:20.763481 sinch-0.4.0/sinch/domains/sms/endpoints/groups/get_phone_numbers_for_group.py
--rw-r--r--   0        0        0     1880 2024-02-05 14:52:20.764742 sinch-0.4.0/sinch/domains/sms/endpoints/groups/list_groups.py
--rw-r--r--   0        0        0     1690 2024-02-05 14:52:20.765346 sinch-0.4.0/sinch/domains/sms/endpoints/groups/replace_group.py
--rw-r--r--   0        0        0     1660 2024-02-05 14:52:20.766092 sinch-0.4.0/sinch/domains/sms/endpoints/groups/update_group.py
--rw-r--r--   0        0        0        0 2023-03-22 17:32:22.984281 sinch-0.4.0/sinch/domains/sms/endpoints/inbounds/__init__.py
--rw-r--r--   0        0        0     1632 2024-02-05 14:52:20.767032 sinch-0.4.0/sinch/domains/sms/endpoints/inbounds/get_incoming_message.py
--rw-r--r--   0        0        0     2056 2024-02-05 14:52:20.767674 sinch-0.4.0/sinch/domains/sms/endpoints/inbounds/list_incoming_messages.py
--rw-r--r--   0        0        0      450 2024-02-01 15:15:33.837832 sinch-0.4.0/sinch/domains/sms/endpoints/sms_endpoint.py
--rw-r--r--   0        0        0        0 2023-03-22 17:32:22.976341 sinch-0.4.0/sinch/domains/sms/enums.py
--rw-r--r--   0        0        0       96 2023-03-22 17:32:22.995387 sinch-0.4.0/sinch/domains/sms/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-22 17:32:22.990043 sinch-0.4.0/sinch/domains/sms/models/__init__.py
--rw-r--r--   0        0        0      483 2023-03-22 17:32:22.994761 sinch-0.4.0/sinch/domains/sms/models/batches/__init__.py
--rw-r--r--   0        0        0     2141 2024-03-26 14:14:43.445958 sinch-0.4.0/sinch/domains/sms/models/batches/requests.py
--rw-r--r--   0        0        0     1012 2023-08-02 08:44:18.971175 sinch-0.4.0/sinch/domains/sms/models/batches/responses.py
--rw-r--r--   0        0        0      385 2023-03-22 17:32:22.989331 sinch-0.4.0/sinch/domains/sms/models/delivery_reports/__init__.py
--rw-r--r--   0        0        0      569 2023-03-22 17:32:22.989786 sinch-0.4.0/sinch/domains/sms/models/delivery_reports/requests.py
--rw-r--r--   0        0        0      711 2023-03-22 17:32:22.989003 sinch-0.4.0/sinch/domains/sms/models/delivery_reports/responses.py
--rw-r--r--   0        0        0      261 2023-03-22 17:32:22.991445 sinch-0.4.0/sinch/domains/sms/models/groups/__init__.py
--rw-r--r--   0        0        0      919 2023-03-22 17:32:22.991894 sinch-0.4.0/sinch/domains/sms/models/groups/requests.py
--rw-r--r--   0        0        0      720 2023-03-22 17:32:22.991057 sinch-0.4.0/sinch/domains/sms/models/groups/responses.py
--rw-r--r--   0        0        0      293 2023-03-22 17:32:22.993119 sinch-0.4.0/sinch/domains/sms/models/inbounds/__init__.py
--rw-r--r--   0        0        0      392 2023-03-22 17:32:22.993554 sinch-0.4.0/sinch/domains/sms/models/inbounds/requests.py
--rw-r--r--   0        0        0      399 2023-03-22 17:32:22.992745 sinch-0.4.0/sinch/domains/sms/models/inbounds/responses.py
--rw-r--r--   0        0        0     4972 2024-02-02 10:49:49.719132 sinch-0.4.0/sinch/domains/verification/__init__.py
--rw-r--r--   0        0        0        0 2024-02-02 10:49:49.719289 sinch-0.4.0/sinch/domains/verification/endpoints/__init__.py
--rw-r--r--   0        0        0     1641 2024-03-19 23:01:52.607191 sinch-0.4.0/sinch/domains/verification/endpoints/get_verification_by_id.py
--rw-r--r--   0        0        0     1753 2024-02-05 14:52:20.771002 sinch-0.4.0/sinch/domains/verification/endpoints/get_verification_by_identity.py
--rw-r--r--   0        0        0     1711 2024-02-05 14:52:20.772598 sinch-0.4.0/sinch/domains/verification/endpoints/get_verification_by_reference.py
--rw-r--r--   0        0        0     1737 2024-02-05 14:52:20.773884 sinch-0.4.0/sinch/domains/verification/endpoints/report_verification_using_id.py
--rw-r--r--   0        0        0     1795 2024-02-05 14:52:20.774995 sinch-0.4.0/sinch/domains/verification/endpoints/report_verification_using_identity.py
--rw-r--r--   0        0        0     2181 2024-03-26 14:14:39.190671 sinch-0.4.0/sinch/domains/verification/endpoints/start_verification.py
--rw-r--r--   0        0        0      489 2024-02-02 10:49:49.723010 sinch-0.4.0/sinch/domains/verification/endpoints/verification_endpoint.py
--rw-r--r--   0        0        0      322 2024-02-02 10:49:49.723498 sinch-0.4.0/sinch/domains/verification/enums.py
--rw-r--r--   0        0        0      105 2024-03-04 11:35:49.951830 sinch-0.4.0/sinch/domains/verification/exceptions.py
--rw-r--r--   0        0        0        0 2024-02-02 10:49:49.724072 sinch-0.4.0/sinch/domains/verification/models/__init__.py
--rw-r--r--   0        0        0      922 2024-02-02 10:49:49.724849 sinch-0.4.0/sinch/domains/verification/models/requests.py
--rw-r--r--   0        0        0     1519 2024-02-02 10:49:49.725245 sinch-0.4.0/sinch/domains/verification/models/responses.py
--rw-r--r--   0        0        0     6454 1970-01-01 00:00:00.000000 sinch-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-22 17:32:22.871176 sinch-1.0.0/LICENSE
+-rw-r--r--   0        0        0     5062 2024-05-20 18:24:11.846360 sinch-1.0.0/README.md
+-rw-r--r--   0        0        0     1068 2024-05-20 18:24:11.846794 sinch-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      297 2024-05-20 18:24:11.847216 sinch-1.0.0/sinch/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-22 17:32:23.035728 sinch-1.0.0/sinch/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-22 17:32:23.037629 sinch-1.0.0/sinch/core/adapters/__init__.py
+-rw-r--r--   0        0        0     1999 2024-02-05 14:52:20.682400 sinch-1.0.0/sinch/core/adapters/asyncio_http_adapter.py
+-rw-r--r--   0        0        0     1767 2024-02-05 14:52:20.683289 sinch-1.0.0/sinch/core/adapters/requests_http_transport.py
+-rw-r--r--   0        0        0        0 2023-03-22 17:32:23.034141 sinch-1.0.0/sinch/core/clients/__init__.py
+-rw-r--r--   0        0        0     1838 2024-05-14 13:11:24.172215 sinch-1.0.0/sinch/core/clients/sinch_client_async.py
+-rw-r--r--   0        0        0     1176 2024-05-14 13:11:24.172398 sinch-1.0.0/sinch/core/clients/sinch_client_base.py
+-rw-r--r--   0        0        0     4878 2024-05-14 13:11:24.172658 sinch-1.0.0/sinch/core/clients/sinch_client_configuration.py
+-rw-r--r--   0        0        0     1768 2024-05-14 13:11:24.172821 sinch-1.0.0/sinch/core/clients/sinch_client_sync.py
+-rw-r--r--   0        0        0      363 2024-05-14 13:11:24.173076 sinch-1.0.0/sinch/core/deserializers.py
+-rw-r--r--   0        0        0      605 2024-02-05 14:52:20.688233 sinch-1.0.0/sinch/core/endpoint.py
+-rw-r--r--   0        0        0      237 2024-02-05 14:52:20.689123 sinch-1.0.0/sinch/core/enums.py
+-rw-r--r--   0        0        0      342 2024-02-05 14:52:20.689975 sinch-1.0.0/sinch/core/exceptions.py
+-rw-r--r--   0        0        0        0 2023-03-22 17:32:23.036538 sinch-1.0.0/sinch/core/models/__init__.py
+-rw-r--r--   0        0        0      359 2024-03-19 22:35:35.576292 sinch-1.0.0/sinch/core/models/base_model.py
+-rw-r--r--   0        0        0      196 2024-02-05 14:52:20.691349 sinch-1.0.0/sinch/core/models/http_request.py
+-rw-r--r--   0        0        0      121 2023-03-22 17:32:23.036376 sinch-1.0.0/sinch/core/models/http_response.py
+-rw-r--r--   0        0        0     4296 2024-02-05 14:52:20.691975 sinch-1.0.0/sinch/core/pagination.py
+-rw-r--r--   0        0        0        0 2023-03-22 17:32:23.039761 sinch-1.0.0/sinch/core/ports/__init__.py
+-rw-r--r--   0        0        0     5223 2024-02-05 14:52:20.693270 sinch-1.0.0/sinch/core/ports/http_transport.py
+-rw-r--r--   0        0        0     1947 2024-02-02 10:49:49.714988 sinch-1.0.0/sinch/core/signature.py
+-rw-r--r--   0        0        0     1868 2024-02-05 14:52:20.694048 sinch-1.0.0/sinch/core/token_manager.py
+-rw-r--r--   0        0        0        0 2024-03-15 18:21:43.126059 sinch-1.0.0/sinch/domains/__init__.py
+-rw-r--r--   0        0        0      797 2023-03-22 17:32:22.998271 sinch-1.0.0/sinch/domains/authentication/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-22 17:32:22.996552 sinch-1.0.0/sinch/domains/authentication/endpoints/__init__.py
+-rw-r--r--   0        0        0     1346 2024-02-05 14:52:20.694827 sinch-1.0.0/sinch/domains/authentication/endpoints/oauth.py
+-rw-r--r--   0        0        0      107 2023-03-22 17:32:22.999421 sinch-1.0.0/sinch/domains/authentication/exceptions.py
+-rw-r--r--   0        0        0        0 2023-03-22 17:32:22.998813 sinch-1.0.0/sinch/domains/authentication/models/__init__.py
+-rw-r--r--   0        0        0      214 2023-03-22 17:32:22.999139 sinch-1.0.0/sinch/domains/authentication/models/authentication.py
+-rw-r--r--   0        0        0    40613 2024-02-05 14:52:20.695759 sinch-1.0.0/sinch/domains/conversation/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-22 17:32:23.007641 sinch-1.0.0/sinch/domains/conversation/endpoints/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-22 17:32:23.005910 sinch-1.0.0/sinch/domains/conversation/endpoints/app/__init__.py
+-rw-r--r--   0        0        0     1923 2024-02-05 14:52:20.696486 sinch-1.0.0/sinch/domains/conversation/endpoints/app/create_app.py
+-rw-r--r--   0        0        0     1309 2024-02-05 14:52:20.697344 sinch-1.0.0/sinch/domains/conversation/endpoints/app/delete_app.py
+-rw-r--r--   0        0        0     1844 2024-02-05 14:52:20.697985 sinch-1.0.0/sinch/domains/conversation/endpoints/app/get_app.py
+-rw-r--r--   0        0        0     1851 2024-02-05 14:52:20.698513 sinch-1.0.0/sinch/domains/conversation/endpoints/app/list_apps.py
+-rw-r--r--   0        0        0     2212 2024-02-05 14:52:20.699033 sinch-1.0.0/sinch/domains/conversation/endpoints/app/update_app.py
+-rw-r--r--   0        0        0     1518 2024-02-05 14:52:20.699864 sinch-1.0.0/sinch/domains/conversation/endpoints/capability.py
+-rw-r--r--   0        0        0        0 2023-03-22 17:32:23.002890 sinch-1.0.0/sinch/domains/conversation/endpoints/contact/__init__.py
+-rw-r--r--   0        0        0     1793 2024-02-05 14:52:20.700683 sinch-1.0.0/sinch/domains/conversation/endpoints/contact/create_contact.py
+-rw-r--r--   0        0        0     1194 2024-02-05 14:52:20.701291 sinch-1.0.0/sinch/domains/conversation/endpoints/contact/delete_contact.py
+-rw-r--r--   0        0        0     1451 2024-02-05 14:52:20.702142 sinch-1.0.0/sinch/domains/conversation/endpoints/contact/get_channel_profile.py
+-rw-r--r--   0        0        0     1721 2024-02-05 14:52:20.702759 sinch-1.0.0/sinch/domains/conversation/endpoints/contact/get_contact.py
+-rw-r--r--   0        0        0     2054 2024-02-05 14:52:20.703414 sinch-1.0.0/sinch/domains/conversation/endpoints/contact/list_contact.py
+-rw-r--r--   0        0        0     1416 2024-02-05 14:52:20.704012 sinch-1.0.0/sinch/domains/conversation/endpoints/contact/merge_contacts.py
+-rw-r--r--   0        0        0     1406 2024-02-05 14:52:20.706455 sinch-1.0.0/sinch/domains/conversation/endpoints/contact/update_contact.py
+-rw-r--r--   0        0        0        0 2023-03-22 17:32:23.015785 sinch-1.0.0/sinch/domains/conversation/endpoints/conversation/__init__.py
+-rw-r--r--   0        0        0     1751 2024-02-05 14:52:20.707197 sinch-1.0.0/sinch/domains/conversation/endpoints/conversation/create_conversation.py
+-rw-r--r--   0        0        0     1354 2024-02-05 14:52:20.707833 sinch-1.0.0/sinch/domains/conversation/endpoints/conversation/delete_conversation.py
+-rw-r--r--   0        0        0     1735 2024-02-05 14:52:20.708378 sinch-1.0.0/sinch/domains/conversation/endpoints/conversation/get_conversation.py
+-rw-r--r--   0        0        0     1469 2024-02-05 14:52:20.709050 sinch-1.0.0/sinch/domains/conversation/endpoints/conversation/inject_message_to_conversation.py
+-rw-r--r--   0        0        0     2575 2024-02-05 14:52:20.710102 sinch-1.0.0/sinch/domains/conversation/endpoints/conversation/list_conversations.py
+-rw-r--r--   0        0        0     1341 2024-02-05 14:52:20.711407 sinch-1.0.0/sinch/domains/conversation/endpoints/conversation/stop_conversation.py
+-rw-r--r--   0        0        0     1882 2024-02-05 14:52:20.711934 sinch-1.0.0/sinch/domains/conversation/endpoints/conversation/update_conversation.py
+-rw-r--r--   0        0        0      502 2023-03-22 17:32:23.010138 sinch-1.0.0/sinch/domains/conversation/endpoints/conversation_endpoint.py
+-rw-r--r--   0        0        0     1414 2024-02-05 14:52:20.713236 sinch-1.0.0/sinch/domains/conversation/endpoints/events.py
+-rw-r--r--   0        0        0        0 2023-03-22 17:32:23.009079 sinch-1.0.0/sinch/domains/conversation/endpoints/message/__init__.py
+-rw-r--r--   0        0        0     1469 2024-02-05 14:52:20.714793 sinch-1.0.0/sinch/domains/conversation/endpoints/message/delete_message.py
+-rw-r--r--   0        0        0     1986 2024-02-05 14:52:20.717035 sinch-1.0.0/sinch/domains/conversation/endpoints/message/get_message.py
+-rw-r--r--   0        0        0     3150 2024-02-05 14:52:20.717636 sinch-1.0.0/sinch/domains/conversation/endpoints/message/list_message.py
+-rw-r--r--   0        0        0     1395 2024-02-05 14:52:20.718772 sinch-1.0.0/sinch/domains/conversation/endpoints/message/send_message.py
+-rw-r--r--   0        0        0     1654 2024-02-05 14:52:20.719387 sinch-1.0.0/sinch/domains/conversation/endpoints/opt_in.py
+-rw-r--r--   0        0        0     1664 2024-02-05 14:52:20.720008 sinch-1.0.0/sinch/domains/conversation/endpoints/opt_out.py
+-rw-r--r--   0        0        0        0 2023-03-22 17:32:23.011410 sinch-1.0.0/sinch/domains/conversation/endpoints/templates/__init__.py
+-rw-r--r--   0        0        0     1721 2024-02-05 14:52:20.720641 sinch-1.0.0/sinch/domains/conversation/endpoints/templates/create_template.py
+-rw-r--r--   0        0        0     1342 2024-02-05 14:52:20.721716 sinch-1.0.0/sinch/domains/conversation/endpoints/templates/delete_template.py
+-rw-r--r--   0        0        0     1696 2024-02-05 14:52:20.722579 sinch-1.0.0/sinch/domains/conversation/endpoints/templates/get_template.py
+-rw-r--r--   0        0        0     1748 2024-02-05 14:52:20.723099 sinch-1.0.0/sinch/domains/conversation/endpoints/templates/list_templates.py
+-rw-r--r--   0        0        0     1836 2024-02-05 14:52:20.724017 sinch-1.0.0/sinch/domains/conversation/endpoints/templates/update_template.py
+-rw-r--r--   0        0        0     1451 2024-02-05 14:52:20.724765 sinch-1.0.0/sinch/domains/conversation/endpoints/transcode.py
+-rw-r--r--   0        0        0        0 2023-03-22 17:32:23.014523 sinch-1.0.0/sinch/domains/conversation/endpoints/webhooks/__init__.py
+-rw-r--r--   0        0        0     1643 2024-02-05 14:52:20.725382 sinch-1.0.0/sinch/domains/conversation/endpoints/webhooks/create_webhook.py
+-rw-r--r--   0        0        0     1308 2024-02-05 14:52:20.728621 sinch-1.0.0/sinch/domains/conversation/endpoints/webhooks/delete_webhook.py
+-rw-r--r--   0        0        0     1612 2024-02-05 14:52:20.729731 sinch-1.0.0/sinch/domains/conversation/endpoints/webhooks/get_webhook.py
+-rw-r--r--   0        0        0     1793 2024-02-05 14:52:20.730906 sinch-1.0.0/sinch/domains/conversation/endpoints/webhooks/list_webhooks.py
+-rw-r--r--   0        0        0     1754 2024-02-05 14:52:20.731594 sinch-1.0.0/sinch/domains/conversation/endpoints/webhooks/update_webhook.py
+-rw-r--r--   0        0        0      728 2023-03-22 17:32:23.000317 sinch-1.0.0/sinch/domains/conversation/enums.py
+-rw-r--r--   0        0        0      105 2023-03-22 17:32:23.032595 sinch-1.0.0/sinch/domains/conversation/exceptions.py
+-rw-r--r--   0        0        0     1843 2023-03-22 17:32:23.025158 sinch-1.0.0/sinch/domains/conversation/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-22 17:32:23.022203 sinch-1.0.0/sinch/domains/conversation/models/app/__init__.py
+-rw-r--r--   0        0        0     1029 2023-03-22 17:32:23.022534 sinch-1.0.0/sinch/domains/conversation/models/app/requests.py
+-rw-r--r--   0        0        0      606 2023-03-22 17:32:23.021990 sinch-1.0.0/sinch/domains/conversation/models/app/responses.py
+-rw-r--r--   0        0        0        0 2023-03-22 17:32:23.023398 sinch-1.0.0/sinch/domains/conversation/models/capability/__init__.py
+-rw-r--r--   0        0        0      231 2023-03-22 17:32:23.023720 sinch-1.0.0/sinch/domains/conversation/models/capability/requests.py
+-rw-r--r--   0        0        0      218 2023-03-22 17:32:23.023214 sinch-1.0.0/sinch/domains/conversation/models/capability/responses.py
+-rw-r--r--   0        0        0        0 2023-03-22 17:32:23.021092 sinch-1.0.0/sinch/domains/conversation/models/contact/__init__.py
+-rw-r--r--   0        0        0     1418 2023-03-22 17:32:23.021408 sinch-1.0.0/sinch/domains/conversation/models/contact/requests.py
+-rw-r--r--   0        0        0      852 2023-03-22 17:32:23.020912 sinch-1.0.0/sinch/domains/conversation/models/contact/responses.py
+-rw-r--r--   0        0        0      292 2023-03-22 17:32:23.032015 sinch-1.0.0/sinch/domains/conversation/models/conversation/__init__.py
+-rw-r--r--   0        0        0     1247 2023-03-22 17:32:23.032302 sinch-1.0.0/sinch/domains/conversation/models/conversation/requests.py
+-rw-r--r--   0        0        0      782 2023-03-22 17:32:23.031696 sinch-1.0.0/sinch/domains/conversation/models/conversation/responses.py
+-rw-r--r--   0        0        0        0 2023-03-22 17:32:23.030231 sinch-1.0.0/sinch/domains/conversation/models/event/__init__.py
+-rw-r--r--   0        0        0      314 2023-03-22 17:32:23.030603 sinch-1.0.0/sinch/domains/conversation/models/event/requests.py
+-rw-r--r--   0        0        0      197 2023-03-22 17:32:23.030043 sinch-1.0.0/sinch/domains/conversation/models/event/responses.py
+-rw-r--r--   0        0        0        0 2023-03-22 17:32:23.026054 sinch-1.0.0/sinch/domains/conversation/models/message/__init__.py
+-rw-r--r--   0        0        0     1060 2023-03-22 17:32:23.026459 sinch-1.0.0/sinch/domains/conversation/models/message/requests.py
+-rw-r--r--   0        0        0      600 2023-03-22 17:32:23.025842 sinch-1.0.0/sinch/domains/conversation/models/message/responses.py
+-rw-r--r--   0        0        0        0 2023-03-22 17:32:23.027339 sinch-1.0.0/sinch/domains/conversation/models/opt_in_opt_out/__init__.py
+-rw-r--r--   0        0        0      458 2023-03-22 17:32:23.027648 sinch-1.0.0/sinch/domains/conversation/models/opt_in_opt_out/requests.py
+-rw-r--r--   0        0        0      306 2023-03-22 17:32:23.027157 sinch-1.0.0/sinch/domains/conversation/models/opt_in_opt_out/responses.py
+-rw-r--r--   0        0        0      291 2023-03-22 17:32:23.028553 sinch-1.0.0/sinch/domains/conversation/models/templates/__init__.py
+-rw-r--r--   0        0        0      642 2023-03-22 17:32:23.029346 sinch-1.0.0/sinch/domains/conversation/models/templates/requests.py
+-rw-r--r--   0        0        0      639 2023-03-22 17:32:23.028276 sinch-1.0.0/sinch/domains/conversation/models/templates/responses.py
+-rw-r--r--   0        0        0        0 2023-03-22 17:32:23.024547 sinch-1.0.0/sinch/domains/conversation/models/transcoding/__init__.py
+-rw-r--r--   0        0        0      260 2023-03-22 17:32:23.024870 sinch-1.0.0/sinch/domains/conversation/models/transcoding/requests.py
+-rw-r--r--   0        0        0      192 2023-03-22 17:32:23.024366 sinch-1.0.0/sinch/domains/conversation/models/transcoding/responses.py
+-rw-r--r--   0        0        0      276 2023-03-22 17:32:23.019781 sinch-1.0.0/sinch/domains/conversation/models/webhook/__init__.py
+-rw-r--r--   0        0        0      740 2023-03-22 17:32:23.020120 sinch-1.0.0/sinch/domains/conversation/models/webhook/requests.py
+-rw-r--r--   0        0        0      576 2023-03-22 17:32:23.019469 sinch-1.0.0/sinch/domains/conversation/models/webhook/responses.py
+-rw-r--r--   0        0        0    12944 2024-02-05 14:52:20.733463 sinch-1.0.0/sinch/domains/numbers/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-22 17:32:22.970908 sinch-1.0.0/sinch/domains/numbers/endpoints/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-04 14:27:43.268520 sinch-1.0.0/sinch/domains/numbers/endpoints/active/__init__.py
+-rw-r--r--   0        0        0     1990 2024-02-05 14:52:20.734796 sinch-1.0.0/sinch/domains/numbers/endpoints/active/get_number_configuration.py
+-rw-r--r--   0        0        0     2921 2024-02-05 14:52:20.736614 sinch-1.0.0/sinch/domains/numbers/endpoints/active/list_active_numbers_for_project.py
+-rw-r--r--   0        0        0     2009 2024-02-05 14:52:20.737576 sinch-1.0.0/sinch/domains/numbers/endpoints/active/release_number_from_project.py
+-rw-r--r--   0        0        0     2133 2024-02-05 14:52:20.738402 sinch-1.0.0/sinch/domains/numbers/endpoints/active/update_number_configuration.py
+-rw-r--r--   0        0        0        0 2023-09-04 14:27:43.269937 sinch-1.0.0/sinch/domains/numbers/endpoints/available/__init__.py
+-rw-r--r--   0        0        0     1478 2024-02-05 14:52:20.739731 sinch-1.0.0/sinch/domains/numbers/endpoints/available/activate_number.py
+-rw-r--r--   0        0        0     2604 2024-02-05 14:52:20.740632 sinch-1.0.0/sinch/domains/numbers/endpoints/available/list_available_numbers.py
+-rw-r--r--   0        0        0     2867 2024-02-05 14:52:20.741488 sinch-1.0.0/sinch/domains/numbers/endpoints/available/rent_any_number.py
+-rw-r--r--   0        0        0     1802 2024-02-05 14:52:20.742314 sinch-1.0.0/sinch/domains/numbers/endpoints/available/search_for_number.py
+-rw-r--r--   0        0        0        0 2024-02-02 10:49:49.715757 sinch-1.0.0/sinch/domains/numbers/endpoints/callbacks/__init__.py
+-rw-r--r--   0        0        0     1146 2024-02-05 14:52:20.743335 sinch-1.0.0/sinch/domains/numbers/endpoints/callbacks/get_configuration.py
+-rw-r--r--   0        0        0     1440 2024-02-05 14:52:20.744589 sinch-1.0.0/sinch/domains/numbers/endpoints/callbacks/update_configuration.py
+-rw-r--r--   0        0        0      482 2023-03-22 17:32:22.972748 sinch-1.0.0/sinch/domains/numbers/endpoints/numbers_endpoint.py
+-rw-r--r--   0        0        0        0 2023-09-04 14:27:43.271177 sinch-1.0.0/sinch/domains/numbers/endpoints/regions/__init__.py
+-rw-r--r--   0        0        0     1899 2024-02-05 14:52:20.747234 sinch-1.0.0/sinch/domains/numbers/endpoints/regions/list_available_regions.py
+-rw-r--r--   0        0        0      186 2023-03-22 17:32:22.969507 sinch-1.0.0/sinch/domains/numbers/enums.py
+-rw-r--r--   0        0        0      100 2023-03-22 17:32:22.975582 sinch-1.0.0/sinch/domains/numbers/exceptions.py
+-rw-r--r--   0        0        0      916 2023-09-04 14:27:43.271965 sinch-1.0.0/sinch/domains/numbers/models/__init__.py
+-rw-r--r--   0        0        0      500 2023-09-04 14:27:43.272197 sinch-1.0.0/sinch/domains/numbers/models/active/__init__.py
+-rw-r--r--   0        0        0      711 2024-02-05 14:52:20.752181 sinch-1.0.0/sinch/domains/numbers/models/active/requests.py
+-rw-r--r--   0        0        0      556 2023-09-04 14:27:43.272975 sinch-1.0.0/sinch/domains/numbers/models/active/responses.py
+-rw-r--r--   0        0        0        0 2023-09-04 14:27:43.273170 sinch-1.0.0/sinch/domains/numbers/models/available/__init__.py
+-rw-r--r--   0        0        0      776 2023-09-05 15:42:43.238636 sinch-1.0.0/sinch/domains/numbers/models/available/requests.py
+-rw-r--r--   0        0        0      826 2023-09-05 15:42:43.239803 sinch-1.0.0/sinch/domains/numbers/models/available/responses.py
+-rw-r--r--   0        0        0        0 2024-02-02 10:49:49.716920 sinch-1.0.0/sinch/domains/numbers/models/callbacks/__init__.py
+-rw-r--r--   0        0        0      204 2024-02-02 10:49:49.717548 sinch-1.0.0/sinch/domains/numbers/models/callbacks/requests.py
+-rw-r--r--   0        0        0      422 2024-02-02 10:49:49.717914 sinch-1.0.0/sinch/domains/numbers/models/callbacks/responses.py
+-rw-r--r--   0        0        0      192 2023-09-04 14:27:43.274147 sinch-1.0.0/sinch/domains/numbers/models/regions/__init__.py
+-rw-r--r--   0        0        0      223 2023-09-04 14:27:43.274387 sinch-1.0.0/sinch/domains/numbers/models/regions/requests.py
+-rw-r--r--   0        0        0      272 2023-09-04 14:27:43.274643 sinch-1.0.0/sinch/domains/numbers/models/regions/responses.py
+-rw-r--r--   0        0        0    22047 2024-02-05 14:52:20.753177 sinch-1.0.0/sinch/domains/sms/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-22 17:32:22.979555 sinch-1.0.0/sinch/domains/sms/endpoints/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-22 17:32:22.985941 sinch-1.0.0/sinch/domains/sms/endpoints/batches/__init__.py
+-rw-r--r--   0        0        0     1785 2024-02-05 14:52:20.754161 sinch-1.0.0/sinch/domains/sms/endpoints/batches/cancel_batch.py
+-rw-r--r--   0        0        0     1833 2024-02-05 14:52:20.754802 sinch-1.0.0/sinch/domains/sms/endpoints/batches/get_batch.py
+-rw-r--r--   0        0        0     2119 2024-02-05 14:52:20.755323 sinch-1.0.0/sinch/domains/sms/endpoints/batches/list_batches.py
+-rw-r--r--   0        0        0     1912 2024-02-05 14:52:20.756145 sinch-1.0.0/sinch/domains/sms/endpoints/batches/replace_batch.py
+-rw-r--r--   0        0        0     1832 2024-02-05 14:52:20.757708 sinch-1.0.0/sinch/domains/sms/endpoints/batches/send_batch.py
+-rw-r--r--   0        0        0     1746 2024-02-05 14:52:20.758398 sinch-1.0.0/sinch/domains/sms/endpoints/batches/send_batch_dry_run.py
+-rw-r--r--   0        0        0     1355 2024-02-05 14:52:20.759101 sinch-1.0.0/sinch/domains/sms/endpoints/batches/send_delivery_feedback.py
+-rw-r--r--   0        0        0     1966 2024-02-05 14:52:20.759556 sinch-1.0.0/sinch/domains/sms/endpoints/batches/update_batch.py
+-rw-r--r--   0        0        0        0 2023-03-22 17:32:22.977507 sinch-1.0.0/sinch/domains/sms/endpoints/delivery_reports/__init__.py
+-rw-r--r--   0        0        0     2445 2024-02-05 14:52:20.760105 sinch-1.0.0/sinch/domains/sms/endpoints/delivery_reports/get_all_delivery_reports_for_project.py
+-rw-r--r--   0        0        0     1966 2024-02-05 14:52:20.760619 sinch-1.0.0/sinch/domains/sms/endpoints/delivery_reports/get_delivery_report_for_batch.py
+-rw-r--r--   0        0        0     2030 2024-02-05 14:52:20.761246 sinch-1.0.0/sinch/domains/sms/endpoints/delivery_reports/get_delivery_report_for_number.py
+-rw-r--r--   0        0        0        0 2023-03-22 17:32:22.980432 sinch-1.0.0/sinch/domains/sms/endpoints/groups/__init__.py
+-rw-r--r--   0        0        0     1558 2024-02-05 14:52:20.761911 sinch-1.0.0/sinch/domains/sms/endpoints/groups/create_group.py
+-rw-r--r--   0        0        0     1190 2024-02-05 14:52:20.762375 sinch-1.0.0/sinch/domains/sms/endpoints/groups/delete_group.py
+-rw-r--r--   0        0        0     1524 2024-02-05 14:52:20.762844 sinch-1.0.0/sinch/domains/sms/endpoints/groups/get_group.py
+-rw-r--r--   0        0        0     1307 2024-02-05 14:52:20.763481 sinch-1.0.0/sinch/domains/sms/endpoints/groups/get_phone_numbers_for_group.py
+-rw-r--r--   0        0        0     1880 2024-02-05 14:52:20.764742 sinch-1.0.0/sinch/domains/sms/endpoints/groups/list_groups.py
+-rw-r--r--   0        0        0     1690 2024-02-05 14:52:20.765346 sinch-1.0.0/sinch/domains/sms/endpoints/groups/replace_group.py
+-rw-r--r--   0        0        0     1660 2024-02-05 14:52:20.766092 sinch-1.0.0/sinch/domains/sms/endpoints/groups/update_group.py
+-rw-r--r--   0        0        0        0 2023-03-22 17:32:22.984281 sinch-1.0.0/sinch/domains/sms/endpoints/inbounds/__init__.py
+-rw-r--r--   0        0        0     1632 2024-02-05 14:52:20.767032 sinch-1.0.0/sinch/domains/sms/endpoints/inbounds/get_incoming_message.py
+-rw-r--r--   0        0        0     2056 2024-02-05 14:52:20.767674 sinch-1.0.0/sinch/domains/sms/endpoints/inbounds/list_incoming_messages.py
+-rw-r--r--   0        0        0      450 2024-02-01 15:15:33.837832 sinch-1.0.0/sinch/domains/sms/endpoints/sms_endpoint.py
+-rw-r--r--   0        0        0        0 2023-03-22 17:32:22.976341 sinch-1.0.0/sinch/domains/sms/enums.py
+-rw-r--r--   0        0        0       96 2023-03-22 17:32:22.995387 sinch-1.0.0/sinch/domains/sms/exceptions.py
+-rw-r--r--   0        0        0        0 2023-03-22 17:32:22.990043 sinch-1.0.0/sinch/domains/sms/models/__init__.py
+-rw-r--r--   0        0        0      483 2023-03-22 17:32:22.994761 sinch-1.0.0/sinch/domains/sms/models/batches/__init__.py
+-rw-r--r--   0        0        0     2141 2024-05-14 13:11:12.897426 sinch-1.0.0/sinch/domains/sms/models/batches/requests.py
+-rw-r--r--   0        0        0     1012 2023-08-02 08:44:18.971175 sinch-1.0.0/sinch/domains/sms/models/batches/responses.py
+-rw-r--r--   0        0        0      385 2023-03-22 17:32:22.989331 sinch-1.0.0/sinch/domains/sms/models/delivery_reports/__init__.py
+-rw-r--r--   0        0        0      569 2023-03-22 17:32:22.989786 sinch-1.0.0/sinch/domains/sms/models/delivery_reports/requests.py
+-rw-r--r--   0        0        0      711 2023-03-22 17:32:22.989003 sinch-1.0.0/sinch/domains/sms/models/delivery_reports/responses.py
+-rw-r--r--   0        0        0      261 2023-03-22 17:32:22.991445 sinch-1.0.0/sinch/domains/sms/models/groups/__init__.py
+-rw-r--r--   0        0        0      919 2023-03-22 17:32:22.991894 sinch-1.0.0/sinch/domains/sms/models/groups/requests.py
+-rw-r--r--   0        0        0      720 2023-03-22 17:32:22.991057 sinch-1.0.0/sinch/domains/sms/models/groups/responses.py
+-rw-r--r--   0        0        0      293 2023-03-22 17:32:22.993119 sinch-1.0.0/sinch/domains/sms/models/inbounds/__init__.py
+-rw-r--r--   0        0        0      392 2023-03-22 17:32:22.993554 sinch-1.0.0/sinch/domains/sms/models/inbounds/requests.py
+-rw-r--r--   0        0        0      399 2023-03-22 17:32:22.992745 sinch-1.0.0/sinch/domains/sms/models/inbounds/responses.py
+-rw-r--r--   0        0        0     6786 2024-05-14 13:11:24.173735 sinch-1.0.0/sinch/domains/verification/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-02 10:49:49.719289 sinch-1.0.0/sinch/domains/verification/endpoints/__init__.py
+-rw-r--r--   0        0        0     1641 2024-04-09 13:38:08.312871 sinch-1.0.0/sinch/domains/verification/endpoints/get_verification_by_id.py
+-rw-r--r--   0        0        0     1753 2024-04-09 13:38:08.313983 sinch-1.0.0/sinch/domains/verification/endpoints/get_verification_by_identity.py
+-rw-r--r--   0        0        0     1711 2024-04-09 13:38:08.314922 sinch-1.0.0/sinch/domains/verification/endpoints/get_verification_by_reference.py
+-rw-r--r--   0        0        0     1737 2024-04-09 13:38:08.316179 sinch-1.0.0/sinch/domains/verification/endpoints/report_verification_using_id.py
+-rw-r--r--   0        0        0     1795 2024-04-09 13:38:08.317037 sinch-1.0.0/sinch/domains/verification/endpoints/report_verification_using_identity.py
+-rw-r--r--   0        0        0     3541 2024-05-14 13:11:24.174039 sinch-1.0.0/sinch/domains/verification/endpoints/start_verification.py
+-rw-r--r--   0        0        0      489 2024-02-02 10:49:49.723010 sinch-1.0.0/sinch/domains/verification/endpoints/verification_endpoint.py
+-rw-r--r--   0        0        0      323 2024-05-14 13:11:24.174341 sinch-1.0.0/sinch/domains/verification/enums.py
+-rw-r--r--   0        0        0      105 2024-03-04 11:35:49.951830 sinch-1.0.0/sinch/domains/verification/exceptions.py
+-rw-r--r--   0        0        0      125 2024-05-14 13:11:24.174610 sinch-1.0.0/sinch/domains/verification/models/__init__.py
+-rw-r--r--   0        0        0     2640 2024-05-14 13:11:24.174919 sinch-1.0.0/sinch/domains/verification/models/requests.py
+-rw-r--r--   0        0        0     1809 2024-05-14 13:11:24.175161 sinch-1.0.0/sinch/domains/verification/models/responses.py
+-rw-r--r--   0        0        0    14168 2024-05-14 13:11:24.175474 sinch-1.0.0/sinch/domains/voice/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 13:11:24.175520 sinch-1.0.0/sinch/domains/voice/endpoints/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 13:11:24.175736 sinch-1.0.0/sinch/domains/voice/endpoints/applications/__init__.py
+-rw-r--r--   0        0        0     1132 2024-05-14 13:11:24.176024 sinch-1.0.0/sinch/domains/voice/endpoints/applications/assign_numbers.py
+-rw-r--r--   0        0        0     1288 2024-05-14 13:11:24.176265 sinch-1.0.0/sinch/domains/voice/endpoints/applications/get_callback_urls.py
+-rw-r--r--   0        0        0     1233 2024-05-14 13:11:24.176503 sinch-1.0.0/sinch/domains/voice/endpoints/applications/get_numbers.py
+-rw-r--r--   0        0        0     1419 2024-05-14 13:11:24.176767 sinch-1.0.0/sinch/domains/voice/endpoints/applications/query_number.py
+-rw-r--r--   0        0        0     1519 2024-05-14 13:11:24.177020 sinch-1.0.0/sinch/domains/voice/endpoints/applications/unassign_number.py
+-rw-r--r--   0        0        0     1544 2024-05-14 13:11:24.177208 sinch-1.0.0/sinch/domains/voice/endpoints/applications/update_callbacks.py
+-rw-r--r--   0        0        0        0 2024-05-14 13:11:24.177249 sinch-1.0.0/sinch/domains/voice/endpoints/callouts/__init__.py
+-rw-r--r--   0        0        0     2444 2024-05-14 13:11:24.177514 sinch-1.0.0/sinch/domains/voice/endpoints/callouts/callout.py
+-rw-r--r--   0        0        0        0 2024-05-14 13:11:24.177573 sinch-1.0.0/sinch/domains/voice/endpoints/calls/__init__.py
+-rw-r--r--   0        0        0     2355 2024-05-14 13:11:24.177896 sinch-1.0.0/sinch/domains/voice/endpoints/calls/get_call.py
+-rw-r--r--   0        0        0     1289 2024-05-14 13:11:24.178173 sinch-1.0.0/sinch/domains/voice/endpoints/calls/manage_call.py
+-rw-r--r--   0        0        0     1188 2024-05-14 13:11:24.178400 sinch-1.0.0/sinch/domains/voice/endpoints/calls/update_call.py
+-rw-r--r--   0        0        0        0 2024-05-14 13:11:24.178439 sinch-1.0.0/sinch/domains/voice/endpoints/conferences/__init__.py
+-rw-r--r--   0        0        0     1270 2024-05-14 13:11:24.178714 sinch-1.0.0/sinch/domains/voice/endpoints/conferences/get_conference.py
+-rw-r--r--   0        0        0     1087 2024-05-14 13:11:24.178928 sinch-1.0.0/sinch/domains/voice/endpoints/conferences/kick_all_participants.py
+-rw-r--r--   0        0        0     1192 2024-05-14 13:11:24.179093 sinch-1.0.0/sinch/domains/voice/endpoints/conferences/kick_participant.py
+-rw-r--r--   0        0        0     1425 2024-05-14 13:11:24.179236 sinch-1.0.0/sinch/domains/voice/endpoints/conferences/manage_participant.py
+-rw-r--r--   0        0        0      461 2024-05-14 13:11:24.179456 sinch-1.0.0/sinch/domains/voice/endpoints/voice_endpoint.py
+-rw-r--r--   0        0        0     1511 2024-05-14 13:11:24.179695 sinch-1.0.0/sinch/domains/voice/enums.py
+-rw-r--r--   0        0        0       98 2024-05-14 13:11:24.179890 sinch-1.0.0/sinch/domains/voice/exceptions.py
+-rw-r--r--   0        0        0      577 2024-05-14 13:11:24.180216 sinch-1.0.0/sinch/domains/voice/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 13:11:24.180262 sinch-1.0.0/sinch/domains/voice/models/applications/__init__.py
+-rw-r--r--   0        0        0      758 2024-05-14 13:11:24.180471 sinch-1.0.0/sinch/domains/voice/models/applications/requests.py
+-rw-r--r--   0        0        0      831 2024-05-14 13:11:24.180616 sinch-1.0.0/sinch/domains/voice/models/applications/responses.py
+-rw-r--r--   0        0        0        0 2024-05-14 13:11:24.180659 sinch-1.0.0/sinch/domains/voice/models/callouts/__init__.py
+-rw-r--r--   0        0        0     1094 2024-05-14 13:11:24.180953 sinch-1.0.0/sinch/domains/voice/models/callouts/requests.py
+-rw-r--r--   0        0        0      164 2024-05-14 13:11:24.181197 sinch-1.0.0/sinch/domains/voice/models/callouts/responses.py
+-rw-r--r--   0        0        0        0 2024-05-14 13:11:24.181236 sinch-1.0.0/sinch/domains/voice/models/calls/__init__.py
+-rw-r--r--   0        0        0      679 2024-05-14 13:11:24.181516 sinch-1.0.0/sinch/domains/voice/models/calls/requests.py
+-rw-r--r--   0        0        0      582 2024-05-14 13:11:24.181763 sinch-1.0.0/sinch/domains/voice/models/calls/responses.py
+-rw-r--r--   0        0        0        0 2024-05-14 13:11:24.181806 sinch-1.0.0/sinch/domains/voice/models/conferences/__init__.py
+-rw-r--r--   0        0        0      559 2024-05-14 13:11:24.182023 sinch-1.0.0/sinch/domains/voice/models/conferences/requests.py
+-rw-r--r--   0        0        0      530 2024-05-14 13:11:24.182184 sinch-1.0.0/sinch/domains/voice/models/conferences/responses.py
+-rw-r--r--   0        0        0        0 2024-05-14 13:11:24.182223 sinch-1.0.0/sinch/domains/voice/models/svaml/__init__.py
+-rw-r--r--   0        0        0      474 2024-05-14 13:11:24.182509 sinch-1.0.0/sinch/domains/voice/models/svaml/actions/__init__.py
+-rw-r--r--   0        0        0     5213 2024-05-14 13:11:24.182794 sinch-1.0.0/sinch/domains/voice/models/svaml/actions/actions.py
+-rw-r--r--   0        0        0      469 2024-05-14 13:11:24.182978 sinch-1.0.0/sinch/domains/voice/models/svaml/instructions/__init__.py
+-rw-r--r--   0        0        0     1815 2024-05-14 13:11:24.183198 sinch-1.0.0/sinch/domains/voice/models/svaml/instructions/instructions.py
+-rw-r--r--   0        0        0     6253 1970-01-01 00:00:00.000000 sinch-1.0.0/PKG-INFO
```

### Comparing `sinch-0.4.0/LICENSE` & `sinch-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/README.md` & `sinch-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 Here you'll find documentation related to the Sinch Python SDK, including how to install it, initialize it, and start developing Python code using Sinch services.
 
 To use Sinch services, you'll need a Sinch account and access keys. You can sign up for an account and create access keys at [dashboard.sinch.com](https://dashboard.sinch.com).
 
 For more information on the Sinch APIs on which this SDK is based, refer to the official [developer documentation portal](developers.sinch.com).
 
-**This SDK is currently available to selected developers for preview use only. It is being provided for the purpose of collecting feedback, and should not be used in production environments.**
 
 - [Prerequisites](#prerequisites)
 - [Installation](#installation)
 - [Getting started](#getting-started)
 - [Logging]()
 
 ## Prerequisites
@@ -69,16 +68,16 @@
 
 ## Products
 
 Sinch client provides access to the following Sinch products:
 - Numbers
 - SMS
 - Verification
-- Conversation API
-- Additional products coming soon!
+- Voice API
+- Conversation API (beta release)
 
 ## Logging
 
 Logging configuration for this SDK utilizes following hierarchy:
 1. If no configuration was provided via `logger_name` or `logger` configurable, SDK will inherit configuration from the root logger with the `Sinch` prefix.
 2. If `logger_name` configurable was provided, SDK will use logger related to that name. For example: `myapp.sinch` will inherit configuration from the `myapp` logger.
 3. If `logger` (logger instance) configurable was provided, SDK will use that particular logger for all its logging operations.
```

### Comparing `sinch-0.4.0/pyproject.toml` & `sinch-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "sinch"
 description = "Sinch SDK for Python programming language"
-version = "0.4.0"
+version = "1.0.0"
 license = "Apache 2.0"
 readme = "README.md"
 authors = [
     "Sinch Developer Experience Team <devexp@sinch.com>",
 ]
 repository = "https://github.com/sinch/sinch-sdk-python"
 documentation = "https://developers.sinch.com"
```

### Comparing `sinch-0.4.0/sinch/core/adapters/asyncio_http_adapter.py` & `sinch-1.0.0/sinch/core/adapters/asyncio_http_adapter.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/core/adapters/requests_http_transport.py` & `sinch-1.0.0/sinch/core/adapters/requests_http_transport.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/core/clients/sinch_client_async.py` & `sinch-1.0.0/sinch/core/clients/sinch_client_async.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from sinch.core.clients.sinch_client_configuration import Configuration
 from sinch.core.token_manager import TokenManagerAsync
 from sinch.core.adapters.asyncio_http_adapter import HTTPTransportAioHTTP
 from sinch.domains.authentication import AuthenticationAsync
 from sinch.domains.numbers import NumbersAsync
 from sinch.domains.conversation import ConversationAsync
 from sinch.domains.sms import SMSAsync
-from sinch.domains.verification import Verification as VerificationAsync
+from sinch.domains.verification import VerificationAsync
+from sinch.domains.voice import VoiceAsync
 
 
 class SinchClientAsync(SinchClientBase):
     """
     Asynchronous implementation of the Sinch Client
     By default this implementation uses HTTPTransportAioHTTP based on AioHTTP library
     Custom Async HTTPTransport implementation can be provided via `transport` argument
@@ -39,7 +40,8 @@
         )
 
         self.authentication = AuthenticationAsync(self)
         self.numbers = NumbersAsync(self)
         self.conversation = ConversationAsync(self)
         self.sms = SMSAsync(self)
         self.verification = VerificationAsync(self)
+        self.voice = VoiceAsync(self)
```

### Comparing `sinch-0.4.0/sinch/core/clients/sinch_client_base.py` & `sinch-1.0.0/sinch/core/clients/sinch_client_base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from logging import Logger
 from abc import ABC, abstractmethod
 from sinch.core.clients.sinch_client_configuration import Configuration
 from sinch.domains.authentication import AuthenticationBase
 from sinch.domains.numbers import NumbersBase
 from sinch.domains.conversation import ConversationBase
 from sinch.domains.sms import SMSBase
+from sinch.domains.voice import VoiceBase
 
 
 class SinchClientBase(ABC):
     """
     Sinch abstract base class for concrete Sinch Client implementations.
     By default, this SDK provides two implementations - sync and async.
     Feel free to utilize any of them for you custom implementation.
     """
     configuration = Configuration
     authentication = AuthenticationBase
     numbers = NumbersBase
     conversation = ConversationBase
     sms = SMSBase
+    voice = VoiceBase
 
     @abstractmethod
     def __init__(
         self,
         key_id: str = None,
         key_secret: str = None,
         project_id: str = None,
```

### Comparing `sinch-0.4.0/sinch/core/clients/sinch_client_configuration.py` & `sinch-1.0.0/sinch/core/clients/sinch_client_configuration.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,35 +29,58 @@
         self.project_id = project_id
         self.application_key = application_key
         self.application_secret = application_secret
         self.connection_timeout = connection_timeout
         self.auth_origin = "auth.sinch.com"
         self.numbers_origin = "numbers.api.sinch.com"
         self.verification_origin = "verification.api.sinch.com"
+        self.voice_applications_origin = "callingapi.sinch.com"
+        self._voice_domain = "{}.api.sinch.com"
+        self._voice_region = None
         self._conversation_region = "eu"
         self._conversation_domain = ".conversation.api.sinch.com"
         self._sms_region = "us"
         self._sms_domain = "zt.{}.sms.api.sinch.com"
         self._templates_region = "eu"
         self._templates_domain = ".template.api.sinch.com"
         self.token_manager = token_manager
         self.disable_https = disable_https
         self.transport: HTTPTransport = transport
 
         self._set_conversation_origin()
         self._set_sms_origin()
         self._set_templates_origin()
+        self._set_voice_origin()
 
         if logger_name:
             self.logger = logging.getLogger(logger_name)
         elif logger:
             self.logger = logger
         else:
             self.logger = logging.getLogger("Sinch")
 
+    def _set_voice_origin(self):
+        if not self._voice_region:
+            self.voice_origin = self._voice_domain.format("calling")
+        else:
+            self.voice_origin = self._voice_domain.format("calling-" + self._voice_region)
+
+    def _set_voice_region(self, region):
+        self._voice_region = region
+        self._set_voice_origin()
+
+    def _get_voice_region(self):
+        return self._voice_region
+
+    voice_region = property(
+        _get_voice_region,
+        _set_voice_region,
+        doc="Voice Region"
+    )
+
     def _set_sms_origin(self):
         self.sms_origin = self._sms_domain.format(self._sms_region)
 
     def _set_sms_region(self, region):
         self._sms_region = region
         self._set_sms_origin()
```

### Comparing `sinch-0.4.0/sinch/core/clients/sinch_client_sync.py` & `sinch-1.0.0/sinch/core/clients/sinch_client_sync.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from sinch.core.token_manager import TokenManager
 from sinch.core.adapters.requests_http_transport import HTTPTransportRequests
 from sinch.domains.authentication import Authentication
 from sinch.domains.numbers import Numbers
 from sinch.domains.conversation import Conversation
 from sinch.domains.sms import SMS
 from sinch.domains.verification import Verification
+from sinch.domains.voice import Voice
 
 
 class SinchClient(SinchClientBase):
     """
     Synchronous implementation of the Sinch Client
     By default this implementation uses HTTPTransportRequests based on Requests library
     Custom Sync HTTPTransport implementation can be provided via `transport` argument
@@ -39,7 +40,8 @@
         )
 
         self.authentication = Authentication(self)
         self.numbers = Numbers(self)
         self.conversation = Conversation(self)
         self.sms = SMS(self)
         self.verification = Verification(self)
+        self.voice = Voice(self)
```

### Comparing `sinch-0.4.0/sinch/core/endpoint.py` & `sinch-1.0.0/sinch/core/endpoint.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/core/pagination.py` & `sinch-1.0.0/sinch/core/pagination.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/core/ports/http_transport.py` & `sinch-1.0.0/sinch/core/ports/http_transport.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/core/signature.py` & `sinch-1.0.0/sinch/core/signature.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/core/token_manager.py` & `sinch-1.0.0/sinch/core/token_manager.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/authentication/__init__.py` & `sinch-1.0.0/sinch/domains/authentication/__init__.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/authentication/endpoints/oauth.py` & `sinch-1.0.0/sinch/domains/authentication/endpoints/oauth.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/__init__.py` & `sinch-1.0.0/sinch/domains/conversation/__init__.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/app/create_app.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/app/create_app.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/app/delete_app.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/app/delete_app.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/app/get_app.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/app/get_app.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/app/list_apps.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/app/list_apps.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/app/update_app.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/app/update_app.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/capability.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/capability.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/contact/create_contact.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/contact/create_contact.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/contact/delete_contact.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/contact/delete_contact.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/contact/get_channel_profile.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/contact/get_channel_profile.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/contact/get_contact.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/contact/get_contact.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/contact/list_contact.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/contact/list_contact.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/contact/merge_contacts.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/contact/merge_contacts.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/contact/update_contact.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/contact/update_contact.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/conversation/create_conversation.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/conversation/create_conversation.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/conversation/delete_conversation.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/conversation/delete_conversation.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/conversation/get_conversation.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/conversation/get_conversation.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/conversation/inject_message_to_conversation.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/conversation/inject_message_to_conversation.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/conversation/list_conversations.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/conversation/list_conversations.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/conversation/stop_conversation.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/conversation/stop_conversation.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/conversation/update_conversation.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/conversation/update_conversation.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/events.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/events.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/message/delete_message.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/message/delete_message.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/message/get_message.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/message/get_message.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/message/list_message.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/message/list_message.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/message/send_message.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/message/send_message.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/opt_in.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/opt_in.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/opt_out.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/opt_out.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/templates/create_template.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/templates/create_template.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/templates/delete_template.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/templates/delete_template.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/templates/get_template.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/templates/get_template.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/templates/list_templates.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/templates/list_templates.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/templates/update_template.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/templates/update_template.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/transcode.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/transcode.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/webhooks/create_webhook.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/webhooks/create_webhook.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/webhooks/delete_webhook.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/webhooks/delete_webhook.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/webhooks/get_webhook.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/webhooks/get_webhook.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/webhooks/list_webhooks.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/webhooks/list_webhooks.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/endpoints/webhooks/update_webhook.py` & `sinch-1.0.0/sinch/domains/conversation/endpoints/webhooks/update_webhook.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/enums.py` & `sinch-1.0.0/sinch/domains/conversation/enums.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/models/__init__.py` & `sinch-1.0.0/sinch/domains/conversation/models/__init__.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/models/app/requests.py` & `sinch-1.0.0/sinch/domains/conversation/models/app/requests.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/models/app/responses.py` & `sinch-1.0.0/sinch/domains/conversation/models/app/responses.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/models/contact/requests.py` & `sinch-1.0.0/sinch/domains/conversation/models/contact/requests.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/models/contact/responses.py` & `sinch-1.0.0/sinch/domains/conversation/models/contact/responses.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/models/conversation/requests.py` & `sinch-1.0.0/sinch/domains/conversation/models/conversation/requests.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/models/conversation/responses.py` & `sinch-1.0.0/sinch/domains/conversation/models/conversation/responses.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/models/message/requests.py` & `sinch-1.0.0/sinch/domains/conversation/models/message/requests.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/models/message/responses.py` & `sinch-1.0.0/sinch/domains/conversation/models/message/responses.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/models/templates/requests.py` & `sinch-1.0.0/sinch/domains/conversation/models/templates/requests.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/models/templates/responses.py` & `sinch-1.0.0/sinch/domains/conversation/models/templates/responses.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/models/webhook/requests.py` & `sinch-1.0.0/sinch/domains/conversation/models/webhook/requests.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/conversation/models/webhook/responses.py` & `sinch-1.0.0/sinch/domains/conversation/models/webhook/responses.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/numbers/__init__.py` & `sinch-1.0.0/sinch/domains/numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/numbers/endpoints/active/get_number_configuration.py` & `sinch-1.0.0/sinch/domains/numbers/endpoints/active/get_number_configuration.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/numbers/endpoints/active/list_active_numbers_for_project.py` & `sinch-1.0.0/sinch/domains/numbers/endpoints/active/list_active_numbers_for_project.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/numbers/endpoints/active/release_number_from_project.py` & `sinch-1.0.0/sinch/domains/numbers/endpoints/active/release_number_from_project.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/numbers/endpoints/active/update_number_configuration.py` & `sinch-1.0.0/sinch/domains/numbers/endpoints/active/update_number_configuration.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/numbers/endpoints/available/activate_number.py` & `sinch-1.0.0/sinch/domains/numbers/endpoints/available/activate_number.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/numbers/endpoints/available/list_available_numbers.py` & `sinch-1.0.0/sinch/domains/numbers/endpoints/available/list_available_numbers.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/numbers/endpoints/available/rent_any_number.py` & `sinch-1.0.0/sinch/domains/numbers/endpoints/available/rent_any_number.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/numbers/endpoints/available/search_for_number.py` & `sinch-1.0.0/sinch/domains/numbers/endpoints/available/search_for_number.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/numbers/endpoints/callbacks/get_configuration.py` & `sinch-1.0.0/sinch/domains/numbers/endpoints/callbacks/get_configuration.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/numbers/endpoints/callbacks/update_configuration.py` & `sinch-1.0.0/sinch/domains/numbers/endpoints/callbacks/update_configuration.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/numbers/endpoints/regions/list_available_regions.py` & `sinch-1.0.0/sinch/domains/numbers/endpoints/regions/list_available_regions.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/numbers/models/__init__.py` & `sinch-1.0.0/sinch/domains/numbers/models/__init__.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/numbers/models/active/requests.py` & `sinch-1.0.0/sinch/domains/numbers/models/active/requests.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/numbers/models/active/responses.py` & `sinch-1.0.0/sinch/domains/numbers/models/active/responses.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/numbers/models/available/requests.py` & `sinch-1.0.0/sinch/domains/numbers/models/available/requests.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/numbers/models/available/responses.py` & `sinch-1.0.0/sinch/domains/numbers/models/available/responses.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/sms/__init__.py` & `sinch-1.0.0/sinch/domains/sms/__init__.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/sms/endpoints/batches/cancel_batch.py` & `sinch-1.0.0/sinch/domains/sms/endpoints/batches/cancel_batch.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/sms/endpoints/batches/get_batch.py` & `sinch-1.0.0/sinch/domains/sms/endpoints/batches/get_batch.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/sms/endpoints/batches/list_batches.py` & `sinch-1.0.0/sinch/domains/sms/endpoints/batches/list_batches.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/sms/endpoints/batches/replace_batch.py` & `sinch-1.0.0/sinch/domains/sms/endpoints/batches/replace_batch.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/sms/endpoints/batches/send_batch.py` & `sinch-1.0.0/sinch/domains/sms/endpoints/batches/send_batch.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/sms/endpoints/batches/send_batch_dry_run.py` & `sinch-1.0.0/sinch/domains/sms/endpoints/batches/send_batch_dry_run.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/sms/endpoints/batches/send_delivery_feedback.py` & `sinch-1.0.0/sinch/domains/sms/endpoints/batches/send_delivery_feedback.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/sms/endpoints/batches/update_batch.py` & `sinch-1.0.0/sinch/domains/sms/endpoints/batches/update_batch.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/sms/endpoints/delivery_reports/get_all_delivery_reports_for_project.py` & `sinch-1.0.0/sinch/domains/sms/endpoints/delivery_reports/get_all_delivery_reports_for_project.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/sms/endpoints/delivery_reports/get_delivery_report_for_batch.py` & `sinch-1.0.0/sinch/domains/sms/endpoints/delivery_reports/get_delivery_report_for_batch.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/sms/endpoints/delivery_reports/get_delivery_report_for_number.py` & `sinch-1.0.0/sinch/domains/sms/endpoints/delivery_reports/get_delivery_report_for_number.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/sms/endpoints/groups/create_group.py` & `sinch-1.0.0/sinch/domains/sms/endpoints/groups/create_group.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/sms/endpoints/groups/delete_group.py` & `sinch-1.0.0/sinch/domains/sms/endpoints/groups/delete_group.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/sms/endpoints/groups/get_group.py` & `sinch-1.0.0/sinch/domains/sms/endpoints/groups/get_group.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/sms/endpoints/groups/get_phone_numbers_for_group.py` & `sinch-1.0.0/sinch/domains/sms/endpoints/groups/get_phone_numbers_for_group.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/sms/endpoints/groups/list_groups.py` & `sinch-1.0.0/sinch/domains/sms/endpoints/groups/list_groups.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/sms/endpoints/groups/replace_group.py` & `sinch-1.0.0/sinch/domains/sms/endpoints/groups/replace_group.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/sms/endpoints/groups/update_group.py` & `sinch-1.0.0/sinch/domains/sms/endpoints/groups/update_group.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/sms/endpoints/inbounds/get_incoming_message.py` & `sinch-1.0.0/sinch/domains/sms/endpoints/inbounds/get_incoming_message.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/sms/endpoints/inbounds/list_incoming_messages.py` & `sinch-1.0.0/sinch/domains/sms/endpoints/inbounds/list_incoming_messages.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/sms/models/batches/requests.py` & `sinch-1.0.0/sinch/domains/sms/models/batches/requests.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/sms/models/batches/responses.py` & `sinch-1.0.0/sinch/domains/sms/models/batches/responses.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/sms/models/delivery_reports/requests.py` & `sinch-1.0.0/sinch/domains/sms/models/delivery_reports/requests.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/sms/models/delivery_reports/responses.py` & `sinch-1.0.0/sinch/domains/sms/models/delivery_reports/responses.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/sms/models/groups/requests.py` & `sinch-1.0.0/sinch/domains/sms/models/groups/requests.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/sms/models/groups/responses.py` & `sinch-1.0.0/sinch/domains/sms/models/groups/responses.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/verification/__init__.py` & `sinch-1.0.0/sinch/domains/verification/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,45 +19,101 @@
     ReportVerificationByIdentityResponse,
     ReportVerificationByIdResponse,
     GetVerificationStatusByIdentityResponse,
     GetVerificationStatusByIdResponse,
     GetVerificationStatusByReferenceResponse
 )
 from sinch.domains.verification.models.requests import (
-    StartVerificationRequest,
+    StartSMSVerificationRequest,
+    StartFlashCallVerificationRequest,
+    StartCalloutVerificationRequest,
+    StartSeamlessVerificationRequest,
     ReportVerificationByIdentityRequest,
     ReportVerificationByIdRequest,
     GetVerificationStatusByIdRequest,
     GetVerificationStatusByIdentityRequest,
     GetVerificationStatusByReferenceRequest
 )
-
-from sinch.domains.verification.enums import VerificationMethod
+from sinch.domains.verification.models import VerificationIdentity
 
 
 class Verifications:
     def __init__(self, sinch):
         self._sinch = sinch
 
-    def start(
+    def start_sms(
+        self,
+        identity: VerificationIdentity,
+        reference: str = None,
+        custom: str = None,
+        expiry: str = None,
+        code_type: str = None,
+        template: str = None
+    ) -> StartVerificationResponse:
+        return self._sinch.configuration.transport.request(
+            StartVerificationEndpoint(
+                request_data=StartSMSVerificationRequest(
+                    identity=identity,
+                    reference=reference,
+                    custom=custom,
+                    expiry=expiry,
+                    code_type=code_type,
+                    template=template
+                )
+            )
+        )
+
+    def start_flash_call(
+        self,
+        identity: VerificationIdentity,
+        reference: str = None,
+        custom: str = None,
+        dial_timeout: int = None
+    ) -> StartVerificationResponse:
+        return self._sinch.configuration.transport.request(
+            StartVerificationEndpoint(
+                request_data=StartFlashCallVerificationRequest(
+                    identity=identity,
+                    reference=reference,
+                    custom=custom,
+                    dial_timeout=dial_timeout
+                )
+            )
+        )
+
+    def start_callout(
         self,
-        identity: dict,
-        method: VerificationMethod,
+        identity: VerificationIdentity,
         reference: str = None,
         custom: str = None,
-        flash_call_options: dict = None
+        speech_locale: str = None
     ) -> StartVerificationResponse:
         return self._sinch.configuration.transport.request(
             StartVerificationEndpoint(
-                request_data=StartVerificationRequest(
+                request_data=StartCalloutVerificationRequest(
                     identity=identity,
-                    method=method,
                     reference=reference,
                     custom=custom,
-                    flash_call_options=flash_call_options
+                    speech_locale=speech_locale
+                )
+            )
+        )
+
+    def start_seamless(
+        self,
+        identity: VerificationIdentity,
+        reference: str = None,
+        custom: str = None
+    ) -> StartVerificationResponse:
+        return self._sinch.configuration.transport.request(
+            StartVerificationEndpoint(
+                request_data=StartSeamlessVerificationRequest(
+                    identity=identity,
+                    reference=reference,
+                    custom=custom
                 )
             )
         )
 
     def report_by_id(
         self,
         id: str,
```

### Comparing `sinch-0.4.0/sinch/domains/verification/endpoints/get_verification_by_id.py` & `sinch-1.0.0/sinch/domains/verification/endpoints/get_verification_by_id.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/verification/endpoints/get_verification_by_identity.py` & `sinch-1.0.0/sinch/domains/verification/endpoints/get_verification_by_identity.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/verification/endpoints/get_verification_by_reference.py` & `sinch-1.0.0/sinch/domains/verification/endpoints/get_verification_by_reference.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/verification/endpoints/report_verification_using_id.py` & `sinch-1.0.0/sinch/domains/verification/endpoints/report_verification_using_id.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/verification/endpoints/report_verification_using_identity.py` & `sinch-1.0.0/sinch/domains/verification/endpoints/report_verification_using_identity.py`

 * *Files identical despite different names*

### Comparing `sinch-0.4.0/sinch/domains/verification/models/responses.py` & `sinch-1.0.0/sinch/domains/verification/models/responses.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,56 @@
 from dataclasses import dataclass
 from sinch.core.models.base_model import SinchBaseModel
 from sinch.domains.verification.enums import VerificationMethod, VerificationStatus
 
 
 @dataclass
+class FlashCallResponse:
+    cli_filter: str
+    interception_timeout: int
+    report_timeout: int
+    deny_call_after: int
+
+
+@dataclass
+class SMSResponse:
+    template: str
+    interception_timeout: str
+
+
+@dataclass
+class DataResponse:
+    target_uri: str
+
+
+@dataclass
 class StartVerificationResponse(SinchBaseModel):
     id: str
     method: VerificationMethod
     _links: list
 
 
 @dataclass
 class StartSMSInitiateVerificationResponse(StartVerificationResponse):
-    sms: dict
+    sms: SMSResponse
 
 
 @dataclass
 class StartFlashCallInitiateVerificationResponse(StartVerificationResponse):
-    flashcall: dict
+    flash_call: FlashCallResponse
 
 
 @dataclass
-class StartCalloutInitiateVerificationResponse(StartVerificationResponse):
-    callout: dict
+class StartDataInitiateVerificationResponse(StartVerificationResponse):
+    seamless: DataResponse
 
 
 @dataclass
-class StartDataInitiateVerificationResponse(StartVerificationResponse):
-    seamless: dict
+class StartCalloutInitiateVerificationResponse(StartVerificationResponse):
+    pass
 
 
 @dataclass
 class VerificationResponse(SinchBaseModel):
     id: str
     method: VerificationMethod
     status: VerificationStatus
```

### Comparing `sinch-0.4.0/PKG-INFO` & `sinch-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinch
-Version: 0.4.0
+Version: 1.0.0
 Summary: Sinch SDK for Python programming language
 Home-page: https://github.com/sinch/sinch-sdk-python
 License: Apache 2.0
 Keywords: sinch,sdk
 Author: Sinch Developer Experience Team
 Author-email: devexp@sinch.com
 Requires-Python: >=3.9
@@ -41,15 +41,14 @@
 
 Here you'll find documentation related to the Sinch Python SDK, including how to install it, initialize it, and start developing Python code using Sinch services.
 
 To use Sinch services, you'll need a Sinch account and access keys. You can sign up for an account and create access keys at [dashboard.sinch.com](https://dashboard.sinch.com).
 
 For more information on the Sinch APIs on which this SDK is based, refer to the official [developer documentation portal](developers.sinch.com).
 
-**This SDK is currently available to selected developers for preview use only. It is being provided for the purpose of collecting feedback, and should not be used in production environments.**
 
 - [Prerequisites](#prerequisites)
 - [Installation](#installation)
 - [Getting started](#getting-started)
 - [Logging]()
 
 ## Prerequisites
@@ -98,16 +97,16 @@
 
 ## Products
 
 Sinch client provides access to the following Sinch products:
 - Numbers
 - SMS
 - Verification
-- Conversation API
-- Additional products coming soon!
+- Voice API
+- Conversation API (beta release)
 
 ## Logging
 
 Logging configuration for this SDK utilizes following hierarchy:
 1. If no configuration was provided via `logger_name` or `logger` configurable, SDK will inherit configuration from the root logger with the `Sinch` prefix.
 2. If `logger_name` configurable was provided, SDK will use logger related to that name. For example: `myapp.sinch` will inherit configuration from the `myapp` logger.
 3. If `logger` (logger instance) configurable was provided, SDK will use that particular logger for all its logging operations.
```

